# KÊNH VIỆT – TRUNG — ADAPTIVE TWO-SIDED STORYTELLING FRAMEWORK V1.0

**Mục đích:** Hệ thống nghiên cứu, chọn cấu trúc, viết, biên tập, kiểm định và đóng gói kịch bản lịch sử **Việt Nam – phương Bắc (938–1885)** cho YouTube AI Voice. Kế thừa *History Channel Framework V3.0* (kể theo chứng cứ, không khuôn cứng). Thêm phần riêng của kênh: **hai phía**, **nguồn phía Bắc**, **cách gọi tên**, **gói đăng**.

## Bắt đầu ở đâu?
1. Đề đã qua cổng chọn đề trong `../VIET_TRUNG_HISTORY_CHANNEL_STRATEGY.md` (§8: Visual Gate → Content Selection → 2 câu Việt–Trung). Framework này bắt đầu **sau** khi đề đã được chọn.
2. Đọc `SKILL.md` để biết thứ tự vận hành và đầu ra.
3. Đọc `CHANNEL_DNA.md` (bất biến), `NARRATIVE_ENGINE.md` (hình dạng kể), `EVIDENCE_GATE.md` (sử liệu hai phía).
4. Điền `TEMPLATES/01`–`03` và `06_SOURCE_CROSSCHECK.md` trước khi khoá bản thảo. Đây là biểu mẫu tư duy, không phải thứ phải hiện ra trong video.
5. Kiểm `QUALITY_GATES.md`, `AUDIENCE_SIMULATION.md`, `RELEASE_CHECKLIST.md`. Điền `TEMPLATES/07_PUBLISH_PACKAGE.md` trước khi đăng.
6. Dùng `WORKFLOW_PROMPTS.md` cho các lệnh ngắn.

## Ranh giới quan trọng
- **Đạt về kể chuyện ≠ đã xác minh sử liệu.** Giữ nguyên nguyên tắc V3.
- **Hai phía ≠ chia đôi thời lượng, và ≠ "hai bên đều đúng".** Hai phía nghĩa là phía Bắc có **phép tính có nguồn**, không phải phản diện vô danh. Kết luận vẫn đi theo chứng cứ.
- **Nguồn phía Bắc không tự động đúng hơn hay sai hơn sử Việt.** Mỗi bên đều có lý do để phóng đại thắng lợi và thu nhỏ thiệt hại của mình. Xem `EVIDENCE_GATE.md`.
- Chưa có kịch bản mẫu Việt–Trung nào được khoá. `REFERENCE_SCRIPTS/README.md` ghi cách dùng tạm *Quang Trung V11* và điều kiện để một tập pilot thành bản mẫu.
- Khung 9 beat ở Strategy §9 là bố cục mặc định cho dựng hình/board. Khi **viết kịch bản**, 9 beat là **chức năng cần làm được**, không phải thứ tự hay số phút bắt buộc (`NARRATIVE_ENGINE.md` §6).

## Cấu trúc
`SKILL.md` (điều phối) · `CHANNEL_DNA.md` (bất biến) · `NARRATIVE_ENGINE.md` (thích ứng) · `EVIDENCE_GATE.md` (sử liệu hai phía) · `HOOK_ENDING_RETENTION.md` (mở/kết/nhịp + khớp tiêu đề) · `VOICE_STYLE_GUIDE.md` (ngôn ngữ đọc + gọi tên) · `AUDIENCE_SIMULATION.md` (kiểm nghe 4 lượt) · `QUALITY_GATES.md` (9 cổng đạt/trượt) · `RELEASE_CHECKLIST.md` (khoá kịch bản + gói đăng) · `WORKFLOW_PROMPTS.md` (lệnh) · `TEMPLATES/` (7 mẫu điền) · `REFERENCE_SCRIPTS/` (bản mẫu và điều kiện chốt).

## Nối với pipeline Cook
Kịch bản `READY FOR VOICE TEST` → `cook-video-uc01` (làm sạch VO, TTS, preproduction P1–P4). Mọi thực thể trong `02_EVIDENCE_LEDGER` mức A/B → hồ sơ `history_dossier_*` (skill `history-fidelity`). Phần **KHÔNG ĐỌC BẰNG AI VOICE** không được đưa vào ô script của Cook.
