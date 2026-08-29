# BẢNG PHÂN TÍCH VÀ LIỆT KÊ STAKEHOLDER (STAKEHOLDER MAP)
**Dự án:** AI Tutor cho Vlearn  
**Bối cảnh chương trình:** Chương trình đào tạo **"AI Thực Chiến"** trên nền tảng Vlearn (dành cho sinh viên năm cuối sắp ra trường và người mới tốt nghiệp chuyển ngành/nâng cao tay nghề để đi làm).  
**Nhóm thực hiện:** Team 333 (Track 1 - Day 27)  
**Thành viên:** 
- Nguyễn Việt Hải (Trưởng nhóm / Product Lead)
- Nguyễn Hoàng Minh (Tech Lead / Core Dev)
- Trịnh Hải Đăng (Data & Prompt Engineer)

---

## I. Khung Khái Niệm & Ma Trận Đánh Giá

1. **Trục đánh giá:**
   - **Influence (Mức độ ảnh hưởng):** Khả năng tác động (quyết định ngân sách, quyền duyệt pilot, tích hợp vào chương trình học, thay đổi kiến trúc) đến kết quả dự án.
   - **Interest (Mức độ quan tâm):** Mức độ sát sao, kỳ vọng và nhu cầu đối với tính năng AI Tutor trong quá trình dạy, học và vận hành chương trình "AI Thực Chiến".
   
2. **4 Vùng phân loại (theo slide):**
   - **Champion (Influence Cao × Interest Cao):** Người bảo trợ dự án, đồng hành cốt lõi, người hưởng lợi lớn và có thẩm quyền cao.
   - **Blocker / Manage Closely (Influence Cao × Interest Thấp/Trung bình):** Người có thẩm quyền quyết định hoặc kiểm duyệt nhưng có thể tạo rào cản nếu thấy rủi ro về chi phí, uy tín hoặc vận hành.
   - **Supporter / Keep Informed (Influence Thấp/Trung bình × Interest Cao):** Người dùng trực tiếp (học viên, lab coach), người ủng hộ nhiệt tình, cung cấp phản hồi thực tế liên tục.
   - **Bystander / Monitor (Influence Thấp × Interest Thấp):** Đối tượng gián tiếp, chỉ cần theo dõi và cập nhật thông tin định kỳ.

3. **Stance (Mức độ ủng hộ thực tế):**
   - 🟢 **Ủng hộ (Supportive):** Nhiệt tình thúc đẩy, sẵn sàng thử nghiệm và hỗ trợ dữ liệu/nguồn lực.
   - 🟡 **Trung lập (Neutral):** Đang quan sát hiệu quả, chưa cam kết, chờ bằng chứng về độ chính xác, tỷ lệ hoàn thành lab và chi phí vận hành.
   - 🔴 **Chưa ủng hộ / E ngại (Resistant / Skeptical):** Lo ngại rủi ro (AI giải hộ khiến học viên lười suy nghĩ, sai lệch kiến thức thực chiến, quá tải hỗ trợ kỹ thuật).

---

## II. Danh Sách Stakeholder Cụ Thể (Chương trình "AI Thực Chiến" - Vlearn)

Dưới đây là danh sách chi tiết các stakeholder được cá nhân hóa sát với bối cảnh chương trình **"AI Thực Chiến"**:

### 1. Giám đốc Chương trình "AI Thực Chiến" (Program Director)
- **Mô tả cụ thể:** Người chịu trách nhiệm cao nhất về chất lượng đầu ra, tỷ lệ học viên có việc làm và hiệu quả kinh doanh của chương trình "AI Thực Chiến" trên Vlearn; có quyền duyệt chính thức việc triển khai Pilot AI Tutor.
- **Influence:** **Rất Cao** (Quyết định đưa AI Tutor vào lộ trình học chính thức, phê duyệt ngân sách API/hạ tầng).
- **Interest:** **Cao** (Muốn tăng tỷ lệ tốt nghiệp (completion rate), giảm tỷ lệ drop-out do học viên bị "ngợp/kẹt" khi làm bài lab thực tế).
- **Vùng phân loại:** **Champion**
- **Stance:** 🟡 **Trung lập** (Cần xem xét báo cáo ROI, chi phí token/học viên và cam kết không gây ảnh hưởng tiêu cực đến uy tín chương trình).
- **Kỳ vọng & Rủi ro:** 
  - *Kỳ vọng:* AI Tutor giúp nâng cao trải nghiệm học tập, tạo điểm nhấn cạnh tranh công nghệ cho chương trình "AI Thực Chiến".
  - *Rủi ro:* Sợ chi phí token vượt ngân sách; sợ AI sinh mã lỗi hoặc giải thích sai kiến thức chuyên sâu.
