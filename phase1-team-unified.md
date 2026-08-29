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

---

# Trang 2 — Pitch & RACI (Bản Thống Nhất Team 333)

---

## Bước 1 — Chọn Stakeholder & Viết Pitch Nháp (Team — 10')

**Stakeholder team chọn để pitch:** **S1 — LC-01, Lab Coach**

*Lý do chọn:* Đây là stakeholder nguy hiểm nhất trong bản đồ — nằm ở vùng Champion (Influence Cao × Interest Cao) nhưng stance thực tế là Chưa ủng hộ. Nếu không xử lý được chỗ này thì nhóm không có môi trường thử nghiệm thật, và LC-01 cũng là người duy nhất có thể chỉ ra nhóm learner im lặng mà team còn thiếu dữ liệu.

---

### Pitch Nháp Của Team (Tối đa nửa trang)

**Kết luận:** Nhóm muốn xin LC-01 mười phút để hỏi một câu: cái gì sẽ khiến chị thấy công cụ này làm chị nhẹ đi chứ không nặng thêm?

**Lý do — Vì sao LC-01 nên quan tâm:**

1. Chị đang chọn ít can thiệp để học viên tự rèn — đó là quyết định sư phạm của chị. Nhưng phần câu hỏi không được trả lời không biến mất, nó đang chảy ra ngoài theo các kênh chị không kiểm soát được.
2. Học viên đang đi tiếp trên câu trả lời mà chính họ không chắc đúng — điều này không phải phỏng đoán mà là lời học viên nói thẳng với nhóm khi được phỏng vấn riêng.
3. Thứ nhóm em làm không phải để trả lời thay chị — nó dừng sớm hơn: giúp học viên nói được chỗ kẹt của mình trước khi câu hỏi thoát ra ngoài hoặc bị bỏ lại.

**Bằng chứng — 3 nguồn phỏng vấn thật:**

- *Từ LC-01:* Mỗi câu hỏi lạ mất 30 giây đến 1 phút chỉ để hiểu học viên cần gì, có lúc hiểu sai ý hỏi, có lúc trả lời không kịp. Phần bị hỏi nhiều nhất là setup môi trường.
- *Từ học viên thuộc nhóm im lặng:* Ngại giơ tay sợ làm chậm mạch bài, chuyển sang hỏi bạn bè, câu trả lời đúng khoảng 80%, vẫn phải đi tiếp dù không chắc.
- *Từ học viên đã dùng AI Tutor cũ:* Thấy không thoả đáng, chụp slide đưa lên ChatGPT bên ngoài, nói nguyên văn *"buộc phải tin thôi"* và *"ngại hỏi lab coach nên bỏ qua"*.

Ba người, ba đường — cùng dẫn tới một chỗ: câu hỏi không được trả lời bằng nguồn kiểm chứng.

**Small ask — Đề nghị hành động nhỏ, cụ thể:**

> Xin LC-01 **10 phút trong tuần này** để trả lời đúng một câu: *"Cái gì sẽ khiến chị thấy công cụ này làm chị nhẹ đi chứ không nặng thêm?"* Nếu câu trả lời cho thấy hướng dùng được, nhóm mới xin thêm: nhờ chị chỉ 2 learner ít đặt câu hỏi nhất lớp để phỏng vấn mở rộng mẫu (10 phút).

---

## Bước 2 — Chuẩn Bị Phản Biện (Team — 5')

**Phản biện có khả năng xảy ra nhất:**

> *"AI đưa ra câu hỏi kẹt sai, học viên copy-paste mù quáng rồi hỏng cả môi trường — lúc đó tôi phải đi gỡ từng máy một."*

Đây là nỗi sợ thật nhất và cụ thể nhất của LC-01 — chị đã nói điều này trong buổi phỏng vấn.

**Câu trả lời dựa trên bằng chứng và hành động giảm rủi ro:**

| Rủi ro | Bằng chứng / Hành động giảm rủi ro |
|---|---|
| AI gợi ý lệnh terminal sai, học viên làm theo, máy hỏng | Hệ thống **không bao giờ đưa lệnh thực thi sẵn** — chỉ gợi ý bước kiểm tra (debugging step) kèm link trích dẫn dòng trong tài liệu lab gốc để học viên đối chiếu. |
| AI trả lời sai ngoài phạm vi tài liệu | **Confidence Threshold 85%:** Nếu điểm tự tin dưới 85%, AI từ chối suy đoán và tự động tạo Ticket báo Coach với đầy đủ context (log lỗi + đoạn chat). |
| Học viên lười đọc tài liệu, ỷ vào AI | **Socratic flow:** AI chỉ đặt câu hỏi gợi mở *"Em đã thử bước nào rồi?"* và *"Trong tài liệu Lab 3 dòng 47 viết gì về bước này?"* — không đưa câu trả lời trực tiếp. |
| Khó đo tác động thật | Team cam kết chạy thử trong sandbox, ghi nhận toàn bộ log trước khi xin chạy trong lớp thật. |

