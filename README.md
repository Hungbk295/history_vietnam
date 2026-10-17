# history_vietnam

Bộ tài liệu cho kênh YouTube faceless **lịch sử Việt Nam – phương Bắc (938–1885)**: chiến lược kênh và framework viết kịch bản. Bản ngày 2026-10-17.

## Đọc theo thứ tự
1. [`VIET_TRUNG_HISTORY_CHANNEL_STRATEGY.md`](VIET_TRUNG_HISTORY_CHANNEL_STRATEGY.md) — **Chiến lược V1.0**: dữ liệu thị trường, định vị, phạm vi, trụ cột, cổng chọn đề, đóng gói, nhịp đăng, **lịch 2 tuần đầu (6 tập + 14 Shorts, title viết sẵn)** và ngân hàng title tuần 3–8.
2. [`VIET_TRUNG_FRAMEWORK_V1/`](VIET_TRUNG_FRAMEWORK_V1/README.md) — **Framework viết kịch bản V1.0**: từ lúc đề đã được chọn tới khi khoá kịch bản và gói đăng. Cùng cấu trúc với History Channel Framework V3, thêm phần hai phía, nguồn phía Bắc, cách gọi tên và gói đăng.
3. [`skills/hook-viet-trung/`](skills/hook-viet-trung/SKILL.md) — **Skill viết hook** (Claude Code): nhiều option hook mở bài theo 7 công thức rút từ 38 phần mở đầu thật, khớp bốn hình dạng A/B/C/D. Cài bằng cách chép thư mục vào `~/.claude/skills/`.
4. [`sources/`](sources/) — tài liệu gốc dùng để chuẩn hoá: chiến lược kênh lịch sử chung V1.0, chiến lược Việt–Trung v0.2 và v0.3, History Channel Framework V3 (kèm 2 kịch bản mẫu Quang Trung V11 và Trần Thủ Độ V24).

## Cấu trúc
```
VIET_TRUNG_HISTORY_CHANNEL_STRATEGY.md   chiến lược kênh V1.0
VIET_TRUNG_FRAMEWORK_V1/
  README.md · SKILL.md                     bắt đầu ở đây · điều phối
  CHANNEL_DNA.md                           bất biến của kênh
  NARRATIVE_ENGINE.md                      chọn hình dạng kể (hai phía)
  EVIDENCE_GATE.md                         sử liệu hai phía + cảnh báo 6 tập pilot
  HOOK_ENDING_RETENTION.md                 mở, kết, nhịp, khớp tiêu đề
  VOICE_STYLE_GUIDE.md                     viết cho tai nghe + bảng gọi tên
  AUDIENCE_SIMULATION.md                   kiểm nghe 4 lượt
  QUALITY_GATES.md                         9 cổng đạt/trượt
  RELEASE_CHECKLIST.md                     khoá kịch bản + gói đăng
  WORKFLOW_PROMPTS.md                      8 lệnh dùng ngay
  TEMPLATES/01–07                          brief, ledger, story map, hook test, audit, đối chiếu nguồn, gói đăng
  REFERENCE_SCRIPTS/README.md              bản mẫu tạm và điều kiện chốt
skills/hook-viet-trung/                    skill viết hook (SKILL.md + references/)
sources/                                   tài liệu gốc
```

## Ghi chú
- Tên skill, tool và đường dẫn như `history-fidelity`, `history_dossier_*`, `cook-video-uc01`, `config/thumb-prompts/…` là của pipeline DNA Spy (Cook), không nằm trong repo này.
- Số liệu thị trường quét ngày 2026-10-17 (vidIQ + YouTube Data API). Mọi sự kiện lịch sử gắn **[K]** phải qua Evidence Gate trước khi vào kịch bản.
