# Trang 1 — Stakeholder Map & Strategy (Bản Thống Nhất Team 333)

**Dự án:** AI Tutor — Diagnostic Refresher cho VLearn Codelabs | **Chương trình:** "AI Thực Chiến"  
**Nhóm:** 333 (Track 1 - Day 27) | **Thành viên:** Nguyễn Việt Hải (2A202601656), Nguyễn Hoàng Minh (2A202601764), Trịnh Hải Đăng (2A202601602)

---

### 1. Danh Sách Stakeholder & Stance Thực Tế

| #      | Stakeholder (Con người cụ thể)           | Quadrant     | Stance thực tế　　 | Phân tích & Căn cứ                                                                                                |
| --------| ------------------------------------------| :------------:| :------------------:| -------------------------------------------------------------------------------------------------------------------|
| **S1** | **LC-01 — Lab Coach kèm lớp Track 1 K4** | **Champion** | 🔴 **Chưa ủng hộ** | E ngại AI gợi ý sai làm hỏng môi trường máy; muốn giữ tính tự chủ cho learner; lo phát sinh thêm việc gỡ lỗi.     |
| **S2** | **Trợ giảng (TA) trực ngoài giờ**        | Supporter    | 🟡 **Trung lập**　　| Sẵn sàng ủng hộ nếu giảm câu hỏi lặp, lo ngại nếu AI giải thích sai khiến TA phải đính chính lại.                 |
| **S3** | **Giảng viên chuyên môn đứng lớp**       | Blocker      | 🔴 **Chưa ủng hộ** | Ưu tiên mạch giảng không bị gián đoạn, lo hallucination làm loãng kiến thức chuẩn.                                |
| **S4** | **Mentor review dự án Track 1**          | **Champion** | 🟢 **Ủng hộ có ĐK** | Ủng hộ nếu nhóm có kỷ luật bằng chứng, kiến trúc an toàn (Guardrails, Evals); phản đối nếu chưa có số liệu đo.    |
| **S5** | **Platform Lead / Tech Lead VLearn**     | **Blocker**  | 🔴 **Chưa ủng hộ** | Nắm quyền cấp API/Widget; lo ngại p95 latency >2s, chi phí token không kiểm soát và rủi ro bảo mật hệ thống live. |
| **S6** | **Học viên "AI Thực Chiến" (End-User)**  | Supporter    | 🟢 **Ủng hộ mạnh**　| (a) Cần chẩn đoán lỗi đúng version môi trường lab; (b) Nhóm im lặng cần hỏi AI tại chỗ không phải ngắt mạch bài.  |
| **S7** | **Tác giả biên soạn Lab Guide & Slide**  | Bystander    | 🟡 **Trung lập**　　| Gián tiếp liên quan vì lỗi setup môi trường chiếm tỷ lệ cao trong lab guide; chưa tiếp xúc.                       |
| **S8** | **Điều phối viên xếp lịch buổi lab**     | Bystander    | 🟡 **Trung lập**　　| Nắm giữ slot lịch lab; cần xin phép trước khi pilot trên lớp thật.                                                |
| **S9** | **Core Team 333 (Hải, Minh, Đăng)**      | Champion     | 🟢 **Ủng hộ 100%**　| Trực tiếp xây dựng giải pháp và chịu trách nhiệm toàn bộ kết quả dự án.                                           |

> **Phát hiện quan trọng:** S1 (LC-01) nằm ở vùng Champion nhưng stance thực tế là **Chưa ủng hộ** (lệch quadrant). Cùng với S5 (Platform Lead), đây là 2 stakeholder có ảnh hưởng cao nhất cần xử lý trước để tránh bị phủ quyết pilot.

---

### 2. Ma Trận Influence × Interest

| | **Interest Thấp** | **Interest Cao** |
|:---:|---|---|
| **Influence Cao** | **BLOCKER (Ưu tiên thuyết phục & xử lý mối lo)**<br>• **S5.** Platform Lead VLearn *(lo latency, chi phí token)*<br>• **S3.** Giảng viên chuyên môn *(lo mạch bài giảng)* | **CHAMPION (Làm việc chặt chẽ & tận dụng ủng hộ)**<br>• **S1.** LC-01 Lab Coach *(nắm vận hành lớp lab — Stance: 🔴)*<br>• **S4.** Mentor Review *(duyệt milestone dự án — Stance: 🟢)*<br>• **S9.** Core Team 333 *(trực tiếp thực hiện)* |
| **Influence Thấp** | **BYSTANDER (Theo dõi định kỳ)**<br>• **S7.** Tác giả Lab Guide<br>• **S8.** Điều phối viên xếp lịch | **SUPPORTER (Giữ thông tin & khai thác feedback)**<br>• **S2.** Trợ giảng TA ngoài giờ<br>• **S6.** Học viên End-User *(nhóm kẹt tool cũ & nhóm ngại hỏi)* |