> **Tóm lại:** Nếu công cụ không chắc, nó im. Nếu học viên cần thêm, nó escalate lên chị kèm đầy đủ thông tin để chị không mất thêm thời gian hỏi lại từ đầu.

---

## Bước 3 — Pitch Cá Nhân (Mỗi Thành Viên — 5')

*Mỗi thành viên tự viết lại để kiểm tra xem có thật sự hiểu thông điệp hay chỉ gật đầu với bản nháp team.*

### Nguyễn Việt Hải

**Kết luận:** Xin chị mười phút để hỏi một câu — không xin phê duyệt gì cả.

**Lý do:** Chị đang chọn ít can thiệp để học viên tự rèn — đó là quyết định sư phạm của chị. Nhưng phần câu hỏi không kịp trả lời không biến mất: nó đang chảy ra ChatGPT bên ngoài và học viên nhận về thứ họ không chắc đúng rồi đi tiếp. Thứ nhóm em muốn làm không phải trả lời thay chị — nó dừng sớm hơn, giúp học viên nói được chỗ mình kẹt là gì trước khi câu hỏi thoát ra ngoài.

**Bằng chứng:** Ba buổi phỏng vấn riêng: từ chính chị (có lúc trả lời không kịp, mỗi câu lạ mất 30–60 giây chỉ để hiểu ý), từ học viên ngại giơ tay (hỏi bạn bè, đúng khoảng 80%, vẫn đi tiếp), từ học viên dùng AI Tutor cũ (*"buộc phải tin thôi"*).

**Small ask:** Mười phút trong tuần này để chị trả lời một câu: *"Cái gì sẽ khiến chị thấy công cụ này làm chị nhẹ đi chứ không nặng thêm?"*

---

### Nguyễn Hoàng Minh

**Kết luận:** Xin mười phút của chị để bàn về việc nhóm làm một thứ giúp học viên **gọi tên đúng chỗ mình đang kẹt trước khi hỏi chị**, chứ không phải một thứ trả lời thay chị.

**Lý do:** Chỗ tốn thời gian của chị nằm ở khâu hiểu câu hỏi, không phải khâu trả lời — chính chị nói mỗi câu hỏi lạ mất từ 30 giây đến 1 phút chỉ để hiểu bạn đó đang cần gì. Nhóm muốn động vào đúng khâu đó. Công cụ không lấy mất phần tự chủ chị đang giữ cho học viên — nó dừng ở chỗ giúp diễn đạt, phần còn lại vẫn là việc của các bạn và của chị. Phần câu hỏi chị không kịp trả lời không biến mất — nó đang chảy ra AI bên ngoài mà không ai kiểm chứng.

**Bằng chứng:** Ba nguồn phỏng vấn thật: từ chị (30–60 giây/câu lạ, có lúc hiểu sai, có lúc không kịp trả lời), từ học viên ngại giơ tay (hỏi bạn bè, 80% đúng, biết vậy vẫn đi tiếp), từ học viên dùng AI cũ (*"buộc phải tin thôi"*).

**Small ask:** Mười phút, một câu duy nhất: *"Cái gì sẽ khiến chị thấy công cụ này làm chị nhẹ đi chứ không nặng thêm?"* — nếu câu trả lời cho thấy hướng dùng được, nhóm xin thêm nhờ chị chỉ 2 learner ít hỏi nhất lớp.

---

### Trịnh Hải Đăng

**Kết luận:** Đề xuất tích hợp cơ chế Diagnostic Refresher & Verification Gate vào Codelabs VLearn để chẩn đoán lỗi môi trường máy và xác thực câu hỏi với tài liệu lab chuẩn trước khi chuyển tiếp cho Coach/TA.

**Lý do:** (1) Triệt tiêu hallucination — hệ thống chỉ trích xuất từ tài liệu Markdown đã kiểm duyệt, kèm link trích dẫn chính xác. (2) Giải phóng thời gian nghẽn đầu giờ cho Coach — tự động xử lý lỗi cài đặt môi trường lặp lại. (3) Kiến trúc 2 tầng (Semantic Cache + Small LLM Router) kiểm soát được chi phí và latency.

