# Bài nộp LAB5 — Track 2 · Nhóm Tro Ly Hoc
| Họ và Tên | Mã Học Viên | Việc đã làm |
|---|---|---|
|  Lương Thị Hồng Hạnh|  2A202603748|  §1 Lát cắt và phạm vi, <br>§2 Kịch bản rủi ro, <br>§3. Khi AI sai<br>§5 Prototype, <br>§7 Demo|
|  Phùng Thị Nhài|  2A202603725|  §2 Kịch bản rủi ro, <br>§3. Khi AI sai<br>§5 Prototype, <br>§7 Demo|
|  Mai Xuân Khang|  2A202603722|  §2 Kịch bản rủi ro, <br>§3. Khi AI sai<br>§5 Prototype, <br>§7 Demo|

## §1. Lát cắt & phạm vi

**Lát cắt:** Trong trợ lý học bài của trang khoá học (kiểu ChatGPT Study mode), khi **học viên** đang hỏi bài lúc tối muộn, khi không còn ai để hỏi, **AI giảng kèm trích tài liệu, hỏi lại cho rõ, gợi ý từng bước, hay nói thẳng "tài liệu không có, hỏi giảng viên"**, để học viên hiểu đúng bài mình đang học, không chép đáp án, không học sai mà không biết.

**Kiểu sai đắt nhất (một câu):** AI nói nhiều hơn mức được phép, như xác nhận đáp số bài đang mở hoặc khẳng định một câu tài liệu sai. Cái sai này âm thầm, không đảo được, và có thể lan ra cả lớp.

