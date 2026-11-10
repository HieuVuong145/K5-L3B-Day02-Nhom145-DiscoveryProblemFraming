# Báo cáo cá nhân — 2A202603816_NguyenVanHung

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Văn Hùng
- MSSV: 2A202603816
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Nhom145
- Link repo nhóm: https://github.com/HieuVuong145/K5-L3B-Day02-Nhom145-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Lặp lại |Giám sát mạng phải phân loại nhiều cảnh báo tương tự, cần nhanh chóng xác định và phân loại các cảnh báo trùng lặp, xác định mức độ ưu tiên |Người giám sát mạng|Nhiều alert xuất hiện trong thời gian ngắn, mất thời gian phân loại khoảng 2 phút/alert|
| 2 |Tốn thời gian |Khi chuẩn bị ôn tập cho một môn học, tôi muốn tổng hợp kiến thức từ nhiều tài liệu thành nội dung ngắn gọn để tiết kiệm thời gian ôn tập. |Sinh viên |Mỗi môn tín chỉ trung bình mất 1,2 ngày đọc lại và tổng hợp kiến thức |
| 3 |Đọc, tổng hợp |Khi phân tích một cảnh báo liên quan đến mã độc hoặc lỗ hổng bảo mật, tôi muốn tra cứu và đối chiếu thông tin từ nhiều nguồn threat intelligence để đánh giá chính xác mức độ nguy hiểm.|Người làm bảo mật|Phải tra cứu thông tin IOC, CVE, malware từ nhiều nguồn, thời gian không xác định chính xác|
| 4 |Tốn thời gian |Khi cần chuyển một báo cáo dài thành slide thuyết trình, tôi muốn nhanh chóng chọn lọc và sắp xếp các nội dung quan trọng thành từng slide để tiết kiệm thời gian chuẩn bị và giúp người nghe dễ nắm bắt thông tin.|Người thường xuyên thuyết trình |Khi chuyển báo cáo thành slide, tôi phải đọc lại nội dung, xác định các luận điểm quan trọng, loại bỏ thông tin không cần thiết và tóm tắt thành các ý ngắn gọn. Theo trải nghiệm cá nhân , thời gian thực tế tùy thuộc vào tài liệu|
| 5 |Tốn thời gian |Khi kiếm việc làm hoặc thực tập, tôi muốn đối chiếu yêu cầu tuyển dụng với kỹ năng hiện có để xác định vị trí phù hợp|Sinh viên sắp tốt nghiệp |Nhiều bài đăng tuyển dụng với nhiều yêu cầu khác nhau, khi tìm kiếm, thường mất khoảng 1,2 tiếng mỗi ngày |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.


- Ý 2,5 AI gợi ý. Giữ lại vì nó đúng là khó khăn từng gặp nhưng chưa nghĩ đến.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |Phân loại cảnh báo giám sát mạng |Có actor rõ ràng, có thời gian xử lý trung bình mỗi alert |Tỉ lệ alert trùng lặp và thời gian 2 phút/alert chưa chắc là đại diện đúng, nó chỉ là ước lượng |
| 2 |Chuyển báo cáo thành slide |Trải nghiệm cá nhân và quy trình khá dễ mô tả |Thời gian thực tế cho từng bước khó ước lượng |
| 3 |Đối chiếu JD với kỹ năng hiện có |Nhu cầu dễ gặp ở sinh viên tìm việc ||

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận nhiều cảnh báo mạng trong thời gian ngắn, tôi muốn xác định các cảnh báo tương tự và phân loại mức độ ưu tiên để giảm thời gian xử lý và hạn chế bỏ sót cảnh báo quan trọng. |
| Actor |Nhân viên giám sát mạng |
| Thời điểm / bối cảnh |Trong ca trực hệ thống giám sát xuất hiện nhiều cảnh báo |
| Quy trình hiện tại (3–7 bước) |Tiếp nhận alert → Đọc log → Kiểm tra cảnh báo tương tự → Đánh giá mức độ ưu tiên → Ghi nhận và xử lý |
| Bottleneck (bước nào, mất bao nhiêu phút) |Kiểm tra đối chiếu các cảnh báo tương tự, tùy thuộc vào số lượng alert mà thời gian khác nhau |
| Impact (nếu không giải thì sao) |Lặp lại và tốn thời gian, có thể làm chậm phát hiện quan trọng|
| Success metric (baseline → target) |Tăng tốc độ xử lý lên khoảng dưới 1 phút/alert với các alert đủ điều kiện phân loại |
| Phương án không dùng AI |Thiết lập rule, correlation, alert grouping, suppression và chuẩn hóa playbook. |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | Rule / Workflow / | 

Quy trình nháp hiện tại:

```text
1. Tiếp nhận cảnh báo
2. Đọc log và thông tin cảnh báo
3. Kiểm tra các cảnh báo tương tự
4. Đánh giá mức độ ưu tiên
5. Ghi nhận, xử lý hoặc chuyển cấp

```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi cần chuyển một báo cáo dài thành slide thuyết trình, tôi muốn nhanh chóng chọn lọc và tóm tắt các nội dung quan trọng để tiết kiệm thời gian chuẩn bị mà vẫn đảm bảo đầy đủ ý chính. |
| Actor | Người thường xuyên thuyết trình |
| Thời điểm / bối cảnh | Khi hoàn thành báo cáo và cần chuẩn bị slide cho buổi thuyết trình. |
| Quy trình hiện tại (3–7 bước) | Đọc báo cáo → Xác định luận điểm chính → Tóm tắt nội dung → Chia slide → Thiết kế và rà soát. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Xác định luận điểm quan trọng và tóm tắt nội dung, chia nội dung cho mỗi slide, thời gian tốn tùy vào tài liệu báo cáo. |
| Impact (nếu không giải thì sao) | Mất thời gian |
| Success metric (baseline → target) | Giảm đa phần thời gian chọn lọc và tóm tắt, đồng thời giữ đầy đủ luận điểm quan trọng của báo cáo. |
| Phương án không dùng AI | Sử dụng mẫu slide có sẵn, tự chuẩn bị nội dung đưa lên slide |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | Workflow kết hợp AI hỗ trợ tóm tắt |

Quy trình nháp hiện tại:

```text
1. Đọc lại báo cáo
2. Xác định luận điểm chính
3. Chọn lọc và tóm tắt
4. Phân chia nội dung thành slide
5. Thiết kế và rà soát slide

```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi tìm kiếm việc làm hoặc thực tập, tôi muốn đối chiếu yêu cầu tuyển dụng với kỹ năng hiện có để xác định vị trí phù hợp và những kỹ năng cần bổ sung. |
| Actor | Sinh viên sắp tốt nghiệp, người tìm việc |
| Thời điểm / bối cảnh | Khi tìm kiếm các vị trí thực tập hoặc tuyển dụng trên website, mạng xã hội và nền tảng việc làm. |
| Quy trình hiện tại (3–7 bước) | Tìm tin tuyển dụng → Đọc JD → Xác định yêu cầu → Đối chiếu với CV/kỹ năng → Lưu hoặc ứng tuyển. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Đọc và đối chiếu nhiều JD có cách diễn đạt khác nhau, khoảng 2 phút mỗi bài, và mất nhiều thời gian cho việc tìm kiếm |
| Impact (nếu không giải thì sao) |Tốn thời gian, có thể bỏ qua vị trí phù hợp hoặc ứng tuyển vào vị trí chưa đáp ứng yêu cầu |
| Success metric (baseline → target) |Giảm thời gian tìm kiếm, đọc và đối chiếu thông tin |
| Phương án không dùng AI |Sử dụng bộ lọc, thanh tìm kiếm của các nền tảng |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | Workflow kết hợp AI |

Quy trình nháp hiện tại:

```text
1. Tìm kiếm tin tuyển dụng
2. Đọc mô tả công việc (JD)
3. Xác định các kỹ năng yêu cầu
4. Đối chiếu với CV và kỹ năng
5. Lưu vị trí hoặc ứng tuyển
```

### Card muốn pitch nhất

