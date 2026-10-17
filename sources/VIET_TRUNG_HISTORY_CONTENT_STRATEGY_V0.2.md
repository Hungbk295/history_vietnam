# KÊNH LỊCH SỬ VIỆT – TRUNG — CONTENT STRATEGY V0.2 (khán giả trẻ · faceless · kể bằng hình)

**Phiên bản:** 0.2 — DỰ THẢO, viết lại từ v0.1 (bản v0.1 xếp "bang giao/sắc phong/cống" là cơ hội số 1; v0.2 bỏ vì khó vẽ và khô với khán giả trẻ)
**Dùng cùng:** `HISTORY_CHANNEL_CONTENT_STRATEGY.md` (V1.0), `channels/lich-su` + `channel-styles/lich-su-ngoai-truyen.md` + `su-viet-dieu-tra.md` (Writer Room), hồ sơ `history_dossier_*`, skill `history-fidelity`
**Nhãn bằng chứng:** **[D]** = có trong dữ liệu spy; **[J]** = phán đoán của người viết, chưa kiểm chứng; **[K]** = sự kiện lịch sử cần qua Evidence Gate trước khi dùng.

## 0. Thay đổi so với v0.1 (và sửa hai kết luận cũ)

| Điểm | v0.1 | v0.2 |
|---|---|---|
| Cơ hội số 1 | Bang giao, sắc phong, cống (0 video) | **Hạ cấp.** 0 video có thể vì đó là giấy tờ, khó vẽ, ít kịch tính [J]. Chỉ làm khi có vật/cảnh gánh (chiếc ấn, người đóng thế) |
| Tiêu chí chọn đề | Có cầu, có khoảng trống | Thêm **Visual Gate**: đề phải ra được 6–10 cảnh vẽ được |
| Khán giả | Người Việt 18–45 (kênh `lich-su`) | **16–28, quen Shorts/TikTok** (§2) |
| "Tóm tắt/Toàn bộ" 3,41× view/sub | Ghi như tín hiệu | **Bỏ.** Chỉ là nhiễu kênh tí hon (xem §1.2) |
| Việt–Trung kém hơn mặt bằng? (trung vị 1.318 vs 3.301 view) | Không nêu | **Kiểm lại: không kém** khi cùng cỡ kênh (§1.1) |

## 1. Dữ liệu — làm lại có kiểm soát cỡ kênh

Nguồn: `writer-room-data/spy/spy.sqlite`, 103 kênh lịch sử Việt, 3.115 video; nhãn Việt–Trung gắn bằng từ khóa tiêu đề (480 video, có nhiễu).

### 1.1 Việt–Trung có yếu hơn đề khác không? **[D] Không**

Trung vị tổng thể 1.318 (nhãn Việt–Trung) so với 3.301 (còn lại) là hiệu ứng cỡ kênh: video Việt–Trung dồn vào kênh nhỏ. Cùng cỡ kênh:

| Số sub kênh | View trung vị, Việt–Trung | View trung vị, đề khác |
|---|---:|---:|
| <1k | 732 (n=218) | 1.076 (n=404) |
| 1–5k | 1.350 (n=128) | 1.537 (n=670) |
| 5–20k | 3.798 (n=78) | 2.936 (n=802) |
| ≥20k | 14.626 (n=56) | 14.495 (n=759) |

Từ 5k sub trở lên, Việt–Trung bằng hoặc hơn mặt bằng. Ở kênh dưới 5k thì thấp hơn nhẹ (nhiễu rộng). **Kết luận:** đề Việt–Trung không phải niche yếu; không có "phần thưởng" riêng, nên **thắng bằng cách kể, không bằng chọn đề**.

### 1.2 Tiêu đề nào hợp? (video ≥7 phút, kênh ≥5k sub, so view/sub trung vị) **[D]**

| Mẫu tiêu đề | n | View/sub | Phần còn lại |
|---|---:|---:|---:|
| **"Vì sao / Tại sao"** | 216 | **0,50** | 0,26 |
| "Bí ẩn / Sự thật / Giải mã" | 222 | 0,37 | 0,27 |
| "Tóm tắt / Toàn bộ / Trọn bộ" | 46 | 0,29 | 0,28 |

