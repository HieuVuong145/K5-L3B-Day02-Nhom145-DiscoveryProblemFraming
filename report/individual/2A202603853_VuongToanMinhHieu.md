# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Vương Toàn Minh Hiếu
- MSSV: 2A202603853
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Nhom145
- Link repo nhóm: https://github.com/HieuVuong145/K5-L3B-Day02-Nhom145-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi di chuyển qua các trục đường vào giờ cao điểm, tôi muốn biết trước ngã tư hoặc đoạn đường nào đng xảy ra ùn tắc, để chủ động rẽ sang cung đường khác tránh kẹt cứng. | Người tham gia giao thông | Thời gian di chuyển tăng lên lặp lại hàng ngày. Trên app bản đồ biểu hiện đường màu đỏ thể hiện đường tắc. |
| 2 | Cần đọc, tổng hợp nhiều thông tin | Khi mua đồ trên sàn thương mại điện tử như Shopee, tôi muốn lọc ra được các đánh giá từ người dùng thật và so sánh mức giá sau khi áp mã giảm giá giữa các shop, để mua sản phẩm tốt với giá hời. | Bản thân khách hàng | Lịch sử tìm kiếm các shop khác nhau với cùng 1 sản phẩm |
| 3 | Pain từ người khác | Khi tôi đi khám bệnh định kỳ, tôi muốn nắm rõ quy trình di chuyển giữa các phòng khám, xét nghiệm và thứ tự chờ đến lượt ở từng khâu, để tôi có thể đi khám với chi phí thời gian tối thiểu. | Người bệnh | Mất thời gian chờ nhiều tiếng cho 1 buổi khám bệnh, lặp lại 2-3 tháng/lần |
| 4 | Lặp lại | Khi báo cáo công việc hàng tuần cho mentor, tôi muốn gom toàn bộ lịch sử cập nhật code, các lỗi đã sửa và kết quả chạy thử nghiệm thành một bản tóm tắt, để mentor nắm rõ tiến độ.| Mentor và người developer | Lịch sử commit trên GitHub và hơn 50 tin nhắn trao đổi rải rác mỗi tuần. |
| 5 | Cần đọc, tổng hợp thông tin | Khi cần tìm quán ăn, địa điểm giải trí cho nhóm bạn, tôi muốn đối chiếu nhanh mức chi phí, vị trí và đánh giá chất lượng thật từ nhiều nền tảng khác nhau, để chốt được địa điểm phù hợp với sở thích và và trong khả năng kinh tế của tất cả thành viên. | Bản thân người chủ trì kế hoạch và những người tham gia kế hoạch | Mất 45–60 phút đọc review và bàn bạc, lặp lại 1–2 lần/tháng; cả nhóm đều mất thời gian, các link review đánh giá được mở nhiều nhưng không thể chốt được địa điểm. |
| 6 | Lặp lại | Khi kết thúc một ngày làm việc hoặc học tập, tôi muốn tổng kết các việc đã hoàn thành, vướng mắc gặp phải cùng những kiến thức vừa tiếp thu được các nhiều nguồn, để viết xong báo cáo Daily Standup nhanh chóng mà không bỏ sót kết quả quan trọng. | Bản thân người viết, mentor,... | Mất 15–25 phút ngồi nhớ lại và soạn daily standup, lặp lại hàng ngày. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Ý 2 và 5, đơn giản 1 phần là vấn đề thường xuyên bản thân hay gặp phải và muốn tìm 1 cách tối ưu để thực hiện.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Khi di chuyển qua các trục đường vào giờ cao điểm, tôi muốn biết trước ngã tư hoặc đoạn đường nào đng xảy ra ùn tắc, để chủ động rẽ sang cung đường khác tránh kẹt cứng. | Xảy ra hàng ngày, mỗi lần tắc cứng làm việc đi học, làm bị muộn. Quy mô người gặp rất lớn và có sẵn dữ liệu đối chiếu từ bản đồ số, camera giao thông công cộng hoặc phản ánh từ cộng đồng. | Độ trễ dữ liệu cảnh báo có đủ nhanh để người lái xe kịp rẽ sang đường khác, và khi nhiều người cùng rẽ sang đường khác thì đường đó có bị tắc nghẽn dây chuyền không. |
| 2 | Khi kết thúc một ngày làm việc hoặc học tập, tôi muốn tổng kết các việc đã hoàn thành, vướng mắc gặp phải cùng những kiến thức vừa tiếp thu được các nhiều nguồn, để viết xong báo cáo Daily Standup nhanh chóng mà không bỏ sót kết quả quan trọng. | Công việc lặp lại đều đặn mỗi tối, mất thời gian nếu ngày nào cũng phải lục lại lịch sử công việc. Toàn bộ dữ liệu đầu vào đều nằm trên máy của người dùng, dễ dàng đo lường thời gian tiết kiệm được và tự kiểm thử giải pháp ngay lập tức mà không phụ thuộc bên thứ ba. |Cách thức gom dữ liệu tự động hay bán tự động có xâm phạm quyền riêng tư cá nhân không.|
| 3 | Khi tôi đi khám bệnh định kỳ, tôi muốn nắm rõ quy trình di chuyển giữa các phòng khám, xét nghiệm và thứ tự chờ đến lượt ở từng khâu, để tôi có thể đi khám với chi phí thời gian tối thiểu. | Mỗi lần đi khám hàng tiếng chờ khám; việc phải di chuyển qua lại nhiều tầng/khu nhà gây lãng phí nhiều thời gian của người khám. | Thứ tự hàng đợi nằm trong hệ thống nội bộ của viện và thay đổi liên tục khi có ca cấp cứu/ưu tiên, cá nhân bên ngoài rất khó lấy được số liệu thời gian thực nếu chỉ dựa vào thông tin công khai. |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi di chuyển qua các trục đường vào giờ cao điểm, tôi muốn biết trước ngã tư hoặc đoạn đường nào đng xảy ra ùn tắc, để chủ động rẽ sang cung đường khác tránh kẹt cứng.|
| Actor | Người tham gia giao thông |
| Thời điểm / bối cảnh | Giờ cao điểm |
| Quy trình hiện tại (3–7 bước) | Mở map -> Chọn lộ trình hay đi -> Gặp đoạn đường tắc -> Mở map tìm đường đi khác -> Chọn đường vòng và di chuyển -> Đi muộn |
| Bottleneck (bước nào, mất bao nhiêu phút) | Đi vào đường tắc đã mất thời gian và mất thêm thời gian tự tìm đường |
| Impact (nếu không giải thì sao) | Mất thêm 20-30p di chuyển |
| Success metric (baseline → target) | Giảm thời gian tham gia giao thông |
| Phương án không dùng AI | Xuất phát sớm hơn khung giờ bình thường hay đi khoảng 30p |
| Giả thuyết về AI (nếu có) | AI tổng hợp dữ liệu thời gian thực từ luồng camera giao thông công cộng, tốc độ di chuyển và tin báo cộng đồng để dự báo điểm nghẽn sớm 10–15 phút, sau đó phát cảnh báo âm thanh điều hướng rẽ trước 1–2 ngã tư |
| Cảm nhận nhanh | Workflow / Agent  |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 45 phút (Chậm hơn bình thường 25–30 phút)

