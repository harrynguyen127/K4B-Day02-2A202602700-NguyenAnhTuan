# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên:
- Mã học viên:
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...):
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem):

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 | Lặp lại | Check email hàng ngày, đọc và phân loại email theo mức độ ưu tiên/loại việc (yêu cầu hỗ trợ, thông báo, spam...) | Bản thân (người trực) | ước tính 30 phút/lần, 2 lần/ngày để đọc + phân loại; 30 email/ngày cần xử lý |
| 2 | Lặp lại | Phân loại và theo dõi tiến độ các task đang làm (ai đang làm gì, task nào trễ) | Bản thân + các thành viên liên quan | phải cập nhật thủ công 3 lần/ngày |
| 3 | Tốn thời gian | Trả lời các câu hỏi lặp lại của người dùng trên nhóm chat (Viber/Lark) | Người dùng trong nhóm + bản thân | 5 câu hỏi/ngày, nhiều câu trùng lặp nội dung; mất 30 phút/câu để trả lời |
| 4 | Lặp lại | Hướng dẫn sử dụng các chương trình/phần mềm cho người dùng mới hoặc chưa quen | Người dùng mới, đồng nghiệp | 5 lượt hướng dẫn/tuần, mỗi lượt mất 60 phút; thường lặp lại cùng 1 nội dung hướng dẫn |
| 5 | Pain từ người khác | Xác định nguyên nhân lỗi do người dùng thao tác sai và hướng dẫn khắc phục | Người dùng gặp lỗi | 3-5 ticket/tuần liên quan lỗi thao tác; mất 30-60 phút để chẩn đoán + hướng dẫn mỗi lần |


> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi:
- Ý dùng được:
- Ý bỏ vì không phải pain thật:

**Self-check Phase 1:**
- [x] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [x] Dùng ít nhất 3/4 lăng kính
- [x] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Check email hàng ngày, đọc và phân loại email theo mức độ ưu tiên/loại việc (yêu cầu hỗ trợ, thông báo, spam...) | Việc lặp đi lặp lại mỗi ngày với khối lượng lớn (~30 email/ngày). Có quy tắc phân loại khá rõ ràng nên AI dễ học. tốn ~1 tiếng/ngày cộng dồn cả tuần | Tiêu chí phân loại "ưu tiên" có đủ rõ ràng để AI làm đúng không, hay còn phụ thuộc ngữ cảnh. Email nhạy cảm/quan trọng có nên để AI đọc trước không |
| 2 | Phân loại và theo dõi tiến độ các task đang làm (ai đang làm gì, task nào trễ) | Đang làm thủ công, dễ sót/trễ. ảnh hưởng cả nhóm chứ không riêng bản thân. có thể tự động hoá bằng cách đồng bộ từ nguồn task có sẵn (chat, ticket) | Dữ liệu tiến độ đang nằm rải rác ở đâu (chat, file, hệ thống nào) để AI lấy được. Ai là người xác nhận task đã xong hay chưa |
| 3 | Trả lời các câu hỏi lặp lại của người dùng trên nhóm chat (Viber/Lark) | Câu hỏi lặp lại nhiều, nội dung khá cố định nên phù hợp để AI trả lời tự động. tốn nhiều thời gian phản hồi (~30 phút/câu). giảm tải sẽ giúp tập trung việc khác | Có bao nhiêu % câu hỏi thực sự lặp lại/định sẵn được, và cần hiểu ngữ cảnh riêng. AI trả lời sai có thể gây hiểu lầm trong nhóm, cần cơ chế review thế nào |

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — Check & phân loại email hàng ngày

