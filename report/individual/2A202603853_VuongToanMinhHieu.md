# Báo cáo cá nhân — 2A202603853_VuongToanMinhHieu

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
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4 — tấp lề tra đường tắt / nhóm FB, mất 8 phút; bước 3 kẹt cứng 12 phút cũng cần được cân nhắc khi chọn bottleneck chính. |
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
| Actor “người tham gia giao thông” còn rộng; nên giới hạn theo phương tiện, tuyến đường hoặc mục đích di chuyển. | Có | Chưa thu hẹp vì chưa có thêm dữ liệu về phương tiện/tuyến đường cụ thể; cần bổ sung trước khi chốt card. |
| Bottleneck đang gộp hai điểm (kẹt tại điểm nóng 12 phút và tấp lề tìm đường 8 phút), còn metric “giảm thời gian tham gia giao thông” chưa có baseline/target rõ ràng. | Có | Đã sửa bottleneck trong card để nêu cụ thể bước 4 và 8 phút, đồng thời ghi nhận bước 3 mất 12 phút. Metric vẫn cần target và cách đo rõ hơn. |
| Giả thuyết dựa vào dữ liệu camera công cộng và dự báo trước 10–15 phút nhưng chưa chứng minh có thể tiếp cận dữ liệu đó; cũng có thể đang chọn Workflow/Agent quá sớm. | Có | Chưa đổi giả thuyết; cần kiểm tra tính sẵn có của dữ liệu và so sánh với phương án đơn giản hơn như cảnh báo dựa trên dữ liệu bản đồ hiện có. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Trình bày 3 candidate: ùn tắc giao thông giờ cao điểm, viết Daily Standup cuối ngày và quy trình đi khám nhiều bước. | Nhóm có thêm các góc nhìn về dự báo ùn tắc, tổng hợp công việc và thời gian chờ khám để đưa vào thảo luận, so sánh với candidate của các thành viên khác. |
| Phản biện bài của bạn khác | Với candidate chuyển báo cáo dài thành slide, tôi hỏi rằng đã có nhiều công cụ AI làm việc này thì giải pháp đề xuất sẽ khác biệt ở điểm nào. | Đưa thêm tiêu chí về mức độ khác biệt và việc xác định đúng pain vào phần thảo luận candidate. |
| Nhận phản biện | Trường hỏi Google Maps đã có giải pháp cho ùn tắc, vậy những tình huống thực tế nào Maps không cập nhật được? | Tôi nhận ra card cần nêu rõ khoảng trống của cách xử lý hiện tại, thay vì chỉ khẳng định cần biết trước điểm tắc. |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | Tôi tham gia phần kiểm chứng và research cho candidate nhóm chọn là xử lý lỗi cài đặt thư viện. Nhóm ghi nhận 3 cuộc phỏng vấn và 8 phản hồi khảo sát; research các công cụ Astral uv, GitHub Copilot in the CLI và pip-tools. | Kết quả tổng hợp ghi nhận 10/11 người từng mất 45–90 phút xử lý lỗi thư viện/môi trường; đồng thời có phản hồi phản bác rằng Docker hoặc lock file có thể giảm đáng kể vấn đề. Research giúp nhóm nhận diện công cụ hiện có và những khoảng trống còn lại. |
| Quy trình nhóm |  |  |
| Problem Statement |  | |
| Mức can thiệp AI |  |  |
| Quyết định | Tôi đánh giá bốn rủi ro Value, Usability, Feasibility và Viability, sau đó chọn **Not Yet** thay vì triển khai ngay. | Ghi nhận pain có bằng chứng ban đầu, nhưng cần kiểm chứng thêm khả năng sử dụng, tính khả thi, độ an toàn của đề xuất và cơ chế backup/rollback trước khi thử nghiệm rộng. Tôi đề xuất pilot giới hạn tối đa 10 trường hợp và ngưỡng dừng đo được. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Gợi ý thêm các tình huống/problem để mở rộng danh sách scan. | Giúp có thêm góc nhìn ngoài những việc đã nghĩ tới; tôi giữ lại ý 2 và 5 vì đây là những tình huống bản thân thường gặp. | Gợi ý của AI tự nó không chứng minh vấn đề xảy ra thường xuyên hay có impact. | Chỉ giữ những ý khớp trải nghiệm thật; dấu hiệu và mức độ của problem cần dựa trên quan sát của mình. |
| CP2 Problem Card | Đóng vai PM hoài nghi để rà soát card giao thông #1. | Chỉ ra actor còn rộng, hai bottleneck đang bị gộp, metric chưa đo được và giả thuyết dữ liệu camera/dự báo chưa được xác minh. | Phản biện chỉ nêu lỗ hổng, không cung cấp bằng chứng thực tế để xác định dữ liệu nào có thể truy cập hoặc target nào khả thi. | Tôi ghi nhận cần thu hẹp actor, tách bottleneck, đo baseline/target và kiểm tra dữ liệu trước khi giữ giả thuyết AI; không xem gợi ý của AI là kết luận đã kiểm chứng. |
| CP4 Research | Hỗ trợ gợi ý hướng tìm kiếm và đối chiếu sơ bộ các công cụ giải quyết vấn đề lỗi môi trường/thư viện. | Giúp tổ chức research theo bước của quy trình và nhận diện khoảng trống giữa quản lý dependency bằng rule với việc giải thích lỗi cho người dùng. | Mô tả hoặc nhận định do AI đưa ra có thể chung chung, lỗi thời hoặc không khớp phiên bản/công cụ; không thể xem là nguồn xác thực. | Đối chiếu thông tin với tài liệu gốc và chỉ ghi các link đã tự mở, kiểm tra; không dùng AI thay cho phỏng vấn/khảo sát người thật. |
| CP5 Quy trình |  |  |  |  |
| CP5–6 Problem Statement |  |  |  |  |
| CP6 Mức can thiệp / quyết định | Dùng AI để hỗ trợ hệ thống hóa bốn rủi ro, cân nhắc quyết định và diễn đạt các kiểm chứng/ngưỡng dừng cho phần quyết định. | Giúp nối các bằng chứng CP4 và các giả định chưa kiểm chứng với lý do chọn **Not Yet**, đồng thời chuyển bước tiếp theo thành các tiêu chí có thể đo. | Đề xuất ban đầu vẫn dựa trên mẫu nhỏ; tính chính xác của AI, an toàn lệnh, backup/rollback và chi phí chưa được thử nghiệm thực tế. | Tôi xem các mức rủi ro và ngưỡng pilot là đề xuất cần cân nhắc, đối chiếu với bằng chứng nhóm; quyết định Not Yet vì Usability và Feasibility vẫn còn rủi ro cao. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?** Trả lời: Problem của các thành viên khác trong team mang tính thực tế nhiều hơn, problem to solution chứ không phải ngược lại, bản thân vẫn còn chưa brainstorm, mở rộng được phạm vi khi đặt vấn đề

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?** Trả lời: Có, hơn một nửa các case mà thành viên đưa ra đều là solution first, nhóm đã có các câu hỏi cho chủ nhân problem đó để phản biện và góp ý sau đó thay đổi.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.** Tôi có nhưng chưa biết sửa lại vấn đề của mình như nào khi có thành viên hỏi tôi về chủ đề tắc đường và google maps, làm thế nào để độ trễ cập nhật dữ liệu là thấp nhất.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?** Kết quả kiểm chứng đưa ra khác hẳn với những suy nghĩ ban đầu tôi đặt ra khi tiếp cận problem đó.