- "Vì sao" vẫn hơn gần gấp đôi sau khi bỏ kênh nhỏ. Riêng khoảng 7–20 phút: 1,45 (n=41) so với 0,07, mẫu nhỏ, chỉ coi là hướng.
- "Tóm tắt/Toàn bộ" 3,41× trong v0.1 **là artifact**: hàng đầu toàn kênh 146–175 sub. Sau khi lọc còn ngang mặt bằng. **Không dùng làm chiến lược.**
- "Bí ẩn/Sự thật" không hơn mặt bằng đáng kể: tránh làm công thức.

### 1.3 Shorts (≤3 phút) **[D, mẫu nhỏ]**

- Có 308 Shorts; 94 gắn nhãn Việt–Trung. Ở kênh ≥5k sub, Shorts Việt–Trung trung vị **10,99k** (n=12) so với 5,32k (n=88) của Shorts đề khác. Mẫu quá nhỏ và dồn vào Dòng Chảy Sử Việt.
- Cùng cỡ kênh ≥5k, trung vị Shorts (6,2k) **bằng** video dài (6,2k). Chưa có bằng chứng Shorts hơn video dài về view.
- Top Shorts: Dòng Chảy 60 giây "Lý Thường Kiệt xuất 10 vạn quân tiến đánh Đại Tống" 46,9k; "Phim" Bạch Đằng (hoạt họa) 27,7k; Lắng Sử "Bị đâm thủng đùi vẫn tỉnh bơ" 20,5k; Dương Tư Húc đánh Mai Hắc Đế 18,8k; "5 vạn quân Xiêm bị xóa sổ trong 1 ngày" 18,8k.
- **Điểm chung:** một cảnh hành động hoặc một con số gây sốc, nói trong 60–130 giây. Không phải tóm tắt triều đại.
- **Kết luận:** Shorts **không thay** video chính; dùng như **trailer và thử hook** (§6). Quyết định chia công sức là [J].

### 1.4 Thị trường (giữ từ v0.1, có chỉnh)

- **Bão hoà:** Trần–Nguyên Mông (85 video), Tây Sơn–Thanh trận Kỷ Dậu (72), Bạch Đằng 938 (56), Lam Sơn (51). 6 video >500k đều của Dòng Chảy Sử Việt **[D]**.
- **Thưa:** Hồ Quý Ly–Minh (18), Mạc Đăng Dung–Minh (15), Pháp–Thanh/Cờ Đen (3), quân Tưởng 1945 (9), trước 938 (~87 nhưng cầu thấp, phần lớn <2k view) **[D]**.
- Dưới cùng cỡ kênh, **"cảnh/vật rõ ràng" thắng "chủ đề rộng"**: chiếc ấn nhà Thanh bị nấu chảy 62,8k, Quang Trung phái người đóng thế mừng thọ Càn Long 80,8k, Gia Long truy đuổi Quang Trung 70k, đều của kênh 5,1k sub **[D]**.

## 2. Khán giả mục tiêu và quy tắc vận hành **[J, dựa V1.0 §9 phần retention]**

**Persona:** 16–28 tuổi, xem Shorts/TikTok nhiều, mở video lịch sử vì tò mò "chuyện gì thực sự xảy ra", bỏ ngay khi thấy "giảng bài". Không cần nhớ niên đại, cần hiểu **ai muốn gì, ai thua gì**.

Quy tắc kể (bắt buộc từ v0.2):