```text
Problem 1 câu:
Mỗi ngày mất ~1 tiếng đọc và phân loại thủ công ~30 email theo mức độ ưu tiên/loại việc.

Actor:
Bản thân (người trực email)

Thời điểm / bối cảnh:
Đầu giờ sáng và giữa buổi chiều, khi email dồn lại cần xử lý trước khi làm việc khác

Current workflow 3-7 bước:
1. Mở hộp thư, lướt qua tiêu đề tất cả email mới
2. Đọc nội dung từng email để hiểu yêu cầu
3. Xác định loại (yêu cầu hỗ trợ / thông báo / spam) và mức ưu tiên
4. Gắn nhãn / chuyển vào thư mục tương ứng
5. Xử lý hoặc chuyển tiếp cho người phù hợp

Bottleneck:
Bước 2-3 (đọc + đánh giá độ ưu tiên) chiếm phần lớn thời gian vì phải đọc kỹ từng email

Impact:
~30 phút/lần x 2 lần/ngày = ~1 tiếng/ngày, tương đương ~5 tiếng/tuần cho việc phân loại thủ công

Success metric:
Giảm thời gian phân loại xuống còn <20 phút/ngày; 100% email được gắn đúng loại/ưu tiên

Non-AI alternative:
Đặt rule lọc email theo từ khóa/người gửi trong hộp thư (filter có sẵn)

AI hypothesis:
AI đọc nội dung email, tự động gắn nhãn loại + mức ưu tiên, chỉ để lại email cần quyết định thủ công cho người dùng review

Quick gut:
[ ] No AI / process fix
[x] Rule
[ ] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #1** (ASCII / Mermaid / ảnh đính kèm):

```text
CURRENT STATE — 30'

[1 Lướt tiêu đề: 5'] → [2 Đọc nội dung: 15'] → [3 Đánh giá ưu tiên: 7'] → [4 Gắn nhãn/chuyển: 3']  <-- bottleneck

FUTURE STATE — 10'