- **Hành động đề xuất:** Trình bày bản Demo Pilot với giới hạn ngân sách rõ ràng (Cost per Active Student), các chỉ số đo lường hiệu quả (KPI: số ca gỡ kẹt thành công, điểm hài lòng CSAT).

---

### 2. Người phụ trách Đào tạo / Quản lý Học tập (Academic / Training Coordinator)
- **Mô tả cụ thể:** Người theo dõi tiến độ nộp bài lab, điểm số, tỷ lệ chuyên cần và hỗ trợ vận hành lớp học hàng ngày cho các lớp "AI Thực Chiến".
- **Influence:** **Trung bình - Cao** (Phối hợp xếp lịch, thu thập phản hồi, có quyền đề xuất dừng hoặc nhân rộng công cụ trong lớp học).
- **Interest:** **Cao** (Trực tiếp đối mặt với tình trạng học viên kêu ca bài khó, nộp bài trễ hạn hoặc bỏ cuộc giữa chừng).
- **Vùng phân loại:** **Champion / Supporter**
- **Stance:** 🟢 **Ủng hộ** (Rất muốn có công cụ tự động hỗ trợ giải tỏa áp lực chăm sóc học viên ngoài giờ).
- **Kỳ vọng & Rủi ro:** 
  - *Kỳ vọng:* AI Tutor hỗ trợ 24/7 giúp học viên nộp bài lab đúng hạn; có dashboard báo cáo các chủ đề/module học viên hay hỏi nhất.
  - *Rủi ro:* Sợ phát sinh thêm việc đối soát nếu học viên khiếu nại do AI trả lời mâu thuẫn với barem chấm.
- **Hành động đề xuất:** Cung cấp báo cáo Analytics tổng hợp "Top 5 lỗi/chủ đề học viên hỏi nhiều nhất trong tuần" để ban đào tạo điều chỉnh nhịp giảng dạy.

---

### 3. Giảng viên Chuyên môn của Chương trình "AI Thực Chiến"
- **Mô tả cụ thể:** Chuyên gia / Senior AI Engineer trực tiếp giảng dạy các buổi lý thuyết chính (Core Modules: ML, Deep Learning, MLOps, LLM Applications).
- **Influence:** **Cao** (Có tiếng nói quyết định về tính chuẩn xác của kiến thức và giáo trình).
- **Interest:** **Trung bình** (Tập trung chính vào bài giảng trên lớp, ít có thời gian trực tiếp ngồi trả lời từng lỗi cú pháp/môi trường của học viên).
- **Vùng phân loại:** **Manage Closely**
- **Stance:** 🔴 **Chưa ủng hộ / E ngại** (Lo sợ AI Tutor đưa ra câu trả lời hời hợt, không đúng tư duy thực chiến chuẩn công nghiệp, hoặc giải hộ khiến học viên không tự rèn luyện tư duy debug).
- **Kỳ vọng & Rủi ro:** 
  - *Kỳ vọng:* AI đóng vai trò "Socratic Tutor" — đặt câu hỏi gợi mở, hướng dẫn cách tra cứu tài liệu và tư duy xử lý lỗi thay vì ném code hoàn chỉnh.
  - *Rủi ro:* AI "chém gió" (hallucination) về các thư viện/công nghệ mới trong chương trình.
- **Hành động đề xuất:** Mời Giảng viên tham gia duyệt System Prompt và thẩm định bộ Ground Truth Benchmark (bộ 30 câu hỏi lab điển hình); thiết lập nguyên tắc AI không viết code trọn gói hộ học viên.

---

