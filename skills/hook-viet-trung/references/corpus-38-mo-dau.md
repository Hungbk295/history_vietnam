# Corpus 38 phần mở đầu — dữ liệu gốc của skill hook-viet-trung

## 1. Cách lấy mẫu (FACT)
- Nguồn danh sách: `writer-room-data/spy/spy.sqlite`, bảng `video_snapshots`; nhãn Việt–Trung bằng từ khoá tiêu đề (có nhiễu).
- Lọc: video ≥7 phút, ≥3.000 view, kênh ≥1.000 sub, tối đa 5 video/kênh, xếp theo view. Loại tay các video không thuộc đề (Lam Sơn 719 năm 1971, tiểu sử Càn Long/Bao Thanh Thiên, v.v.).
- Lấy ~1.000 ký tự đầu transcript qua **Writer Room Spy MCP** (`spy_videos_batch`, include transcript). Transcript phần lớn là phụ đề tự động (có lỗi chính tả), 5/38 là phụ đề thủ công.
- 1 mẫu (`3SWv8Y1iAPg`, 3 làng Thanh Hoá 1886) ngoài đề Việt–Trung (đối thủ là Pháp); giữ vì là hook mẫu của kênh LSNT.
- **Giới hạn:** một người gán nhãn (model), chưa chấm chéo; chỉ đọc ~150 chữ đầu mỗi video; 38 mẫu trên 12 kênh; thiên về video nổi. Không có số liệu giữ chân (retention) hay CTR.

## 2. Cờ nhãn
`G` chào/đăng ký/ru ngủ trước cảnh đầu · `L` có từ mang lập trường trong phần mở (giặc, bọn chúng, kẻ thù, xâm lược, tàn bạo…) · `D` có ngày/năm cụ thể trong ~50 chữ đầu · `F` câu đầu là cảnh/hành động/vật cụ thể · `S` nói rõ nhãn nguồn/dã sử trong phần mở · `T` dùng ngôi "tôi" · `Q` câu hỏi nêu rõ trong phần mở.

## 3. Số đếm (n = 38)
| Đặc điểm | Số hook |
|---|---:|
| `D` ngày/năm trong ~50 chữ đầu | 20 |
| `L` từ mang lập trường | 18 |
| `Q` câu hỏi nêu rõ trong phần mở | 15 |
| `F` câu đầu là cảnh/hành động/vật cụ thể | 13 |
| `G` chào/đăng ký/ru ngủ trước cảnh đầu | 9 |
| `S` nhãn nguồn/dã sử nói rõ | 6 |
| `T` ngôi "tôi" | 4 |
| Thoại tái hiện kiểu phim (Mọt Sử, Việt Sử Kiêu Hùng) | 7 |
| Bài thơ/trích dẫn mở đầu | 2 |
| Recap bối cảnh triều đại làm phần mở (thêm 2 hook sau bài thơ) | 3 |

**Quan sát lệch kênh (KHÔNG phải luật):** 9 hook có `F` mà không `G` và không `L` có view/sub trung vị ≈12,3; 9 hook có `G` có trung vị ≈0,7. Nhưng nhóm đầu gần như toàn kênh nhỏ (view/sub vốn cao ở kênh nhỏ) và nhóm sau gồm 5 video của một kênh 51,8k sub. Cỡ kênh là biến gây nhiễu; skill không dựa vào con số này để xếp công thức.

**Bốn hook của Lịch Sử Ngoại Truyện trong mẫu** (view/sub 7,9–15,8 trên kênh ~5,1k sub): cả bốn có `D`, `F`, `Q`, không `G`, không `L`; một nói rõ nhãn nguồn (`S`). Đây là lý do bốn hình dạng A/B/C/D của Framework được giữ làm khung.

