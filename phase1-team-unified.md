# Trang 1 — Stakeholder Map & Strategy (Bản Thống Nhất Team 333)

**Dự án:** AI Tutor — Diagnostic Refresher cho VLearn Codelabs  
**Nhóm:** 333 (Track 1 - Day 27)  
**Thành viên:**
- Nguyễn Việt Hải
- Nguyễn Hoàng Minh 
- Trịnh Hải Đăng 


---

## Bước 2 — Gộp Danh Sách, Loại Trùng & Đặt Lên Ma Trận (Team — 7')

### 2.1 Bảng Gộp & Loại Trùng

Ba bản cá nhân liệt kê tổng cộng 23 dòng stakeholder. Sau khi đối chiếu theo con người cụ thể (không theo nhãn chức danh), team thống nhất gộp thành **9 stakeholder không trùng** dưới đây.

| # | Stakeholder (Tên thống nhất) | Ghi chú gộp |
|---|---|---|
| **S1** | **LC-01 — Lab Coach đang kèm lớp Track 1 K4** | Cả 3 đều liệt kê. Có dữ liệu phỏng vấn trực tiếp từ Coach. |
| **S2** | **Trợ giảng (TA) nhận tin nhắn / email ngoài giờ** | Tách riêng khỏi LC-01 vì vai trò khác (vá tạm ngoài giờ vs. đứng lớp chính). |
| **S3** | **Giảng viên chuyên môn đứng lớp Track 1** | Senior AI Engineer giảng Core Modules; tách riêng Mentor vì vai trò khác nhau. |
| **S4** | **Mentor đang review dự án nhóm 333 ở Track 1** | Tách riêng Giảng viên vì vai trò khác nhau (duyệt milestone dự án vs. dạy nội dung môn học). |
| **S5** | **Platform Lead / Tech Lead nền tảng VLearn** | Bổ sung từ góc nhìn kỹ thuật — người nắm quyền phê duyệt tích hợp API/Widget. |
| **S6** | **Học viên "AI Thực Chiến" — Nhóm End-User đã phỏng vấn** | Gộp hai learner đại diện đã phỏng vấn: (a) learner đã dùng AI Tutor cũ nhưng vẫn phải nhảy ra ngoài vì sai context; (b) learner thuộc nhóm im lặng, ngại giơ tay hỏi giữa lớp. Hai trường hợp đại diện cho hai pain khác nhau nhưng cùng một lời giải. |
| **S7** | **Tác giả biên soạn Lab Guide & Slide (Curriculum Author)** | Phát hiện setup môi trường bị hỏi nhiều nhất → tài liệu setup là một phần của vấn đề và lời giải. |
| **S8** | **Điều phối viên xếp lịch buổi lab** | Tách riêng vì cần xin slot lab cụ thể cho pilot (người giữ lịch ≠ người duyệt nội dung). |
| **S9** | **Core Team 333 (Hải, Minh, Đăng)** | Cả 3 đều tự liệt kê; trực tiếp làm và chịu trách nhiệm kết quả dự án. |

> **Stakeholder bị loại khi gộp:**
> - *Giám đốc Chương trình "AI Thực Chiến"* — Team chưa xác định được một con người cụ thể có thể liên hệ trong tuần này. Giữ lại như stakeholder tiềm năng cần xác minh sau, không đặt lên ma trận chính.
> - *Nhà tuyển dụng / Đối tác Doanh nghiệp* — Quá xa so với vấn đề cụ thể đang giải quyết (khâu xác minh lỗi trong lab). Chuyển xuống danh sách theo dõi dài hạn.
---

### 2.2 Ma Trận Stakeholder Map Thống Nhất (Influence × Interest)