### 4. Đội ngũ Lab Coach / Trợ giảng Thực hành
- **Mô tả cụ thể:** Các kỹ sư trợ giảng trực tiếp kèm cặp học viên làm bài lab, chữa bài tập lớn (Capstone Project) và giải đáp thắc mắc kỹ thuật.
- **Influence:** **Trung bình** (Người hướng dẫn thao tác trực tiếp, ảnh hưởng lớn đến thói quen sử dụng công cụ của học viên).
- **Interest:** **Rất Cao** (Thường xuyên bị quá tải tin nhắn hỏi sửa lỗi môi trường (CUDA, Docker, thư viện conflict), syntax bug vào khung giờ 22h - 2h sáng).
- **Vùng phân loại:** **Supporter**
- **Stance:** 🟢 **Ủng hộ nhiệt tình** (AI Tutor là "tuyến phòng thủ đầu tiên" giải quyết 70-80% câu hỏi cơ bản về lỗi môi trường và cú pháp).
- **Kỳ vọng & Rủi ro:** 
  - *Kỳ vọng:* AI Tutor lọc bớt các câu hỏi lặp đi lặp lại để Lab Coach tập trung review kiến trúc và logic bài Capstone Project.
  - *Rủi ro:* Khi AI trả lời sai, Lab Coach mất thêm thời gian giải thích lại từ đầu.
- **Hành động đề xuất:** Tích hợp nút "Chuyển tiếp cho Lab Coach" (Escalate to Human Coach) kèm theo toàn bộ đoạn chat tóm tắt khi AI không giải quyết được vấn đề sau 3 lượt trao đổi.

---

### 5. Học viên "AI Thực Chiến" (End-Users)
- **Mô tả cụ thể:** Sinh viên năm cuối ngành CNTT/Toán-Tin hoặc người mới tốt nghiệp có áp lực học nhanh để làm đồ án tốt nghiệp và phỏng vấn việc làm; thường tự thực hành lab ngoài giờ hành chính.
- **Influence:** **Thấp - Trung bình** (Người sử dụng trực tiếp, quyết định mức độ tương tác và sự hài lòng của tính năng).
- **Interest:** **Rất Cao** (Cần người hướng dẫn tức thì 24/7 khi bị nghẽn (stuck) ở các bước cài đặt môi trường, cấu hình pipeline hoặc hiểu luồng thuật toán).
- **Vùng phân loại:** **Supporter**
- **Stance:** 🟢 **Ủng hộ** (Muốn được hỏi thoải mái mọi câu hỏi từ cơ bản đến nâng cao mà không ngại hay sợ bị phán xét).
- **Kỳ vọng & Rủi ro:** 
  - *Kỳ vọng:* Phản hồi nhanh, hướng dẫn từng bước (step-by-step), giải thích tường tận log lỗi và gợi ý cách debug thực tế.
  - *Rủi ro:* Ức chế nếu bot trả lời vòng vo, lý thuyết suông, không bám sát đề bài lab của chương trình Vlearn.
- **Hành động đề xuất:** Tối ưu hóa giao diện nhập code/log lỗi thuận tiện; cơ chế feedback tức thì 1-click (👍 Giải thích dễ hiểu / 👎 Chưa đúng trọng tâm) để AI tự điều chỉnh.

---

### 6. Đội ngũ Kỹ thuật & Hạ tầng Nền tảng Vlearn (LMS Platform Team)
- **Mô tả cụ thể:** Kỹ sư phụ trách hạ tầng LMS, quản lý tài khoản học viên, tích hợp API/Webhook và cơ sở dữ liệu khóa học "AI Thực Chiến".
- **Influence:** **Cao** (Có quyền cấp quyền truy cập dữ liệu đề lab, token auth và phê duyệt bảo mật tích hợp).
- **Interest:** **Thấp - Trung bình** (Quan tâm đến độ ổn định, không làm sập LMS và không làm lộ đề/dữ liệu độc quyền).
- **Vùng phân loại:** **Blocker / Manage Closely**
- **Stance:** 🟡 **Trung lập** (Ưu tiên an toàn hệ thống và bảo mật).
- **Kỳ vọng & Rủi ro:** Yêu cầu API chuẩn xác, không gây nghẽn database, đảm bảo dữ liệu trao đổi tuân thủ bảo mật nội bộ.
- **Hành động đề xuất:** Cung cấp tài liệu tích hợp API rõ ràng, cơ chế Rate Limiting, cam kết lưu trữ dữ liệu an toàn.

---

### 7. Nhà tuyển dụng / Đối tác Doanh nghiệp nhận học viên "AI Thực Chiến"
- **Mô tả cụ thể:** Các công ty công nghệ, AI startups đang tìm kiếm nhân sự thực chiến tốt nghiệp từ chương trình Vlearn.
- **Influence:** **Trung bình** (Quyết định uy tín thương hiệu và giá trị thực tế của chương trình).
- **Interest:** **Trung bình** (Quan tâm học viên có năng lực tư duy giải quyết vấn đề độc lập hay chỉ ỷ lại vào công cụ AI có sẵn).
- **Vùng phân loại:** **Bystander / Keep Informed**
- **Stance:** 🟡 **Trung lập**
- **Kỳ vọng & Rủi ro:** Kỳ vọng học viên tốt nghiệp thành thạo kỹ năng sử dụng AI như một trợ thủ đắc lực (AI-augmented Engineer) nhưng vẫn nắm vững bản chất thuật toán.
- **Hành động đề xuất:** Định vị AI Tutor là công cụ rèn luyện kỹ năng prompt & debug chuẩn mực theo quy trình phát triển phần mềm hiện đại.