---

### 3. Chiến Lược & Hành Động Cụ Thể 1–2 Tuần Cho 4 Stakeholder Ưu Tiên

| Nhóm | Stakeholder | Mối quan tâm cốt lõi | Hành động cụ thể 1–2 tuần tới (Who, What, When) |
|---|---|---|---|
| **Tận dụng ủng hộ** | **S4. Mentor Review** *(Ủng hộ)* | Kỷ luật bằng chứng, kiến trúc an toàn, bộ metrics đo lường rõ ràng. | **Đăng:** Đẩy code Automated Evals pipeline + RAG 2 tầng lên repo trước **thứ Sáu**. **Minh:** Nộp mục "Điều chưa chứng minh". **Hải:** Tổng hợp 1 trang evidence map từ 3 nguồn phỏng vấn để Mentor duyệt. |
| **Tận dụng ủng hộ** | **S6. Học viên End-User** *(Ủng hộ)* | Phản hồi tại chỗ trong 2s, đúng context tài liệu môn, không bị hallucinate. | **Đăng:** Thu thập 15 log lỗi terminal từ buổi lab để làm test case sống. **Hải:** Tạo micro-survey 3 câu (<1p). **Minh:** Nhờ LC-01 chỉ 2 học viên ít hỏi nhất để phỏng vấn 10 phút mở rộng mẫu. |
| **Ưu tiên thuyết phục** | **S1. LC-01 Lab Coach** *(Chưa ủng hộ)* | Không phá vỡ tính tự chủ của học viên; không làm hỏng máy; không tạo thêm việc gỡ lỗi. | **Minh:** Xin gặp LC-01 **10 phút tuần này**, hỏi đúng 1 câu: *"Cái gì khiến chị thấy công cụ làm chị nhẹ đi chứ không nặng thêm?"*. **Đăng:** Trình bày cơ chế Verification Gate (chỉ gợi ý debug + citation, không ném code) và nút "Báo Coach" kèm ticket tự điền. |
| **Ưu tiên thuyết phục** | **S5. Platform Lead** *(Chưa ủng hộ)* | Hiệu năng p95 <1.2s, chi phí <$0.02/phiên, bảo mật API, không ảnh hưởng LMS. | **Đăng:** Hoàn thiện kiến trúc RAG 2 tầng (Cache + Small Router) kèm tài liệu OpenAPI Spec. **Hải:** Sau khi Mentor duyệt, xin lịch họp 30 phút ở tuần 2 để xin cấp quyền Sandbox API. |

<div style="page-break-after: always;"></div>

# Trang 2 — Pitch & RACI (Bản Thống Nhất Team 333)

---

## 1. Pitch "Conclusion First" Dành Cho S1 (LC-01 — Lab Coach)

> **🎯 KẾT LUẬN TRƯỚC:**  
> **"Nhóm em xin chị 10 phút trong tuần này để hỏi đúng một câu: *Cái gì sẽ khiến chị thấy một công cụ giúp học viên tự gọi tên chỗ kẹt của mình làm chị nhẹ đi chứ không nặng thêm?* — Nhóm em không xin duyệt sản phẩm, cũng không làm công cụ trả lời thay chị."**

### 💡 Ba Lý Do Chính:
1. **Đúng chỗ nghẽn thật của Coach:** Chị từng chia sẻ mỗi câu hỏi lạ mất từ 30s–1p chỉ để hiểu học viên đang kẹt gì (và có lúc hiểu sai ý). Công cụ chỉ tập trung giúp học viên làm rõ câu hỏi trước khi tìm Coach.
2. **Bảo toàn nguyên tắc sư phạm:** Công cụ tuân thủ Socratic flow — chỉ gợi ý bước kiểm tra và dẫn nguồn tài liệu lab, hoàn toàn không đưa code giải sẵn, giữ trọn tính tự chủ cho học viên rèn luyện tư duy debug.
3. **Chặn rò rỉ câu hỏi ra ngoài thiếu kiểm chứng:** Câu hỏi Coach không kịp giải đáp đang bị học viên đưa lên ChatGPT ngoài và nhận về code sai phiên bản thư viện nhưng vẫn "buộc phải tin".

