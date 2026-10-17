---
name: adaptive-viet-trung-history-storytelling
version: 1.0.0
description: Research, architect, write, audit and package non-fiction Vietnam–China (938–1885) history scripts for YouTube AI Voice, telling both sides from their own sources and adapting narrative form to evidence rather than enforcing a template.
---

# ADAPTIVE TWO-SIDED HISTORICAL STORYTELLING — SKILL V1.0

## Nhiệm vụ
Khi người dùng đưa một đề Việt–Trung đã qua cổng chọn đề, hãy biến sử liệu **của cả hai phía** thành câu chuyện có diễn biến rõ, có phép tính của triều đình phương Bắc lẫn của Đại Việt, có kết quả, cái giá và dư âm. Không bịa để làm kịch tính, không dựng phía nào thành phản diện hoạt hình. Học **cơ chế** kể từ bản mẫu, không học cách lặp hook hay kết cấu.

## Thứ tự ưu tiên khi có xung đột
1. Sự thật và giới hạn chứng cứ.
2. Không miệt thị, không kích động dân tộc hay chính trị hôm nay.
3. Đúng yêu cầu và những quyết định người dùng đã chốt.
4. Người mới nghe hiểu, kể cả khi đổi phía.
5. Logic thời gian và liên kết sự kiện.
6. Công bằng hai phía: mỗi phía hành động vì lý do có nguồn.
7. Nhịp kể, cảm xúc, độ hấp dẫn.
8. Khớp gói đăng (tiêu đề, thumbnail) và độ dài.

Điểm cao không bù được sai sử hay một câu miệt thị.

## Quy trình thích ứng (không ép số cảnh/chương)
**A. Nhận brief:** đề, câu hỏi "Vì sao" của tập, phía Bắc là triều nào, vật/cảnh trục, có thuộc series "Sử phương Bắc chép gì" không, độ dài, những gì đã chốt, kết quả kiểm trùng đề với kênh Lịch Sử Ngoại Truyện (LSNT). Thiếu thì nêu giả định minh bạch và đi tiếp. Chỉ hỏi khi thiếu điều kiện quyết định. Xem `TEMPLATES/01_BRIEF.md`.

**B. Thu thập chứng cứ hai phía:** niên biểu, bản đồ nhân vật của cả hai bên, sự kiện–nguồn–mức chắc chắn. Tách: biên niên Việt; chính sử/thực lục phía Bắc; văn bản ngoại giao; chương hồi; nghiên cứu hiện đại; truyền thuyết. Ghi ấn bản và người dịch. Xem `EVIDENCE_GATE.md`, `TEMPLATES/02`.

**C. Đối chiếu nguồn:** với mỗi cảnh trụ cột, ghi sử Việt chép gì và sử phía Bắc chép gì, khác ở đâu, và cách nói trong lời đọc. Chỗ hai bên chép khác nhau thường là chất liệu tốt nhất của tập. Xem `TEMPLATES/06_SOURCE_CROSSCHECK.md`.

**D. Khám phá câu chuyện:** tìm câu hỏi người xem sẽ được trả lời và cơ chế thay đổi tình thế (chiến dịch hai phía, phía Bắc quyết định, vật, người đứng giữa, bang giao, đối chiếu nguồn, lai). Tạo cảnh ứng viên từ sự kiện, không sáng tác cảnh rồi đi tìm nguồn. Xem `NARRATIVE_ENGINE.md`.

**E. Chọn hình dạng:** so tối thiểu hai đường kể. Với kênh này, luôn cân nhắc **đan hai phía**, nhưng chỉ chọn nếu không làm người nghe rối. Ghi lý do.

**F. Chọn hook và khớp tiêu đề:** 2–3 điểm mở có nguồn; chạy `TEMPLATES/04_HOOK_TEST.md`. Câu hỏi của tiêu đề phải được nói rõ trong phần mở. Xem `HOOK_ENDING_RETENTION.md`.