---

### 8. Core Team dự án (Nguyễn Việt Hải, Nguyễn Hoàng Minh, Trịnh Hải Đăng)
- **Mô tả cụ thể:** 
  - *Nguyễn Việt Hải (Product Lead):* Định hình trải nghiệm học tập, luồng nghiệp vụ sư phạm AI Tutor và điều phối dự án.
  - *Nguyễn Hoàng Minh (Tech Lead):* Xây dựng kiến trúc hệ thống RAG, tối ưu hóa latency và tích hợp giao diện.
  - *Trịnh Hải Đăng (Data & Prompt Engineer):* Thu thập giáo trình/đề lab "AI Thực Chiến", tinh chỉnh Prompt phân vai và đo lường độ chính xác.
- **Influence:** **Rất Cao** (Trực tiếp hiện thực hóa ý tưởng và định hình sản phẩm).
- **Interest:** **Rất Cao** (Đạt kết quả xuất sắc cho Gate 0 và hoàn thiện giải pháp AI Tutor thực tế).
- **Vùng phân loại:** **Champion**
- **Stance:** 🟢 **Ủng hộ 100%**
- **Hành động đề xuất:** Triển khai theo dõi sát mục tiêu Gate 0, thử nghiệm sớm trên các bài lab thực tế của chương trình.

---

## III. Bảng Tổng Hợp Ma Trận Stakeholder (Influence × Interest × Stance)

| STT | Stakeholder cụ thể | Influence | Interest | Phân loại Vùng | Stance (Thái độ) | Chiến lược tương tác chính |
| :--- | :--- | :---: | :---: | :---: | :---: | :--- |
| **1** | **Giám đốc Chương trình "AI Thực Chiến"** | **Rất Cao** | **Cao** | **Champion** | 🟡 Trung lập | Báo cáo bài toán ROI, cam kết kiểm soát chi phí token & an toàn dữ liệu |
| **2** | **Người phụ trách Đào tạo (Academic Coordinator)** | **Trung bình - Cao** | **Cao** | **Champion / Supporter** | 🟢 Ủng hộ | Cung cấp Weekly Learning Analytics (chủ đề học viên hay vướng nhất) |
| **3** | **Giảng viên Chuyên môn (Core Instructors)** | **Cao** | **Trung bình** | **Manage Closely** | 🔴 E ngại / Chưa ủng hộ | Mời thẩm định Prompt Socratic (gợi mở tư duy, không đưa sẵn code) |
| **4** | **Đội ngũ Lab Coach / Trợ giảng Thực hành** | **Trung bình** | **Rất Cao** | **Supporter** | 🟢 Ủng hộ nhiệt tình | Giảm tải câu hỏi lặp lại; tích hợp luồng Escalate câu hỏi khó lên Coach |
| **5** | **Học viên sắp/đã ra trường (End-Users)** | **Thấp - TB** | **Rất Cao** | **Supporter** | 🟢 Ủng hộ | Hỗ trợ gỡ kẹt lab 24/7 từng bước; thu thập phản hồi 1-click 👍/👎 |
| **6** | **Kỹ thuật & Hạ tầng LMS Vlearn** | **Cao** | **Thấp - TB** | **Blocker / Manage Closely** | 🟡 Trung lập | Cung cấp API spec chuẩn, đảm bảo Rate Limit và an toàn bảo mật Auth |
| **7** | **Nhà tuyển dụng / Đối tác Doanh nghiệp** | **Trung bình** | **Trung bình** | **Bystander** | 🟡 Trung lập | Định hướng xây dựng năng lực tư duy giải quyết vấn đề với AI |
| **8** | **Core Team 333 (Hải, Minh, Đăng)** | **Rất Cao** | **Rất Cao** | **Champion** | 🟢 Ủng hộ 100% | Phân công RACI chặt chẽ, tối ưu hóa Prompt và kiến trúc RAG |

---
