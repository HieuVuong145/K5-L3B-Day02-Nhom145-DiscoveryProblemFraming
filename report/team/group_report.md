# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: Nhóm 145
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Khi gặp lỗi trong quá trình cài đặt thư viện lập trình, tôi muốn kiểm tra nguyên nhân và cách khắc phục theo một quy trình thống nhất, để không phải xử lý lại từ đầu.
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
| 7 |Nguyễn Đình Trường |Khi cần tìm một linh kiện điện tử phù hợp với yêu cầu kỹ thuật, tôi muốn so sánh được thông số và khả năng tương thích của nhiều linh kiện, để tránh chọn sai linh kiện và phải thay thế. |Kỹ sư thiết kế phần cứng |Công đoạn đọc datasheet, trích xuất thông số và đối chiếu khả năng tương thích mất khoảng 35–55 phút. Tổng quy trình tìm kiếm và lựa chọn một linh kiện mất khoảng 60–95 phút. | AI sẽ được thể hiện như nào tại chưa thấy rõ vai trò của AI trong problem? (Hiếu) |
| 8 |Nguyễn Đình Trường |	Khi cần viết tài liệu kỹ thuật từ ghi chú hoặc kết quả công việc, tôi muốn trình bày thông tin theo một cấu trúc thống nhất, để giảm công sức biên soạn và hạn chế sai lệch. |Người viết tài liệu kỹ thuật |Bước 3 và 4: Phân loại thông tin và biên soạn tài liệu. Thông tin đầu vào nằm ở nhiều nguồn, không đồng nhất về cách diễn đạt và mức độ chi tiết. Người viết phải tự xác định nội dung nào thuộc mục nào, chuyển ghi chú thành câu văn kỹ thuật và đảm bảo không làm sai lệch ý nghĩa ban đầu. Đây là hai công đoạn có khả năng tiêu tốn nhiều thời gian nhất. | |
| 9 |Nguyễn Đình Trường |Khi gặp lỗi trong quá trình cài đặt thư viện lập trình, tôi muốn kiểm tra nguyên nhân và cách khắc phục theo một quy trình thống nhất, để không phải xử lý lại từ đầu. |	Lập trình viên |Bước 5 và bước 6: Thử phương án khắc phục và kiểm tra lại, mất khoảng 30 phút (chiếm 49,2% tổng thời gian 61 phút). | |
| 10 |Nguyễn Hồng Thắng |AI Homework Assistant |Phụ huynh (người sử dụng chính); học sinh (người thực hiện); giáo viên (người giao bài). |Bước 2–4: phải chuyển đổi giữa nhiều nguồn và tổng hợp thủ công. Bước 5–6: khó xác minh tình trạng thực tế. Giả định ban đầu: 20–40 phút/ngày. |Hùng: Vẫn có phần lớn bài tập được giao qua bài vở, xử lý kiểu gì? Việc tổng hợp từ nhiều nguồn thì kết nối với Zalo, website trường học và Google Classroom bằng cách nào? Các nền tảng này có hỗ trợ API và cấp quyền truy cập phù hợp hay không?|
| 11 |Nguyễn Hồng Thắng |Tự động lập thông báo tiền điện, nước |Chủ nhà, người quản lý tòa nhà, kế toán và khách thuê. |Bước 2–4: nhập liệu và đối chiếu nhiều nguồn. Bước 5–6: tính toán, kiểm tra và nhập lại dữ liệu. Giả định ban đầu: 5–10 phút/đơn vị thuê, chưa tính xử lý sai lệch. | Vai trò của AI là gì khi những công việc này hoàn toàn có thể dựa vào 1 thuật toán định sẵn để tính? (Hiếu) |
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