|  | **Interest Thấp** | **Interest Cao** |
|---|---|---|
| **Influence Cao** | **BLOCKER — Ưu tiên thuyết phục, giữ hài lòng, xử lý mối lo** | **CHAMPION — Làm việc chặt chẽ, tận dụng sự ủng hộ** |
|  | **S5.** Platform Lead / Tech Lead VLearn *(quyết định tích hợp API, lo latency & token cost, ít quan tâm đến nội dung sư phạm)* | **S1.** LC-01, Lab Coach *(nắm vận hành buổi lab, chịu hậu quả trực tiếp nếu AI hướng dẫn sai)* |
|  | **S3.** Giảng viên chuyên môn *(có quyền phủ quyết mạch bài giảng, nhưng ít có thời gian theo dõi tính năng AI Tutor)* | **S4.** Mentor review dự án *(duyệt milestone, quyết định nhóm đi tiếp hay quay lại)* |
|  |  | **S9.** Core Team 333 *(trực tiếp làm và chịu trách nhiệm toàn bộ)* |
| **Influence Thấp** | **BYSTANDER — Theo dõi** | **SUPPORTER — Giữ thông tin, khai thác feedback** |
|  | **S7.** Tác giả Lab Guide & Slide *(gián tiếp tạo ra lỗi setup nhưng không có quyền quyết định dự án)* | **S2.** Trợ giảng TA ngoài giờ *(gánh câu hỏi tràn ra ngoài buổi lab, cảm nhận đầu tiên nếu giải pháp tăng/giảm tải)* |
|  | **S8.** Điều phối viên xếp lịch *(giữ lịch lab nhưng không liên quan trực tiếp đến nội dung pilot)* | **S6.** Học viên "AI Thực Chiến" — Nhóm End-User đã phỏng vấn *(hai pain: kẹt vì AI Tutor cũ sai context; và ngại giơ tay giữa lớp)* |

---

### 2.3 Kiểm Tra Stance Thực Tế — Đối Chiếu Với Nhãn Quadrant

| # | Stakeholder | Quadrant | Stance thực tế | Khớp / Lệch? | Căn cứ & Giải thích |
|---|---|---|---|---|---|
| **S1** | LC-01, Lab Coach | **Champion** | 🔴 **Chưa ủng hộ** | ⚠️ **LỆCH** | Cả Minh và Đăng đều xác nhận: chị cố ý ít can thiệp để learner tự chủ. Một công cụ đẩy thêm câu trả lời sẵn đi ngược lựa chọn sư phạm của chị. Chị e ngại AI hướng dẫn sai làm hỏng môi trường code → chị phải đi gỡ thủ công. **Đây là stakeholder nguy hiểm nhất vì nằm ở Champion nhưng stance là Chưa ủng hộ.** |
| **S2** | Trợ giảng TA ngoài giờ | Supporter | 🟡 **Trung lập** (nghiêng lo ngại) | ≈ Khớp | Minh: phụ thuộc vào việc tính năng làm tải tăng hay giảm, chưa có dữ liệu. Đăng: sẵn sàng ủng hộ nếu giảm câu hỏi lặp, e ngại nếu AI sai phải giải thích lại. |
| **S3** | Giảng viên chuyên môn | **Blocker** | 🔴 **Chưa ủng hộ / E ngại** | ✅ Khớp | Hải: Lo AI "chém gió" (hallucination), muốn Socratic Tutor chứ không muốn ném code sẵn. Minh: Chưa tiếp xúc, suy đoán quan tâm mạch bài giảng không bị cắt. |
| **S4** | Mentor review dự án | Champion | 🟢 **Ủng hộ có điều kiện** | ✅ Khớp | Cả 3 thống nhất: Mentor ủng hộ nếu nhóm giữ kỷ luật bằng chứng, có kiến trúc an toàn (Guardrails, Evals) và Golden Dataset. Phản đối ngay nếu tuyên bố validated khi chưa đủ dữ liệu. |
| **S5** | Platform Lead VLearn | **Blocker** | 🔴 **Chưa ủng hộ** | ✅ Khớp | E ngại p95 latency >2s và chi phí API không kiểm soát. Yêu cầu Rate Limiting và bảo mật tích hợp. |
| **S6** | Học viên "AI Thực Chiến" — Nhóm End-User đã phỏng vấn | Supporter | 🟢 **Ủng hộ mạnh** | ✅ Khớp | (a) Rất mong có công cụ chẩn đoán lỗi chính xác, đúng version thư viện, không bị gợi ý deprecated package. (b) Cần hỏi AI ngay tại chỗ mà không phải ngắt mạch giảng. |
| **S7** | Tác giả Lab Guide & Slide | Bystander | 🟡 **Trung lập** | ✅ Khớp | Có thể thấy bị soi nếu dữ liệu cho thấy tài liệu setup là nguồn gây kẹt chính. Chưa tiếp xúc. |
| **S8** | Điều phối viên xếp lịch | Bystander | 🟡 **Trung lập** | ✅ Khớp | Chưa tiếp xúc. Cần xin slot nếu muốn thử nghiệm trên buổi lab thật. |
| **S9** | Core Team 333 | Champion | 🟢 **Ủng hộ tuyệt đối** | ✅ Khớp | Cả 3 đồng lòng 100%. |

