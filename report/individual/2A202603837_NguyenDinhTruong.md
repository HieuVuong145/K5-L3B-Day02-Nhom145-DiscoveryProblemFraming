# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Đình Trường
- MSSV: 2A202603837
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Nhóm 145
- Link repo nhóm: https://github.com/HieuVuong145/K5-L3B-Day02-Nhom145-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Tốn thời gian |Khi cần tìm một linh kiện điện tử phù hợp với yêu cầu kỹ thuật, tôi muốn so sánh được thông số và khả năng tương thích của nhiều linh kiện, để tránh chọn sai linh kiện và phải thay thế. |Kỹ sư thiết kế phần cứng |Mất tổng 60-95 phút để tìm linh kiện trên các trang linh kiện điện tử và phân tích thông số để chọn được phù hợp 1 linh kiện điện tử phù hợp với mạch điện |
| 2 |Cần đọc, tổng hợp nhiều thông tin |Khi lựa chọn một thiết bị công nghệ đã qua sử dụng, tôi muốn đánh giá được tình trạng phần cứng và mức độ phù hợp với nhu cầu, để hạn chế rủi ro mua phải thiết bị không đáp ứng kỳ vọng. |Người mua laptop, Pc và thiết bị công nghệ |Khi mua Laptop, pc 2nd online hoặc trực tiếp, có thông tin về linh kiện trong thiết bị mặc dù còn bảo hành, nhưng khi về nhà sử dụng tuổi thọ thấp bị hỏng trong vòng 1 tuần ngay sau khi mua |
| 3 |Pain từ người khác |Khi người dùng gửi báo cáo lỗi phần mềm, tôi muốn nhận được đầy đủ thông tin về tình huống phát sinh và các bước tái hiện lỗi, để xác định nguyên nhân mà không phải yêu cầu bổ sung nhiều lần. |Người sử dụng phần mềm |Có thể kiểm tra các báo cáo lỗi, yêu cầu hỗ trợ và lịch sử trao đổi trên hệ thống quản lý công việc. Cần thống kê số báo cáo thiếu thông tin và số lần phải hỏi lại. |
| 4 |Lặp lại |Khi cần viết tài liệu kỹ thuật từ ghi chú hoặc kết quả công việc, tôi muốn trình bày thông tin theo một cấu trúc thống nhất, để giảm công sức biên soạn và hạn chế sai lệch. |Người viết tài liệu kỹ thuật |Trong quá trình xây dựng tài liệu kỹ thuật, thông tin đầu vào thường nằm rải rác trong ghi chú, nội dung trao đổi và kết quả nghiên cứu. Chẳng hạn, bộ yêu cầu gồm 113 yêu cầu sản phẩm (PRS), được cập nhật qua nhiều phiên bản SRS như v0.6 và v0.7. Người viết phải tổng hợp, sắp xếp và chuẩn hóa nội dung trước khi đưa vào tài liệu chính thức.|
| 5 |Lặp lại |Khi gặp lỗi trong quá trình cài đặt thư viện lập trình, tôi muốn kiểm tra nguyên nhân và cách khắc phục theo một quy trình thống nhất, để không phải xử lý lại từ đầu. |Lập trình viên |Trong quá trình thực hiện các bài tập lập trình Python, tôi từng gặp tình trạng chương trình không thể chạy do thiếu thư viện hoặc phiên bản thư viện không tương thích. Khi gặp lỗi, tôi phải đọc thông báo trong Terminal, tìm kiếm nội dung lỗi trên Google hoặc Stack Overflow, đối chiếu các phiên bản thư viện và thử nhiều cách cài đặt khác nhau. Một lần xử lý có thể mất khoảng 20–40 phút, tùy thuộc vào mức độ phức tạp của lỗi.|

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-Giữ lại
Problem 04: Tự động tổng hợp và chuẩn hóa tài liệu kỹ thuật từ ghi chú, nội dung trao đổi và kết quả nghiên cứu.
Lý do: Trong quá trình xây dựng tài liệu CANVista, thông tin nằm ở nhiều nguồn khác nhau. Việc tổng hợp và chuẩn hóa nội dung diễn ra nhiều lần, tốn công sức và có nguy cơ bỏ sót thông tin. AI có thể hỗ trợ tổng hợp, phân loại và chuyển đổi nội dung theo cấu trúc tài liệu thống nhất.
-Bỏ: Lăng kính: Lặp lại,	Khi sử dụng máy tính hằng ngày, tôi muốn tự động sắp xếp các biểu tượng trên màn hình theo nhóm, để dễ tìm kiếm và sử dụng.	Người sử dụng máy tính. Lí do:	Vấn đề nhỏ, không gây ảnh hưởng đáng kể đến hiệu suất công việc và có thể tự xử lý nhanh chóng.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |Khi cần tìm một linh kiện điện tử phù hợp với yêu cầu kỹ thuật, tôi muốn so sánh được thông số và khả năng tương thích của nhiều linh kiện, để tránh chọn sai linh kiện và phải thay thế.|Có trải nghiệm thực tế, mất khoảng 1–2 giờ để tìm kiếm, đọc thông số và lựa chọn một linh kiện. AI có thể hỗ trợ đọc datasheet, so sánh thông số và kiểm tra điều kiện tương thích. |Chưa đo thời gian cho nhiều lần lựa chọn linh kiện; chưa xác định mức độ chính xác của kết quả AI.|
| 2 |Khi cần viết tài liệu kỹ thuật từ ghi chú hoặc kết quả công việc, tôi muốn trình bày thông tin theo một cấu trúc thống nhất, để giảm công sức biên soạn và hạn chế sai lệch.  |Có bối cảnh thực tế từ dự án với nhiều yêu cầu PRS, tài liệu SRS và các phiên bản cập nhật. AI có thể hỗ trợ tổng hợp ghi chú, phân loại yêu cầu, soạn thảo và đối chiếu nội dung giữa các phiên bản. |Chưa đo chính xác thời gian cho từng loại tài liệu; chưa đánh giá khả năng AI phát hiện đầy đủ các yêu cầu bị thiếu hoặc mâu thuẫn. |
| 3 |Khi gặp lỗi trong quá trình cài đặt thư viện lập trình, tôi muốn kiểm tra nguyên nhân và cách khắc phục theo một quy trình thống nhất, để không phải xử lý lại từ đầu. |Đây là tình huống thường gặp khi thiết lập môi trường Python, cài đặt package hoặc xử lý xung đột phiên bản. Quy trình minh họa mất khoảng 61 phút, trong đó 30 phút dành cho thử phương án khắc phục và kiểm tra lại. AI có thể phân tích log lỗi và đề xuất cách xử lý. |Chưa có số liệu đo thời gian từ nhiều tình huống thực tế; chưa xác định tỷ lệ AI đề xuất đúng phương án và khả năng xử lý các lỗi phức tạp. |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi cần tìm một linh kiện điện tử phù hợp với yêu cầu kỹ thuật, tôi muốn so sánh được thông số và khả năng tương thích của nhiều linh kiện, để tránh chọn sai linh kiện và phải thay thế.|
| Actor |Kỹ sư thiết kế phần cứng |
| Thời điểm / bối cảnh |Khi thiết kế mạch điện, nghiên cứu linh kiện mới hoặc tìm linh kiện thay thế cho một linh kiện hiện tại. |
| Quy trình hiện tại (3–7 bước) |	1. Xác định yêu cầu kỹ thuật. 2. Tìm kiếm linh kiện trên các trang nhà sản xuất và nhà cung cấp. 3. Tải datasheet 4. Đọc và trích xuất thông số 5. So sánh thông số giữa các linh kiện 6. Kiểm tra khả năng tương thích với mạch điện 7. Lựa chọn linh kiện phù hợp. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Công đoạn đọc datasheet, trích xuất thông số và đối chiếu khả năng tương thích mất khoảng 35–55 phút. Tổng quy trình tìm kiếm và lựa chọn một linh kiện mất khoảng 60–95 phút.|
| Impact (nếu không giải thì sao) |Tốn thời gian nghiên cứu, có nguy cơ chọn sai thông số, phát sinh chi phí mua linh kiện thay thế và chỉnh sửa thiết kế.|
| Success metric (baseline → target) |Baseline: Khoảng 60-95 phút/lần lựa chọn (theo trải nghiệm đã cung cấp). Target: Giảm ít nhất 30% thời gian tìm kiếm và so sánh; đảm bảo các thông số quan trọng được kiểm chứng bằng datasheet. |
| Phương án không dùng AI |Tạo benchmark so sánh thông số, đánh giá độ phù hợp của từng liên kiện đối với yêu cầu sản phầm|
| Giả thuyết về AI (nếu có) |AI sẽ tìm linh kiện, đọc datasheet của linh kiện, tổng hợp thông số, lọc các linh kiện không đáp ứng và có thể recommend được nên dùng linh kiện chuẩn cho trường hợp cố định |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```
HIỆN TẠI — 85 phút
[1 Xác định yêu cầu: 5'] → [2 Tìm kiếm linh kiện: 15'] → [3 Lọc linh kiện: 10']
→ [4 Tải Datasheet: 5'] → [5 Đọc và trích xuất dữ liệu: 25'] 
→ [6 So sánh và kiểm tra linh kiện: 20']← BOTTLENECK → [7 Lựa chọn: 5']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story |Khi cần viết tài liệu kỹ thuật từ ghi chú hoặc kết quả công việc, tôi muốn trình bày thông tin theo một cấu trúc thống nhất, để giảm công sức biên soạn và hạn chế sai lệch. |
| Actor |Người viết tài liệu kỹ thuật |
| Thời điểm / bối cảnh |Khi xây dựng SRS, tài liệu kiến trúc phần mềm, tài liệu đặc tả yêu cầu hoặc cập nhật tài liệu sau các buổi họp, nghiên cứu và đánh giá.|
| Quy trình hiện tại (3–7 bước) |1. Thu thập thông tin từ ghi chú, email, tài liệu và trao đổi. 2. Đọc và xác định thông tin liên quan 3. Phân loại thông tin theo chủ đề hoặc yêu cầu. 4. Biên soạn nội dung theo cấu trúc tài liệu. 5. Đối chiếu với yêu cầu và tài liệu trước đó. 6. Kiểm tra nội dung thiếu, trùng lặp hoặc mâu thuẫn. 7. Chỉnh sửa và cập nhật phiên bản tài liệu. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 3 và 4: Phân loại thông tin và biên soạn tài liệu. Thông tin đầu vào nằm ở nhiều nguồn, không đồng nhất về cách diễn đạt và mức độ chi tiết. Người viết phải tự xác định nội dung nào thuộc mục nào, chuyển ghi chú thành câu văn kỹ thuật và đảm bảo không làm sai lệch ý nghĩa ban đầu. Đây là hai công đoạn có khả năng tiêu tốn nhiều thời gian nhất. |
| Impact (nếu không giải thì sao) |Tốn thời gian cho công việc biên soạn lặp lại; có nguy cơ bỏ sót yêu cầu, trùng lặp nội dung, sai lệch giữa các phiên bản và phát sinh thêm vòng đánh giá, chỉnh sửa. |
| Success metric (baseline → target) |Giảm ít nhất 30% thời gian biên soạn so với baseline đo thực tế; giảm số lỗi thiếu thông tin, trùng lặp và sai cấu trúc sau khi rà soát.|
| Phương án không dùng AI |Xây dựng template SRS thống nhất, sử dụng checklist kiểm tra nội dung, quy định cách đặt tên và phân loại thông tin, đồng thời quản lý phiên bản bằng Git hoặc hệ thống quản lý tài liệu. |
| Giả thuyết về AI (nếu có) |AI có thể đọc và tổng hợp ghi chú, phân loại thông tin theo cấu trúc tài liệu, chuyển nội dung thô thành văn phong kỹ thuật, hỗ trợ đối chiếu các phiên bản và cảnh báo những yêu cầu bị thiếu hoặc có khả năng mâu thuẫn. Người viết vẫn kiểm tra và xác nhận nội dung trước khi đưa vào tài liệu chính thức. |
| Cảm nhận nhanh |Workflow|

Quy trình nháp hiện tại:

```text
HIỆN TẠI - 115 phút
[1 Thu thập thông tin: 10'] → [2 Đọc và chọn lọc thông tin: 10'] → [3 Phân loại thông tin: 20']← BOTTLENECK
→ [4 Biên soạn tài liệu: 30']← BOTTLENECK → [5 Đối chiếu yêu cầu: 15'] 
→ [6 Kiểm tra nội dung: 10'] → [7 Chỉnh sửa và cập nhật phiên bản: 10']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story |Khi gặp lỗi trong quá trình cài đặt thư viện lập trình, tôi muốn kiểm tra nguyên nhân và cách khắc phục theo một quy trình thống nhất, để không phải xử lý lại từ đầu.|
| Actor |Lập trình viên |
| Thời điểm / bối cảnh |Khi tạo môi trường Python mới, cài đặt thư viện từ requirements.txt, tích hợp API hoặc chạy chương trình trong môi trường có các phiên bản thư viện khác nhau. |
| Quy trình hiện tại (3–7 bước) | 1. Phát hiện lỗi (3 phút): Chạy chương trình hoặc cài đặt thư viện và nhận thông báo lỗi trên Terminal 2. Đọc và xác định lỗi (5 phút): Kiểm tra thông báo lỗi, xác định thư viện hoặc thành phần có khả năng gặp vấn đề. 3. Tìm kiếm nguyên nhân (10 phút): Tra cứu Google, Stack Overflow hoặc tài liệu chính thức của thư viện. 4. Đối chiếu phiên bản (13 phút): Kiểm tra phiên bản Python, package và các thư viện phụ thuộc để lựa chọn phương án phù hợp. 5. Thử phương án khắc phục (15 phút): Cài đặt lại thư viện, thay đổi phiên bản hoặc điều chỉnh môi trường Python. 6. Kiểm tra lại chương trình (15 phút): Chạy lại chương trình để xác nhận lỗi đã được giải quyết và không phát sinh lỗi mới. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 5 và bước 6: Thử phương án khắc phục và kiểm tra lại, mất khoảng 30 phút (chiếm 49,2% tổng thời gian 61 phút).|
| Impact (nếu không giải thì sao) |- Gián đoạn tiến độ lập trình do môi trường không hoạt động, mất thời gian tra cứu và thử nghiệm nhiều phương án, có nguy cơ làm phát sinh lỗi mới khi thay đổi phiên bản thư viện, khó tái sử dụng cách khắc phục nếu không ghi lại nguyên nhân và giải pháp |
| Success metric (baseline → target) |Baseline: Khoảng 61 phút xử lý một tình huống lỗi (ước tính minh họa), target: Giảm ít nhất 30% thời gian xử lý, tương đương còn khoảng 43 phút hoặc ít hơn, theo dõi thêm tỷ lệ khắc phục thành công và số lần phải thử lại. |
| Phương án không dùng AI |Sử dụng venv, quản lý package bằng requirements.txt, xây dựng checklist kiểm tra phiên bản, lưu lại lỗi thường gặp và cách khắc phục, sử dụng Git để quản lý cấu hình. |
| Giả thuyết về AI (nếu có) |AI có thể đọc log Terminal, phân tích phiên bản Python và package, xác định nguyên nhân có khả năng gây lỗi, đề xuất lệnh cài đặt hoặc điều chỉnh phiên bản và hướng dẫn kiểm tra lại. Người dùng xác nhận trước khi thực thi. |
| Cảm nhận nhanh |Workflow|

Quy trình nháp hiện tại:

```text
HIỆN TẠI - 115 phút
[1 Thu thập thông tin: 3'] → [2 Đọc và cxác định lỗi: 5'] → [3 Tìm kiếm nguyên nhân: 10']
→ [4 Đối chiếu phiên bản: 13'] → [5 Thử phương án khắc phục: 15']← BOTTLENECK 
→ [6 Kiểm tra lại chương trình: 15']← BOTTLENECK 
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao:Việc tìm kiếm linh kiện phù hợp với yêu cầu kỹ thuật đòi hỏi phải tra cứu thông tin từ nhiều nguồn, so sánh thông số và kiểm tra khả năng tương thích. Quá trình này mất khoảng 1–2 giờ để lựa chọn một linh kiện phù hợp. Nếu chọn sai, có thể ảnh hưởng đến thiết kế phần cứng, phát sinh chi phí và thời gian thay thế. AI có tiềm năng hỗ trợ tìm kiếm, đối chiếu thông số và đề xuất linh kiện phù hợp nhanh hơn.
- Câu hỏi muốn nhóm phản biện: Làm thế nào để xây dựng một AI có thể tìm kiếm và so sánh linh kiện từ nhiều nhà cung cấp, đồng thời đảm bảo thông số kỹ thuật và khả năng tương thích của linh kiện được đề xuất là chính xác?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
|Thông tin linh kiện nằm ở nhiều nguồn khác nhau, khó so sánh trực tiếp.|Có |Bổ sung bước thu thập và chuẩn hóa thông số từ nhiều nhà cung cấp. |
|AI có thể đề xuất linh kiện dựa trên thông tin thiếu hoặc không chính xác.|Có|Bổ sung yêu cầu đối chiếu datasheet chính thức và kỹ sư phải xác nhận trước khi lựa chọn linh kiện.|
|Bài toán còn rộng, chưa xác định rõ loại tài liệu cần xử lý.|Có|Giới hạn phạm vi vào tài liệu kỹ thuật như SRS, đặc tả yêu cầu và tài liệu kiến trúc phần mềm.|
|Quy trình xử lý lỗi chưa được chia thành các bước cụ thể.|Có|Bổ sung quy trình 6 bước từ phát hiện lỗi, đọc thông báo lỗi đến khắc phục và kiểm tra lại.|

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card |Pitch Xử lý lỗi cài đặt thư viện | Vào shortlist và được chọn |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm |Phân tích quy trình As-Is, xác định bottleneck tại bước thử phương án khắc phục và kiểm tra lại. Đề xuất quy trình To-Be kết hợp Rule, AI và con người. |Làm rõ công đoạn tốn nhiều thời gian nhất (30/61 phút), xác định vai trò của AI trong phân tích lỗi và đề xuất cách khắc phục, đồng thời giữ quyền kiểm soát cho lập trình viên. |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan |Gợi ý và phân tích các bài toán thực tế. |Mở rộng ý tưởng, hỗ trợ viết Job Story. |Một số ý tưởng còn chung chung, thiếu bottleneck cụ thể. |Chọn lọc và điều chỉnh theo tính thực tế của vấn đề. |
| CP2 Problem Card |Hỗ trợ phân nhóm candidate, xây dựng OST và shortlist. |Giúp hệ thống hóa các vấn đề và so sánh giữa các candidate. |Có lúc nhầm opportunity với solution, điểm số chưa có đủ bằng chứng. |Điều chỉnh các nhánh opportunity và lựa chọn #9 dựa trên khả năng kiểm chứng thực tế. |
| CP5 Quy trình |Chuyển mô tả sang Mermaid|Nhanh |Quy trình đề xuất đôi khi chưa sát thực tế, target còn mang tính giả định. |Bổ sung vòng lặp xử lý lỗi, xác định boundary và phân biệt số liệu thực tế với mục tiêu kỳ vọng. |



---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Khi nghe các vấn đề của các thành viên khác, tôi nhận ra một vấn đề thực tế không nhất thiết phải có AI mới giải quyết được. Mỗi candidate có đặc điểm và mức độ khả thi khác nhau. Ví dụ, bài toán so sánh linh kiện điện tử có quy trình rõ ràng nhưng đòi hỏi kiến thức chuyên môn; bài toán quản lý yêu cầu sửa chữa có nhiều bên tham gia nhưng cần thêm dữ liệu thực tế. Qua đó, tôi học được cách nhìn nhận vấn đề từ góc độ người dùng, quy trình và khả năng kiểm chứng thay vì chỉ đánh giá mức độ thú vị của ý tưởng.
**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Đối với tôi người trong nhóm, ban đầu đã bị solution-first trước khi hiểu vấn đề và khi trao đổi với các thành viên trong nhóm thì cũng có thấy phần nào mọi người cũng đang có một chút là đang solution trước, sau đó nhóm đã thảo luận và nhận ra rằng là nhóm đang tìm giải pháp cho 1 vấn đề mơ hồ, nhóm đã bắt đầu lại ngay từ bước ban đầu là xác định rõ vấn đề hiểu rõ vấn đề có bắt nguồn từ đâu, actor là ai và như thế nào, từ đó nhóm tổng kết lại và giúp nhau rút kinh nghiệm.
**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Tôi rất đồng ý khi bị phản biện. Cụ thể là về problem card #1 của tôi là về tìm linh kiện điện tử, lúc đầu thì ý tưởng của tôi đã nêu không rõ công việc của AI như thế nào, giải thích khá là lệch so với đúng những gì mà AI nên làm trong dự án của tôi. Từ đó nhận ra rằng cần có phản biện để được phát triển hơn cũng như có góc nhìn khác về dự án không chỉ dự án này mà các dự án sau này nữa.
**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Điều khiến tôi chú ý là không phải mọi lỗi cài đặt thư viện đều cần đến AI. Một số lỗi phổ biến có thể giải quyết bằng checklist hoặc các quy tắc đơn giản. Điều này khiến tôi nhận ra cần xác định đúng phạm vi sử dụng AI, tránh đưa AI vào chỉ vì muốn sản phẩm có tính ứng dụng AI. Tuy nhiên, tôi chưa trực tiếp phụ trách CP4 nên chưa thể đưa ra kết luận từ kết quả phỏng vấn hoặc research của nhóm.
**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Điều khó nhất đối với tôi là phân biệt giữa vấn đề thực tế của người dùng và giải pháp mà nhóm muốn xây dựng. Ban đầu, tôi dễ tập trung vào việc AI có thể phân tích log và đề xuất cách sửa lỗi như thế nào. Tuy nhiên, khi viết Problem Statement, tôi phải quay lại xác định Actor, quy trình, bottleneck và tác động thực tế. Ngoài ra, việc sử dụng số liệu cũng cần cẩn thận vì 61 phút chỉ là kết quả của trường hợp đã khảo sát, chưa thể đại diện cho tất cả lập trình viên.
**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Nếu làm lại, tôi sẽ dành nhiều thời gian hơn để xác minh vấn đề ngay từ CP1 và CP2, thay vì chỉ tập trung hoàn thiện nội dung và chấm điểm candidate. Tôi cũng sẽ yêu cầu làm rõ nguồn gốc của các số liệu trước khi sử dụng chúng làm baseline. Tôi muốn phản biện nhóm mạnh hơn ở hai điểm: liệu bottleneck có thực sự cần AI giải quyết hay chỉ cần Rule, và liệu giải pháp đề xuất có tạo ra cải thiện đủ lớn so với quy trình hiện tại hay không.
**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
Bài toán nhóm tôi lựa chọn là hỗ trợ lập trình viên xử lý lỗi trong quá trình cài đặt thư viện Python. Quy trình hiện tại gồm đọc lỗi, kiểm tra môi trường, tìm kiếm nguyên nhân, thử cách khắc phục và kiểm tra lại. Bottleneck chính nằm ở bước thử phương án và kiểm tra lại, mất khoảng 30 phút trong tổng thời gian 61 phút của trường hợp đã khảo sát. Nhóm đặt mục tiêu giảm tổng thời gian xử lý xuống không quá 40 phút và thời gian bottleneck xuống không quá 15 phút. AI chỉ được phân tích log và đề xuất phương án, không tự ý chạy lệnh hoặc thay đổi môi trường lập trình. Các lỗi đơn giản có thể xử lý bằng Rule, còn AI hỗ trợ những lỗi phức tạp cần phân tích thêm ngữ cảnh. Lập trình viên vẫn là người kiểm tra, phê duyệt và quyết định thực hiện phương án khắc phục.
---

## 7. Tài liệu tham khảo

-
