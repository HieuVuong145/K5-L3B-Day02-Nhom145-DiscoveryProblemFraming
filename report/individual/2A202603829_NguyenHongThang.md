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

### Problem Card #1 - AI Homework Assistant

| Trường | Nội dung |
|---|---|
| Job Story | Khi giáo viên giao bài tập qua nhiều kênh như LMS, Zalo, vở ghi và thông báo trực tiếp, tôi muốn tổng hợp tất cả nhiệm vụ học tập vào một nơi và theo dõi tiến độ hoàn thành, để không bỏ sót bài và chủ động hỗ trợ con học tập. |
| Actor |Phụ huynh (người sử dụng chính); học sinh (người thực hiện); giáo viên (người giao bài). |
| Thời điểm / bối cảnh |Hàng ngày, đặc biệt sau giờ học và buổi tối khi phụ huynh kiểm tra bài tập, kế hoạch học tập và deadline của con. |
| Quy trình hiện tại (3–7 bước) |1. Nhận thông báo giao bài từ giáo viên. 2. Đăng nhập LMS kiểm tra từng môn. 3. Đọc thông báo Zalo, email và kiểm tra vở ghi. 4. Ghi lại bài tập và hạn nộp. 5. Hỏi con về tình trạng hoàn thành. 6. Kiểm tra bài làm và trạng thái nộp trên LMS. 7. Nhắc nhở những nhiệm vụ chưa hoàn thành. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 2–4: phải chuyển đổi giữa nhiều nguồn và tổng hợp thủ công. Bước 5–6: khó xác minh tình trạng thực tế. Giả định ban đầu: 20–40 phút/ngày. |
| Impact (nếu không giải thì sao) |Bỏ sót bài, quên deadline, học sinh bị động, phụ huynh mất thời gian, phát sinh mâu thuẫn do nhắc nhở thường xuyên. |
| Success metric (baseline → target) |Baseline giả định: 20–40 phút/ngày. Target: giảm ít nhất 50% thời gian tổng hợp; ít nhất 95% nhiệm vụ được ghi nhận chính xác; giảm ít nhất 50% số bài bị bỏ sót. |
| Phương án không dùng AI |Google Sheets hoặc ứng dụng quản lý công việc, phụ huynh nhập bài tập, môn học, deadline và trạng thái thủ công. |
| Giả thuyết về AI (nếu có) |AI sử dụng OCR, NLP và Agent để đọc thông báo, ảnh chụp và dữ liệu LMS; tự trích xuất môn học, nội dung, deadline, phân loại nhiệm vụ, phát hiện trùng lặp và nhắc nhở. |
| Cảm nhận nhanh | AI hỗ trợ thu thập, xử lý và điều phối; phụ huynh xác nhận thông tin quan trọng.|

Quy trình nháp hiện tại:
```text
Giáo viên giao bài
       ↓
Phụ huynh nhận thông báo
       ↓
Kiểm tra LMS + Zalo + vở ghi
       ↓
Tự tổng hợp danh sách bài tập
       ↓
Hỏi con về tiến độ
       ↓
Kiểm tra bài làm và trạng thái nộp
       ↓
Nhắc nhở và theo dõi

Quy trình mong muốn

    LMS + Zalo + Email + Ảnh chụp
                 ↓
          AI thu thập dữ liệu
                 ↓
       OCR + NLP trích xuất bài tập
                 ↓
      Danh sách nhiệm vụ tập trung
                 ↓
       Phụ huynh xác nhận dữ liệu
                 ↓
      Theo dõi tiến độ + Deadline
                 ↓
       Nhắc nhở + Báo cáo hàng ngày
```

### Problem Card #2 - Tự động lập thông báo tiền điện, nước