### 📊 Bằng Chứng Thực Chứng (3 nguồn phỏng vấn riêng):
- **Từ LC-01:** Mất 30s–1p/câu lạ để hiểu ý; câu ngoài trọng tâm phải bỏ; setup môi trường là phần bị hỏi dồn dập nhất.
- **Từ học viên ngại hỏi (Nhóm im lặng):** Sợ làm chậm mạch lớp nên không dám hỏi Coach, quay sang hỏi bạn (đúng khoảng 80%), nhiều khi tiếp thu kiến thức sai lệch.
- **Từ học viên dùng AI cũ:** AI cũ trả lời sai ngữ cảnh môn học, đành chụp ảnh đưa ChatGPT ngoài: *"Anh buộc phải tin thôi vì ngại hỏi Coach"*.

### 🤝 Small Ask:
**Xin 10 phút của LC-01 trong tuần này** để lắng nghe tiêu chí "làm nhẹ việc cho Coach". Nếu thuận lợi, xin chị chỉ giúp 2 học viên ít đặt câu hỏi nhất lớp để nhóm phỏng vấn 10 phút bổ sung dữ liệu.

---

## 2. Phản Biện Chính & Cách Xử Lý Rủi Ro Kỹ Thuật

- **Phản biện từ Coach & Tech Lead:** *"AI đưa ra câu lệnh sai làm hỏng môi trường máy học viên, hoặc sinh thói quen ỷ lại khiến Coach phải đi dọn rác."*
- **Cách xử lý của Team 333:**
  1. **Grounding 100% & Citation:** AI chỉ trích xuất giải pháp từ Lab Guide Markdown đã duyệt, kèm link dẫn chính xác dòng tài liệu.
  2. **Confidence Threshold 85%:** Nếu điểm tự tin <85%, AI từ chối suy đoán và tự động điền mẫu Ticket (kèm chat log + error log) chuyển thẳng đến Coach.
  3. **Socratic Guardrails:** AI chỉ đặt câu hỏi gợi mở từng bước kiểm tra, tuyệt đối không sinh toàn bộ khối code hoàn chỉnh.

---

## 3. RACI Matrix Cho Các Nhiệm Vụ Cốt Lõi (1–2 Tháng Tới)

| Nhiệm Vụ Trọng Tâm | Hải (Product) | Minh (Scope/Data) | Đăng (Tech) | LC-01 (Coach) | Platform Lead | Mentor |
|---|:---:|:---:|:---:|:---:|:---:|:---:|
| **1. Khóa phạm vi use case (Lab Diagnostic)** | **A** | R | C | C | I | C |
| **2. Thu thập error log & dữ liệu phỏng vấn** | C | I | **A / R** | C | I | I |
| **3. Xây dựng RAG Pipeline & Sandbox MVP** | I | C | **A / R** | I | C | I |
| **4. Thiết kế Prompt, Evals & Đo Hallucination** | R | C | **A** | C | I | C |
| **5. Triển khai Demo / Pilot trong buổi lab thật** | R | **A** | R | C | C | I |
| **6. Phê duyệt tích hợp chính thức vào VLearn** | R | C | R | C | **A** | C |

*Quy tắc chuẩn: Mỗi dòng chỉ có đúng 1 **A** (Accountable). R = Responsible, C = Consulted, I = Informed.*

<div style="page-break-after: always;"></div>

# Trang 3 — AI Team Design (Bản Thống Nhất Team 333)

---

## 1. Team Architecture: Mô Hình Embedded

**Lựa chọn:** **Embedded (Năng lực AI nhúng trực tiếp trong Squad sản phẩm).**  
**Lý do:** Team gồm 3 thành viên đang ở giai đoạn xây dựng MVP cho 1 use case duy nhất (Codelabs). Mô hình nhúng trực tiếp giúp squad ra quyết định nhanh, lặp nhanh giữa Prompt/RAG và phản hồi từ lớp học mà không phát sinh độ trễ điều phối như Centralized.

---

## 2. Core Roles & Extended Roles

```
[ AI Product / Squad Lead: Hải ] <---> [ Scope & Data / Ops Lead: Minh ]
                   \                         /
                    \                       /
                 [ AI / RAG Engineer Lead: Đăng ]
                                |
       ( Consulted: LC-01 Coach | Platform Lead | Mentor )
```

