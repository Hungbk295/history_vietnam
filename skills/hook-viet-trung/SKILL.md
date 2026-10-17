---
name: hook-viet-trung
description: >
  Viết nhiều option hook mở bài (beat 1 + câu beat 2 nói lại câu hỏi tiêu đề) cho một tập
  kênh lịch sử Việt–Trung (938–1885), dựng từ 7 công thức rút từ 38 phần mở đầu thật của các
  kênh sử Việt và khớp bốn hình dạng A/B/C/D của Framework Việt–Trung V1.0. Dùng khi người dùng
  đưa tiêu đề/phiếu đề xuất và muốn chọn hook, nói "viết hook cho tập này", "cho tôi các kiểu
  hook Việt–Trung", "hook tập Tôn Sĩ Nghị", "hook Short". Chỉ làm hook (và hook Shorts), không
  viết cả kịch bản; viết toàn văn thì dùng Framework Việt–Trung (WORKFLOW_PROMPTS lệnh 2).
  Chi tiết lịch sử chỉ lấy từ dossier đã duyệt (history_dossier_*) hoặc phiếu đề; không bịa.
---

# Hook Việt–Trung — công thức hook theo chất liệu của tập

Skill **không chọn hook hay nhất**. Nó đưa nhiều option từ nhiều công thức khác nhau cho đúng tập
đang làm, để người dùng so sánh và chọn. Nó mở rộng **bước F** của Framework Việt–Trung V1.0
("chọn hook và khớp tiêu đề", `HOOK_ENDING_RETENTION.md` + `TEMPLATES/04_HOOK_TEST.md`), không thay
bước đó. Bốn hình dạng đã khoá là **A hành động · B nghịch lý · C vật · D hai bộ sử**; bảy công
thức bên dưới nằm dưới bốn hình dạng này hoặc mở rộng chúng.

Bản này mô phỏng cấu trúc skill `hook-doi-thu` v2 (phép thử chất liệu → mỗi công thức một option
→ danh sách công thức bị loại → không xếp hạng), nhưng nguồn là 38 hook lịch sử Việt, không phải
tài chính.

## Nguồn và độ tin cậy (đọc trước khi dùng)

- **FACT:** 38 phần mở đầu (video ≥7 phút, đề Việt–Trung, 12 kênh, tối đa 5 video/kênh), lấy
  ~1.000 ký tự đầu transcript qua Writer Room Spy MCP. Chi tiết và bảng nhãn ở
  `references/corpus-38-mo-dau.md`.
- **FACT:** nhãn do một người gán (model), chưa chấm chéo; transcript đa số là phụ đề tự động có
  lỗi. n nhỏ, nên mọi số là xu hướng.
- **FACT:** đây là **tần suất, không phải hiệu quả**. Không xếp công thức theo lượt xem. Có một
  quan sát lệch kênh (xem corpus §3) nhưng bị nhiễu cỡ kênh nên không dùng làm luật.
- **FACT:** 4 trong 38 mẫu là của kênh Lịch Sử Ngoại Truyện; chúng khớp gần như đúng bốn hình dạng
  A/B/C/D, nên bốn hình dạng được giữ làm khung.
- **SUY LUẬN:** công thức H6, H7 (phía Bắc vào trước; người ở giữa) có rất ít mẫu trong corpus;
  khung của chúng lấy từ Framework (`HOOK_ENDING_RETENTION` B, trụ cột 2 và 4) và 6 hook viết sẵn
  ở Strategy §12. Luôn ghi "mẫu mỏng".

## Đầu vào

Phiếu đề xuất của tập (`TEMPLATES/01_BRIEF` hoặc Strategy §8.4). Cần có: **tiêu đề A** (và B/C
nếu có), trụ cột, **cảnh trục / vật trục**, người phía Bắc là ai, **id dossier** hoặc nguồn cho
cảnh mở. Thiếu thì hỏi **một lần duy nhất**, tối đa 3 câu (tiêu đề đã chốt chưa; cảnh trục/vật là
gì; dossier id hay nguồn nào đứng sau cảnh mở). Không hỏi lại điều đã có trong phiếu.

Lấy chi tiết bằng `history_dossier_list` rồi `history_dossier_get` (chỉ dùng hồ sơ
`status: approved` làm chi tiết chắc; `draft` thì coi là [K]).

## Quy trình

1. Đọc phiếu, lấy dossier (nếu có).
2. Chạy **Phép thử chất liệu** (bảng dưới). Mỗi "có" mở công thức tương ứng.
3. **Gắn nhãn mọi chi tiết cụ thể** định dùng: `[Đ:id]` từ dossier approved · `[N]` từ nguồn ghi
   trong phiếu · `[K]` chưa kiểm. Hook chỉ được chứa `[Đ]`/`[N]`.