1. **Hook 5–10 giây:** một cảnh có thật, hành động hoặc vật cụ thể, kèm một câu hỏi "Vì sao" (không mở bằng bối cảnh triều đại).
2. **Một nhân vật trục; tối đa 3 tên riêng có mặt trên hình** mỗi video; tên phụ gọi bằng chức ("viên tướng Minh", "sứ giả Tống").
3. **Một cái giá cụ thể (stake):** nhân vật có thể mất gì (mạng, ngai, thành). Viết thành câu ngay đầu.
4. **Không nhảy năm khi không có cảnh bản đồ hoặc thanh thời gian.** Mỗi lần đổi mốc phải có một beat bản đồ.
5. **Ngôn ngữ nói cho tai:** câu ≤ ~15 chữ khi kể diễn biến; thuật ngữ cổ (đạo, lộ, châu) đổi sang cụm dễ hiểu ở lần đầu.
6. **Đối chiếu hai phía bằng hình:** cảnh phía Bắc và cảnh phía Việt xen kẽ có chủ đích (màu/bố cục khác nhau).
7. **Kết bằng hình ảnh và câu hỏi tập sau;** không giảng bài học (giữ G7).
8. **Độ dài chính 8–12 phút** (1.600–2.200 chữ; mẫu Ngoại Truyện 1.900–2.400 chữ). Video >35 phút chỉ là bản đầy đủ làm sau, không là loại chủ lực **[D: 35–60 phút có view/sub trung vị thấp nhất, ~0,33]**.

## 3. Định vị

**Historical Event-Driven Storytelling cho người trẻ: Việt Nam và phương Bắc qua những cảnh quyết định.** Mỗi tập có một **cảnh trục** (hoặc vật trục) người xem nhớ được, và một câu hỏi "Vì sao" mà tập trả lời bằng phép tính của cả hai phía.

Tuyên ngôn: *Không chỉ kể ai thắng. Kể cảnh quyết định, người đứng trong cảnh đó đang sợ gì, và vì sao cảnh ấy đổi cả cục diện.*

## 4. Phạm vi — ĐỀ XUẤT (giữ như v0.1)

Lõi **938 → 1885**; nối **1884–85 Pháp–Thanh** và **1945 quân Tưởng** nếu có cảnh vẽ được; trước 938 chỉ làm tập mở đầu; sau 1950 chờ chốt (§11). Lý do thêm: trước 938 cầu thấp **[D]**; 1950–1991 nhạy cảm nguồn **[J]** và sổ tay G2/G8 giới hạn.

## 5. Visual Gate — cổng mới, đặt TRƯỚC Content Selection Gate

Một đề chỉ qua nếu trả lời được 5 câu bằng cảnh cụ thể, không bằng khái niệm:

1. **6–10 cảnh then chốt** mà mỗi cảnh viết được thành một câu: *ai · ở đâu · làm gì · vật gì trong tay/trên bàn*.
2. **Một vật/motif trục** lặp mở–giữa–kết (cọc, ấn, ống đồng, cầu phao, lá cờ...).
3. **Ít nhất 2 beat bản đồ/số** (hướng tiến quân, số quân, khoảng cách, ngày) để HF+ dựng.
4. **Số gương mặt có tên ≤ 3**; phần còn lại là đám đông vô danh hoặc chức danh.
5. **Cảnh đắt có đường ra:** hành động/trận → Omni; bối cảnh thiếu dossier (kiến trúc, trang phục) → ghi chi phí làm hồ sơ.

**Chấm Visual (0–10):** cảnh vẽ được (0–3) + vật trục (0–2) + beat bản đồ/số (0–2) + ít mặt có tên (0–2) + dossier sẵn (0–1). **<6: không vào danh sách; 6–7: làm khi có ngân sách hồ sơ; ≥8: ưu tiên.** Đây là thang [J], hiệu chỉnh sau 5 video đầu bằng thời gian làm hình và số ảnh phải gen lại.

**Đề thất bại điển hình:** điểm ngoặt là thư từ, chiếu chỉ, đàm phán trong phòng kín. Chỉ vào khi có vật hoặc cảnh gánh (ví dụ chiếc ấn bị nấu chảy, người đóng thế đi mừng thọ).

## 6. Ràng buộc pipeline faceless (Cook/DNA Spy)