**6.5. Điều khó nhất khi viết Problem Statement là gì?** Brainstorm một vấn đề thực sự mang tính thực tiễn với bằng chứng có thể chứng minh được bằng con số, dữ liệu,...

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?** Nếu làm lại tôi sẽ phân tích vấn đề xem đã có những giải pháp đề xuất nào chưa nếu không có mới xem xét lựa chọn đề tài. Tôi sẽ phản biện nhóm mạnh hơn ở điểm sử dụng dữ liệu thực để chứng minh.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình. Trả lời: Phát sinh problem từ một lĩnh vực nào đó có thể do lặp đi lặp lại, vấn đề gây mất thời gian, thiếu thông tin xác thức và phả ánh của người khác. Xác định được vấn đề sẽ phải đi trực quan hoá vấn đề bằng Card gồm các trường như actor, người bị ảnh hưởng, tại sao, bottlenecks của vấn đề, giải pháp nếu không có và có AI. Thống kê và gom các problem rồi phân thành các nhóm có độ giống nhau rồi xét tính thực thi được giải pháp với vấn đề bằng con số. Sau khi chọn được vấn đề sẽ vạch ra giới hạn của bài toán. Nếu bài toán dễ ở mức có thể triển khai giải pháp tối ưu 1 cách nhanh chóng mà không cần AI thì sẽ triển khai luôn. Còn bắt buộc cần sử dụng AI để có thể tối thiểu hoá chi phí giải quyết vấn đề và thời gian thì nên sử dụng. 

---

## 7. Tài liệu tham khảo

-