> **Phát hiện quan trọng nhất khi đối chiếu stance:** Hai stakeholder nằm ở vùng có Influence Cao nhưng stance thực tế lại **Chưa ủng hộ** — đó là **S1 (LC-01)** và **S5 (Platform Lead VLearn)**. Ngoài ra **S3 (Giảng viên chuyên môn)** ở Blocker cũng E ngại. Đây là 3 người team cần ưu tiên xử lý trước, vì họ có khả năng cản trở dự án dù nằm ở vị trí khác nhau trên bản đồ.

---

## Bước 3 — Chọn 4 Stakeholder Ưu Tiên & Chiến Lược Cụ Thể (Team — 8')

### ✅ 2 Stakeholder Đang Ủng Hộ Mạnh → Tận Dụng Sức Ảnh Hưởng

---

#### ⭐ Ưu tiên A: S4 — Mentor Review Dự Án Track 1

| Câu hỏi | Trả lời của team |
|---|---|
| **Họ quan tâm điều gì?** | Kỷ luật bằng chứng: nhóm có dữ liệu thật chưa, có kiến trúc an toàn chưa, có đo lường định lượng chưa (Hallucination Rate, Citation Precision). Mentor không chấp nhận tuyên bố "validated" khi chưa đủ số liệu. |
| **Họ có thể giúp dự án thế nào?** | (1) Duyệt cho nhóm đi tiếp milestone → mở cánh cửa pilot. (2) Giới thiệu nhóm tới các stakeholder khác trong hệ sinh thái VLearn (Giám đốc chương trình, Platform Lead) nếu demo đủ thuyết phục. (3) Cho phản hồi sắc bén về kiến trúc RAG, giúp nhóm tránh sai hướng kỹ thuật sớm. |
| **Hành động cụ thể 1–2 tuần tới** | **Đăng:** Hoàn thiện code pipeline Automated Evals (đo Hallucination Rate & Citation Precision) và đẩy lên GitHub repo trước **thứ Sáu tuần này**. Gửi kèm bản kiến trúc RAG 2 tầng (Semantic Cache + Small LLM Router) để Mentor review. **Minh:** Nộp kèm mục "Điều em chưa chứng minh" (mục 7 trong bản cá nhân) — không giấu chỗ yếu, thể hiện kỷ luật bằng chứng. **Hải:** Tổng hợp bảng đối chiếu dữ liệu phỏng vấn 3 nguồn (Coach + 2 learner đại diện đã phỏng vấn) thành 1 trang evidence map cho Mentor duyệt nhanh. → **Mục tiêu:** Sau buổi review, nhờ Mentor giới thiệu nhóm tới Platform Lead VLearn để xin 30 phút trình bày kiến trúc tích hợp. |

---

#### ⭐ Ưu tiên B: S6 — Học viên "AI Thực Chiến" (Nhóm End-User đã phỏng vấn)