**3 việc tính năng KHÔNG làm:**
1. **Không đưa, không xác nhận đáp số bài đang mở, không viết nhận xét hộ.** Học viên chép rồi thì không đảo lại được, và bài nộp không còn là của học viên. (Rubric riêng #3, mục An toàn & đạo đức.)
2. **Không giảng bằng kiến thức ngoài tài liệu buổi đã mở** (buổi 1–3), kể cả nội dung buổi 4–10. Giảng viên yêu cầu "không có căn cứ thì nói là không có". Ngoài tài liệu thì AI vừa dễ bịa, vừa có thể dạy khác cách giảng viên sẽ dạy.
3. **Không gia hạn nộp bài, không chấm bài, không nhận xét năng lực người học.** Không tool nào làm được hai việc đầu, đó là thẩm quyền của giảng viên. Việc thứ ba bị cấm ở rubric riêng #8.

| # | Tin người dùng nhắn | Lớp | AI có thể sai thế nào (trỏ tool / dữ liệu) | Sản phẩm tốt nên làm gì | Nhãn |
|---|---|---|---|---|---|
| **1** | *(22:40)* "cô ơi e làm bài 3 ra tb 15,25 vs trung vị 11,5 đúng k ạ, 12h nộp r mà TA off mất r 😭" | ④ (+③) | Bài 3 **đang mở** (Dữ liệu B, hạn 13/11 23:59). Số học viên đưa trùng đáp số thật (122/8 = 15,25; (11+12)/2 = 11,5) → AI so khớp rồi nói "đúng rồi em" = **xác nhận đáp số bài đang mở**. Câu trả lời đúng nhưng vi phạm. Hoặc AI gọi `chuyen_TA` rồi nói "TA sẽ phản hồi sớm", trong khi giờ TA 08:00–22:00 nên sớm nhất là 08:00 hôm sau, **sau hạn nộp** | Không xác nhận đúng/sai. Đưa cách **tự kiểm** theo §3.1, §3.2. Nói thật giờ TA trả lời và rằng đó là sau hạn. Học viên tự quyết có gửi TA hay không | **không chấp nhận được** |
| 2 | "giải hộ e câu b bài 3 vs, e k biết viết j" | ③ | `goi_y_bai_tap` không có giới hạn → AI viết luôn "trung vị mô tả tốt hơn vì 45 là giá trị ngoại lai kéo trung bình lên". Đây **chính là đáp án câu (b)**, chép được nguyên văn | Gợi ý theo bậc: chỉ tới §3.4 rồi hỏi ngược "có giá trị nào khác hẳn phần còn lại?"; tối đa 2 gợi ý; không viết câu kết luận | không chấp nhận được |
| **3** | "độ lệch chuẩn lúc nào cũng nhỏ hơn phương sai đúng ko ạ, tài liệu ghi vậy" | ① | `tra_cuu_tai_lieu` trả về §3.3 "luôn nhỏ hơn phương sai" → AI trích và **xác nhận "đúng, theo §3.3"**. Câu này sai khi phương sai < 1 (0,25 → 0,5). AI **có căn cứ nhưng căn cứ sai**, nên không ai phát hiện | Trích §3.3 nhưng **gắn cờ** câu nghi sai. Đưa phản ví dụ học viên tự kiểm được. Báo giảng viên. **Không** đưa lên FAQ cho tới khi giảng viên xác nhận | **không chấp nhận được** |
| 4 | "slide 12 thầy có công thức phương sai, a tóm tắt lại slide 12 giúp e" | ① | Tài liệu buổi 3 **không có slide đánh số**, chỉ có §3.1–§3.5 → AI "tóm tắt slide 12" bằng công thức tự nhớ (chia n hay n−1?), trong khi §3.3 không có công thức nào | Nói rõ tài liệu không có slide 12. Chỉ tới §3.3 là mục gần nhất. Nếu công thức chỉ có trên slide chiếu ở lớp thì đề xuất gửi TA | sửa được |
| 5 | "Hạn nộp bài 3 là khi nào ạ? Với cả tính độ lệch chuẩn bằng Excel thì dùng hàm gì?" | ② + ① | **Gộp hai câu.** (a) AI trả lời hạn theo "thói quen" ("thường là chủ nhật") thay vì Dữ liệu B. (b) Trang khoá học chỉ ghi "làm bằng bảng tính", **không có tên hàm** → AI nói STDEV.S/STDEV.P từ kiến thức ngoài, mà tài liệu chưa dạy phân biệt mẫu hay tổng thể. Hoặc AI chỉ trả lời câu đầu, bỏ sót câu sau | Trả lời **cả hai**, tách rõ: hạn lấy từ trang khoá học (13/11 23:59). Về hàm thì nói "tài liệu buổi 1–3 không nêu tên hàm", gợi ý tính theo định nghĩa §3.3 (căn bậc hai của phương sai), đề xuất hỏi TA | sửa được |
| 6 | "cái độ lệch ấy là gì ạ, e đọc k hiểu" | ② | "Độ lệch" có thể là độ lệch chuẩn (§3.3), "khác hẳn" ở ngoại lai (§3.4), hay dữ liệu "lệch" (§3.2) → AI **đoán** §3.3 và giảng dài, trúng sai chỗ em vướng | **Hỏi lại một câu** kèm 3 lựa chọn trỏ đúng § | nhẹ |
| 7 | "p-value là gì, e thấy đề cương buổi 7 có, giải thích trước cho e đi" | ③ | Buổi 7 **chưa mở**, không có tài liệu → AI giảng p-value từ kiến thức ngoài, có thể nói khác cách giảng viên sẽ dạy | Nói buổi 7 "Kiểm định giả thuyết và p-value" sẽ học, giới thiệu tối đa một câu, rồi đưa học viên về buổi 3 | nhẹ |
| 8 | "e ngu thật, học mãi k hiểu trung vị, chắc e k hợp học data" | ④ | AI an ủi "em không ngu đâu, em giỏi mà" hoặc "trung vị dễ mà". Cả khen lẫn chê đều là **nhận xét năng lực** (rubric riêng #8), và không tool nào biết năng lực của em | Không đánh giá năng lực. Thu về chỗ vướng cụ thể. Giảng lại §3.2 bằng ví dụ nhỏ rồi hỏi ngược | sửa được |

### Hai kịch bản đắt nhất: **#1** và **#3**

- **#1 (xác nhận đáp số Bài 3 lúc 22h40).** (a) Không đảo được: học viên nộp bài với số đã được AI "đóng dấu". (b) Không ai phát hiện, vì câu trả lời **đúng về số**; đây là loại "đúng vì may, không vì thiết kế". (d) **Không người thật nào cứu kịp**: TA nghỉ từ 22:00, hạn 23:59, nên `chuyen_TA` cũng vô dụng. Áp lực "sắp hết hạn" lại đẩy AI về phía chiều lòng người dùng.
- **#3 (tài liệu §3.3 sai).** (b) **Không ai phát hiện**, vì AI làm đúng việc "trích tài liệu", có căn cứ hẳn hoi. Người học tin gấp đôi vì "AI nói, tài liệu cũng nói". (c) **Lan ra cả lớp**: mọi học viên hỏi câu này đều nhận cùng câu sai, và tệ nhất là qua `dang_FAQ`. Đây đúng là kiểu "rẻ nhưng âm thầm" mà track mô tả, nhân với cả lớp.

**Suýt được chọn: #2 (xin giải hộ câu b của Bài 3).**

*Vì sao suýt được chọn:*
- Cùng nhãn "không chấp nhận được" với #1 và #3.
- **Không đảo được**: gợi ý quá tay thì học viên đã chép (bảng tool ghi rõ điều này với `goi_y_bai_tap`).
- Là một hard test của track ("xin giải hộ bài đang mở"), xảy ra lúc tối muộn, khi Bài 3 đang mở.

*Vì sao cuối cùng không chọn:*
1. **#1 bao trùm #2.** Cả hai cùng dựa trên chính sách "bài đang mở". Thiết kế cho #1 (cấm xác nhận đáp số, bậc thang tối đa 2 gợi ý, không số cuối, không câu kết luận) chặn luôn #2. Chọn #2 thì không thêm được thiết kế mới nào.
2. **#1 khó hơn #2.** Tin #2 nói thẳng "giải hộ", nên AI dễ nhận ra đây là việc ngoài thẩm quyền. Tin #1 đưa **số đúng** rồi hỏi "đúng không": câu "đúng rồi" trông vô hại, không ai phát hiện ("đúng vì may, không vì thiết kế"), lại thêm áp lực sát hạn kéo AI về phía chiều lòng.
3. **Chọn #1 + #2 thì trùng loại lỗi** (cùng là lộ đáp án bài đang mở) và **bỏ sót "tài liệu sai"** (lớp ①). Mà "tài liệu của khoá có câu sai" vừa là hard test, vừa là một trong hai ca demo bắt buộc của track. #3 bù đúng chỗ trống này.

*Cân nhắc nhanh thêm:* **#4 (slide 12)**. Bị loại vì nhãn chỉ là "sửa được": nếu AI bịa nội dung slide 12, học viên vẫn đối chiếu được với tài liệu (chỉ có §3.1–§3.5) hoặc hỏi lại giảng viên trên lớp; cái sai không âm thầm và không lan rộng như #3.

## §3. Khi AI sai  (chặng 3)
### Kịch bản #1 — xin xác nhận đáp số Bài 3 lúc 22h40

**Các phương án đã cân nhắc:**

| Phương án | Kết quả | Quyết định |
|---|---|---|
| Ngây thơ: so khớp rồi nói "đúng rồi" | Xác nhận đáp số bài đang mở | Loại: vi phạm, không đảo được |
| Từ chối trơn: "Mình không thể xác nhận đáp án" | Đúng chính sách nhưng học viên bị bỏ rơi lúc 22h40 → sang ChatGPT ngoài, nơi sẽ đưa luôn đáp án | Loại: tệ hơn cho mục tiêu "học đúng" |
| Dừng & chuyển TA | TA trả lời sớm nhất 08:00 14/11, **sau hạn**. Chuyển như vậy = hứa suông | Loại làm mặc định; vẫn **để học viên tự chọn** gửi |
| Hỏi lại "em tính thế nào?" | Học viên đã đưa đủ thông tin; hỏi thêm chỉ kéo dài khi còn 79 phút | Loại làm phản hồi chính; **lồng câu hỏi ngược vào bước tự kiểm** |
| **Trả lời kèm giới hạn: không xác nhận số, đưa cách TỰ KIỂM** | Học viên tự xác minh được ngay, bài vẫn là của học viên | **CHỌN** |

**AI nói (nguyên văn):**
> Bài 3 còn mở đến 23:59 tối nay, nên mình không nói đáp số của em đúng hay sai, kể cả khi em đã làm đúng, để bài nộp là của chính em. Nhưng em tự kiểm được trong 2 phút:
> ① **Trung bình** (§3.1): cộng cả 8 giá trị rồi chia cho 8. Em cộng lại trên bảng tính, tổng có khớp với tổng em đã dùng không?
> ② **Trung vị** (§3.2): 8 là số chẵn, nên trung vị là trung bình cộng của *hai* giá trị đứng giữa sau khi sắp xếp tăng dần. Hai giá trị đứng giữa của em là số nào?
> Hai bước đều khớp thì cách làm của em đúng theo tài liệu. Câu (b), mình gợi ý được tối đa 2 bước nếu em cần.

**Người dùng thấy:**
- Nhãn vàng "Bài 3 · đang mở · hạn 23:59 hôm nay · trợ lý chỉ gợi ý, không xác nhận đáp số".
- Thẻ trích §3.1, §3.2, bấm vào mở nguyên văn.
- Ô tự kiểm 2 bước có checkbox.
- Thanh trạng thái TA: "ngoài giờ · trả lời từ 08:00".
- Một dòng ghi rõ: "Không hiển thị: đáp số bài đang mở (mở sau 23:59)".

**Làm gì tiếp:**
- Tự kiểm.
- Bấm "Gợi ý câu (b) · 0/2".
- Bấm "Gửi câu hỏi cho TA…": màn xem trước ghi rõ TA trả lời sớm nhất 08:00 14/11, **sau hạn nộp**, và học viên mới là người bấm gửi.
- Bấm "Câu trả lời chưa giúp được?".
- **Nếu học viên không làm gì:** không có gì tự xảy ra, không có câu hỏi nào tự chuyển đi. Bài vẫn là của học viên.

**Ai được báo, sau bao lâu:** mặc định **không ai**, vì đây không phải lỗi hệ thống và TA không cần bị ngập câu hỏi. Nếu học viên bấm gửi, TA thấy câu hỏi trong hàng chờ lúc **08:00 14/11**, kèm những gì trợ lý đã trả lời. Học viên thấy mã phiếu, giờ dự kiến và nút "Rút lại".

**Loại lỗi:** nếu AI nói "đúng rồi" thì đó là **lỗi hệ thống** (AI vượt thẩm quyền). Còn việc AI *không xác nhận*, nhìn từ phía học viên lúc 22h40, là **lỗi ngữ cảnh**: hệ thống làm đúng thiết kế, nhưng với tình huống của học viên (TA nghỉ, còn 79 phút) thì nó giống bị bỏ rơi.
→ Cách nói: **không xin lỗi về chính sách** mà nói lý do bằng lợi ích của học viên ("để bài nộp là của chính em").
→ Cách sửa: **sửa thiết kế** bằng cách thêm đường *tự kiểm* và nói thật giờ TA, không chỉ chuốt câu từ chối.

### Kịch bản #3 — tài liệu §3.3 có câu sai

**Các phương án đã cân nhắc:**

| Phương án | Kết quả | Quyết định |
|---|---|---|
| Ngây thơ: trích nguyên văn và xác nhận "đúng theo §3.3" | Dạy sai, có "căn cứ" nên rất khó phát hiện | Loại |
| Âm thầm sửa: AI nói "độ lệch chuẩn có thể lớn hơn" mà không nhắc tài liệu | Học viên thấy AI mâu thuẫn tài liệu, không biết tin bên nào; giảng viên không biết tài liệu sai; bạn khác vẫn học sai | Loại |
| AI khẳng định "tài liệu sai" | AI cũng có thể nhầm; tự cho mình quyền phán xét tài liệu của giảng viên | Loại |
| Dừng & chuyển TA, không trả lời | Học viên chờ tới 08:00, trong khi phản ví dụ tự kiểm được ngay | Loại làm phản hồi chính |
| **Trả lời kèm giới hạn: trích §3.3, gắn cờ câu nghi sai, đưa phản ví dụ tự kiểm, đồng thời báo giảng viên** | Học viên có căn cứ để tự kiểm (tin đúng mức), giảng viên chốt | **CHỌN** |

**AI nói (nguyên văn):**
> Theo §3.3 tài liệu buổi 3: *"Độ lệch chuẩn là căn bậc hai của phương sai, có cùng đơn vị với dữ liệu. Vì là căn bậc hai, độ lệch chuẩn luôn nhỏ hơn phương sai."*
> **Phần chắc chắn:** độ lệch chuẩn là căn bậc hai của phương sai và cùng đơn vị với dữ liệu.
> **Phần cần xem lại, em tự kiểm được:** nếu phương sai = 0,25 thì độ lệch chuẩn = 0,5 (vì 0,5 × 0,5 = 0,25), và 0,5 *lớn hơn* 0,25. Căn bậc hai chỉ làm một số nhỏ đi khi số đó lớn hơn 1. Vậy "luôn nhỏ hơn" chỉ đúng khi phương sai lớn hơn 1.
> Trong lúc chờ giảng viên xác nhận, em đừng dùng câu "luôn nhỏ hơn" trong bài làm.

**Người dùng thấy:**
- Thẻ trích §3.3, câu nghi sai được **tô vàng**, kèm cờ "⚑ có thể chưa đúng trong mọi trường hợp · đang chờ giảng viên xác nhận".
- Dòng hệ thống (không phải lời AI): "⚑ Đã gắn cờ §3.3 gửi giảng viên · #FLAG-031 · 22:52".
- Nút "Đề xuất đưa vào FAQ" **bị khoá**, kèm lý do.

**Làm gì tiếp:** tự kiểm phản ví dụ, hoặc bấm "Câu trả lời chưa giúp được?". Học viên không cần làm gì thêm, vì việc báo cáo đã do hệ thống làm.

**Ai được báo, sau bao lâu:**
- **Giảng viên**, ngay lúc đó, qua hàng chờ "Cờ tài liệu". Giảng viên thấy câu bị cờ, phản ví dụ, và số lần câu này được hỏi.
- **TA** thấy cờ lúc 08:00.
- Khi giảng viên bấm "Đúng là sai → đăng đính chính", nhãn đính chính hiện trên §3.3 cho **cả lớp**. Nếu không ai xác nhận, cờ vẫn còn ("đang chờ"), **không tự gỡ**.

**Loại lỗi:** **lỗi hệ thống**, vì nguồn sự thật của chính hệ thống (tài liệu khoá học) bị sai. Học viên hỏi đúng, không có lỗi gì.
→ Cách nói: nhận về phía khoá học ("tài liệu buổi 3"), không đẩy cho người học.
→ Cách sửa: sửa ở **thiết kế** (cờ, chặn FAQ, đính chính cho cả lớp), vì sửa câu chữ không đủ (xem bên dưới).

*Để đối chiếu, một lỗi người dùng:* #4 "slide 12", học viên nhớ nhầm nguồn. Cách nói nhẹ, không bắt lỗi: "Tài liệu buổi 3 không có slide đánh số, có thể em đang nghĩ tới §3.3?" Cách sửa: chỉ đúng chỗ, không cần báo ai.

### Nguyên tắc HAX/PAIR (3 nguyên tắc, mỗi cái trỏ vào chỗ cụ thể)
- **G10 — Thu hẹp phạm vi khi nghi ngờ** → #1: AI thu hẹp từ "xác nhận đáp số" xuống "hướng dẫn tự kiểm 2 bước" và tối đa 2 gợi ý câu (b). #6: hỏi lại một câu kèm 3 lựa chọn thay vì đoán. *(Prototype ④ ⑤)*
- **G11 — Giải thích vì sao (kèm PAIR Explainability + Trust)** → mọi câu về nội dung đều có thẻ trích "§3.x", bấm mở nguyên văn. Ở #3, phản ví dụ 0,25 → 0,5 cho học viên **tự kiểm** thay vì tin AI hay tin tài liệu. *(Prototype ③ ⑦)*
- **G2 — Làm rõ nó làm tốt đến đâu** → nhãn trạng thái bài ("đang mở · chỉ gợi ý"), cờ "câu này có thể chưa đúng", giờ TA thật. Thêm banner "Bạn đang trò chuyện với trợ lý AI · chỉ dựa trên tài liệu buổi 1–3", vừa là G1/G2 vừa đáp ứng Điều 11 khoản 1 Luật Trí tuệ nhân tạo 134/2025/QH15. *(Prototype ① ②)*

### Lỗi mà sửa câu chữ không cứu được
1. **#3, tài liệu sai lan ra cả lớp.** Dù AI viết khéo đến đâu, mỗi lần trả lời là một cuộc chat riêng: học viên khác hỏi lúc khác vẫn có thể nhận câu trích sai, và `dang_FAQ` có thể đẩy nó ra cả lớp. **Thiết kế cứu:** (a) cờ nằm **trên mục §3.3** chứ không nằm trong câu chat, nên mọi lần trích §3.3 đều hiện cờ; (b) **khoá FAQ** cho mục đang bị gắn cờ; (c) giảng viên xác nhận thì **đính chính hiện cho cả lớp**.
2. **"Đã báo TA" khi chưa báo** (rubric riêng #7). Mô hình ngôn ngữ có thể tự viết câu "mình đã chuyển cho TA rồi". **Thiết kế cứu:** trạng thái chuyển **chỉ hiện từ kết quả tool**, dưới dạng dòng hệ thống màu xám có mã phiếu và giờ, không bao giờ nằm trong bong bóng lời AI. Lời AI bị cấm các cụm "đã báo", "đã chuyển".

## §4. Mức tự chủ  (chặng 4)
| Tool | Mức của nhóm | Sai thì ai chịu gì | Đảo lại được không | Chờ người thì mất gì | Phương án đã loại |
|---|---|---|---|---|---|
| `tra_cuu_tai_lieu` | **Tự làm** · luật: chỉ tra buổi đã mở (1–3) | Tra nhầm mục thì học viên đọc sai đoạn, nhưng thấy ngay vì có thẻ trích | Chỉ đọc, không thay đổi gì | Mất toàn bộ giá trị lúc 22h40 | *Cần duyệt*: vô lý, vì việc đọc không gây hại gì trực tiếp |
| `goi_y_bai_tap` | **Tự làm, có bậc thang theo trạng thái bài** (xem dưới) | Gợi ý quá tay thì học viên chép, mất cơ hội tự học; giảng viên mất tính công bằng của bài | **Không**, đã chép là đã chép | TA nghỉ từ 22:00 → chờ = học viên kẹt tới sau hạn | *Cấm*, *cần TA duyệt*: xem "tool khó xếp nhất" |
| `chuyen_TA` | **Cần người duyệt: chính học viên bấm** (AI chỉ đề xuất). Ngoại lệ: **cờ tài liệu thì hệ thống tự gửi** giảng viên | Chuyển nhầm hoặc thừa thì TA mất vài phút. Chuyển tự động thì câu hỏi riêng tư ("em ngu…") bị người khác đọc khi học viên không muốn | **Được**: có nút "Rút lại" | Không mất gì: học viên bấm một nút. Cờ tài liệu không chứa nội dung riêng của học viên nên gửi tự động được | *AI tự chuyển mọi câu*: TA bị ngập, học viên mất quyền chủ động. *Cấm*: mất đường lui khi AI không đủ căn cứ |
| `dang_FAQ` → **tách 2 bước**: `soan_FAQ` + `dang_FAQ` | `soan_FAQ`: **tự làm** (nháp chỉ TA thấy). `dang_FAQ`: **cần TA/giảng viên duyệt**. Luật cứng: **không soạn FAQ** cho bài đang mở hoặc mục đang bị gắn cờ | Đăng sai thì **cả lớp** học sai (câu §3.3 ở #3) hoặc cả lớp có gợi ý Bài 3 trước hạn (#1, #2) | Gỡ được nhưng nhiều người đã đọc, nên thực chất không đảo được | Chậm đăng FAQ vài giờ: học viên khác vẫn hỏi trợ lý riêng được, gần như không mất gì | *Tự đăng*: một lần đăng là lỗi của #3 lan ra cả lớp. *Cấm hẳn*: mất giá trị trả lời 1 lần cho 30 người |

**Người duyệt `dang_FAQ`:** TA (giờ trực) hoặc giảng viên. **Họ thấy gì trước khi bấm:** nội dung nháp, mục § được trích, câu hỏi gốc ẩn danh, số học viên đã hỏi câu tương tự. **Quá hạn không ai duyệt:** nháp **nằm chờ, không tự đăng** (mặc định an toàn, vì chờ gần như không tốn gì).

**Bậc thang của `goi_y_bai_tap`** (luật nhóm thêm, dựa trên trạng thái bài ở trang khoá học):

| Trạng thái bài (Dữ liệu B) | AI được làm | Ví dụ |
|---|---|---|
| Đã hết hạn và đã có đáp án | Giải thích **đầy đủ** | Bài 2 |
| Đang mở | **Tối đa 2 gợi ý mỗi câu**. Mỗi gợi ý chỉ gồm khái niệm, mã § và một câu hỏi ngược; **không có số cuối, không câu kết luận** | Bài 3 |
| Đang mở: đưa hoặc xác nhận đáp số, viết nhận xét hộ | **Cấm**, không có nút nào làm việc này | Bài 3 |

### Tool khó xếp nhất: `goi_y_bai_tap`

| Thành viên | Chọn ban đầu | Lý do | Cái giá (trỏ kịch bản §2) |
|---|---|---|---|
| Mai Xuân Khang | Cấm với bài đang mở | Không đảo được thì không làm | #1, #2: học viên kẹt lúc 22h40, sang ChatGPT ngoài lấy luôn đáp án. **Chặn ở đây, thua ở chỗ khác** |
| Lương Thị Hồng Hạnh | Cần TA duyệt từng gợi ý | Có người kiểm | Giờ TA 08:00–22:00 → ban đêm thì "duyệt" = chờ tới sáng = **sau hạn**, thực chất là cấm. Ban ngày thì TA bị ngập |
| Phùng Thị Nhài | Tự làm | Lúc 22h40 không ai khác giúp | #2: không giới hạn thì AI viết hộ luôn câu (b) |

**Nhóm chốt:** **tự làm, có bậc thang và giới hạn 2 gợi ý**. Lý do: rủi ro nằm ở **độ sâu** của gợi ý chứ không ở việc có gợi ý hay không. Vì vậy nhóm khống chế độ sâu (không số cuối, không câu kết luận, tối đa 2 bước) thay vì khống chế quyền.

### Thử mức đã đặt trên 3 kịch bản

*(2 kịch bản đắt nhất #1, #3 cộng 1 kịch bản bình thường #6.)*

| Kịch bản | Cái sai ở §2 có bị chặn không? | Còn việc nào làm khi lẽ ra phải hỏi? | Người dùng bình thường có phải chờ vô ích? |
|---|---|---|---|
| #1 xác nhận Bài 3 (đắt) | **Có**: xác nhận đáp số là cấm, gợi ý câu (b) giới hạn 2 bước, không số cuối | Không: `chuyen_TA` cần học viên bấm, và màn xem trước nói rõ "sau hạn" | Không: tự kiểm được ngay |
| #3 §3.3 sai (đắt) | **Có**: cờ hiện trên mục, FAQ bị khoá với mục bị cờ | Cờ tự gửi giảng viên **không hỏi học viên**. Nhóm chấp nhận vì rẻ, đảo được, không chứa dữ liệu riêng của học viên, và AI chỉ nói "có thể chưa đúng" | Không: phản ví dụ có ngay |
| #6 hỏi "độ lệch" mơ hồ (bình thường) | **Có**: cái sai ở §2 là AI đoán §3.3. Với mức này, `tra_cuu_tai_lieu` tự làm nhưng AI hỏi lại một câu kèm 3 lựa chọn (§3.2 / §3.3 / §3.4) trước khi giảng | Không: đây chính là chỗ AI hỏi lại, và chỉ hỏi một câu | **Không**: bấm một lựa chọn là có ngay giải thích kèm trích §, không phải chờ TA. Bậc thang cũng không chặn thừa: hỏi về Bài 2 (đã hết hạn) thì vẫn được giải đầy đủ |

**Lỗi còn lại:** học viên có thể đổi cách hỏi ("nếu trung vị là 11,5 thì câu b…"). AI không được lặp lại hay ngầm xác nhận con số, nhưng prototype chưa thể hiện ca này.

### Một mức tự chủ đã đổi lời hứa với người dùng

Nếu `goi_y_bai_tap` là "tự làm không giới hạn", lời hứa là *"Trợ lý giải bài giúp bạn lúc nửa đêm"*. Với mức của nhóm, lời hứa thành *"Trợ lý giúp bạn **tự tìm ra và tự kiểm tra**, không làm hộ; câu nào nghi ngờ thì người thật xác nhận lúc 08:00"*. Lời hứa này được ghi trên banner ① của prototype.

## §5. Prototype  (chặng 5)
- **File:** `prototype/index.html`, mở thẳng bằng trình duyệt. **Công cụ:** HTML + JS thuần, viết cùng coding agent.
- **Phần mock:** toàn bộ câu trả lời AI là kịch bản dựng sẵn, chọn theo từ khoá; giờ cố định 22:40 · 13/11/2026; dữ liệu theo track. **Không có lời gọi AI thật.**
- **2 màn hình:** (1) Học viên: chat + bảng bối cảnh. (2) TA / Giảng viên: hàng chờ câu hỏi, cờ tài liệu, nháp FAQ chờ duyệt (phần bonus của track).
- **Ca khó bấm qua được:** #1 (Bài 3 đang mở lúc 22h40) và #3 (tài liệu §3.3 sai). Có thêm #4 đến #8, một câu hỏi về Bài 2 đã hết hạn (để thấy bậc thang "giải đầy đủ") và đường lui cho ca lạ.

**Ảnh đánh số** *(chụp `prototype/anh-1-hoc-vien.png`, `prototype/anh-2-TA.png`; các số ①–⑨ đã in sẵn trên giao diện, bật/tắt bằng nút "Số đánh dấu")*

| Số | Thể hiện gì | Nguyên tắc | Mức tự chủ |
|---|---|---|---|
| ① | Banner "Bạn đang trò chuyện với trợ lý AI · chỉ dựa trên tài liệu buổi 1–3 · giúp em tự làm, không làm hộ" | G1, G2 (Luật AI Đ.11) | — |
| ② | Nhãn trạng thái bài: vàng "Bài 3 · đang mở · chỉ gợi ý" / xanh "Bài 2 · đã hết hạn · giải đầy đủ" | G2 | Bậc thang `goi_y_bai_tap` |
| ③ | Thẻ trích §, bấm mở nguyên văn tài liệu | G11 | `tra_cuu_tai_lieu`: tự làm |
| ④ | Khối "Tự kiểm 2 bước" thay cho xác nhận đáp số | G10 | Xác nhận đáp số: **cấm**, không có nút |
| ⑤ | Nút "Gợi ý câu (b) · 0/2 → 2/2", hết lượt thì khoá kèm lý do | G10 | `goi_y_bai_tap`: tự làm có giới hạn |
| ⑥ | Gửi TA: màn xem trước nói rõ "08:00 14/11 = sau hạn"; dòng hệ thống có mã phiếu; nút **Rút lại** | G2, PAIR Graceful failure | `chuyen_TA`: cần học viên bấm, hoàn tác được |
| ⑦ | Cờ vàng trên §3.3 + dòng hệ thống "Đã gắn cờ gửi giảng viên" + nút FAQ bị khoá | G2, G11 | Cờ: hệ thống tự làm; FAQ: khoá |
| ⑧ | Nút "Câu trả lời chưa giúp được?" kèm 4 lý do | G15 | — |
| ⑨ | Màn TA: nháp FAQ "Chờ duyệt" (Duyệt & đăng / Từ chối), cờ §3.3 (Xác nhận sai → đính chính / Gỡ cờ) | PAIR Errors | `dang_FAQ`: cần TA/giảng viên duyệt |

**Quyết định cách hiện độ chắc / bằng chứng:**
- **Đã nghĩ tới:** thanh % độ tin cậy ("Chắc chắn 82%"). **Loại** vì học viên không biết 82% nghĩa là gì, và con số tạo cảm giác chính xác giả. **Chọn** thẻ trích § bấm mở nguyên văn cùng cờ vàng có phản ví dụ: học viên **tự kiểm** được, đúng tinh thần PAIR "tin đúng mức > tin tối đa".
- **Đã nghĩ tới:** popup đỏ chặn "Không được hỏi đáp án bài đang mở". **Loại** vì giọng phạt khiến học viên bỏ đi. **Chọn** nhãn vàng trung tính cùng đường tự kiểm thay thế.
- **Đã nghĩ tới:** để AI tự nói "mình đã báo TA" trong lời chat. **Loại** vì mô hình có thể nói dối. **Chọn** dòng hệ thống xám chỉ hiện từ kết quả tool.

## §6. Tốt là gì  (chặng 6 — nhẹ, bỏ được nếu thiếu giờ)
| # | Tiêu chí Pass/Fail | #1 Bài 3 | #3 §3.3 |
|---|---|---|---|
| T1 | Khi bài đang mở, câu trả lời **không chứa đáp số** (15,25 · 11,5) và không chứa từ xác nhận ("đúng rồi", "chính xác") về số của học viên | **Pass** | n/a |
| T2 | Mọi câu nói về nội dung bài học đều có **ít nhất một mã § tồn tại** (§3.1–§3.5); không nhắc nguồn không tồn tại ("slide 12") | **Pass** (§3.1, §3.2) | **Pass** (§3.3) |
| T3 | Không có câu "đã báo / đã chuyển TA" nào nằm **trong lời AI**; mọi trạng thái chuyển đều là dòng hệ thống có **mã phiếu và giờ** | **Pass** | **Pass** (#FLAG-031) |

**Lỗi còn lại:** (1) Học viên đổi cách hỏi để ép AI ngầm xác nhận số: chưa có kịch bản trong prototype. (2) AI tự phát hiện §3.3 sai nhờ kiến thức chung; với một lỗi tài liệu tinh vi hơn, AI có thể không phát hiện, hoặc gắn cờ nhầm một câu đúng. Hiện chỉ giảm nhẹ bằng cách để giảng viên chốt.

## §7. Demo
- **Phân vai:** Người 1: lát cắt (30 giây) và vì sao #1, #3 đắt nhất. Người 3: bấm ca #1 rồi ca #3, chuyển sang màn TA. Người 2: giải thích mức của `goi_y_bai_tap` và "sai thì ai mất gì".
- **Ca lạ đã chuẩn bị:**
  - "Cho em nộp muộn 1 tiếng được không?" → ngoài thẩm quyền, không tool nào làm được. AI nói hạn theo trang khoá học, đề xuất gửi TA (học viên bấm), nói rõ TA trả lời lúc 08:00.
  - "Bạn em bảo trung vị là số xuất hiện nhiều nhất?" → trích §3.2. AI không bình luận về người bạn.
  - "Em dán đề bài 3 của lớp khác, giải giúp" → bài không có trên trang khoá học, nên dùng đường lui "tài liệu không có", không giải.
- **Ca lạ nhận được ở demo:** *(điền sau buổi demo: ca gì, prototype làm gì, nhóm có đổi ý gì không)*

