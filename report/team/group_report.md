# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: Nhóm 145
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu):
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 |Nguyễn Văn Hùng |Khi nhận nhiều cảnh báo mạng trong thời gian ngắn, tôi muốn xác định các cảnh báo tương tự và phân loại mức độ ưu tiên để giảm thời gian xử lý và hạn chế bỏ sót cảnh báo quan trọng. |Nhân viên giám sát mạng |Kiểm tra đối chiếu các cảnh báo tương tự, tùy thuộc vào số lượng alert mà thời gian khác nhau |Thắng - đã có nhiều giải pháp tương tự |
| 2 |Nguyễn Văn Hùng |Khi cần chuyển một báo cáo dài thành slide thuyết trình, tôi muốn nhanh chóng chọn lọc và tóm tắt các nội dung quan trọng để tiết kiệm thời gian chuẩn bị mà vẫn đảm bảo đầy đủ ý chính. |	Người thường xuyên thuyết trình |Xác định luận điểm quan trọng và tóm tắt nội dung, chia nội dung cho mỗi slide, thời gian tốn tùy vào tài liệu báo cáo. |Hiếu: có  nhiều AI đã thực hiện, cần có giải pháp khác biệt|
| 3 |Nguyễn Văn Hùng |Khi tìm kiếm việc làm hoặc thực tập, tôi muốn đối chiếu yêu cầu tuyển dụng với kỹ năng hiện có để xác định vị trí phù hợp và những kỹ năng cần bổ sung. |Sinh viên sắp tốt nghiệp, người tìm việc |Đọc và đối chiếu nhiều JD có cách diễn đạt khác nhau, khoảng 2 phút mỗi bài, và mất nhiều thời gian cho việc tìm kiếm |Trường: cách giải quyết để giúp ứng viên tìm được đúng vị trí mà không bỏ lỡ |
| 4 |Vương Toàn Minh Hiếu |Khi di chuyển qua các trục đường vào giờ cao điểm, tôi muốn biết trước ngã tư hoặc đoạn đường nào đng xảy ra ùn tắc, để chủ động rẽ sang cung đường khác tránh kẹt cứng. |Người tham gia giao thông |Bước 3,4 vì đi vào đường tắc đã mất thời gian và mất thêm thời gian tự tìm đường |Trường: gmaps đã có giải pháp, các vấn đề thực tế gmaps không update được? |
| 5 |Vương Toàn Minh Hiếu |Khi kết thúc một ngày làm việc hoặc học tập, tôi muốn tổng kết các việc đã hoàn thành, vướng mắc gặp phải cùng những kiến thức vừa tiếp thu được các nhiều nguồn, để viết xong báo cáo Daily Standup nhanh chóng mà không bỏ sót kết quả quan trọng. |Sinh viên CNTT, dev |Lục lại lịch sử mất thời gian và phải viết các nội dung thành các mục chi tiết và hợp lý |Thắng: đối tượng rộng, cần giới hạn |
| 6 |Vương Toàn Minh Hiếu |Khi tôi đi khám bệnh định kỳ, tôi muốn nắm rõ quy trình di chuyển giữa các phòng khám, xét nghiệm và thứ tự chờ đến lượt ở từng khâu, để tôi có thể đi khám với chi phí thời gian tối thiểu. |Người bệnh đi khám |Thời gian di chuyển qua các phòng, toà nhà và thời gian xếp hàng rất lâu |Hùng: giống hệ thống tra cứu, chưa rõ ứng dụng AI |
| 7 |Nguyễn Đình Trường |Khi cần tìm một linh kiện điện tử phù hợp với yêu cầu kỹ thuật, tôi muốn so sánh được thông số và khả năng tương thích của nhiều linh kiện, để tránh chọn sai linh kiện và phải thay thế. |Kỹ sư thiết kế phần cứng |Công đoạn đọc datasheet, trích xuất thông số và đối chiếu khả năng tương thích mất khoảng 35–55 phút. Tổng quy trình tìm kiếm và lựa chọn một linh kiện mất khoảng 60–95 phút. | |
| 8 |Nguyễn Đình Trường |	Khi cần viết tài liệu kỹ thuật từ ghi chú hoặc kết quả công việc, tôi muốn trình bày thông tin theo một cấu trúc thống nhất, để giảm công sức biên soạn và hạn chế sai lệch. |Người viết tài liệu kỹ thuật |Bước 3 và 4: Phân loại thông tin và biên soạn tài liệu. Thông tin đầu vào nằm ở nhiều nguồn, không đồng nhất về cách diễn đạt và mức độ chi tiết. Người viết phải tự xác định nội dung nào thuộc mục nào, chuyển ghi chú thành câu văn kỹ thuật và đảm bảo không làm sai lệch ý nghĩa ban đầu. Đây là hai công đoạn có khả năng tiêu tốn nhiều thời gian nhất. | |
| 9 |Nguyễn Đình Trường |Khi gặp lỗi trong quá trình cài đặt thư viện lập trình, tôi muốn kiểm tra nguyên nhân và cách khắc phục theo một quy trình thống nhất, để không phải xử lý lại từ đầu. |	Lập trình viên |Bước 5 và bước 6: Thử phương án khắc phục và kiểm tra lại, mất khoảng 30 phút (chiếm 49,2% tổng thời gian 61 phút). | |
| 10 |Nguyễn Hồng Thắng |AI Homework Assistant |Phụ huynh (người sử dụng chính); học sinh (người thực hiện); giáo viên (người giao bài). |Bước 2–4: phải chuyển đổi giữa nhiều nguồn và tổng hợp thủ công. Bước 5–6: khó xác minh tình trạng thực tế. Giả định ban đầu: 20–40 phút/ngày. | |
| 11 |Nguyễn Hồng Thắng |Tự động lập thông báo tiền điện, nước |Chủ nhà, người quản lý tòa nhà, kế toán và khách thuê. |Bước 2–4: nhập liệu và đối chiếu nhiều nguồn. Bước 5–6: tính toán, kiểm tra và nhập lại dữ liệu. Giả định ban đầu: 5–10 phút/đơn vị thuê, chưa tính xử lý sai lệch. | |
| 12 |Nguyễn Hồng Thắng |Quản lý yêu cầu sửa chữa của khách thuê |Khách thuê (người phản ánh); người quản lý tòa nhà (người tiếp nhận và điều phối); kỹ thuật viên (người xử lý); chủ nhà (người giám sát). |Bước 1–3: thông tin không đầy đủ, phải hỏi lại nhiều lần. Bước 4–5: mất thời gian tìm người xử lý và theo dõi. Giả định ban đầu: 10–20 phút tiếp nhận và điều phối mỗi sự cố, chưa tính thời gian sửa chữa. | |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A. Tổng hợp và xử lý thông tin từ nhiều nguồn |#5 – Daily Standup; #8 – Biên soạn tài liệu kỹ thuật; #10 – AI Homework Assistant |Người dùng phải thu thập, đọc, chọn lọc, phân loại và tổng hợp thông tin từ nhiều nguồn khác nhau để tạo ra một nội dung có cấu trúc. Quá trình này tốn thời gian và có nguy cơ bỏ sót thông tin quan trọng. |
| B. Tra cứu, so sánh và đối chiếu thông tin |#3 – Đối chiếu việc làm với kỹ năng; #7 – So sánh linh kiện điện tử |Người dùng phải tìm kiếm và đối chiếu nhiều nguồn thông tin có cách trình bày khác nhau để đưa ra lựa chọn phù hợp. Việc so sánh thủ công mất thời gian và có thể dẫn đến quyết định sai. |
| C. Giám sát, phát hiện và xử lý vấn đề |#1 – Phân loại cảnh báo mạng; #9 – Khắc phục lỗi cài đặt thư viện; #12 – Quản lý yêu cầu sửa chữa khách thuê |Người dùng gặp khó khăn trong việc nhận diện vấn đề, xác định nguyên nhân hoặc mức độ ưu tiên và theo dõi quá trình xử lý. Có nguy cơ bỏ sót vấn đề hoặc xử lý chậm.|
| D. Tối ưu quy trình và thời gian thực hiện công việc |#2 – Chuyển báo cáo thành slide; #11 – Lập thông báo tiền điện, nước|Người dùng phải thực hiện nhiều công đoạn thủ công, lặp lại để hoàn thành một công việc có đầu ra tương đối chuẩn hóa. Việc này tiêu tốn thời gian và dễ phát sinh sai sót.|
| E. Tìm kiếm và điều hướng theo tình huống thực tế |#4 – Tránh ùn tắc giao thông; #6 – Điều hướng quy trình khám bệnh|Người dùng thiếu thông tin kịp thời về tình trạng thực tế và phương án di chuyển hoặc thứ tự thực hiện phù hợp, dẫn đến thời gian chờ đợi và di chuyển không cần thiết.|

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME:
Giảm thời gian và sai sót trong quá trình
xử lý thông tin, ra quyết định và
thực hiện công việc.

├── Opportunity A:
│   Khó khăn khi thu thập, chọn lọc và
│   tổng hợp thông tin từ nhiều nguồn.
│
├── Opportunity B:
│   Khó khăn khi đối chiếu, phân tích
│   thông tin và đưa ra quyết định.
│
└── Opportunity C:
    Thiếu thông tin kịp thời để theo dõi,
    phối hợp và tối ưu quy trình.
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- AI Homework Assistant

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| | | | | | | | | |
| | | | | | | | | |
| | | | | | | | | |

**Candidate được chọn:**

**Vì sao chọn:**

**Vì sao loại các candidate còn lại:**

**Xử lý bất đồng (nếu có):**

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này:

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | |
| Câu nói đáng nhớ nhất (nguyên văn) | |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | |
| Hiện đang xử lý bằng cách nào (workaround)? | |
| Mất bao lâu, bao lần? | |
| Insight / opportunity rút ra | |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| | | | |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| | | | | | |
| | | | | | |
| | | | | | |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text

```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | | | |
| Tổng thời gian | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Rủi ro mới phát sinh | | | |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

-

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | | | | |
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