| Câu hỏi | Trả lời của team |
|---|---|
| **Họ quan tâm điều gì?** | Trường hợp (a) — learner kẹt vì AI Tutor cũ: Cần công cụ chẩn đoán lỗi chính xác, gắn đúng version thư viện/môi trường lab, không bị gợi ý deprecated package như khi dùng AI bên ngoài. Trường hợp (b) — learner ngại giơ tay: Cần nút "hỏi AI" ngay tại chỗ mà không phải ngắt mạch giảng, phản hồi trong 2 giây. |
| **Họ có thể giúp dự án thế nào?** | (1) Cung cấp log lỗi terminal thực tế để nạp bộ test RAG pipeline (test case sống). (2) Làm Beta Tester đầu tiên cho prototype. (3) Feedback 1-click (👍/👎) giúp đo chất lượng phản hồi. (4) Nếu hài lòng → truyền miệng trong lớp, kéo thêm learner thử nghiệm (organic adoption). |
| **Hành động cụ thể 1–2 tuần tới** | **Đăng:** Thu thập **15 log lỗi terminal thực tế** từ nhóm learner đã phỏng vấn trong buổi lab gần nhất để nạp vào bộ dữ liệu test RAG. **Hải:** Thiết kế form khảo sát vi mô (3 câu, <1 phút) cho nhóm learner đánh giá sau mỗi lần dùng prototype: "AI có trả lời đúng vấn đề em đang kẹt không?", "Em có phải ra ngoài hỏi thêm nguồn khác không?", "Điểm 1–5". **Minh:** Nhờ LC-01 chỉ thêm **2 learner ít đặt câu hỏi nhất** trong lớp (nhóm im lặng còn thiếu từ Chặng 3) → xin phỏng vấn ngắn 10 phút để mở rộng mẫu. |

---

### 🔴 2 Stakeholder Chưa Ủng Hộ / Có Rủi Ro Cản Trở → Ưu Tiên Thuyết Phục

---

#### 🚨 Ưu tiên C: S1 — LC-01, Lab Coach

| Câu hỏi | Trả lời của team |
|---|---|
| **Họ quan tâm điều gì?** | (1) Tự chủ của learner: Chị cố ý ít can thiệp để learner tự rèn tư duy debug. (2) Không bị thêm việc: Chị đã thừa nhận có lúc trả lời không kịp, không muốn AI tạo thêm vấn đề phải đi gỡ. (3) An toàn môi trường: Nếu AI gợi ý sai lệnh terminal, máy học viên hỏng → chị phải gỡ thủ công từng máy. |
| **Họ có thể cản trở dự án thế nào?** | LC-01 là người đứng lớp chính. Nếu chị không đồng ý cho AI Tutor chạy trong buổi lab, nhóm không có môi trường thử nghiệm thật. Chị có thể phủ quyết bất kỳ tính năng nào xen vào mạch bài lab mà chị đang quản lý. Ngoài ra, chị là nguồn giới thiệu duy nhất tới nhóm learner im lặng mà nhóm đang thiếu. |
| **Hành động cụ thể 1–2 tuần tới** | **Minh (người đã phỏng vấn chị):** Xin gặp lại LC-01 **10 phút trong tuần này**, hỏi thẳng một câu duy nhất: *"Cái gì sẽ khiến chị thấy công cụ này làm chị nhẹ đi chứ không nặng thêm?"* — đổi khung từ "thêm việc" sang "bớt việc". **Đăng:** Thiết kế cơ chế **Verification Gate & Socratic Prompting** — AI chỉ gợi ý bước kiểm tra từng phần kèm citation nguồn tài liệu lab, **không bao giờ đưa code hoàn chỉnh** → trình bày cho chị xem prototype trước khi chạy trong lớp. Tích hợp nút **"Báo Coach"** với ticket điền sẵn thông tin lỗi (context chat + log lỗi) để chị nhận được đầy đủ bối cảnh khi cần can thiệp. **Hải:** Chuẩn bị bảng so sánh "Có AI Tutor vs. Không có AI Tutor" trên các chỉ số chị quan tâm: số câu hỏi lặp mà chị phải trả lời / số máy bị hỏng môi trường / thời gian learner bị kẹt trung bình → dùng số liệu thật từ buổi lab quan sát để thuyết phục. |

