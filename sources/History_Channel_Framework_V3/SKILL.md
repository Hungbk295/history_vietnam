---
name: adaptive-vietnamese-history-storytelling
version: 3.0.0
description: Research, architect, write and audit non-fiction Vietnamese history scripts for YouTube AI Voice, adapting narrative form to evidence rather than enforcing a template.
---

# ADAPTIVE HISTORICAL STORYTELLING — SKILL V3.0

## Nhiệm vụ
Khi người dùng đưa một chủ đề lịch sử, hãy biến sử liệu thành câu chuyện có diễn biến rõ, nhân vật hành động có căn cứ, kết quả và dư âm; không bịa để làm kịch tính. Học **cơ chế** từ hai bản chốt trong `REFERENCE_SCRIPTS/`, không học cách lặp y hệt hook hoặc kết cấu.

## Thứ tự ưu tiên khi có xung đột
1. Sự thật/giới hạn chứng cứ; 2. đúng yêu cầu và những quyết định người dùng đã chốt; 3. người mới nghe hiểu; 4. logic thời gian và liên kết sự kiện; 5. nhịp kể, cảm xúc và độ hấp dẫn; 6. tối ưu độ dài. Điểm cao không bù được sai sử.

## Quy trình thích ứng (không ép số cảnh/chương)
**A. Nhận brief:** Nắm chủ đề, phạm vi, người xem, độ dài nếu có, mức nghiên cứu và bản nào đã chốt. Nếu thiếu, đưa ra giả định minh bạch và tiếp tục; chỉ hỏi khi thiếu điều kiện quyết định. Xem `TEMPLATES/01_BRIEF.md`.

**B. Thu thập chứng cứ:** Lập niên biểu, bản đồ nhân vật, sự kiện–nguồn–mức chắc chắn; tách nguồn sơ cấp/biên niên, sử thuật văn học, nghiên cứu hiện đại, truyền thuyết. Ghi chính xác đoạn/ấn bản khi có. Xem `EVIDENCE_GATE.md`.

**C. Khám phá câu chuyện:** Tìm câu hỏi người xem sẽ được giải đáp; nhận diện cơ chế thay đổi tình thế (chiến dịch, chính biến, đại án, ngoại giao, tiểu sử, xã hội hoặc lai). Tạo cảnh ứng viên từ sự kiện, không sáng tác cảnh rồi đi tìm nguồn. Xem `NARRATIVE_ENGINE.md`.

**D. Chọn hình dạng:** So sánh tối thiểu hai đường kể có thể thực hiện: tuyến tính; mở ở bước ngoặt rồi hồi cố; song tuyến; nhiều điểm nhìn; diễn tiến theo chứng cứ. Chọn đường ít làm người nghe rối nhất mà vẫn làm nổi bật sự thay đổi tình thế. Không bắt buộc có hồi cố.

**E. Chọn hook:** Đưa ra 2–3 điểm mở dựa trên sự kiện có nguồn, đánh giá hiểu nhanh / mối nguy hay bất thường / lời hứa / nguy cơ tiết lộ kết quả / tải tên riêng. Chọn một, không ép “giây 3 phải có gươm”.

**F. Viết toàn văn:** Viết liền mạch để đọc thành tiếng; dùng quan hệ thời gian, nhân quả, đồng thời, tương phản đúng bản chất; giải thích bối cảnh tại thời điểm cần; cao trào nảy sinh từ lịch sử. Phân biệt trích dẫn thật với lời kể. Xem `VOICE_STYLE_GUIDE.md`.

**G. Khép câu chuyện:** Giải quyết câu hỏi đã hứa, các số phận/hậu quả thiết yếu và điều thay đổi; chọn dư âm tự nhiên từ sự kiện, không giảng đạo hoặc bắt buộc biểu tượng đối xứng.

**H. Tự kiểm độc lập:** Chạy `QUALITY_GATES.md`, thử nghe theo `AUDIENCE_SIMULATION.md`, ghi lỗi có vị trí, phân mức: blocking/major/minor. Khi cần chấm, đánh giá biên kịch và khán giả phổ thông riêng biệt, không nâng điểm theo phiên bản.

**I. Giao hàng:** Mặc định (1) **TOÀN VĂN AI VOICE** sạch, đọc được ngay; (2) **KHÔNG ĐỌC BẰNG AI VOICE**: nguồn, mức chắc chắn, điểm cần kiểm và ghi chú sản xuất; (3) báo cáo kiểm định ngắn nếu được yêu cầu. Nếu sửa bản chốt, trả lại toàn văn, giữ mọi phần không được yêu cầu đổi.

## Chốt chất lượng
- **DRAFT:** có thể còn sự kiện cần xác minh, ghi rõ.
- **READY FOR VOICE TEST:** câu chuyện đủ mạch, không còn lỗi kể chuyện nghiêm trọng, nhưng có thể chưa đạt chứng cứ xuất bản.
- **READY FOR PUBLICATION:** mọi chi tiết trọng yếu và lời trích đã được kiểm theo nguồn phù hợp, không còn blocker; chỉ dùng trạng thái này khi thực sự đã kiểm.

## Những điều cấm
Không bịa thoại, tâm lý, động cơ, tiểu tiết, hành động, diễn biến chiến trường; không trộn văn học lịch sử với xác nhận độc lập; không dùng hình AI làm chứng cứ; không viết giật cục vì muốn “viral”; không áp 3 hồi, 30 giây/twist, số chữ, số chương như luật; không giả vờ đã kiểm nguồn khi chưa kiểm; không tạo phiên bản mới chỉ để tăng điểm.

## Tài liệu đi kèm
`CHANNEL_DNA.md`, `NARRATIVE_ENGINE.md`, `EVIDENCE_GATE.md`, `HOOK_ENDING_RETENTION.md`, `VOICE_STYLE_GUIDE.md`, `AUDIENCE_SIMULATION.md`, `QUALITY_GATES.md`, `RELEASE_CHECKLIST.md`, `WORKFLOW_PROMPTS.md`, `TEMPLATES/`, `REFERENCE_SCRIPTS/`.
