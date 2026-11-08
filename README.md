# Vật bí ẩn trong nhà: game mở đầu MLN131, Nhóm 6

Mini game mở đầu cho phần thuyết trình *Xây dựng gia đình Việt Nam trong thời kỳ quá độ lên chủ nghĩa xã hội*. Toàn bộ game nằm trong một file `index.html`, chạy offline, không cần cài đặt hay mạng. Thời lượng khoảng 4–5 phút.

**Chơi ngay:** https://mln131-vat-bi-an.vercel.app

## Cách chạy

- **Offline:** tải repo về (Code → Download ZIP), giải nén, mở `index.html` bằng Chrome hoặc Edge.
- **Online:** mở https://mln131-vat-bi-an.vercel.app. Trang được deploy trên Vercel từ nhánh `main`, mỗi lần push lên `main` sẽ tự cập nhật.

Lần đầu bấm vào trang để trình duyệt cho phát âm thanh. Bấm **Toàn màn hình** khi chiếu.

## Luật chơi

Đoán một thứ nhà nào cũng có: remote TV, nồi cơm điện, nhóm chat gia đình, mâm cơm, sổ hộ khẩu, Tết. Gợi ý hiện dần như tin nhắn trong nhóm chat, từ khó đến dễ. Chỉ cần nói đúng vật đó là được, không cần đúng từng chữ.

Mỗi gợi ý có 15 giây. Hết giờ thì tự hiện gợi ý tiếp, hết gợi ý cuối thì tự lộ đáp án.

Ai đoán ra thì giơ tay. Đoán càng sớm thì kẹo càng nhiều:

| Lúc đoán đúng | Phần thưởng |
|---|---|
| Sau gợi ý 1 | 3 kẹo |
| Sau gợi ý 2 | 2 kẹo |
| Từ gợi ý 3 trở đi | 1 kẹo |

Màn cuối dẫn vào bài: những thứ rất quen ấy đã khác ngày xưa thế nào, và vì sao lại khác.

## Phím tắt cho người điều khiển

| Phím | Tác dụng |
|---|---|
| `Space` / `→` | Hiện gợi ý tiếp / sang vật tiếp theo |
| `Enter` | Có người đoán đúng: lộ đáp án và báo số kẹo |
| `A` | Không ai đoán ra: lộ đáp án |
| `P` | Dừng / chạy tiếp đồng hồ (hoặc bấm vào đồng hồ) |
| `E` | Mở màn sửa đồ vật |
| `M` | Bật / tắt nhạc nền |
| `F` | Toàn màn hình |

## Sửa đồ vật và gợi ý

Bấm **✏️ Sửa đồ vật** (hoặc phím `E`) ngay trong game. Ở đó có thể:

- thêm, xoá, đổi thứ tự các vật;
- sửa đáp án, các cách nói khác vẫn tính đúng;
- thêm, xoá, đổi thứ tự gợi ý (bao nhiêu gợi ý cũng được, xếp từ khó đến dễ);
- chọn emoji minh hoạ và màu chủ đạo cho từng vật (nền, khung chat, nút đổi theo màu này);
- chỉnh số giây mỗi gợi ý (0 là tắt đồng hồ) và bật/tắt tự hiện gợi ý khi hết giờ.

Bản sửa được lưu tự động **trong trình duyệt của máy đang mở**, không ảnh hưởng người khác. Muốn mang sang máy chiếu thì bấm **Xuất file** để tải `vat-bi-an.json`, rồi trên máy kia bấm **Nhập file**. **Về mặc định** để quay lại 6 vật ban đầu.

Muốn đổi bản mặc định cho mọi người thì sửa `DEFAULT_ITEMS` trong `index.html` rồi push lên `main`.

## Ghi chú kỹ thuật

- Toàn bộ game nằm trong một file `index.html`: cảnh phòng khách vẽ bằng SVG, âm thanh và nhạc nền tự tổng hợp bằng Web Audio, không cần file ngoài.
- Font Baloo 2 (SIL Open Font License 1.1) được nhúng sẵn trong file nên chạy offline vẫn đúng font.