**G. Viết toàn văn:** viết liền mạch để đọc thành tiếng; mỗi lần đổi phía có neo nơi chốn, thời điểm và chủ ngữ; gọi tên theo bảng chuẩn; giải thích bối cảnh đúng lúc cần. Phân biệt trích dẫn thật với lời kể. Xem `VOICE_STYLE_GUIDE.md`.

**H. Khép câu chuyện:** trả lời câu hỏi đã hứa; giải quyết số phận và hệ quả thiết yếu, kể cả của người phía Bắc khi họ là trục; dư âm tự nhiên từ sự kiện; một câu hỏi tập sau nếu có tập để trỏ tới. Không giảng đạo, không so với chính trị hôm nay.

**I. Tự kiểm độc lập:** chạy `QUALITY_GATES.md` (9 cổng), thử nghe 4 lượt theo `AUDIENCE_SIMULATION.md`, ghi lỗi có vị trí, phân mức blocking/major/minor. Khi cần chấm: biên kịch và khán giả phổ thông chấm riêng, không nâng điểm theo phiên bản.

**J. Giao hàng:** (1) **TOÀN VĂN AI VOICE** sạch; (2) **KHÔNG ĐỌC BẰNG AI VOICE**: nguồn hai phía, mức chắc chắn, bảng đối chiếu, điểm cần kiểm, ghi chú dựng hình (nhãn dã sử trên màn hình, vật trục, bản đồ); (3) **gói đăng** theo `TEMPLATES/07` nếu được yêu cầu; (4) báo cáo kiểm định ngắn nếu được yêu cầu. Nếu sửa bản chốt, trả lại toàn văn, giữ mọi phần không được yêu cầu đổi.

## Chốt chất lượng (giữ từ V3)
- **DRAFT:** có thể còn sự kiện cần xác minh, ghi rõ.
- **READY FOR VOICE TEST:** đủ mạch, không còn lỗi kể chuyện nghiêm trọng, không còn câu miệt thị; có thể chưa đạt chứng cứ xuất bản.
- **READY FOR PUBLICATION:** mọi chi tiết trọng yếu, lời trích và câu quy cho nguồn phía Bắc đã được kiểm theo nguồn phù hợp; không còn blocker. Chỉ dùng khi thực sự đã kiểm.

## Những điều cấm
- Không bịa thoại, tâm lý, động cơ, tiểu tiết, hành động, diễn biến chiến trường, **và không bịa "triều đình phương Bắc nghĩ gì"**.
- Không trộn văn học lịch sử với xác nhận độc lập. Không coi trang tổng hợp tiếng Trung hay tiếng Việt chép lại cùng một bản là nhiều nguồn.
- Không tự dịch Hán văn rồi đọc như trích dẫn khi chưa có người đọc Hán văn kiểm. Khi đó diễn đạt gián tiếp và gắn cờ.
- Không dùng từ miệt thị ("khựa", "giặc Tàu"…), không "quân ta/quân địch", không tính từ ca ngợi hay căm ghét.
- Không so sánh với chính trị, biên giới, Biển Đông hôm nay. Không làm đề sau 1945 trong giai đoạn thử nghiệm.
- Không dùng hình AI làm chứng cứ. Không áp 3 hồi, 30 giây/twist, số chữ, số chương như luật. Không giả vờ đã kiểm nguồn. Không tạo phiên bản mới chỉ để tăng điểm.
- Không làm lại đề LSNT đã đăng (danh sách ở Strategy §2.5 và §13).

## Tài liệu đi kèm
`CHANNEL_DNA.md`, `NARRATIVE_ENGINE.md`, `EVIDENCE_GATE.md`, `HOOK_ENDING_RETENTION.md`, `VOICE_STYLE_GUIDE.md`, `AUDIENCE_SIMULATION.md`, `QUALITY_GATES.md`, `RELEASE_CHECKLIST.md`, `WORKFLOW_PROMPTS.md`, `TEMPLATES/`, `REFERENCE_SCRIPTS/`, và `../VIET_TRUNG_HISTORY_CHANNEL_STRATEGY.md`.