4. Viết **một option cho mỗi công thức khả dụng**. Mục tiêu 4–7 option; ít hơn thì nói rõ vì sao.
   Mỗi option là **beat 1 (25–45 chữ, đọc ≈10 giây) + câu beat 2** (câu hỏi của tiêu đề, nguyên
   văn hoặc gần nguyên văn, kèm một cái giá/số). Đếm chữ thật.
5. Option nào cần chi tiết `[K]` để hay lên thì viết **bản an toàn** không có nó, và liệt kê chi
   tiết đó ở "Cần xác minh". Không đưa `[K]` vào lời đọc.
6. Cuối bảng liệt kê **công thức bị loại** kèm lý do một dòng (thiếu chất liệu gì).
7. Điền các cột kiểm có thể kiểm máy móc của `04_HOOK_TEST` (đếm tên, có/không); cột chủ quan ghi
   "cần nghe thử bằng AI Voice".
8. Không nói option nào "hay nhất". Chỉ được nói option nào **rủi ro** vì thiếu dữ kiện/dossier.
9. Người dùng chọn xong thì chuyển option đó sang Framework (lệnh 2 "Viết ngay bản hoàn chỉnh")
   làm đầu vào cho phần mở.

## Phép thử chất liệu

| Câu hỏi về tập | Nếu có, mở công thức |
|---|---|
| Có cảnh có ngày/mùa, nơi chốn, **một hành động nhìn thấy được** có nguồn? | **H1 Cảnh có ngày** (A) |
| Có hai điều trái nhau ngay trong sự kiện (có tất cả mà làm điều lạ; dặn không đánh mà vẫn đánh; thắng mà ký từ bỏ)? | **H2 Nghịch lý hai vế** (B); nếu vế lạ nằm ở phía Bắc thì ưu tiên **H6** |
| Có vật trục tả được kích thước/chất liệu/nơi đặt từ dossier? | **H3 Vật cận cảnh** (C) |
| Có hai con số đối cặp (to/nhỏ, trước/sau), có nguồn và đơn vị? | **H5 Số đối cặp** (mở rộng B, C) |
| Hai bộ sử chép khác nhau, hoặc chi tiết chỉ một phía chép, **và chỗ khác ấy là trục tập**? | **H4 Hai bộ sử** (D) |
| Có một người phía Bắc (chức danh + tên + vai) đang ở một vị trí hoặc đưa một quyết định có nguồn? | **H6 Phía Bắc vào trước** |
| Có một người đứng giữa hai phía hoặc hai lựa chọn có nguồn? | **H7 Người ở giữa** |
| Cảnh mở có dã sử/truyền thuyết? | Bắt buộc H4, hoặc viết dạng **hỏi** kèm nhãn trên hình; không khẳng định |

## Bảy công thức

Chi tiết, mẫu trích từ corpus và giới hạn từng công thức: `references/cong-thuc-hook.md`.
Nguyên văn 38 phần mở đầu để đối chiếu nhãn: `references/corpus-38-nguyen-van.md` (không chép câu chữ vào hook mới).
Ví dụ chạy thử đầy đủ một tập (định dạng đầu ra, nhãn dossier, công thức bị loại): `references/vi-du-chay-thu-tap1.md`.

| Công thức | Hình dạng | Khung (beat 1) | Neo | Bẫy |
|---|---|---|---|---|
| **H1 Cảnh có ngày** | A | Ngày/mùa + nơi → ai làm gì (một hành động) → một vật hoặc số → bỏ lửng | CẢNH | Chi tiết giác quan dựng thêm (tay run, mồ hôi...) |
| **H2 Nghịch lý hai vế** | B | "Họ có/đạt [X]… vậy mà [Y trái ngược]" | CẶP | Vế sau phải có nguồn, không phải suy diễn tâm lý |
| **H3 Vật cận cảnh** | C | Vật + kích thước/chất liệu + nơi đặt → người xem **chưa** biết vì sao quan trọng | VẬT | Tả vật theo tưởng tượng thay vì theo dossier |
| **H4 Hai bộ sử** | D | "Sử [A] chép… sử [B] chép… hoặc chỉ [một phía] chép" → câu hỏi | NGUỒN | Chỉ dùng khi chỗ khác là trục; không phán ai đúng |
| **H5 Số đối cặp** | B/C | Hai số có đơn vị đặt cạnh nhau ngay câu đầu | SỐ | Số không nguồn, đơn vị lẫn (vạn/nghìn) |
| **H6 Phía Bắc vào trước** | B | Chức danh + tên + vai của người phía Bắc, đang làm/giữ gì → điều trái kỳ vọng | NGƯỜI BẮC | Quá 3 tên; giới thiệu thiếu vai |
| **H7 Người ở giữa** | A/B | Một người, hai lựa chọn hoặc hai bờ → cái giá của mỗi lựa chọn | NGƯỜI | Độc thoại nội tâm, tâm lý không nguồn |

## Luật khi viết option

