# Phase 4. Team Health & Competency — Phần Cá Nhân

**Họ tên:** Nguyễn Việt Hải
**MSSV:** 2A202601656
**Nhóm:** 333
**Case:** A. AI Tutor, Diagnostic Refresher (VLearn Codelabs)
**Bước:** 1. Cá nhân — Tự chấm Team Health (5 phút)

> Đây là bản tự chấm cá nhân của em. Điểm số không phải để so sánh mà để buộc em nói thật — một điểm cao mà không giải thích được là bằng chứng của gì thì không có giá trị bằng một điểm thấp kèm lý do cụ thể.

---

## 1. Bảng Tự Chấm Team Health

| Khía cạnh | Điểm (1–5) | Căn cứ chấm |
|---|:---:|---|
| **Chất lượng AI** | **3** | Prototype RAG đã có, Socratic flow đã thiết kế, nhưng chưa có Golden Dataset để đo Hallucination Rate và Citation Precision trên dữ liệu thực tế. Chưa có một buổi kiểm thử nào với học viên thật. Điểm 3 vì có nền nhưng chưa đo được. |
| **Tiến độ** | **3** | Ba file phân tích cá nhân đã xong, bản thống nhất đã gộp, Pitch và RACI đã có. Nhưng chưa có dòng code chạy được trong tay học viên, chưa có cuộc gặp nào với LC-01 được xác nhận. Đang đúng hướng nhưng chưa có artifact kỹ thuật nào bàn giao được. |
| **Tinh thần team** | **4** | Ba người phân công rõ, không có thành viên im lặng, bản thống nhất phản ánh đúng góc nhìn của từng người chứ không phải một người viết hộ cả nhóm. Điểm không phải 5 vì chưa có thời điểm nào team thật sự bất đồng và xử lý được bất đồng đó — chưa biết team sẽ phối hợp thế nào khi có áp lực thật. |
| **Tốc độ ra sản phẩm** | **2** | Hiện tại từ ý tưởng đến thứ học viên thực sự chạm vào được là khoảng cách còn rất lớn. Chưa có prototype nào học viên mở ra dùng được, kể cả trong môi trường sandbox. Điểm 2 vì biết mình đang chậm — chưa có thứ gì để thử là tín hiệu cảnh báo rõ nhất ở giai đoạn này. |

**Tổng điểm trung bình: 3.0 / 5**

---

## 2. Chỗ Em Lo Nhất

**Tốc độ ra sản phẩm là khía cạnh em lo nhất**, không phải vì điểm thấp nhất mà vì nó là điều duy nhất mà team không thể bù bằng phân tích thêm hay tài liệu thêm.

Hiện tại team đang có rất nhiều thứ trên giấy — bản đồ stakeholder, pitch, RACI, kiến trúc RAG — nhưng chưa có thứ gì học viên chạm vào được. Nếu team tiếp tục như vậy thêm 1–2 tuần mà vẫn chưa có prototype để LC-01 nhìn vào, thì mọi cuộc thuyết phục đều dựa trên chữ, không dựa trên thứ thật.

Rủi ro cụ thể: khi xin gặp LC-01, nếu chị hỏi *"Cho tôi xem thử nó hoạt động thế nào"* mà nhóm không có gì để chạy, cuộc gặp mất rất nhiều uy tín.

---

## 3. Chỗ Em Thấy Tốt Nhất — Và Vì Sao Không Dám Cho Điểm Cao Hơn

**Tinh thần team là điểm cao nhất (4/5)**. Ba người phân công rõ, không có ai biến mất, bản thống nhất thật sự phản ánh đủ ba góc nhìn khác nhau — góc data (Hải), góc sư phạm/scope (Minh), góc kỹ thuật (Đăng).

Nhưng em không cho 5 vì một lý do cụ thể: **chưa có bất đồng thật sự nào xảy ra và được xử lý**. Khi mọi người đồng ý với nhau quá dễ, có thể là vì mọi người thật sự cùng hướng, hoặc có thể là vì chưa có đủ áp lực để bất đồng lộ ra. Em chưa biết cái nào đúng với team 333.

---

## 4. Tự Đặt Vị Trí Theo Competency Framework

| Mức | Mô tả trong slide | Tự đánh giá |
|---|---|---|
| **L1 — AI Literate** | Hiểu AI là gì, biết dùng tool AI trong công việc hàng ngày | ✅ Đạt rõ ràng |
| **L2 — AI Practitioner** | Có thể thiết kế luồng nghiệp vụ có AI, biết đặt prompt, đánh giá output, hiểu giới hạn của model | ✅ Đang ở mức này — phần thiết kế Socratic Prompt, định nghĩa Verification Gate, và viết test case từ phỏng vấn đều thuộc L2 |
| **L3 — AI Builder** | Xây hệ thống AI end-to-end: RAG, fine-tuning, Evals pipeline, deploy, monitor | ⚠️ Chưa đến — em có thể đọc hiểu kiến trúc RAG 2 tầng mà Đăng thiết kế, nhưng tự xây từ đầu thì chưa đủ |

**Kết luận:** Em hiện ở **L2 vững**, đang tiến về phía L3 nhưng cần thực hành kỹ thuật nhiều hơn để đến được đó.

---

## 5. Năng Lực Cần Nâng Tiếp Theo

**Từ L2 → L3 — cụ thể là:** Tự thiết kế và chạy một Evals pipeline nhỏ trên bộ 25–30 câu hỏi test case thật, không chỉ đọc kết quả từ pipeline của Đăng.

**Lý do:** Ở vai trò Product Lead, nếu em không tự đọc được output của Evals, em sẽ phải phụ thuộc vào Đăng để biết sản phẩm có tốt không. Điều đó có nghĩa là mỗi lần stakeholder hỏi về chất lượng AI, em phải hỏi lại Đăng trước khi trả lời — đó là điểm yếu rõ ràng trong vai trò người đứng ra thuyết phục.

**Hành động cụ thể trong 2 tuần tới:**
- Cùng Đăng chạy thử pipeline Evals trên 10 ca lỗi đầu tiên — không chỉ nhìn, mà tự tay viết ít nhất 5 test case và kiểm tra output
- Đọc tài liệu Ragas hoặc LangSmith (30 phút) để hiểu các metric mình đang dùng đo cái gì và không đo được cái gì

---

## 6. Một Điều Nhóm Phải Nói Thật Với Nhau

Trong bảng RACI ở Trang 2, Minh là A cho công việc Demo/Pilot. Nhưng nếu cuộc gặp với LC-01 không ra kết quả trong tuần này, nhóm cần họp lại và quyết định rõ: **pilot có bị hoãn không, và hoãn đến khi nào?**

Đây là câu hỏi mà team chưa có câu trả lời thành văn bản. Nếu không thống nhất trước, mỗi người sẽ có deadline khác nhau trong đầu mà không ai biết.

---

> **Ghi nhớ khi nhìn lại bản này:** Điểm số không quan trọng bằng lý do đằng sau điểm số. Nếu 2 tuần nữa điểm Tốc độ ra sản phẩm vẫn là 2 mà không có lý do mới, đó là tín hiệu đáng lo hơn là điểm số bản thân nó.
