# Phase 1. Stakeholder Map và Chiến Lược — Phần Cá Nhân

**Họ tên:** Trịnh Hải Đăng**MSSV:** 2A202601602**Nhóm:** 333 (Nguyễn Hoàng Minh, Nguyễn Việt Hải, Trịnh Hải Đăng)**Vai trò:** Technical Lead & Architecture / Design**Case:** A. AI Tutor, Diagnostic Refresher (VLearn Codelabs)**Bước:** Cá nhân — Liệt kê Stakeholder & Chiến lược ban đầu (Phase 1)

> **Ghi chú:** Đây là bài làm cá nhân của Trịnh Hải Đăng (Tech Lead) dựa trên góc nhìn kỹ thuật hệ thống, tích hợp nền tảng VLearn và phỏng vấn học viên Đức (người đã dùng AI Tutor tích hợp sẵn nhưng vẫn phải nhảy ra ngoài vì sai context). Bản này được chuẩn bị để mang vào bàn thảo luận thống nhất chung cùng Minh và Hải.

---

## 0. Bối Cảnh Cá Nhân Neo Vào Trước Khi Liệt Kê

Từ góc nhìn Kỹ thuật & Kiến trúc giải pháp (Tech Lead), em neo vào Problem Hypothesis đã chốt ở Chặng 3:

> **Khi** học viên gặp lỗi môi trường/cú pháp trong bài lab, học viên cần một câu trả lời chính xác, gắn đúng phiên bản tài liệu môn học. **Hiện tại**, AI Tutor tích hợp sẵn trên VLearn chỉ đọc text tài liệu chung chung mà thiếu khâu chẩn đoán lỗi môi trường máy học viên (environment diagnostic) và thiếu cổng xác minh (verification gate). Khi học viên chuyển sang dùng ChatGPT/Claude bên ngoài, AI ngoài trả về mã nguồn sai phiên bản thư viện hoặc sai context môi trường lab, khiến học viên càng kẹt nặng hơn hoặc copy-paste mù quáng làm hỏng môi trường máy.

### Tiêu Chí Phân Loại Stakeholder Của Em:

1. **Người nắm hạ tầng kỹ thuật / API / quyền tích hợp** trên nền tảng VLearn Codelabs.
2. **Người vận hành trực tiếp lớp học** chịu ảnh hưởng nếu hệ thống gặp lỗi hoặc tạo thêm gánh nặng hỗ trợ.
3. **Học viên chịu đau kỹ thuật** (technical pain) khi nhận câu trả lời AI thiếu kiểm chứng.

---

## 1. Danh Sách 8 Stakeholder Cụ Thể (Góc Nhìn Tech & Product)

| # | Stakeholder Cụ Thể                                                         | Lý Do Là Stakeholder Trực Tiếp Của Vấn Đề Này                                                                                                                                                                       |
| - | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1 | **Platform Lead / Tech Lead nền tảng VLearn**                        | Người nắm quyền cấp API key, phê duyệt quyền tích hợp Extension/Widget vào giao diện Codelabs. Có quyền phủ quyết kỹ thuật nếu hệ thống gây lag hoặc tốn quá nhiều chi phí token.                 |
| 2 | **LC-01, Lab Coach Track 1**                                           | Người đứng lớp chính. Nếu AI Tutor gợi ý sai lệnh terminal, máy học viên bị lỗi môi trường và LC-01 sẽ là người phải đi gỡ thủ công từng máy.                                                  |
| 3 | **Học viên Đức (Learner em phỏng vấn ở Chặng 2)**              | Người dùng đại diện: Đã dùng AI Tutor cũ của VLearn nhưng thấy câu trả lời chung chung, ra ngoài dùng ChatGPT thì bị gợi ý thư viện deprecated. Là nhân chứng sống cho nhu cầu xác thực lỗi. |
| 4 | **Học viên Đạt (Learner ngại giơ tay)**                          | Người dùng đại diện cho nhóm im lặng: Thấy lớp đông, ngại gọi coach ngắt mạch giảng, rất cần 1 nút "Diagnostic Refresher" chẩn đoán lỗi tại chỗ trong 2 giây.                                     |
| 5 | **Mentor Review Dự Án Track 1**                                      | Người đánh giá kỹ thuật và tính khả thi của giải pháp, đòi hỏi kiến trúc RAG rõ ràng, có guardrails và có dataset kiểm thử tự động (Evals).                                                      |
| 6 | **Trợ Giảng (TA Support Ngoài Giờ)**                               | Người trực tiếp giải quyết các vé ticket hỗ trợ sau giờ học. Nếu AI Tutor chẩn đoán tốt lỗi cài đặt, khối lượng ticket của TA sẽ giảm mạnh.                                                      |
| 7 | **Curriculum Author (Tác giả biên soạn Lab Guide)**                | Người quản lý source tài liệu Markdown. Hệ thống RAG cần đánh index từ tài liệu này; nếu tài liệu cập nhật version mới, RAG pipeline phải sync theo.                                                   |
| 8 | **Hai bạn cùng Squad 333 (Nguyễn Hoàng Minh, Nguyễn Việt Hải)** | Minh giữ vai Product Lead (chốt scope, làm việc với Coach), Hải giữ vai Research & Data Lead (lập dataset eval). Là cộng sự trực tiếp cùng làm và chịu trách nhiệm.                                       |