| Trường | Nội dung |
|---|---|
| Job Story | Khi đến kỳ thanh toán tiền điện, nước cho các căn hộ và văn phòng cho thuê, tôi muốn tự động thu thập, tổng hợp và tính toán chỉ số tiêu thụ để lập thông báo thanh toán chính xác, nhanh chóng và giảm công việc thủ công. |
| Actor | Chủ nhà, người quản lý tòa nhà, kế toán và khách thuê. |
| Thời điểm / bối cảnh | Định kỳ hàng tháng, khi chốt chỉ số công tơ và lập thông báo thanh toán cho khách thuê. |
| Quy trình hiện tại (3–7 bước) | 1. Chụp ảnh công tơ nước và công tơ điện. 2. Truy xuất dữ liệu điện từ phần mềm giám sát. 3. Nhập chỉ số điện, nước vào Excel. 4. Đối chiếu chỉ số với kỳ trước. 5. Tính sản lượng và chi phí. 6. Nhập dữ liệu vào mẫu thông báo thanh toán. 7. Xuất và gửi thông báo cho khách thuê. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–4: nhập liệu và đối chiếu nhiều nguồn. Bước 5–6: tính toán, kiểm tra và nhập lại dữ liệu. Giả định ban đầu: 5–10 phút/đơn vị thuê, chưa tính xử lý sai lệch. |
| Impact (nếu không giải thì sao) | Tốn thời gian, nhầm chỉ số, sai số tiền thanh toán, khiếu nại từ khách thuê và khó truy xuất lịch sử. |
| Success metric (baseline → target) | Baseline giả định: 5–10 phút/đơn vị. Target: giảm ít nhất 70% thời gian lập thông báo; độ chính xác tính toán đạt 100% trên bộ dữ liệu đã xác nhận; giảm tối đa nhập liệu trùng lặp. |
| Phương án không dùng AI | Excel có công thức tự động, biểu mẫu nhập liệu thống nhất, Power Query để tổng hợp dữ liệu. |
| Giả thuyết về AI (nếu có) | OCR đọc chỉ số công tơ từ ảnh; Agent thu thập dữ liệu từ Excel/phần mềm điều hòa, đối chiếu kỳ trước, phát hiện bất thường và tự động tạo thông báo theo mẫu. |
| Cảm nhận nhanh | Workflow + Agent. OCR và AI xử lý dữ liệu đầu vào; công thức tính tiền phải được kiểm soát bằng quy tắc xác định. |

**Quy trình nháp hiện tại:**
```text
Đến kỳ chốt tiền hàng tháng
          ↓
Chụp ảnh công tơ điện, nước
          ↓
Truy xuất dữ liệu điện điều hòa
          ↓
Nhập và tổng hợp Excel
          ↓
Đối chiếu kỳ trước
          ↓
Tính toán tiền điện, nước
          ↓
Lập thông báo và gửi khách thuê
```

**Quy trình mong muốn:**
```text
Ảnh công tơ + File Excel + Dữ liệu điều hòa
                    ↓
              AI thu thập dữ liệu
                    ↓
           OCR + Chuẩn hóa dữ liệu
                    ↓
          Đối chiếu và phát hiện lỗi
                    ↓
          Tính toán theo quy tắc
                    ↓
          Người quản lý xác nhận
                    ↓
          Tạo thông báo tự động
                    ↓
              Gửi khách thuê
```

### Problem Card #3 - – Quản lý yêu cầu sửa chữa của khách thuê