- AI Homework Assistant là tên giải pháp, không phải opportunity. Nhu cầu thực tế là phụ huynh gặp khó khăn khi thu thập, tổng hợp và theo dõi bài tập của con từ nhiều nguồn.

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #9 - Xử lý lỗi cài đặt thư viện |5 |4 |3 |4 |5 |4 |4 |29 |
| #7 - Tìm kiếm, lựa chọn linh kiện điện tử |5 |5 |3 |4 |4 |4 |3 |27 |
| #12 - Quản lý yêu cầu sửa chữa khách thuê|4 |5 |2 |3 |4 |4 |3 |24 |

**Candidate được chọn:** #9 - Xử lý lỗi cài đặt thư viện

**Vì sao chọn:** Candidate #9 đạt 29/35 điểm, cao nhất trong ba vấn đề được đưa vào shortlist. Vấn đề có đối tượng sử dụng rõ ràng, quy trình xử lý cụ thể và có khả năng kiểm chứng trong môi trường lập trình. Nhóm có thể chủ động tái hiện các lỗi phổ biến như thiếu thư viện hoặc xung đột phiên bản, ghi nhận thời gian xử lý, số lần thử và kết quả khắc phục.

Ngoài ra, nhóm có thể so sánh các phương án không dùng AI như checklist, tài liệu hướng dẫn và công cụ quản lý dependency với phương án sử dụng AI để phân tích log và đề xuất cách xử lý. Điều này phù hợp với mục tiêu của bài lab là lựa chọn mức can thiệp công nghệ dựa trên vấn đề thực tế.

**Vì sao loại các candidate còn lại:**
- #7 – Tìm kiếm và lựa chọn linh kiện điện tử: Vấn đề có tính thực tiễn và quy trình rõ ràng, nhưng việc kiểm tra tính tương thích của linh kiện đòi hỏi kiến thức phần cứng chuyên sâu. Nhóm cần thêm dữ liệu và tiêu chí đánh giá để xác nhận độ chính xác của kết quả.

- #12 – Quản lý yêu cầu sửa chữa khách thuê: Bằng chứng định lượng còn hạn chế, thời gian xử lý hiện mới là giả định. Việc thu thập dữ liệu thực tế cũng phụ thuộc vào khả năng tiếp cận người quản lý tòa nhà và khách thuê.

**Xử lý bất đồng (nếu có):** 

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Lập trình viên thường xuyên mất từ 30–60 phút cho mỗi sự cố lỗi xung đột thư viện/môi trường và cảm thấy đây là công việc gây ức chế, gián đoạn mạch làm việc. | Value | 5 | 3 | Có |
| 2 | Phần lớn thời gian bị lãng phí là ở khâu tra cứu phân tán và thử-sai (trial and error) các lệnh sửa ngẫu nhiên trên terminal, chứ không phải ở bước đọc thông báo lỗi. | Value | 5 | 2 | Có |
| 3 | Log lỗi terminal (stack trace, pip dependency conflict) kết hợp thông tin môi trường (`python -V`, `pip list`, OS) chứa đủ ngữ cảnh để AI chẩn đoán chính xác nguyên nhân gốc rễ mà không cần đọc toàn bộ mã nguồn dự án. | Feasibility | 4 | 3 | — |
| 4 | Lập trình viên không tin tưởng để AI tự động thực thi lệnh chạy ngầm (blind execution) vì sợ làm hỏng luôn virtual environment; họ muốn thấy lệnh gợi ý kèm giải thích rõ ràng trước khi xác nhận chạy. | Usability | 5 | 2 | Có |
| 5 | Chi phí gọi API/AI chẩn đoán lỗi terminal nằm trong mức chấp nhận được đối với lập trình viên cá nhân hoặc nhóm nhỏ (dưới 10.000 VNĐ/tháng nếu dùng các mô hình nhỏ/nhẹ). | Viability | 3 | 3 | — |