---

## 2. Bản Đồ Stakeholder Map Cá Nhân (Influence × Interest)
|                           | **Interest Thấp**                                                                                                                                  | **Interest Cao**                                                                                                                                                                                                         |
| ------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Influence Cao**   | **BLOCKER (Ưu tiên thuyết phục kỹ thuật)**• **Platform Lead VLearn** *(Quyết định tích hợp API, lo ngại latency & token cost)* | **CHAMPION (Người ủng hộ chủ chốt)**• **LC-01, Lab Coach** *(Nắm vận hành buổi lab)*• **Mentor Review Track 1** *(Duyệt milestone dự án)*• **Core Squad 333 (Minh, Hải, Đăng)** |
| **Influence Thấp** | **BYSTANDER (Theo dõi)**• **Curriculum Author** *(Biên soạn tài liệu)*• **Điều phối viên xếp lịch lớp**                 | **SUPPORTER (Ủng hộ & Cung cấp dữ liệu)**• **Học viên Đức & Đạt** *(Người dùng thử nghiệm)*• **Trợ giảng TA ngoài giờ**                                                              |

---

## 3. Kiểm Tra Stance Thực Tế (Mức Độ Ủng Hộ)

| Stakeholder                        | Quadrant  | Stance Thực Tế                    | Căn Cứ & Góc Nhìn Kỹ Thuật                                                                                                                      |
| ---------------------------------- | --------- | ----------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Platform Lead VLearn**     | Blocker   | **Chưa ủng hộ**            | E ngại việc nhúng AI trực tiếp vào Codelabs làm chậm p95 latency (>2s) và đội chi phí API gọi LLM không kiểm soát được.            |
| **LC-01, Lab Coach**         | Champion  | **Chưa ủng hộ / E ngại**  | Sợ AI đưa câu trả lời ăn sẵn khiến học viên lười suy nghĩ, và sợ AI hướng dẫn sai làm hỏng môi trường code.                   |
| **Mentor Track 1**           | Champion  | **Ủng hộ có điều kiện** | Ủng hộ giải pháp nếu có kiến trúc an toàn (Guardrails, Fallback khi confidence < 85%) và có bộ Golden Dataset đo lường định lượng. |
| **Học viên Đức & Đạt** | Supporter | **Ủng hộ mạnh**            | Rất mong có công cụ chẩn đoán lỗi chính xác ngay tại chỗ để tự sửa bài mà không bị kẹt cả buổi.                                |
| **Trợ giảng ngoài giờ**  | Supporter | **Trung lập**                | Sẵn sàng ủng hộ nếu công cụ giảm được câu hỏi lặp, nhưng e ngại nếu AI trả lời sai họ sẽ phải giải thích lại từ đầu.      |
| **Core Squad 333**           | Champion  | **Ủng hộ tuyệt đối**     | 100% đồng lòng triển khai giải pháp kỹ thuật tối ưu.                                                                                        |

---

## 4. Chiến Lược Kỹ Thuật & Hành Động 1–2 Tuần Tới (Trịnh Hải Đăng)

| Stakeholder                        | Mục Tiêu Tác Động                       | Hành Động Kỹ Thuật Cụ Thể Trong 1-2 Tuần (Đăng phụ trách)                                                                                                                                                                         |
| ---------------------------------- | -------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Platform Lead VLearn**     | Thuyết phục về hiệu năng và chi phí   | Xây dựng bản mô tả kiến trúc RAG 2 tầng (Semantic Cache + Small LLM Router); chạy benchmark chứng minh p95 latency < 1.2s và chi phí < $0.02/lab session.                                                                         |
| **LC-01 (Lab Coach)**        | Thuyết phục về độ an toàn & giảm tải | Thiết kế cơ chế**Verification Gate & Socratic Prompting**: AI chỉ gợi ý bước kiểm tra từng phần kèm citation, không cho chép thẳng code; tích hợp nút fallback "Báo Coach" với ticket điền sẵn thông tin lỗi. |
| **Mentor Review**            | Chứng minh kỷ luật kỹ thuật             | Hoàn thiện code pipeline tích hợp Automated Evals (đo Hallucination rate và Citation precision) đẩy lên GitHub repo.                                                                                                                 |
| **Học viên Đức / Đạt** | Thu thập test case thực tế                | Lấy 15 log lỗi terminal thực tế của học viên trong buổi lab gần nhất để nạp vào bộ dữ liệu test của RAG pipeline.                                                                                                           |

---

## 5. Đóng Góp Của Đăng Khi Gộp Nhóm Vào Bản Thống Nhất Chung
- Bổ sung mảnh ghép **Platform Lead / Hạ tầng kỹ thuật** (chỗ mà bản nháp của Minh còn thiếu) vào ô Blocker cần thuyết phục.
- Đưa ra giải pháp kỹ thuật cụ thể (Deterministic Citation, Confidence Threshold 85%, Fallback Template) để xử lý triệt để phản biện của Lab Coach LC-01.
- Định hình cấu trúc **Embedded Squad** linh hoạt và cam kết nâng cấp năng lực từ L2 lên L3 AI Builder trong 30 ngày.