| Trường | Nội dung |
|---|---|
| Job Story |Khi khách thuê phản ánh sự cố điện, nước, điều hòa hoặc thiết bị trong căn hộ, tôi muốn tự động tiếp nhận, phân loại và theo dõi yêu cầu sửa chữa để xử lý nhanh chóng, tránh thất lạc thông tin và nâng cao chất lượng dịch vụ.|
| Actor |Khách thuê (người phản ánh); người quản lý tòa nhà (người tiếp nhận và điều phối); kỹ thuật viên (người xử lý); chủ nhà (người giám sát). |
| Thời điểm / bối cảnh |	Phát sinh hàng ngày, bất cứ khi nào khách thuê gặp sự cố trong quá trình sử dụng căn hộ hoặc văn phòng. |
| Quy trình hiện tại (3–7 bước) |1. Khách thuê gọi điện hoặc nhắn tin Zalo báo sự cố. 2. Người quản lý tiếp nhận và ghi nhớ thông tin. 3. Hỏi thêm về vị trí, loại sự cố và mức độ nghiêm trọng. 4. Liên hệ kỹ thuật viên phù hợp. 5. Theo dõi quá trình sửa chữa. 6. Xác nhận với khách thuê sau khi xử lý. 7. Lưu lại thông tin và chi phí sửa chữa. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 1–3: thông tin không đầy đủ, phải hỏi lại nhiều lần. Bước 4–5: mất thời gian tìm người xử lý và theo dõi. Giả định ban đầu: 10–20 phút tiếp nhận và điều phối mỗi sự cố, chưa tính thời gian sửa chữa. |
| Impact (nếu không giải thì sao) |Sự cố bị xử lý chậm, thông tin thất lạc, khách thuê không hài lòng, khó kiểm soát chi phí và lịch sử bảo trì thiết bị. |
| Success metric (baseline → target) |Baseline giả định: 10–20 phút tiếp nhận và điều phối/sự cố. Target: giảm ít nhất 50% thời gian tiếp nhận; 100% yêu cầu được ghi nhận; ít nhất 90% yêu cầu được phân loại đúng và có người phụ trách. |
| Phương án không dùng AI |Google Forms hoặc ứng dụng quản lý ticket; khách thuê điền biểu mẫu, người quản lý phân công kỹ thuật viên và cập nhật trạng thái thủ công. |
| Giả thuyết về AI (nếu có) |AI Agent đọc nội dung tin nhắn, nhận diện loại sự cố, vị trí, mức độ ưu tiên; tự tạo ticket, đề xuất kỹ thuật viên, nhắc tiến độ và tổng hợp báo cáo. |
| Cảm nhận nhanh | Workflow + Agent. AI hỗ trợ tiếp nhận, phân loại và điều phối; người quản lý quyết định với sự cố nghiêm trọng hoặc cần phê duyệt chi phí. |

Quy trình nháp hiện tại:
```text
Khách thuê phát sinh sự cố
           ↓
Gọi điện / Nhắn Zalo
           ↓
Người quản lý tiếp nhận
           ↓
Hỏi thêm thông tin và xác định sự cố
           ↓
Tìm kiếm kỹ thuật viên
           ↓
Điều phối và theo dõi sửa chữa
           ↓
Xác nhận kết quả với khách thuê
           ↓
Lưu lịch sử sửa chữa

Quy trình mong muốn
    Khách thuê gửi tin nhắn / Ảnh / Video
                 ↓
             AI tiếp nhận
                 ↓
       Phân loại loại sự cố, vị trí
                 ↓
        Đánh giá mức độ ưu tiên
                 ↓
          Tạo phiếu yêu cầu
                 ↓
       Đề xuất kỹ thuật viên phù hợp
                 ↓
       Người quản lý xác nhận
                 ↓
       Theo dõi tiến độ sửa chữa
                 ↓
       Xác nhận và lưu lịch sử
```

### Card muốn pitch nhất

- Card số: 01
- Vì sao: Xuất phát từ nhu cầu thực tế của phụ huynh: bài tập được giao qua nhiều kênh như LMS, Zalo, vở ghi hoặc thông báo trực tiếp. Phụ huynh mất thời gian tổng hợp, theo dõi và nhắc con hoàn thành bài. Tôi muốn giải quyết vấn đề này bằng một trợ lý AI.
- Câu hỏi muốn nhóm phản biện: Làm thế nào để lấy thông tin bài tập từ LMS một cách tự động và ổn định? Nếu LMS không cung cấp API hoặc không cho phép truy cập dữ liệu thì có giải pháp thay thế nào?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
|Phụ thuộc vào khả năng truy cập dữ liệu LMS; mỗi trường có thể sử dụng một hệ thống khác nhau. |Đồng ý |Không giả định có thể kết nối trực tiếp với mọi LMS. Cần khảo sát LMS thực tế và kiểm tra khả năng cung cấp API. |
|Dữ liệu bài tập đến từ nhiều nguồn, có thể trùng lặp hoặc thiếu hạn nộp.|Đồng ý|Bổ sung bước AI chuẩn hóa, phát hiện trùng lặp và yêu cầu phụ huynh xác nhận thông tin chưa rõ.|
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