## 4. Bảng nhãn (nguyên văn từng đoạn: `corpus-38-nguyen-van.md`, cùng số thứ tự #)
| # | videoId | Kênh | Sub | View | View/sub | Dạng mở chính | Cờ |
|---|---|---|---:|---:|---:|---|---|
| 1 | `dWOqP_OgEsI` | Dòng Chảy | 99.7k | 2202.9k | 22.1 | tuyên ngôn hào hùng | L |
| 2 | `mI5INEpqLLw` | Dòng Chảy | 99.7k | 1700.3k | 17.1 | thơ trích + bối cảnh | LD |
| 3 | `bgr7SmnD1PY` | Dòng Chảy | 99.7k | 1570.8k | 15.8 | tuyên ngôn hào hùng | L |
| 4 | `ozaxTFM1ZGA` | Dòng Chảy | 99.7k | 1245.7k | 12.5 | cảnh có ngày + số | LDF |
| 5 | `bgcblhyYPBw` | Dòng Chảy | 99.7k | 604.6k | 6.1 | bối cảnh/recap | LD |
| 6 | `7y3fPCx1PgU` | Việt Sử Kiêu Hùng | 83.1k | 174.9k | 2.1 | thoại tái hiện (phim) | L |
| 7 | `Ye1ek1ideN0` | Hồn Thiêng | 30.3k | 119.7k | 4.0 | thơ trích + bối cảnh | LD |
| 8 | `IXoDgMQRdHc` | Nghe Sử | 1.2k | 111.9k | 91.0 | chào/đăng ký + câu hỏi nghịch lý | GLQ |
| 9 | `cszdx1e8OC4` | Lắng Sử | 31.7k | 85.4k | 2.7 | vật + dã sử có nhãn | FS |
| 10 | `juShm65-AxI` | LSNT | 5.1k | 80.8k | 15.8 | nghịch lý hai vế + số + hai nguồn | DFSQ |
| 11 | `oBTzJan3_no` | Lắng Sử | 31.7k | 75.1k | 2.4 | "bạn hãy hình dung" + cảnh | D |
| 12 | `mrY4_t8imck` | Mọt Sử | 7.3k | 73.2k | 10.0 | thoại tái hiện (phim) | – |
| 13 | `j2caV3ZspUE` | LSNT | 5.1k | 70.0k | 13.7 | nghịch lý hai vế + vật | DFQ |
| 14 | `zf8KTqAjxdg` | LSNT | 5.1k | 62.9k | 12.3 | vật cận cảnh có ngày + số | DFQ |
| 15 | `63ra1DsDgWI` | Sử Việt Dễ Hiểu | 10.5k | 58.4k | 5.6 | cảnh có ngày (có chi tiết dựng thêm) + chào/đăng ký | DFG |
| 16 | `p0rB0VRq4sU` | Sử Ký Nước Nam | 1.3k | 53.2k | 41.2 | vật/cảnh trục + hai lớp sử liệu/truyền thuyết | FST |
| 17 | `TX70w0ZsZEQ` | Mọt Sử | 7.3k | 44.1k | 6.1 | thoại tái hiện (phim) | L |
| 18 | `sdvrX6wqzXo` | Việt Sử Kiêu Hùng | 83.1k | 41.7k | 0.5 | thoại tái hiện (phim) | L |
| 19 | `3SWv8Y1iAPg` | LSNT | 5.1k | 40.4k | 7.9 | cảnh có ngày + số đối cặp (ngoài đề Việt–Trung) | DFQ |
| 20 | `YbnNzhbSFlM` | Sử Việt | 51.8k | 33.1k | 0.6 | chào/ru ngủ + bối cảnh có ngày | GLD |
| 21 | `w4Id6ePjURI` | Sử Ký Nước Nam | 1.3k | 32.7k | 25.3 | "bạn hãy hình dung" + cảnh có ngày | DFTQ |
| 22 | `vDlDBoPQMMw` | Mọt Sử | 7.3k | 31.3k | 4.3 | thoại tái hiện (phim) | D |
| 23 | `uZuWu-kv2Jc` | Sử Việt | 51.8k | 30.9k | 0.6 | chào/ru ngủ + cảnh có ngày | GDFQ |
| 24 | `uktLQ-m1psk` | Mọt Sử | 7.3k | 28.9k | 4.0 | thoại tái hiện (phim) | L |
| 25 | `wtzcOlcPq2g` | Mọt Sử | 7.3k | 28.0k | 3.8 | thoại tái hiện (phim) | – |
| 26 | `vsktxwp5sDE` | Lắng Sử | 31.7k | 21.0k | 0.7 | chào + "hãy tưởng tượng" + so sánh đại chúng | GL |
| 27 | `Q_M4NwD22es` | Sử Ký Oai Hùng | 7.6k | 18.7k | 2.5 | bối cảnh/recap | LD |
| 28 | `cm0SjsXE3tE` | Sử Việt | 51.8k | 17.6k | 0.3 | chào/ru ngủ + giới thiệu nhân vật | G |
| 29 | `BXbkOVJLJlc` | Sử Ký Nước Nam | 1.3k | 14.1k | 10.9 | nghịch lý + nguồn chép ít | DSTQ |
| 30 | `Lc72eLQFOCA` | Sử Việt Dễ Hiểu | 10.5k | 14.0k | 1.3 | câu hỏi tiêu đề + cảnh có ngày | DFQ |
| 31 | `XmQUQgpWBYE` | Sử Việt | 51.8k | 14.0k | 0.3 | chào/ru ngủ + câu hỏi | GLQ |
| 32 | `KBAm_R5EZ-g` | Sử Ký Nước Nam | 1.3k | 13.6k | 10.5 | cảnh có ngày + vật + "câu trả lời ngắn bỏ sót" | DFQ |
| 33 | `9zEkxo_qTq0` | Sử Việt | 51.8k | 12.5k | 0.2 | chào/ru ngủ + bối cảnh | GL |
| 34 | `1cnN0E7iJAI` | Sử Ký Oai Hùng | 7.6k | 11.2k | 1.5 | bối cảnh/ẩn dụ bàn cờ | L |
| 35 | `yMA92Eq_3a8` | Nghe Sử | 1.2k | 11.1k | 9.0 | chào/đăng ký + câu hỏi tổng quát | GQ |
| 36 | `QH15LeBMiHs` | Sử Việt Bí Ẩn | 1.6k | 7.2k | 4.4 | hình ảnh sốc + nhãn nguồn + mục lục câu hỏi | FSLQ |
| 37 | `QrKK7Ex-Nxk` | Sử Việt Dễ Hiểu | 10.5k | 6.8k | 0.6 | nghịch lý + câu hỏi | DQ |
| 38 | `IZTtbnn4_LE` | Sử Ký Nước Nam | 1.3k | 12.3k | 9.5 | số đối cặp + nhãn nguồn hai bên | DSTQ |

Ghi chú các giá trị: `Dòng Chảy` = Dòng Chảy Sử Việt; `LSNT` = Lịch Sử Ngoại Truyện; `Hồn Thiêng` = Hồn Thiêng Sử Việt. View, sub tại thời điểm quét 2026-10 (`spy.sqlite`).