[1 Xem Maps ở nhà: 3'] → [2 Chạy xe theo lộ trình: 10'] → [3 Kẹt cứng tại điểm nóng: 12'] ← BOTTLENECK 1
→ [4 Tấp lề tra đường tắt / nhóm FB: 8'] ← BOTTLENECK 2 → [5 Đi vòng qua ngõ nhỏ: 10'] → [6 Báo trễ giờ: 2']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi kết thúc một ngày làm việc hoặc học tập, tôi muốn tổng kết các việc đã hoàn thành, vướng mắc gặp phải cùng những kiến thức vừa tiếp thu được các nhiều nguồn, để viết xong báo cáo Daily Standup nhanh chóng mà không bỏ sót kết quả quan trọng.|
| Actor | Sinh viên CNTT, dev |
| Thời điểm / bối cảnh | Cuối ngày làm việc |
| Quy trình hiện tại (3–7 bước) | Rà soát lịch sử commit -> Lục lại tab trình duyệt, tài liệu đọc trong ngày -> Tin nhắn trao đổi -> Gom các ý rời rạc -> Viết tóm tắt báo cáo thành từng mục|
| Bottleneck (bước nào, mất bao nhiêu phút) | Lục lại lịch sử mất thời gian và phải viết các nội dung thành các mục chi tiết và hợp lý |
| Impact (nếu không giải thì sao) | Mỗi ngày mất khoảng 30p-1h cho công việc ngắn |
| Success metric (baseline → target) | Tiết kiệm thời gian viết Daily Standup, đầy đủ tính chất công việc học tập được báo cáo |
| Phương án không dùng AI | Tạo sẵn template, mỗi khi xong công việc là ghi chú luôn |
| Giả thuyết về AI (nếu có) | AI đọc lịch sử commit, danh sách trình duyệt, tài liệu được mở,... |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 25 phút

[1 Xem Git commits: 3'] → [2 Lục lại tab & tài liệu đã đọc: 6'] ← BOTTLENECK 1 → [3 Lướt chat Discord/Zalo: 3']
→ [4 Gom ý ra nháp: 3'] → [5 Viết đúc kết việc làm & bài học: 7'] ← BOTTLENECK 2 → [6 Soát & gửi: 3']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi tôi đi khám bệnh định kỳ, tôi muốn nắm rõ quy trình di chuyển giữa các phòng khám, xét nghiệm và thứ tự chờ đến lượt ở từng khâu, để tôi có thể đi khám với chi phí thời gian tối thiểu. |
| Actor | Người bệnh đi khám |
| Thời điểm / bối cảnh | Buổi sáng/chiều các ngày trong tuần khi lượng bệnh nhân đông nhất |
| Quy trình hiện tại (3–7 bước) | 1. Xếp hàng lấy số và làm thủ tục tại quầy tiếp đón · 2. Chờ khám lâm sàng tổng quát ban đầu để nhận phiếu chỉ định · 3. Đóng tiền viện phí · 4. Tự tìm đường đi và xếp hàng lần lượt tại 3–4 phòng cận lâm sàng (lấy máu, siêu âm, X-quang, điện tim) · 5. Ngồi chờ lấy kết quả xét nghiệm · 6. Quay lại phòng khám ban đầu chờ bác sĩ đọc kết quả và kê đơn |
| Bottleneck (bước nào, mất bao nhiêu phút) | Thời gian di chuyển qua các phòng, toà nhà và thời gian xếp hàng rất lâu |
| Impact (nếu không giải thì sao) | Mất thời gian chờ nhiều tiếng cho 1 buổi khám |
| Success metric (baseline → target) | Rút ngắn quy trình khám |
| Phương án không dùng AI | Đặt lịch khám trước, hoặc đặt lịch hẹn giờ qua ứng dụng bệnh viện và chuẩn bị bản đồ bệnh viện |
| Giả thuyết về AI (nếu có) | AI phân tích danh sách chỉ định trên phiếu khám kết hợp với độ dài hàng đợi và thời gian xử lý trung bình tại từng phòng (lấy máu, siêu âm, X-quang) để gợi ý lộ trình di chuyển tối ưu theo thời gian thực (đi phòng nào trước, phòng nào sau) kèm thông báo nhắc khi sắp đến số |
| Cảm nhận nhanh | Rule / Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 210 phút (3,5 giờ)

[1 Lấy số & thủ tục: 20'] → [2 Khám ban đầu: 25'] → [3 Đóng phí: 10']
→ [4 Đi tìm & xếp hàng 3–4 phòng xét nghiệm/siêu âm: 95'] ← BOTTLENECK
→ [5 Chờ kết quả xét nghiệm: 40'] → [6 Bác sĩ đọc kết quả & kê đơn: 20']
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Vấn đề đông người gặp phải nhất, giải quyết được vấn đề sẽ tiết kiệm được thời gian di chuyển của người tham gia giao thông.
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