- Card số: #1 - Phân loại cảnh báo giám sát mạng
- Vì sao: Vấn đề có actor cụ thể, công việc lặp lại, đầu vào là các cảnh báo có cấu trúc và có thể đánh giá qua thời gian phân loại. Tuy nhiên, vẫn tùy vào việc hệ thống dùng đã hỗ trợ correlation, grouping hoặc suppression đến mức nào.
- Câu hỏi muốn nhóm phản biện: Liệu việc phân loại cảnh báo chậm chủ yếu do số lượng cảnh báo trùng lặp, hay do thiếu ngữ cảnh và quy trình xử lý chưa được chuẩn hóa? Nếu sử dụng rule và alert grouping đã giải quyết được phần lớn vấn đề thì có thực sự cần AI không?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Thời gian 2 phút/alert chưa rõ cách đo | Đồng ý | |
| Chưa chứng minh AI tốt hơn phương án rule/workflow | Đồng ý | |
| Thời gian 2 phút/alert chưa rõ cách đo | Đồng ý | |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card |Đưa ra ba candidate: phân loại cảnh báo mạng, chuyển báo cáo thành slide, đối chiếu JD với kỹ năng. |Có ba mục đề xuất trong `group_report.md` phần 2.1 (candidate #1–#3), các vấn đề này được đưa vào bước hội tụ nhóm. |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: Với bài điều hướng khám bệnh, hỏi điểm khác biệt với hệ thống tra cứu và vai trò thật của AI. Với Homework Assistant, đặt câu hỏi về bài tập trong vở, kết nối Zalo/LMS/Google Classroom, API và quyền truy cập. |Làm rõ rủi ro thu thập dữ liệu từ nhiều nguồn và yêu cầu không bắt đầu bằng giải pháp AI. |
| Nhận phản biện | Câu hỏi tôi nhận được: Candidate #1: Thắng hỏi về các giải pháp đã có; #2: Hiếu hỏi về điểm khác biệt so với công cụ AI hiện có; #3: Trường hỏi cách giúp ứng viên tìm đúng vị trí.| Tôi đã sửa gì:|
| Gom cluster / cây OST |Trao đổi cách gom nhóm vấn đề theo pain (tổng hợp thông tin, đối chiếu/ra quyết định, theo dõi quy trình) và chỉnh cách diễn đạt opportunity thay vì solution. |Bản hội tụ có tại `group_report.md` phần 2.3 |
| Chọn candidate problem |Đánh giá shortlist #9/#7/#12 theo 7 tiêu chí, rà soát độ tin cậy của số liệu và lý do chọn #9. |`group_report.md` mục 2.4. Điểm số mang tính đánh giá nhóm |
| Kiểm chứng / research |Có đặt câu hỏi phản biện về khả năng thu thập dữ liệu từ các nguồn Zalo/LMS. | |
| Quy trình nhóm |Sử dụng kết quả CP5 làm đầu vào để đánh giá các mức can thiệp tại mục 6, 7. | |
| Problem Statement |Phát triển Problem Statement v1 |`group_report.md` mục 7, target vẫn là giả thuyết/pilot, không phải kết quả thực nghiệm. |
| Mức can thiệp AI |Phân tích ma trận độ mơ hồ × độ phức tạp, so sánh No AI/Rule/Workflow/Agent, xây dựng AI Canvas và đánh giá hướng augment với Human-in-the-Loop. |Đề xuất Workflow có AI hỗ trợ chẩn đoán và lập trình viên kiểm soát lệnh |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan |Gợi ý thêm vấn đề và chuẩn hóa Job Story. |Gọi ý và hoàn thiện tốt |Gợi ý chung chung, không cụ thể thực tế |Giữ những khó khăn đã gặp |
| CP2 Problem Card |PHản biện bottelneck, baseline, phương án không dùng AI |Đánh giá đúng số liệu ước lượng khác với số liệu đo |Dễ đưa target khi chưa đủ baseline tin cậy |Gọi lại đúng số liệu ước lượng, bổ sung phương án Rule/Workflow và cách đo |
| CP3 Hội tụ nhóm |Rà soát và đánh giá kết quả |Đánh giá và đưa ra thêm các tiêu chí đánh giá khác quan hơn | |Áp dụng thêm các tiêu chí đánh giá nhóm thấy hợp lý |
| CP5 Quy trình |Đọc tài liệu và đánh giá CP5 |Giúp hiểu thời điểm AI có thể can thiệp và quy trình người dùng | |Chỉ dùng để tham chiếu cho phần sau, không phụ trách |
| CP6 Mức can thiệp / quyết định |Nhờ AI giải thích và trình bày ma trận mơ hồ x phức tạp, so sánh các mức can thiệp |Hộ trợ lập luận cho Workflow có AI, với HITL |Ma trận còn thiếu và khó hiểu ban đầu |Chuyển thành bảng Markdown 2x2, giữ quyền phê duyệt, thực thi ở lập trình viên và không mặc định AI tốt hơn rule |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Có những bài toán đã có các giải pháp hiện tại, cần đánh giá và đề xuất kỹ lưỡng trước khi đi sâu vào, xem có ích gì không, có ưu điểm gì không.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
AI Homework Assitant rất hữu ích nhưng có rất nhiều vấn đề khi đi vào hiểu thêm như bài tập loại bài vở kiểm tra kiểu gì, các ứng dụng, nền tảng có chức năng gọi API không, khả năng thực tế đến đâu, cách AI xử lý các loại đầu vào khác nhau... Cảm thấy khó, chưa xử lý.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Có. Với việc hỗ trợ các nhân viên giám sát mạng với các alert lặp lại, các hệ thống hiện đại ngày nay đa phần đều sở hữu, từ các rules, offense, đến cả các chức năng AI tích hợp

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Không, bởi đa phần đều là các vấn đề khá quen thuộc 

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Chưa thực sự làm và có các số liệu thực tế, khá khó để đánh giá đúng

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Nếu làm lại, tôi sẽ muốn đề xuất vấn đề ưu tiên của cá nhân mình khác đi, vì tôi lúc đó cũng biết có khá nhiều hướng giải pháp cho giám sát mạng, tuy nhiên điều đó đến từ trải nghiệm cá nhân từ lúc mới tiếp xúc các hệ thống giám sát mạng nên tôi ưu tiên.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
Đề xuất các problem thực tế mà mọi người gặp phải, gây ra các vấn đề mất thời gian, lặp đi lặp lại, ... Sau đó làm rõ các problem đó với trường thông tin đánh giá ban đầu như actor, bottlenecks,... Sau đó thống kê, gom nhóm các problem tương tự, thực hiện chấm điểm các candidate trên các tiêu chí khác nhau, chọn ra problem. Sau đó đánh giá, vạch ra ranh giới cho AI, kiểm chứng các mức độ can thiệp AI, đánh giá khách quan problem ưu tiên dùng gì. Cuối cùng đưa ra quyết định.

---

## 7. Tài liệu tham khảo

-
