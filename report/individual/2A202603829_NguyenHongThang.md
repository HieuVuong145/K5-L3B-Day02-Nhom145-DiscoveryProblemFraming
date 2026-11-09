# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Hồng Thắng
- MSSV: 2A202603829
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Nhóm 145
- Link repo nhóm: https://github.com/HieuVuong145/K5-L3B-Day02-Nhom145-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |	Lặp lại |Khi lập thông báo tiền điện, nước hàng tháng, tôi muốn tự động tổng hợp chỉ số công tơ để giảm thời gian tính toán và sai sót. | Chủ nhà, kế toán, khách thuê| 10–30 căn hộ/văn phòng; thực hiện hàng tháng; phải nhập nhiều số liệu thủ công.|
| 2 |	Lặp lại |Khi lập hồ sơ thẩm định giá bất động sản, tôi muốn tự động thu thập và chuẩn hóa dữ liệu tài sản so sánh để nâng cao hiệu suất. |Thẩm định viên, trưởng phòng |Mỗi hồ sơ phải tìm kiếm, kiểm tra và so sánh nhiều bất động sản. |
| 3 | Tốn thời gian|Khi kiểm tra bản vẽ thiết kế MEP, tôi muốn tự động phát hiện các điểm thiếu hoặc xung đột để hạn chế sai sót khi thi công. |Kỹ sư thiết kế, nhà thầu, chủ đầu tư | Phải kiểm tra nhiều bản vẽ, nhiều hệ thống và phối hợp giữa các bộ môn.|
| 4 |Pain từ người khác |Khi khách thuê phản ánh sự cố điện, nước hoặc điều hòa, tôi muốn có hệ thống tiếp nhận và phân loại yêu cầu để xử lý nhanh chóng. |Khách thuê, ban quản lý, kỹ thuật viên |Nhiều kênh tiếp nhận như điện thoại, Zalo; thông tin dễ thất lạc, khó theo dõi. |
| 5 |Lặp lại |Khi giáo viên giao bài tập qua nhiều kênh, tôi muốn tổng hợp tất cả bài tập vào một danh sách để không bỏ sót nhiệm vụ của con. | Phụ huynh, học sinh|Phải kiểm tra LMS, nhóm Zalo, vở ghi và thông báo giáo viên hàng ngày. |
| 6 |Tốn thời gian |Khi muốn biết tình hình học tập của con, tôi muốn xem nhanh tiến độ hoàn thành bài tập trên LMS để không phải đăng nhập và kiểm tra từng môn. |Phụ huynh | Phải truy cập nhiều môn học, kiểm tra trạng thái từng bài.|
| 7 |Pain từ người khác |Khi con chưa hoàn thành bài tập nhưng không chủ động báo cáo, tôi muốn biết tình trạng thực tế để hỗ trợ thay vì phải liên tục hỏi và kiểm tra. |Phụ huynh, học sinh | Phụ huynh phải nhắc nhiều lần; dễ phát sinh mâu thuẫn.|
| 8 |Tốn thời gian | Khi có nhiều con học các lớp khác nhau, tôi muốn theo dõi nhiệm vụ của từng con trên một giao diện chung để tiết kiệm thời gian quản lý.| Phụ huynh, các con|Phải theo dõi nhiều tài khoản, lớp học và lịch học. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |Tổng hợp bài tập học sinh từ nhiều kênh (LMS, Zalo, vở ghi, thông báo giáo viên). | Vấn đề xảy ra hàng ngày, thông tin phân tán, phụ huynh phải kiểm tra và tổng hợp thủ công. Có khả năng ứng dụng AI để đọc, nhận diện, phân loại và quản lý nhiệm vụ tập trung.|Khả năng truy cập dữ liệu LMS; mức độ đa dạng của các kênh giao bài; độ chính xác khi AI nhận diện nội dung và deadline. |
| 2 |Tự động tổng hợp chỉ số điện, nước và lập thông báo thanh toán. |Công việc lặp lại hàng tháng, có quy trình rõ ràng, nhiều dữ liệu đầu vào và đầu ra có thể kiểm chứng. Có tiềm năng ứng dụng OCR và AI Agent để tự động hóa toàn bộ quy trình. | Độ chính xác khi đọc ảnh công tơ; khả năng lấy dữ liệu điện điều hòa; mức độ khác biệt giữa các biểu mẫu thanh toán.|
| 3 |Tiếp nhận và phân loại yêu cầu sửa chữa của khách thuê. |Thông tin đến từ nhiều kênh, ảnh hưởng trực tiếp đến trải nghiệm khách thuê và hiệu quả vận hành. AI có thể phân loại sự cố, xác định mức độ ưu tiên và điều phối kỹ thuật viên. |Số lượng sự cố thực tế mỗi tháng; thời gian xử lý hiện tại; khả năng tích hợp các kênh liên lạc. |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi …, tôi muốn …, để … |
| Actor | |
| Thời điểm / bối cảnh | |
| Quy trình hiện tại (3–7 bước) | |
| Bottleneck (bước nào, mất bao nhiêu phút) | |
| Impact (nếu không giải thì sao) | |
| Success metric (baseline → target) | |
| Phương án không dùng AI | |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết |

Quy trình nháp hiện tại:

```text

```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi …, tôi muốn …, để … |
| Actor | |
| Thời điểm / bối cảnh | |
| Quy trình hiện tại (3–7 bước) | |
| Bottleneck (bước nào, mất bao nhiêu phút) | |
| Impact (nếu không giải thì sao) | |
| Success metric (baseline → target) | |
| Phương án không dùng AI | |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết |

Quy trình nháp hiện tại:

```text

```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi …, tôi muốn …, để … |
| Actor | |
| Thời điểm / bối cảnh | |
| Quy trình hiện tại (3–7 bước) | |
| Bottleneck (bước nào, mất bao nhiêu phút) | |
| Impact (nếu không giải thì sao) | |
| Success metric (baseline → target) | |
| Phương án không dùng AI | |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết |

Quy trình nháp hiện tại:

```text

```

### Card muốn pitch nhất

- Card số:
- Vì sao:
- Câu hỏi muốn nhóm phản biện:

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| | | |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | | | | |
| CP2 Problem Card | | | | |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-
