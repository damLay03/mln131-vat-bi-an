# Vật bí ẩn trong nhà: game mở đầu MLN131, Nhóm 6

Mini game mở đầu cho phần thuyết trình *Xây dựng gia đình Việt Nam trong thời kỳ quá độ lên chủ nghĩa xã hội*. Toàn bộ game nằm trong một file `index.html`, chạy offline, không cần cài đặt hay mạng. Thời lượng khoảng 4–5 phút.

## Cách chạy

- **Offline:** tải repo về (Code → Download ZIP), giải nén, mở `index.html` bằng Chrome hoặc Edge.
- **Online:** bật GitHub Pages (Settings → Pages → Branch `main`, thư mục `/ (root)`), rồi mở link Pages.

Lần đầu bấm vào trang để trình duyệt cho phát âm thanh. Bấm **Toàn màn hình** khi chiếu.

## Luật chơi

Đoán một thứ nhà nào cũng có: remote TV, nồi cơm điện, nhóm chat gia đình, mâm cơm, sổ hộ khẩu, Tết. Mỗi vật có 4 gợi ý hiện dần từ khó đến dễ, kèm ô chữ trống cho biết số chữ cái.

Ai đoán ra thì giơ tay. Đoán càng sớm thì kẹo càng nhiều:

| Lúc đoán đúng | Phần thưởng |
|---|---|
| Sau gợi ý 1 | 3 kẹo |
| Sau gợi ý 2 | 2 kẹo |
| Sau gợi ý 3 hoặc 4 | 1 kẹo |

Màn cuối dẫn vào bài: những thứ rất quen ấy đã khác ngày xưa thế nào, và vì sao lại khác.

## Phím tắt cho người điều khiển

| Phím | Tác dụng |
|---|---|
| `Space` / `→` | Hiện gợi ý tiếp / sang vật tiếp theo |
| `Enter` | Có người đoán đúng: lộ đáp án và báo số kẹo |
| `A` | Không ai đoán ra: lộ đáp án |

## Sửa nội dung

Mở `index.html` và tìm `const ITEMS`. Mỗi vật có:

- `answer`: đáp án
- `accept`: các cách nói khác vẫn tính đúng
- `clues`: 4 gợi ý, xếp từ khó đến dễ

Số kẹo theo từng gợi ý nằm ở `PRIZE`.
