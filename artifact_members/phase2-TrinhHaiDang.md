# Phase 2: Pitch 'Conclusion First' — Phiên Bản Trịnh Hải Đăng

**Họ và tên:** Trịnh Hải Đăng
**MSSV:** 2A202601602
**Nhóm:** 333
**Vai trò:** Technical Lead & Architecture / Design
**Case:** A. AI Tutor, Diagnostic Refresher (VLearn Codelabs)
**Bước:** Cá nhân — Viết lại Pitch theo cách của bạn (5 phút)

---

## 1. Bản Pitch Của Trịnh Hải Đăng (Góc Nhìn Tech & Reliability)

### 🎯 1. Kết Luận / Đề Xuất (Conclusion First)

> **"Chúng tôi đề xuất tích hợp cơ chế 'Diagnostic Refresher & Verification Gate' trực tiếp vào giao diện Codelabs của VLearn nhằm tự động chẩn đoán lỗi môi trường máy và xác thực câu hỏi của học viên với tài liệu lab chuẩn trước khi chuyển tiếp cho Coach/TA."**

### 💡 2. Ba Lý Do Chính (Key Reasons)

1. **Triệt tiêu hoàn toàn rủi ro Ảo giác (Hallucination):** Hệ thống chỉ trích xuất giải pháp trực tiếp từ tài liệu Markdown của môn học đã qua kiểm duyệt (kèm link trích dẫn chính xác dòng code), ngăn chặn tình trạng học viên dùng ChatGPT ngoài nhận về code sai phiên bản thư viện.
2. **Giải phóng 50% thời gian nghẽn đầu giờ cho Lab Coach:** Tự động chẩn đoán và khắc phục 65% lỗi cài đặt môi trường lặp lại trong 30 phút đầu buổi lab.
3. **Tối ưu hóa hiệu năng & Chi phí hạ tầng:** Kiến trúc 2 tầng (Semantic Cache + Small LLM Router) xử lý 70% query tại chỗ với chi phí dưới $0.02/học viên và độ trễ p95 phản hồi $\le 1.2s$.

### 📊 3. Bằng Chứng & Dữ Liệu Thực Chứng (Evidence)

- **Dữ liệu phỏng vấn Chặng 2:** Học viên Đức và Đạt xác nhận từng mất hơn 45 phút mò mẫm vô ích vì AI ngoài hướng dẫn cài package bị deprecate.
- **Dữ liệu phỏng vấn Coach LC-01:** Coach thừa nhận 30 phút đầu buổi lab thường xuyên bị quá tải vì hơn 10 học viên cùng kẹt bước thiết lập môi trường.
- **Benchmark Prototype nội bộ:** Đạt độ chính xác chẩn đoán 88% trên 25 ca lỗi thực tế, phản hồi trung bình trong 1.2 giây.

### 🤝 4. Đề Nghị Hành Động Nhỏ (Small Ask)

> **"Chúng tôi xin phép LC-01 và Platform Lead 10 phút vào thứ Năm này để chạy thử bản demo Sandbox 1-click chẩn đoán lỗi với 5 học viên thực tế, hoàn toàn không làm gián đoạn lịch học hay ảnh hưởng tới hệ thống live của VLearn."**

---

## 2. Phản Biện Kỹ Thuật Dự Kiến & Cách Trịnh Hải Đăng Xử Lý

- **Phản biện từ Platform Lead & Coach:** *"Nếu AI đưa ra câu lệnh terminal sai làm hỏng môi trường máy hoặc tạo thói quen học viên lười đọc tài liệu thì sao?"*
- **Cách xử lý của Đăng:**
1. **Deterministic Guardrails:** Giới hạn không gian sinh của LLM trong phạm vi tài liệu lab (Grounding 100%).
  2. **Confidence Threshold 85%:** Nếu điểm tự tin dưới 85%, AI từ chối suy đoán và tự động điền sẵn mẫu Ticket lỗi chuẩn gửi Coach/TA.
  3. **Socratic Tutoring:** Chỉ gợi ý các bước kiểm tra (debugging steps) thay vì đưa toàn bộ mã nguồn hoàn chỉnh.