Giả định nhóm kiểm chứng trong buổi này: Giả định #1, #2 và #4.

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn, Log, ticket

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Backend Developer (1.5 năm kinh nghiệm làm việc với Python/FastAPI) |
| Câu nói đáng nhớ nhất (nguyên văn) | *"Có hôm cài thêm package mới để làm xuất báo cáo Excel, nó báo lỗi xung đột phiên bản `pydantic` với thư viện cũ, mình ngồi gõ `pip install --upgrade` loạn xạ mất gần 2 tiếng, cuối cùng hỏng luôn virtualenv đành phải xóa đi tạo lại từ đầu."* |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | 3 ngày trước khi cài thư viện xử lý ảnh OpenCV trên máy Mac Apple Silicon, bị lỗi C++ wheel build fail. |
| Hiện đang xử lý bằng cách nào (workaround)? | Copy đoạn log dài trên Terminal dán lên Google / ChatGPT, thử từng lệnh gợi ý; nếu vỡ môi trường thì đành xóa hẳn folder `.venv` và cài lại từ đầu. |
| Mất bao lâu, bao lần? | 45–60 phút mỗi lần gặp lỗi lạ; tần suất khoảng 2–3 lần/tháng. |
| Insight / opportunity rút ra | Nỗi sợ lớn nhất không phải là không tìm ra cách sửa, mà là việc thử các phương án sửa không được kiểm soát làm "nát" môi trường (dependency hell). Lập trình viên rất cần một lộ trình chẩn đoán có giải thích và cơ chế thử nghiệm an toàn (dry-run/backup). |

**Interview snapshot #2:**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Sinh viên năm 4 ngành CNTT / Data Science |
| Câu nói đáng nhớ nhất (nguyên văn) | *"Mỗi lần clone repo đồ án của thầy hoặc nhóm khác về mà chạy `pip install -r requirements.txt` bị lỗi C++ build tools hay mismatch version Python là em toát mồ hôi, ngồi tra StackOverflow cả buổi chiều."* |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Tuần trước khi thiết lập môi trường chạy mô hình PyTorch kết hợp CUDA cho môn học Deep Learning. |
| Hiện đang xử lý bằng cách nào (workaround)? | Chụp màn hình hỏi bạn bè hoặc xóa bớt các dòng trong file requirements rồi cài tay từng package một để xem gói nào bị lỗi. |
| Mất bao lâu, bao lần? | Khoảng 60–90 phút; xảy ra mỗi khi bắt đầu môn học mới, clone dự án mới hoặc chuyển môi trường máy tính. |
| Insight / opportunity rút ra | Lỗi môi trường xảy ra nặng nhất khi liên quan đến OS-specific libraries (C++ compiler, binary wheels, phiên bản Python). Cần phân biệt rõ lỗi cú pháp mã nguồn vs lỗi môi trường hệ thống. |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Phỏng vấn sâu (The Mom Test) + Khảo sát nhanh | 3 người phỏng vấn sâu + 8 người khảo sát nhanh trong lớp | 10/11 người xác nhận từng mất từ 45–90 phút chỉ để giải quyết lỗi thư viện/môi trường; 9/11 người đồng ý rằng bước "thử các lệnh sửa trên terminal" là bước tốn thời gian và rủi ro nhất. | 1 lập trình viên kinh nghiệm chia sẻ: *"Nếu dự án dùng Docker chuẩn hoặc uv lock file thì hiếm khi gặp lỗi, chỉ những ai quản lý môi trường thủ công bằng pip không ghim version mới hay bị."* |
**Nhóm đã sửa problem thế nào sau kiểm chứng:**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **Astral uv** (Python package & project manager) | `https://docs.astral.sh/uv/` | Bước 4 (Đối chiếu phiên bản) và Bước 5 (Thử phương án khắc phục) | Cực nhanh (viết bằng Rust), tích hợp thuật toán giải quyết xung đột (PubGrub resolver), tự động tạo lockfile đảm bảo môi trường tái lập. | Là công cụ dòng lệnh thuần túy (Rule-based), không giải thích nguyên nhân bằng ngôn ngữ tự nhiên đối với các lỗi build C/C++, compiler OS (thiếu wheel, thiếu gcc). Người mới vẫn bối rối khi đọc log xung đột dài. | Cần tận dụng tư duy phân tích cây phụ thuộc chuẩn xác, kết hợp AI để giải thích nguyên nhân gốc rễ và đề xuất cách xử lý phù hợp cho người dùng. |
| **GitHub Copilot in the CLI** | `https://docs.github.com/en/copilot/github-copilot-in-the-cli` | Bước 2 (Đọc và xác định lỗi) và Bước 3 (Tìm kiếm nguyên nhân, gợi ý lệnh sửa) | Giải thích câu lệnh và gợi ý lệnh sửa ngay trên Terminal thông qua giao diện dòng lệnh, không cần chuyển ngữ cảnh sang trình duyệt. | Hay đưa ra gợi ý chung chung mang tính chất "thử xem sao" (như `pip install --force-reinstall`), không kiểm tra trạng thái tương thích toàn bộ môi trường ảo hiện tại, dễ gây "ảo giác" (hallucination) tạo lệnh không tương thích với OS/Python version. | AI cần nhận được input ngữ cảnh đầy đủ (Python version, OS, pip list/virtualenv info) thay vì chỉ đọc mỗi vài dòng log cuối của Terminal. |
| **pip-tools** (`pip-compile` & `pip-sync`) | `https://github.com/jazzband/pip-tools` | Quản lý phiên bản và đồng bộ môi trường (No AI / Rule) | Khóa chính xác cây phụ thuộc, đảm bảo tính đồng nhất giữa môi trường dev và production. | Không có cơ chế tự giải thích hoặc gợi ý giải pháp khi xảy ra mâu thuẫn giữa 2 thư viện cấp 1 đòi 2 phiên bản khác nhau của thư viện cấp 2. | Rule-based quản lý lockfile là nền tảng an toàn, AI đóng vai trò tư vấn khi có xung đột logic hoặc thiếu dependencies hệ thống. |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text
HIỆN TẠI — 6 bước, 61 phút, 6/6 bước thủ công