[1 AI đọc & gợi ý nhãn: 2'] → [2 AI gắn nhãn tự động: 1'] → [3 User review email quan trọng: 7']  <-- human boundary

Fallback: nếu AI gắn sai nhãn thì user tự sửa lại nhãn, email không tự động gửi đi khi chưa review
```

File đính kèm (nếu vẽ riêng): `01-individual-problem-scan-workflow-card-1.png`

---

#### Problem Card #2 — Theo dõi tiến độ các task đang làm

```text
Problem 1 câu:
Phải cập nhật thủ công 3 lần/ngày để biết ai đang làm gì và task nào đang trễ, dễ sót thông tin.

Actor:
Bản thân (người tổng hợp) + các thành viên liên quan

Thời điểm / bối cảnh:
Rải rác trong ngày, mỗi khi cần biết trạng thái task để báo cáo hoặc nhắc việc

Current workflow 3-7 bước:
1. Vào từng nhóm chat / kênh để hỏi tiến độ từng người
2. Ghi chú lại thủ công vào file/sổ theo dõi
3. Đối chiếu với deadline đã đặt ra
4. Xác định task nào trễ / có nguy cơ trễ
5. Nhắc lại người phụ trách nếu cần

Bottleneck:
Bước 1-2 (hỏi từng người + ghi chú thủ công) tốn thời gian và dễ sót vì thông tin rải rác nhiều kênh

Impact:
Cập nhật thủ công 3 lần/ngày, từng bị sót/trễ do không có bảng theo dõi tự động cập nhật

Success metric:
Có 1 bảng trạng thái task cập nhật gần real-time, giảm số lần phải hỏi thủ công xuống 1 lần/ngày

Non-AI alternative:
Dùng công cụ quản lý task có sẵn (Trello/Notion) để mọi người tự cập nhật trạng thái

AI hypothesis:
AI tổng hợp tin nhắn cập nhật tiến độ từ các kênh chat, tự động điền vào bảng theo dõi và cảnh báo task có nguy cơ trễ

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #2:**

```text
CURRENT STATE — 45'/ngày (3 lần x 15')

[1 Hỏi từng người: 20'] → [2 Ghi chú thủ công: 15'] → [3 Đối chiếu deadline: 10']  <-- bottleneck

FUTURE STATE — 15'/ngày

[1 AI tổng hợp update từ chat: 5'] → [2 AI cập nhật bảng trạng thái: 3'] → [3 User review & nhắc task trễ: 7']  <-- human boundary

Fallback: nếu AI tổng hợp thiếu/sai thì user tự hỏi lại trực tiếp người phụ trách task đó
```

File đính kèm: `01-individual-problem-scan-workflow-card-2.png`

---

#### Problem Card #3 — Trả lời câu hỏi lặp lại trên nhóm chat

```text
Problem 1 câu:
Mỗi ngày mất nhiều thời gian trả lời ~5 câu hỏi trên nhóm chat, nhiều câu có nội dung trùng lặp.

Actor:
Người dùng trong nhóm (người hỏi) + bản thân (người trả lời)

Thời điểm / bối cảnh:
Trong giờ làm việc, khi người dùng cần hỗ trợ nhanh qua Viber/Lark

Current workflow 3-7 bước:
1. Người dùng gửi câu hỏi lên nhóm chat
2. Bản thân đọc và xác định câu hỏi thuộc loại gì
3. Tìm lại thông tin/hướng dẫn liên quan (nếu đã từng trả lời trước đó)
4. Soạn câu trả lời phù hợp với tình huống cụ thể
5. Gửi trả lời và theo dõi xem người hỏi đã rõ chưa

Bottleneck:
Bước 3-4 (tìm lại thông tin cũ + soạn lại câu trả lời từ đầu dù câu hỏi tương tự đã trả lời trước đó)

Impact:
~5 câu hỏi/ngày x 30 phút/câu = ~2.5 tiếng/ngày dành cho trả lời chat

Success metric:
Giảm thời gian trả lời trung bình xuống <10 phút/câu cho câu hỏi lặp lại; chỉ còn xử lý thủ công câu hỏi mới/phức tạp

Non-AI alternative:
Tạo file FAQ / tài liệu hướng dẫn có sẵn để gửi link khi có câu hỏi trùng

AI hypothesis:
AI dựa trên lịch sử câu hỏi/trả lời để tự động trả lời các câu hỏi lặp lại, chỉ đẩy lên cho bản thân xử lý khi câu hỏi mới hoặc AI không chắc chắn

Quick gut:
[ ] No AI / process fix
[ ] Rule
[ ] Workflow
[x] Agent
[ ] Chưa biết
```

**Draft workflow Card #3:**

```text
CURRENT STATE — 30'/câu

[1 Đọc câu hỏi: 3'] → [2 Xác định loại: 5'] → [3 Tìm lại info cũ: 12'] → [4 Soạn & gửi trả lời: 10']  <-- bottleneck

FUTURE STATE — 8'/câu

[1 AI phát hiện câu hỏi trùng & soạn trả lời: 2'] → [2 User review nhanh: 3'] → [3 Gửi trả lời: 3']  <-- human boundary

Fallback: nếu AI không chắc chắn hoặc câu hỏi mới thì tự động chuyển cho bản thân trả lời trực tiếp
```

File đính kèm: `01-individual-problem-scan-workflow-card-3.png`

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

```text
Card #3 — Trả lời câu hỏi lặp lại của người dùng trên nhóm chat (Viber/Lark)
```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text
Workflow hiện tại: đọc câu hỏi → xác định loại → tìm lại thông tin cũ → soạn & gửi trả lời, mất ~30 phút/câu và lặp lại ~5 câu/ngày (~2.5 tiếng/ngày).
Future state rút xuống ~8 phút/câu nhờ AI phát hiện câu hỏi trùng và soạn sẵn câu trả lời, người dùng chỉ review nhanh trước khi gửi.
Impact: tiết kiệm được phần lớn thời gian phản hồi hàng ngày, giúp tập trung xử lý các câu hỏi mới/phức tạp hơn thay vì lặp lại câu trả lời cũ.
```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text
1. Với đặc điểm câu hỏi lặp lại có pattern rõ, liệu một rule-based FAQ đơn giản có giải quyết được phần lớn vấn đề mà không cần đến Agent không?
2. Nếu AI trả lời sai/hiểu nhầm ngữ cảnh trong nhóm chat, cơ chế review hiện tại đã đủ để tránh gây hiểu lầm hay chưa?
```

**AI phản biện Card (nếu có):**
- Điểm yếu AI chỉ ra:
- Tôi sửa gì:

### Self-check nộp phần 01
- [x] Có 5+ problems + top 3 Cards đủ field
- [x] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [x] Đã chọn 1 card pitch + câu hỏi challenge