- **Hình:** vẽ cách điệu theo DNA gốc lịch sử (#164 trung lập; #152 thế kỷ 19 nếu cần), **không đưa ảnh thật vào gen** (ảnh tư liệu chỉ để agent hiểu).
- **Nhân vật:** đám đông vô danh dùng bình thường; số khuôn mặt có tên tăng chi phí và rủi ro lệch mặt giữa các cảnh, nên Visual Gate giới hạn ≤3.
- **Quy trình bắt buộc:** hồ sơ `history_dossier_*` đã duyệt → `history_check_prompts` → **1 ảnh mẫu duyệt trước khi gen hàng loạt** (skill `history-fidelity`).
- **Phân công kỹ thuật:** cảnh hành động/trận → Omni (clip 4–10s); số, bản đồ, nhãn → HF+; tránh chữ do model ảnh tự gen.
- **Chi phí theo đề:** đề đã có dossier duyệt (Quang Trung, Tôn Sĩ Nghị, Lê Chiêu Thống, Ngọc Hồi, Khương Thượng, cầu phao sông Nhị...) rẻ nhất; đề mới phải làm dossier trước (thêm 1 bước).
- **Shorts:** cắt từ cảnh mạnh nhất của video chính (45–90s, 1 cảnh + 1 con số), đăng trước/song song để thử hook. Chưa có bằng chứng Shorts hơn video dài (§1.3), nên chỉ coi là kênh thử, không phân bổ ngân sách lớn.

## 7. Năm trụ cột — chỉnh lại theo hình và người trẻ (tỷ trọng THỬ NGHIỆM)

| Trụ cột | Tỷ trọng | /20 | Khác v0.1 |
|---|---:|---:|---|
| **1. Trận đánh và cú xoay thế trận** (kể bằng cảnh, bản đồ) | **30%** | 6 | Tăng: hợp Omni/HF+, cầu có sẵn. Chỉ làm đề có góc "vì sao", tránh tóm tắt cuộc kháng chiến |
| **2. Phía Bắc quyết định: vì sao họ đến, vì sao họ dừng** | **25%** | 5 | Giảm nhẹ, vẫn là điểm khác biệt |
| **3. Vật và khoảnh khắc đáng nhớ** (ấn, ống đồng, cọc, người đóng thế, cầu phao) | **20%** | 4 | **Mới.** Gộp phần "hậu thế/ký ức" và "bang giao" nhưng chỉ khi có vật/cảnh gánh |
| **4. Người đứng giữa hai bên** (hàng tướng, sứ, phản bội, cầu viện) | **20%** | 4 | Tăng: nhân vật trục dễ cho khán giả bám |
| **5. Chính sách, bang giao, cống, sắc phong** | **5%** | 1 | **Hạ mạnh.** Chỉ 1 tập, qua vật/cảnh |

Mỗi video một trụ chính. Không ép quota; đề không qua Visual Gate thì bỏ.

## 8. Backlog xếp lại theo điểm Visual (cảnh dưới đây là ĐỀ XUẤT [K], chưa kiểm chứng)

Điểm Visual là [J]. Cột "Cầu/cung" dùng [D] (video trong nhóm). Mỗi dòng nêu cảnh trục và vì sao thị trường còn chỗ.

| # | Đề | Trụ | Cảnh trục (vật/motif) | 6–10 cảnh vẽ được (rút gọn) | Điểm Visual | Dossier | Cầu/cung [D] |
|---|---|---|---|---|---:|---|---|
| 1 | **Tôn Sĩ Nghị chạy qua cầu phao sông Nhị, đêm 1789** | 1 | Cầu phao | Quân Thanh ăn Tết trong Thăng Long; hành quân thần tốc Tam Điệp; đồn Ngọc Hồi; Đống Đa; cầu phao sập/quá tải; Tôn Sĩ Nghị bỏ ấn | **9** | **Có 5 hồ sơ duyệt** | Cung cao ở nhóm trận, nhưng góc "kẻ thua chạy" hiếm |
| 2 | **Quang Trung phái người đóng thế sang mừng thọ Càn Long** | 3 | Người đóng thế/lễ phục | Cảnh Nguyễn Huệ nhận chiếu; chọn người giống; đoàn sứ; chầu Càn Long; trở về | **8** | Có Quang Trung | Video tương tự đạt 80,8k trên kênh 5k sub **[D]**, nhưng 1 video; nhiều tập có thể |
| 3 | **Hồ Quý Ly và quân Minh: Đa Bang 1407** | 1 | Thành Đa Bang (hoả khí) | Hồ Quý Ly xin phong, bị lừa; Minh tiến quân; trận Đa Bang; bị bắt; mất nước | 7 | Chưa có | Cầu đã chứng minh: video Đa Bang 394k **[D]**; cung 18 video **[D]** |
| 4 | **Liễu Thăng và ải Chi Lăng 1427 (kể từ phía Minh)** | 2 | Ải/vực hiểm | Hai đạo quân; Liễu Thăng tiến; mai phục; Liễu Thăng chết; viện binh tan | 7 | Chưa có; trang phục Lê sơ ở trạng thái nháp | Cung 51 video Lam Sơn **[D]**, nhưng góc "kể từ phía Minh" hiếm [J] |
| 5 | **Thoát Hoan chui ống đồng, 1288** | 1/3 | Ống đồng | Quân Nguyên rút; ống đồng; Hưng Đạo; mai phục; trốn | 7 (**rủi ro**: truyền thống kể, cần phân biệt chính sử và dã sử) | Chưa có | Cung rất dày (85) **[D]**; chỉ vào nếu có góc mới |
| 6 | **Mạc Đăng Dung quỳ ở ải Nam Quan 1540** | 4 | Ải Nam Quan + tờ hàng | Triều Mạc bị Minh dọa; đi sứ; quỳ ở ải; dâng đất/đổi lấy hoà; phản ứng trong nước | 7 | Chưa có | Cung 15 video, 14k view cao nhất **[D]**; Shorts "Mạc Đăng Dung quỳ ở ải Nam Quan" 2,97k **[D]** |
| 7 | **Chiếc ấn nhà Thanh phong cho Gia Long bị nấu chảy, 1884** | 3 | Chiếc ấn bạc | Lễ phong; ấn ở Huế; Pháp buộc Huế; nấu chảy; hậu quả | 7 | Có de Courcy, Huế 1885 (nháp) | Video này đạt 62,8k trên kênh 5k sub **[D]**; làm tiếp đề "Pháp–Thanh" |
| 8 | **Lê Chiêu Thống cầu viện Thanh** | 4 | Cầu cứu thư/quân cờ | Lê Chiêu Thống chạy; sang Thanh; Tôn Sĩ Nghị; về Thăng Long; bị bỏ rơi | 6 | Có Lê Chiêu Thống | Chưa thấy đủ video cùng góc (cung thấp) [J] |
| 9 | **Lý Thường Kiệt: đêm Như Nguyệt, Nam quốc sơn hà, và vì sao Tống dừng** | 2 | Bài thơ/dòng sông | Tiến đánh Ung Châu; phòng tuyến Như Nguyệt; bài thơ; Tống hết lương; hoà | 6 | Chưa có | Shorts Lý Thường Kiệt 46,9k **[D]**; Cầu cao cạnh tranh Dòng Chảy |
| 10 | **Hàm Tử: Toa Đô bị chặn (1285)** | 1 | Biển/thuyền | Hai đạo quân Nguyên; Trần Nhật Duật; trận Hàm Tử; Toa Đô chết | 6 | Chưa có | Mọt Sử đã làm sâu (73k) [D]; cần góc mới |
| 11 | **Nùng Trí Cao giữa Tống và Đại Việt (1048–55)** | 4 | Lá cờ | Nùng Trí Cao xin thuộc; bị từ chối; nổi dậy; đánh Quảng Châu; thất bại | 5 | Chưa có | Hầu như chưa có video [J, chưa quét]; ít nhận biết với giới trẻ |
| 12 | **Sắc phong và cống Gia Long–Thanh** | 5 | Thư/lễ vật | Gần như chỉ thủ tục | **3** | Chưa có | 0 video **[D]** nhưng **loại khỏi top**; gộp vào #7 |
| — | Tập Tống 981 "vì sao Tống kinh sợ Lê Hoàn" | 2 | Tù binh/sứ | Hội đồng Tống; đánh 981; sứ; Lê Hoàn tiếp sứ | 5 | Chưa có | Lắng Sử 75k [D]; điểm Visual thấp: nhiều phòng họp |

## 9. Lộ trình 20 video thử nghiệm — chỉnh theo Visual và rủi ro

**Đợt 1 (1–5):** #1 (cầu phao; rẻ nhất, dossier sẵn) → #2 (đóng thế) → #7 (chiếc ấn) → #3 (Đa Bang) → #6 (Nam Quan). Mục tiêu: kiểm hai giả thuyết — "Vì sao + vật trục" cho retention tốt, và "cảnh cầu phao/ấn" làm ra hình ổn định.
**Đợt 2 (6–12):** #4, #8, #9, #10, #5 (nếu có góc), #11, 1 tập phía Bắc (Tống 981 hoặc Hốt Tất Liệt).
**Đợt 3 (13–20):** Cờ Đen/Pháp–Thanh, 1945 quân Tưởng (nếu qua Evidence Gate), bang giao #12 qua vật, các tập bản đầy đủ 20–35 phút cho chuỗi đã chạy tốt.
**Mỗi tập có 1–2 Shorts** cắt từ cảnh trục; theo dõi riêng (§10).

## 10. Đo lường sau 20 video

Giữ V1.0 §9, thêm: (a) view/sub so với mốc §1.2 (≈0,5 với tiêu đề "Vì sao"); (b) retention 0–30s của hook có cảnh vs hook có câu hỏi; (c) điểm Visual so với retention và số ảnh phải gen lại; (d) Shorts có kéo người sang video chính không (CTR trang kênh, view video chính sau ngày đăng Short); (e) bình luận hỏi "ai là ai" (dấu hiệu quá nhiều tên). Chỉ giữ thang Visual nếu tương quan với retention.

## 11. Quyết định cần bạn chốt

1. **Phạm vi:** lõi 938–1885, hay 938–1945 như V1.0, hay mở thêm trước 938?
2. **Giai đoạn 1950–1991** (1974, 1979, 1988): làm, hoãn hay loại?
3. **Một kênh riêng hay series trong kênh V1.0?**
4. **Nguồn phía Bắc:** bắt buộc mỗi tập, hay chấp nhận kể qua sử Việt kèm ghi chú?
5. **Xung đột giọng điệu (cần bạn quyết):** để tiếp cận người trẻ, có cho phép **ẩn dụ đại chúng nhẹ** (ví dụ "Aquaman đời thực", "debut 10 điểm" — Lắng Sử 21k/20k **[D]**) và nhịp nhanh kiểu Shorts không? Sổ tay `lich-su` hiện cấm so sánh với đời sống hôm nay (G7/AVOID) và cấm xưng "tôi". Phương án đề xuất [J]: **cho ẩn dụ vui về mặt hình ảnh/vật thể, vẫn cấm so với chính trị và đời sống hôm nay, giữ giọng điềm tĩnh.**
6. **Đóng thế, ống đồng, cọc, cầu phao:** các chi tiết này nửa chính sử nửa dã sử; chấp nhận kể với nhãn "theo truyền thuyết/dã sử" hay chỉ kể phần có chính sử?

## 12. Giới hạn dữ liệu

- Nhãn đề tài bằng từ khóa tiêu đề, không đọc nội dung; có nhiễu. Mỗi kênh tối đa ~50 video nên thiên về video nổi.
- View/sub dùng số sub lúc quét; so sánh ở §1 dùng trung vị và lọc kênh ≥5k sub. Mẫu Shorts và mẫu "Vì sao 7–20 phút" nhỏ: chỉ là hướng.
- Chưa có retention, CTR, độ tuổi người xem; "khán giả 16–28" là giả định về persona, không đo được từ dữ liệu này.
- Điểm Visual, lộ trình và mọi nhận định đánh dấu [J] là phán đoán chờ kiểm bằng dữ liệu 5 video đầu. Sự kiện đánh dấu [K] chưa qua Evidence Gate; không dùng làm dữ kiện kịch bản.