**Bằng chứng:** Phỏng vấn Chặng 2 xác nhận học viên mất hơn 45 phút vì AI ngoài gợi ý package deprecated. Coach thừa nhận 30 phút đầu buổi lab thường xuyên quá tải.

**Small ask:** Xin LC-01 và Platform Lead 10 phút vào thứ Năm này để chạy demo Sandbox 1-click chẩn đoán lỗi với 5 học viên thực tế — không làm gián đoạn lịch học, không ảnh hưởng hệ thống live.

---

## Bước 4 — RACI Matrix (Team — 10')

**Công việc quan trọng của dự án trong 1–2 tháng tới:**

| Công việc | Hải (Product Lead) | Minh (Scope Owner) | Đăng (Tech Lead) | LC-01 (Lab Coach) | Platform Lead VLearn | Mentor |
|---|:---:|:---:|:---:|:---:|:---:|:---:|
| **1. Xác định & khóa scope use case** | **A** | **R** | C | C | I | C |
| **2. Thu thập dữ liệu lab & log lỗi thực tế** | C | I | **A / R** | C | I | I |
| **3. Xây dựng RAG Pipeline & MVP kỹ thuật** | I | C | **A / R** | I | C | I |
| **4. Thiết kế Prompt, Evals & kiểm thử chất lượng** | R | C | **A** | C | I | C |
| **5. Demo / Pilot trong buổi lab thực tế** | R | **A** | R | C | C | I |
| **6. Quyết định tích hợp chính thức vào VLearn** | R | C | R | C | **A** | C |

**Chú thích:**
- **R — Responsible:** Người trực tiếp thực hiện công việc
- **A — Accountable:** Người chịu trách nhiệm cuối cùng nếu công việc không xong (mỗi hàng chỉ có **1 A**)
- **C — Consulted:** Cần hỏi ý kiến trước khi quyết định
- **I — Informed:** Cần được thông báo kết quả

**Ghi chú từng công việc:**

1. **Xác định & khóa scope use case** — Hải là A vì scope ảnh hưởng đến toàn bộ milestone; Minh là R vì Minh có dữ liệu phỏng vấn Coach trực tiếp nhất. LC-01 và Mentor được C để tránh scope creep sau.

2. **Thu thập dữ liệu lab & log lỗi** — Đăng là A+R vì dữ liệu là đầu vào của pipeline kỹ thuật; LC-01 được C để xin quyền truy cập log lỗi thực tế từ buổi lab.

3. **Xây dựng RAG Pipeline & MVP** — Đăng là A+R toàn bộ. Platform Lead được C sớm để tránh xung đột tích hợp sau khi đã build xong.

4. **Thiết kế Prompt, Evals & kiểm thử** — Đăng là A (chịu trách nhiệm chất lượng kỹ thuật cuối); Hải là R (viết test case từ dữ liệu phỏng vấn); LC-01 và Mentor được C để thẩm định tính đúng sư phạm.

5. **Demo / Pilot trong buổi lab thực tế** — Minh là A vì Minh là đầu mối với LC-01; Hải và Đăng đều R (chuẩn bị kịch bản demo và hỗ trợ kỹ thuật).

6. **Quyết định tích hợp chính thức** — Platform Lead là A duy nhất vì quyền này thuộc về nền tảng VLearn. Team chỉ có thể cung cấp bằng chứng và xin; không ai trong team có thể là A cho công việc này.

---

> **Quy tắc kiểm tra RACI của team:**
> - Mỗi hàng có đúng **1 A** — nếu có 2 A, cần quyết định ai là người chịu trách nhiệm cuối.
> - Không có hàng nào toàn C/I mà không có R — ai đó phải trực tiếp làm.
> - LC-01 và Platform Lead chỉ ở C hoặc I — họ là stakeholder ngoài team, không là người thực hiện.

---

# Trang 3 — AI Team Design (Bản Thống Nhất Team 333)

---

## Bước 1 — Chọn Team Architecture (5')

**Team 333 chọn: Embedded**

**Lý do (1–2 câu):**

Team hiện có 3 người, đang ở giai đoạn MVP cần đi nhanh từ prototype đến pilot trong một môi trường duy nhất (VLearn Codelabs). Ở quy mô này, nhúng toàn bộ năng lực AI trực tiếp vào squad sản phẩm là lựa chọn duy nhất thực tế — không cần và không đủ người để duy trì một hub AI trung tâm riêng biệt.