---

#### 🚨 Ưu tiên D: S5 — Platform Lead / Tech Lead Nền Tảng VLearn

| Câu hỏi | Trả lời của team |
|---|---|
| **Họ quan tâm điều gì?** | (1) Hiệu năng hệ thống: p95 latency không được vượt 2 giây khi nhúng AI vào Codelabs. (2) Chi phí API: Token cost phải kiểm soát được, không đội ngân sách. (3) Bảo mật: Không làm lộ đề lab/dữ liệu độc quyền, tuân thủ OAuth2 phân quyền. (4) Ổn định: Không làm sập LMS, không gây nghẽn database. |
| **Họ có thể cản trở dự án thế nào?** | Platform Lead nắm quyền cấp API key, phê duyệt quyền tích hợp Extension/Widget vào giao diện Codelabs. Có quyền phủ quyết kỹ thuật nếu kiến trúc không đạt chuẩn hiệu năng/bảo mật. Không có sự đồng ý của Platform Lead = không thể tích hợp vào VLearn = dự án chỉ tồn tại trên giấy. |
| **Hành động cụ thể 1–2 tuần tới** | **Đăng:** Xây dựng bản **kiến trúc RAG 2 tầng** (Semantic Cache layer + Small LLM Router) với benchmark chứng minh **p95 latency < 1.2 giây** và **chi phí < $0.02/lab session**. Viết tài liệu API Integration Spec (OpenAPI format). **Minh:** Chuẩn bị bản cam kết kỹ thuật gồm: cơ chế Rate Limiting (max N requests/phút/học viên), Async/WebSocket architecture, test tải (Load Testing) kết quả trước khi deploy. Nêu rõ scope: widget sidebar, không can thiệp luồng chính của Codelabs. **Hải:** Sau khi Mentor duyệt (Ưu tiên A), nhờ Mentor giới thiệu → **xin 30 phút họp với Platform Lead trước cuối tuần thứ 2** để trình bày kiến trúc + benchmark. Mục tiêu cuộc họp: xin quyền truy cập sandbox API của VLearn để chạy prototype trên môi trường staging. |

---

## Tóm Tắt Ma Trận Hành Động 1–2 Tuần

| Tuần | Hải (Product Lead) | Minh (Scope Owner) | Đăng (Tech Lead) |
|---|---|---|---|
| **Tuần 1** | Tổng hợp evidence map từ 3 nguồn phỏng vấn (Coach + 2 learner đại diện) để gửi Mentor | Gặp lại LC-01 10 phút: hỏi "Cái gì khiến chị nhẹ đi?" + Nhờ chỉ 2 learner im lặng để phỏng vấn mở rộng mẫu | Hoàn thiện Automated Evals pipeline (Hallucination Rate + Citation Precision) → push GitHub |
| **Tuần 2** | Thiết kế form khảo sát vi mô cho nhóm learner đã phỏng vấn (3 câu, <1 phút) + chuẩn bị bảng so sánh "Có/Không AI Tutor" | Nộp bản cam kết kỹ thuật (Rate Limit, Load Test, Scope widget) + hỗ trợ Hải xin meeting Platform Lead | Viết kiến trúc RAG 2 tầng + Benchmark latency & cost + API Integration Spec → trình bày cho LC-01 cơ chế Verification Gate |

---

> **Nguyên tắc chung:** Mỗi hành động phải gọi tên được *ai làm*, *làm gì*, *trước ngày nào* và *kết quả bàn giao là gì*. Không viết chiến lược kiểu "Giữ liên hệ tốt" hay "Tăng cường hợp tác".
