# Thỏ Vượt Rào

Lấy cảm hứng từ màn hình chạm ở khu vui chơi trong siêu thị: đàn thỏ đi
từ trái sang phải trên bãi cỏ. Bé dùng tay vẽ lên màn hình để tạo
đường cầu vồng — thỏ gặp đường vẽ sẽ dừng lại, "suy nghĩ" một chút rồi
tự chọn cách vượt qua: nhảy qua, chui thấp xuống dưới, hoặc lùi lại đổi
làn để tìm khe hở. Đường vẽ tự mờ dần và biến mất sau vài giây (giống
phấn màu), nên bé vẽ lại thoải mái. Không có thắng/thua.

Chỉ có 1 file `index.html` (HTML/CSS/JS thuần + Canvas, không cần cài
đặt gì). Đây là một game con trong bộ game — xem cách deploy chung ở
[`../README.md`](../README.md).

## Chạy thử ngay trên máy

```bash
cd src/games/tho-vuot-rao
python3 -m http.server 8000
# rồi mở http://localhost:8000
```

## Cách chơi

- Kéo ngón tay (hoặc chuột) trên màn hình để vẽ đường cầu vồng.
- Thỏ đi tới đường vẽ sẽ dừng lại, rồi tự nhảy qua / chui dưới / vòng
  sang làn khác — mỗi lần khác nhau, không đoán trước được.
- Đường vẽ tự mờ dần sau khoảng 6 giây rồi biến mất hẳn.
- Nút 🧹 góc trên bên trái: xóa hết đường đang vẽ ngay lập tức.
- Nút 🔊 góc trên bên phải: tắt/bật âm thanh (tiếng "bíu" khi thỏ nhảy
  và tiếng chuông nhỏ khi thỏ vượt qua thành công).

## Ghi chú kỹ thuật

- Vẽ bằng Canvas 2D, mỗi nét vẽ tô màu theo dải hue tăng dần dọc theo
  chiều dài nét → hiệu ứng cầu vồng thật (không phải màu cố định).
- Va chạm giữa thỏ và đường vẽ tính theo khoảng cách điểm, không dùng
  pixel canvas, nên chạy mượt kể cả khi vẽ nhiều.
- Hỗ trợ vẽ nhiều ngón tay cùng lúc (multi-touch) qua Pointer Events.