- **Core Roles (Hiện tại — Giai đoạn MVP):**
  - **AI Product / Squad Lead (Nguyễn Việt Hải):** Định hình luồng sư phạm, chuẩn hóa test cases, quản lý stakeholder và tiến độ.
  - **AI Engineer / RAG Builder (Trịnh Hải Đăng):** Thiết kế 2-layer RAG, Verification Gate, Prompt Guardrails, Automated Evals.
  - **Scope Owner & Data Researcher (Nguyễn Hoàng Minh):** Thu thập dữ liệu phỏng vấn, đo đếm pain points, làm việc trực tiếp với LC-01.
  - **Domain Expert (LC-01 — Consulted):** Thẩm định tính đúng đắn về mặt sư phạm của Prompt.
  - **Platform Specialist (Platform Lead — Consulted):** Cung cấp API spec và hạ tầng Sandbox.
- **Extended Roles (Khi Scale sau Pilot):** *MLOps & Automated Monitoring, Forward Deployed Engineer (tích hợp sang các môn khác), Legal/Data Compliance (bảo mật log học viên).*

---

## 3. Capability Gap & Priority Resourcing (Cách Bổ Sung Năng Lực)

| Capability Gap | Phương án | Lý do lựa chọn (Vì sao không Hire/Outsource) | Thời điểm cần |
|---|:---:|---|---|
| **1. UX / UI Design (Sidebar Widget)** | **Partner** | Chưa cần tuyển full-time cho 1 tính năng sidebar; outsource bên ngoài tốn lead-time và thiếu bối cảnh lớp học. **Giải pháp:** Hợp tác với team Design của VLearn hoặc cộng tác viên UX trong chương trình "AI Thực Chiến". | Trước buổi pilot đầu tiên |
| **2. Domain Expert Sư phạm chính thức** | **Partner** | Cần chuyên môn định kỳ (30p/tuần), không cần làm 8h/ngày. **Giải pháp:** Mời LC-01 làm *Pedagogy Advisor* đồng hành sau cuộc gặp Small Ask 10 phút. | Ngay trong tuần này (trước khi chốt Prompt) |
| **3. MLOps & Continuous Eval Pipeline** | **Outsource (Tool)** | Tuyển MLOps full-time ở quy mô 3 người là lãng phí; **Giải pháp:** Tích hợp platform có sẵn (LangSmith / Ragas / Evidently AI) để theo dõi chất lượng. | Sau MVP, trước khi mở rộng >50 học viên |

---

## 4. Squad Goal

> **🎯 SQUAD GOAL TEAM 333:**  
> **"Squad 333 sở hữu toàn diện pipeline AI Tutor — Diagnostic Refresher và chịu trách nhiệm đưa trải nghiệm gỡ lỗi của học viên VLearn từ hiện trạng *'kẹt bài không có nguồn kiểm chứng, phải hỏi AI ngoài rồi buộc phải tin'* đến *'nhận gợi ý chẩn đoán xác thực từ tài liệu môn học trong vòng 1.2 giây — trước khi cần escalate lên Coach.'*"**

<div style="page-break-after: always;"></div>

# Trang 4 — Team Health & Growth Plan (Bản Thống Nhất Team 333)

---

## 1. Bảng Điểm Tự Chấm Team Health (Thang 1–5)

| Khía Cạnh Đánh Giá | Hải | Minh | Đăng | Điểm TB | Nhận Xét Cốt Lõi |
|---|:---:|:---:|:---:|:---:|---|
| **Chất lượng AI (AI Quality)** | 3.0 | 2.0 | 3.5 | **2.8** | Thiết kế kiến trúc an toàn đã có, nhưng chưa chạy benchmark thực tế trên Golden Dataset. |
| **Tiến độ cam kết (Milestones)** | 3.0 | 3.0 | 4.5 | **3.5** | Hoàn thành tốt deadline lớp học; nhưng các cam kết tự đặt (phỏng vấn nhóm im lặng) còn trễ. |
| **Tinh thần Team (Safety)** | 4.0 | 4.0 | 4.5 | **4.2** | Giao tiếp cởi mở, dám chỉ ra thiếu sót của nhau (Minh chỉ ra các số liệu cam kết chưa đo). |
| **Tốc độ ra sản phẩm (Velocity)** | 2.0 | 1.0 | 3.5 | **2.2 ⚠️** | **Điểm nghẽn lớn nhất:** Chưa có prototype chạy được trên máy để học viên/Coach tương tác. |