1. **Không bịa**: sự kiện, số, thoại, tâm lý, tiểu tiết nhìn thấy, "triều đình phương Bắc nghĩ gì".
   Mỗi chi tiết cụ thể phải có nhãn `[Đ]` hoặc `[N]`. Corpus có mẫu vi phạm: một hook mở bằng "đôi
   tay siết chặt vào tay vịn ghế đến tái nhợt" không có nguồn nào; đừng viết kiểu đó.
2. **Không mở bằng chào, đăng ký, ru ngủ, "hôm nay"**. Không "tôi" (G6). 9/38 hook corpus mở
   bằng chào/đăng ký/ru ngủ trước cảnh đầu tiên. Không "hãy nhắm mắt/hãy hình dung/tưởng tượng".
3. **Không từ mang lập trường hoặc miệt thị**: giặc, quân ta, bọn chúng, kẻ thù, tàn bạo, ngu
   muội, "hào hùng", "hồn thiêng". Gọi theo triều (nhà Tống/Nguyên/Minh/Thanh), theo bảng
   `VOICE_STYLE_GUIDE.md`. Dùng "xâm lược" chỉ như tên sự kiện chuẩn. 18/38 hook corpus có
   loại từ này trong phần mở.
4. **Dã sử thì hỏi, không khẳng định**; ghi `[nhãn trên hình: theo dã sử/truyền thuyết]`.
5. **Tối đa 3 tên riêng trong 30 chữ đầu.** Người phía Bắc lần đầu: **chức danh + tên + vai**.
   Tên khó đọc bằng AI Voice: ghi cách đọc ở phần KHÔNG ĐỌC.
6. **Không mở bằng bối cảnh triều đại** hoặc recap tập trước (Strategy §9 quy tắc bắt buộc).
7. **Câu beat 2 nói đúng câu hỏi của tiêu đề** (khớp tiêu đề). Hook không hứa điều thân bài không
   trả, không tiết lộ đáp án/cao trào.
8. **Tránh sáo đã mòn trong corpus**: mở bằng bài thơ *Nam quốc sơn hà* (2/38); tuyên ngôn "đỉnh
   cao nghệ thuật quân sự / hồn thiêng sông núi" (2/38); mở bằng Bạch Đằng làm câu đầu (3/38);
   chào "quý vị… ru vào giấc ngủ" (5 video cùng một kênh). Tiêu đề có "Bạch Đằng" chiếm
   30/377 video dài Việt–Trung, tức đề rất chật.
9. **Hình ảnh hôm nay** (tên đường, di tích) thuộc beat 8, không đưa vào hook.
10. **Hook phải vẽ/dựng được**: beat 1 có thể thành 1–2 cảnh (Omni 4–6s + ảnh), ≤3 mặt có tên; số
    và bản đồ làm bằng HF+. Ghi lane gợi ý cho từng option.

## Định dạng đầu ra

```
Tập: [tiêu đề A] | Trụ: ... | Dossier: [id...] | Chất liệu có: ... | Chất liệu thiếu: ...

Option 1 — [H?] (hình dạng A/B/C/D; neo: ...; hợp tiêu đề: A/B/C)
Beat 1 (N chữ): "..."
Beat 2 (N chữ): "..."
Chi tiết dùng: [Đ:id] ..., [N] ...
Cần xác minh [K]: ... (bản an toàn đã bỏ chi tiết này)
Dựng được bằng: Omni/ảnh/HF+ (số mặt có tên: n)
Thân bài phải trả: ... (beat/neo trả lại)
Kiểm máy: tên trong 30 chữ = n ≤3? · người phía Bắc có chức danh+vai? · có từ cấm? · có dã sử → đã hỏi + nhãn? · nói rõ câu hỏi tiêu đề? · lộ cao trào? | Cần nghe thử: người mới hiểu ngay?

...

Công thức bị loại: [H?] — thiếu [chất liệu]
Rủi ro vì thiếu dữ kiện: [option nào, vì sao]
```

## Hook Shorts (45–90 giây)

Nếu người dùng nhắm Short: **12–25 chữ**, một cảnh + một con số + một câu hỏi, cắt từ beat 1, 5
hoặc 6 của tập chính (Strategy §9.3, không tóm tắt triều đại). Không cần nhắc tiêu đề dài; vẫn áp
luật 1–5. Short mở bằng H1/H3/H5 trước, H4 sau.

## Không làm

- Không viết toàn văn, không đề xuất tiêu đề (tiêu đề đã chốt ở phiếu; muốn đổi tiêu đề thì dùng
  Strategy §10).
- Không dùng corpus làm nguồn sự thật: câu chữ của đối thủ không được chép, chỉ mượn khung. Số,
  tên, năm trong `references/` chỉ để minh hoạ cấu trúc.
- Không xếp "hay nhất", không dựa lượt xem để chấm công thức.
- Không ghi vào `synced/`; không đụng skill `hook-doi-thu` (tài chính) hay `hook-writer`.