[1 Phát hiện lỗi: 3']
→ [2 Đọc và xác định lỗi: 5']
→ [3 Tìm kiếm nguyên nhân: 10']
→ [4 Đối chiếu phiên bản: 13']
→ [5 Thử phương án khắc phục: 15'] ← BOTTLENECK
→ [6 Kiểm tra lại chương trình: 15'] ← BOTTLENECK
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Lập trình viên|Lệnh cài đặt thư viện, môi trường lập trình | Thông báo lỗi| 3 phút|Có thể xảy ra do thiếu dependency, sai phiên bản hoặc xung đột môi trường |
| 2 |Lập trình viên | Error message, traceback |Nhận diện dấu hiệu và thành phần gây lỗi |5 phút |Phải tự xác định phần thông tin quan trọng trong log |
| 3 |Lập trình viên |Python, pip, OS, virtual environment, dependency |Thông tin cấu hình môi trường |10 phút |Kiểm tra phiên bản và tìm kiếm nguyên nhân qua Google, Stack Overflow, tài liệu chính thức |     
| 4 | Lập trình viên|Thông tin lỗi, cấu hình môi trường, kết quả tra cứu |Xác định nguyên nhân và phương án khắc phục phù hợp |13 phút |Đối chiếu phiên bản Python, thư viện và các dependency để tránh xung đột |
| 5 | Lập trình viên|Phương án khắc phục đã lựa chọn |Thay đổi môi trường hoặc phiên bản thư viện |15 phút |Phải thử cài đặt lại, đổi phiên bản hoặc điều chỉnh môi trường; có thể phát sinh lỗi mới |
| 6 | Lập trình viên|Môi trường sau khi điều chỉnh, chương trình cần chạy |Kết quả xác nhận cài đặt thành công hoặc lỗi còn tồn tại |15 phút |Chạy lại chương trình và kiểm tra; nếu chưa thành công phải quay lại bước tìm nguyên nhân |

**Bottleneck chính:** Bước 5 và bước 6 là bottleneck chính, chiếm tổng cộng 30 phút (49,2% tổng thời gian 61 phút). Lập trình viên phải tự thử các phương án khắc phục, điều chỉnh môi trường và chạy lại chương trình để xác nhận kết quả. Nếu phương án không phù hợp hoặc phát sinh lỗi mới, quy trình phải lặp lại, khiến thời gian xử lý kéo dài.

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
TƯƠNG LAI — 5 bước, khoảng 35 phút, 2/5 bước thủ công

[1 Thu thập log lỗi và môi trường: 3']       ← RULE / SCRIPT
→ [2 Kiểm tra lỗi phổ biến: 2']              ← RULE
→ [3 Phân tích lỗi và đề xuất cách sửa: 5']  ← AI
→ [4 Lập trình viên kiểm tra và thực hiện: 20'] ← CON NGƯỜI
→ [5 Chạy lại và xác nhận kết quả: 5']       ← CON NGƯỜI

BOUNDARY:
AI chỉ phân tích log lỗi, thông tin môi trường và đề xuất phương án. AI không tự chạy lệnh, cài/gỡ thư viện, thay đổi phiên bản Python,
chỉnh sửa môi trường ảo hoặc file cấu hình khi chưa được lập trình viên phê duyệt.
PHƯƠNG ÁN QUAY VỀ:
Nếu AI đề xuất sai, độ tin cậy thấp hoặc lỗi không được khắc phục, lập trình viên bỏ đề xuất và chuyển sang quy trình tra cứu thủ công
qua tài liệu chính thức, Stack Overflow hoặc GitHub.
```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước |6 | 5| |
| Tổng thời gian |61 phút |Khoảng 35 phút | |
| Số bước thủ công | 6/6 |2/5 |Lập trình viên vẫn kiểm tra và thực hiện |
| Bottleneck chính |Thử phương án + kiểm tra lại (30 phút) |Lập trình viên kiểm tra và thực hiện (20 phút) | Giữ con người kiểm soát việc thay đổi môi trường|
| Rủi ro mới phát sinh | |AI đề xuất sai, không phù hợp phiên bản hoặc gây lỗi mới |Xử lý bằng Rule, Boundary và phương án quay về |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** |Lập trình viên, đặc biệt là người thường xuyên cài đặt, cập nhật và quản lý thư viện trong các dự án Python.|
| **Quy trình** |Khi cài đặt thư viện gặp lỗi, lập trình viên đọc thông báo lỗi, kiểm tra môi trường, tìm kiếm nguyên nhân trên tài liệu hoặc diễn đàn, lựa chọn phương án khắc phục, thử thực hiện và chạy lại để xác nhận kết quả.|
| **Bottleneck** |Công đoạn thử phương án khắc phục và kiểm tra lại mất nhiều thời gian do lập trình viên phải tự lựa chọn, thực hiện và đánh giá nhiều cách xử lý. Công đoạn này hiện mất khoảng 30 phút, chiếm 49,2% tổng thời gian xử lý 61 phút trong trường hợp đã khảo sát. |
| **Impact** |Tăng thời gian xử lý sự cố, làm gián đoạn quá trình phát triển phần mềm và khiến lập trình viên phải lặp lại các thao tác tra cứu, cài đặt và kiểm tra.|
| **Success Metric** (baseline → target, cách đo) |Thời gian xử lý: 61 phút → ≤ 40 phút/lỗi. Thời gian tại bottleneck: 30 phút → ≤ 15 phút. Cách đo: ghi nhận thời gian từ lúc phát sinh lỗi đến khi cài đặt thành công, đồng thời đo riêng thời gian thử và kiểm tra phương án trên cùng một tập lỗi thử nghiệm. Đây là mục tiêu pilot cần kiểm chứng, không phải kết quả đã đạt được. |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) |Hệ thống chỉ hỗ trợ phân tích log, kiểm tra thông tin môi trường và đề xuất phương án. AI không tự động thực thi lệnh, thay đổi phiên bản Python, xóa hoặc cài đặt thư viện, sửa file cấu hình hay thay đổi dependency của dự án khi chưa có sự phê duyệt của lập trình viên. Với lỗi liên quan đến bảo mật, dữ liệu nhạy cảm hoặc không đủ thông tin để xác định nguyên nhân, hệ thống phải cảnh báo và yêu cầu con người kiểm tra.|

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:
- Phản biện 1: Việc xử lý lỗi cài đặt thư viện đã có nhiều công cụ hỗ trợ như Google, Stack Overflow, GitHub và các AI coding assistant. Cần làm rõ giải pháp của nhóm khác biệt ở điểm nào.
    Ý kiến nhóm: Đồng ý một phần. Nhóm không hướng tới xây dựng một công cụ hỏi đáp lập trình tổng quát, mà tập trung vào quy trình phân tích lỗi cài đặt thư viện dựa trên error log và thông tin môi trường cụ thể để đề xuất phương án khắc phục phù hợp.
- Phản biện 2: Không phải lỗi cài đặt nào cũng cần AI. Nhiều lỗi phổ biến có thể xử lý bằng checklist hoặc các quy tắc cố định.
    Ý kiến nhóm: Đồng ý. Nhóm sẽ so sánh phương án No AI, Rule, Workflow và Agent để xác định trường hợp nào cần AI, tránh sử dụng AI không cần thiết.
- Phản biện 3: AI có thể đề xuất lệnh không phù hợp với môi trường hoặc gây xung đột dependency nếu người dùng thực hiện máy móc.
    Ý kiến nhóm: Đồng ý. Hệ thống chỉ đề xuất phương án và giải thích nguyên nhân, không tự động thực thi lệnh. Lập trình viên phải kiểm tra và phê duyệt trước khi áp dụng.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp
| Độ phức tạp \ Độ mơ hồ | Thấp | Cao |
|---|---|---|
| **Cao** | Workflow theo quy trình xác định | **Workflow + AI / Agent (Bài toán #9)** |
| **Thấp** | No AI / Rule | AI hỗ trợ phân tích |

**Bài của nhóm nằm ở ô:** Độ mơ hồ cao - Độ phức tạp cao (đối với lỗi dependency và môi trường phức tạp).

**Vì sao:**

- **Độ mơ hồ cao:** Một thông báo lỗi cài đặt thư viện có thể xuất phát từ nhiều nguyên nhân như xung đột dependency, phiên bản Python không tương thích hoặc thiếu công cụ build. Không phải lúc nào cũng có thể xác định chính xác nguyên nhân chỉ dựa vào thông báo lỗi ban đầu.

- **Độ phức tạp cao:** Quá trình khắc phục có thể cần đối chiếu phiên bản Python, hệ điều hành, các package và quan hệ dependency. Việc thay đổi một thư viện có thể ảnh hưởng đến các thư viện khác, khiến quy trình phải lặp lại nhiều lần.

**Mức can thiệp đề xuất:** Workflow kết hợp AI.

Mặc dù bài toán có cả độ mơ hồ và độ phức tạp cao trong một số tình huống, chưa cần triển khai Agent tự chủ. Quy trình chẩn đoán có thể được xác định trước, AI chỉ hỗ trợ phân tích nguyên nhân và đề xuất phương án. Lập trình viên vẫn là người phê duyệt, thực hiện và kiểm tra kết quả.

Đối với các lỗi đơn giản, hệ thống ưu tiên Rule hoặc checklist thay vì sử dụng AI.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** |Checklist, hướng dẫn xử lý lỗi, tài liệu lỗi thường gặp|Người dùng gặp lỗi đơn giản, nguyên nhân rõ ràng |Vẫn phải tra cứu, đối chiếu và thử nghiệm thủ công |Không ưu tiên |
| **Rule** |Script kiểm tra Python, pip, virtualenv, dependency và nhận diện lỗi theo mẫu |Lỗi có dấu hiệu xác định, có thể viết quy tắc xử lý |Không bao quát hết các lỗi phụ thuộc ngữ cảnh |Dùng hỗ trợ |
| **Workflow** |Script thu thập môi trường → Rule kiểm tra → AI phân tích log → người dùng phê duyệt → kiểm tra kết quả |Quy trình các bước xác định trước nhưng cần AI diễn giải lỗi đa dạng |AI chẩn đoán sai hoặc đề xuất thay đổi không phù hợp |Đề xuất chọn |
| **Agent** |AI tự chọn công cụ, chạy lệnh kiểm tra và lặp lại các bước sửa lỗi |Khi thực sự cần tự điều chỉnh kế hoạch xử lý theo kết quả mới và có môi trường thử nghiệm an toàn |Có thể sửa sai dependency, thay đổi hoặc làm hỏng môi trường |Chưa chọn |

**Mức chọn:** Workflow có tích hợp AI tại bước phân tích và đề xuất phương án khắc phục.

**Vì sao không chọn mức đơn giản hơn:** Checklist và Rule hữu ích đối với lỗi phổ biến, nhưng có thể chưa đủ khi thông báo lỗi phụ thuộc vào nhiều phiên bản thư viện, hệ điều hành và quan hệ dependency. Workflow cho phép kết hợp kiểm tra có cấu trúc với AI để diễn giải ngữ cảnh, đồng thời giữ việc thay đổi môi trường dưới quyền kiểm soát của lập trình viên.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? |AI phân tích log và thông tin môi trường để dự đoán nhóm lỗi, nguyên nhân có khả năng xảy ra và đề xuất phương án xử lý kèm giải thích. |
| **Judgment** — con người cân nhắc, quyết định gì? |Lập trình viên đánh giá nguyên nhân AI đưa ra, đối chiếu với cấu hình và quyết định có chấp nhận phương án hay không. |
| **Action** — hành động cuối cùng là gì, ai làm? |Lập trình viên thực hiện phương án được lựa chọn, kiểm tra lại chương trình và xác nhận kết quả. AI không tự chạy lệnh. |
| **Outcome** — đo kết quả bằng gì? |Giảm thời gian xử lý lỗi, giảm số lần thử sai, tăng tỷ lệ khắc phục thành công và không gây lỗi mới. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? |Error log, traceback, phiên bản Python, OS, danh sách package, file requirements hoặc lockfile nếu có. Các dữ liệu nhạy cảm phải được loại bỏ trước khi đưa vào AI. |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? |Ghi nhận phương án AI đề xuất có đúng không, người dùng có chấp nhận không, số lần thử và trạng thái môi trường sau khi xử lý. |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**?
Augment - AI hỗ trợ lập trình viên.
AI được sử dụng để phân tích lỗi, giải thích nguyên nhân và đề xuất phương án. Lập trình viên vẫn là người kiểm tra, lựa chọn và thực hiện.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:
Trong phạm vi bài toán này, chẩn đoán sai và đề xuất một phương án sửa không an toàn có thể nguy hiểm hơn việc chưa xác định được nguyên nhân.

Ví dụ, AI nhận định sai nguyên nhân và đề xuất nâng cấp hàng loạt package có thể tạo thêm xung đột dependency. Ngược lại, nếu AI bỏ sót nguyên nhân, người dùng thường vẫn có thể quay về quy trình tra cứu thủ công.

Biện pháp kiểm soát:
- AI giải thích lý do của đề xuất và cảnh báo các thay đổi có rủi ro.
- Không tự thực thi lệnh sửa.
- Lập trình viên kiểm tra trước khi áp dụng.
- Khi thiếu dữ liệu, AI phải yêu cầu bổ sung hoặc chuyển về xử lý thủ công.
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