---

## 2. Phân Tích Chênh Lệch & Vấn Đề Ưu Tiên Cần Giải Quyết

- **Khía cạnh thấp nhất:** **Tốc độ ra sản phẩm (2.2/5)** — Cả 3 đều nhận thấy team đang có nhiều tài liệu nhưng chưa có dòng code prototype nào đến tay người dùng thật.
- **Chênh lệch lớn nhất:** **Tiến độ (Đăng 4.5 vs Minh 3.0)** — Đăng nhìn theo deliverables nộp bài, Minh tính cả nợ tồn đọng (dữ liệu nhóm im lặng chưa lấy). Team thống nhất chốt điểm 3.0 để giữ kỷ luật thực tế.
- **Phát hiện quan trọng về Chất lượng AI:** Minh chỉ ra các số liệu như $85\%$ confidence, $<1.2s$ latency, $<\$0.02$ chi phí là mục tiêu kỹ thuật, chưa qua đo lường thực tế → **Team quyết định không dùng các số liệu này để hứa hẹn với Coach khi chưa có kết quả test**.
- **🚨 VẤN ĐỀ ƯU TIÊN SỐ 1:** **Chưa có Interactive Prototype để chứng minh với LC-01.** Nếu không có bản chạy thử, cuộc gặp thuyết phục LC-01 sẽ mất uy tín và không xin được slot pilot.

---

## 3. Nâng Cấp Năng Lực Cá Nhân (Competency Framework L1 / L2 / L3)

| Thành Viên & Vai Trò | Level Hiện Tại | Competency Cần Nâng Tiếp Theo | Hành Động Cụ Thể Trong 30 Ngày |
|---|:---:|---|---|
| **Nguyễn Việt Hải** *(AI Product Lead)* | **L2 (Practitioner)** | Đọc hiểu & phân tích trực tiếp output từ automated evals (không phụ thuộc Tech Lead). | Tự tay chạy 5 test cases trên Evals pipeline của Đăng và viết báo cáo nhận xét chất lượng độc lập. |
| **Nguyễn Hoàng Minh** *(Scope / Data Lead)* | **L2 (Practitioner)** | Định lượng hóa insight phỏng vấn thành metrics đo lường (thay vì chỉ mô tả định tính). | Chuyển đổi 3 pain points của Coach thành chỉ số đếm được (tần suất câu hỏi lặp, thời gian kẹt trung bình). |
| **Trịnh Hải Đăng** *(AI / Tech Lead)* | **L2 → L3 (Builder)** | Tự động hóa hoàn toàn quy trình CI/CD Evals cho RAG pipeline (thay vì test tay). | Tích hợp framework Evals tự động (Ragas/LangSmith) chạy tự động trên 25 test cases mỗi lần commit. |

---

## 4. Growth Plan 30 Ngày (Tối Đa 3 Hành Động Cụ Thể)

| Vấn Đề Cần Giải Quyết | Hành Động 30 Ngày Cụ Thể | Owner | Deadline | Dấu Hiệu Hoàn Thành (Definition of Done) |
|---|---|:---:|:---:|---|
| **1. Chưa có prototype cho user thử** | Xây dựng bản CLI Prototype 1-click (Input: log lỗi terminal $\rightarrow$ Output: Socratic debugging steps kèm citation). | **Đăng** | Thứ Sáu (Tuần 1) | Hải và Minh chạy thử được trên máy cá nhân không cần Đăng hướng dẫn. |
| **2. Cam kết kỹ thuật chưa có số liệu đo** | Chạy automated evals trên 25 ca lỗi thực tế từ log lab; đo lường chính xác Hallucination Rate và Citation Precision. | **Đăng** (chạy)<br>**Hải** (đối soát) | Cuối Tuần 2 | Bản báo cáo kiểm thử có dữ liệu thực tế đính kèm vào tài liệu pitch. |
| **3. Thiếu dữ liệu nhóm learner im lặng** | Gặp LC-01 xin kết nối 2 học viên ít đặt câu hỏi nhất để phỏng vấn sâu 10 phút/bạn về hành vi khi gặp lỗi. | **Minh** | Cuối Tuần 2 | Hoàn thành biên bản phỏng vấn 2 learner mới, bổ sung vào Evidence Map. |