> **Kiểm tra:** Mô hình Centralized đòi hỏi đội AI trung tâm phục vụ nhiều team/sản phẩm — không phù hợp khi team chỉ đang xây một tính năng. Mô hình Hybrid phù hợp hơn khi có nhiều squad cần dùng chung cơ sở hạ tầng AI — chưa đến giai đoạn này. Team sẽ cân nhắc chuyển sang Hybrid khi VLearn muốn nhân rộng AI Tutor sang các môn học khác hoặc track khác.

---

## Bước 2 — Xác Định Core Roles & Capability Gap (8')

### 2.1 Sơ Đồ Vai Trò Hiện Tại (Ai đang làm gì)

| Vai trò | Người đảm nhận | Mô tả thực tế |
|---|---|---|
| **AI Product / Squad Lead** | Nguyễn Việt Hải | Định hình trải nghiệm học tập, thiết kế luồng nghiệp vụ sư phạm, điều phối milestone và stakeholder |
| **AI Engineer / RAG Engineer** | Trịnh Hải Đăng | Xây dựng RAG pipeline, thiết kế Prompt & Verification Gate, đo lường Evals (Hallucination Rate, Citation Precision) |
| **Data / Backend / Scope Owner** | Nguyễn Hoàng Minh | Thu thập dữ liệu phỏng vấn, quản lý scope, đầu mối với LC-01 và vận hành lớp học |
| **Domain Expert (Pedagogy)** | LC-01 — Lab Coach *(Consulted, ngoài team)* | Thẩm định tính đúng sư phạm của Socratic Prompt, cung cấp log lỗi và phản hồi từ buổi lab thật |
| **Platform / Integration** | Platform Lead VLearn *(Consulted, ngoài team)* | Cấp API access, phê duyệt tích hợp Widget vào Codelabs |

### 2.2 Core Roles — Cần Ngay (Must-have để đưa MVP ra pilot)

| Vai trò | Trạng thái | Ai đang cover |
|---|---|---|
| AI Product / Squad Lead | ✅ Có | Hải |
| AI Engineer (RAG + Prompt) | ✅ Có | Đăng |
| Data collector / Scope manager | ✅ Có | Minh |
| Domain Expert (Pedagogy) | ⚠️ Partial — Consulted only | LC-01 (ngoài team, chưa cam kết chính thức) |
| UX / Interface designer | ❌ Thiếu | Chưa có ai |

### 2.3 Extended Roles — Cần Khi Scale (Post-pilot)

| Vai trò | Vì sao cần khi scale |
|---|---|
| MLOps / Evals specialist | Khi cần tự động hóa pipeline đánh giá chất lượng phản hồi AI theo thời gian thực trên toàn bộ lớp học |
| Forward Deployed Engineer | Khi VLearn muốn tích hợp AI Tutor sang các track/môn học khác, cần người trực tiếp làm việc với team kỹ thuật VLearn |
| Legal / Data Compliance | Khi xử lý log lỗi và chat history học viên ở quy mô lớn — cần tuân thủ quy định bảo vệ dữ liệu người dùng |
| AI Ethics / Guardrails reviewer | Khi scale sang nhiều môn học — cần người định kỳ audit Prompt và output để tránh bias sư phạm |
| Curriculum domain specialist | Khi mở rộng sang môn học khác ngoài Lab setup (ví dụ: Data Science, MLOps) — cần chuyên gia từng môn |

### 2.4 Capability Gap — Tóm Tắt

| Gap | Mức độ cấp thiết | Giai đoạn cần |
|---|---|---|
| **UX / Product design** | 🔴 Cấp thiết — ảnh hưởng ngay đến usability của pilot | Trước pilot đầu tiên |
| **Domain expert cam kết chính thức (LC-01 hoặc Giảng viên)** | 🔴 Cấp thiết — không có người thẩm định sư phạm thì không dám release | Trước khi hoàn thiện Prompt |
| **MLOps / Automated Evals pipeline** | 🟡 Quan trọng nhưng chưa blocking | Sau MVP, trước khi scale |

---

## Bước 3 — Priority Resourcing (Cách Bổ Sung Năng Lực) (7')

Chọn 3 capability gap quan trọng nhất và phương án bổ sung:

---

### Gap 1: UX / Interface Design

| | |
|---|---|
| **Capability gap** | Không có người thiết kế giao diện — prototype hiện tại là text-only, chưa có luồng UX cụ thể cho học viên dùng trong lúc làm lab |
| **Phương án** | **Partner** — Làm việc với VLearn's design team (nếu có) hoặc nhờ một sinh viên UX/UI trong chương trình "AI Thực Chiến" tham gia với vai trò cộng tác viên có hướng dẫn |
| **Vì sao không Hire / Outsource** | Quá sớm để hire full-time UX ở giai đoạn MVP chỉ 1 tính năng. Outsource freelance UX thường tốn 2–3 tuần lead time và không hiểu đủ context của buổi lab. Partner là đường nhanh nhất để có mockup dùng được. |
| **Khi nào cần** | **Trước pilot đầu tiên** — cần ít nhất 1 màn hình wireframe để học viên và LC-01 có thứ nhìn vào khi demo |

---

### Gap 2: Domain Expert Cam Kết Chính Thức (Pedagogy Reviewer)

| | |
|---|---|
| **Capability gap** | LC-01 và Giảng viên chuyên môn hiện chỉ ở vai Consulted, chưa cam kết chính thức. Nếu không có người thẩm định sư phạm, team không có cơ sở để tuyên bố Socratic Prompt đúng hướng dạy. |
| **Phương án** | **Partner** — Sau cuộc gặp 10 phút xin Small Ask từ LC-01, nếu phản hồi tích cực, mời chị tham gia với vai trò **Pedagogy Advisor** (không cần hợp đồng, chỉ cần cam kết 30 phút/tuần review output mẫu) |
| **Vì sao không Hire / Outsource** | Không cần hire full-time — cần ý kiến chuyên môn định kỳ, không cần người làm việc 8 tiếng/ngày. Outsource chuyên gia giáo dục bên ngoài sẽ mất thời gian onboard context VLearn Codelabs. LC-01 đã có đủ context, chỉ cần chuyển từ Consulted thành cam kết nhẹ. |
| **Khi nào cần** | **Ngay tuần này** — trước khi hoàn thiện System Prompt và bộ Golden Dataset kiểm thử |

---

### Gap 3: MLOps / Automated Evals Pipeline

| | |
|---|---|
| **Capability gap** | Đăng đang tự xây Evals pipeline thủ công. Khi số lượng câu hỏi và log tăng lên sau pilot, cần hệ thống tự động đánh giá chất lượng phản hồi AI định kỳ (Hallucination Rate, Citation Recall, User Satisfaction score). |
| **Phương án** | **Outsource (công cụ/platform)** — Dùng công cụ Evals có sẵn (ví dụ: LangSmith, Ragas, hoặc Evidently AI) thay vì tự xây từ đầu. Không cần hire MLOps engineer ở giai đoạn này. |
| **Vì sao không Hire / Partner** | Hire MLOps engineer ở giai đoạn 3 người là quá sớm và quá tốn. Partner với đơn vị MLOps bên ngoài thêm overhead quản lý. Dùng platform công cụ có sẵn là đủ cho quy mô pilot. |
| **Khi nào cần** | **Sau MVP, trước khi scale sang >50 học viên** — khi lượng interaction đủ lớn để cần dashboard theo dõi chất lượng tự động |

---

## Bước 4 — Chốt Squad Goal (5')

> **"Team/Squad 333 sở hữu toàn bộ pipeline AI Tutor — Diagnostic Refresher và chịu trách nhiệm đưa trải nghiệm hỏi đáp trong buổi lab của học viên VLearn từ hiện trạng *'kẹt mà không có nguồn kiểm chứng, phải đi hỏi AI bên ngoài rồi buộc phải tin'* đến *'có câu trả lời được xác thực từ tài liệu lab trong vòng 2 giây — trước khi cần escalate lên Coach.'"***

---

### Giải thích từng phần của Squad Goal

| Phần | Nội dung | Vì sao chọn cách diễn đạt này |
|---|---|---|
| **Sở hữu gì** | Toàn bộ pipeline AI Tutor — Diagnostic Refresher | Team chịu trách nhiệm đầu-cuối: từ Prompt design, RAG pipeline, đến giao diện học viên dùng — không phải chỉ một phần kỹ thuật |
| **Từ hiện trạng** | Kẹt mà không có nguồn kiểm chứng | Lấy nguyên lời học viên nói trong phỏng vấn: *"buộc phải tin thôi"* — đây là pain thật, không phải pain team tự nghĩ ra |
| **Đến đích** | Có câu trả lời xác thực trong 2 giây, trước khi cần escalate lên Coach | Số 2 giây là cam kết kỹ thuật (p95 latency); "trước khi cần escalate" nhắc nhở team rằng Coach vẫn là tuyến cuối — AI chỉ là tuyến đầu |

---

> **Lưu ý:** Squad Goal này được viết cho giai đoạn Pilot — sẽ được cập nhật lại khi team đủ dữ liệu để mở rộng sang các môn học hoặc track khác trong chương trình "AI Thực Chiến".
