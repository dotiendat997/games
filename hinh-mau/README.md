# Hình Và Màu - Bé Vui Chơi

Các hình học màu sắc (tròn, vuông, tam giác, chữ nhật, ngôi sao, trái tim,
hình thoi) bay lơ lửng trên màn hình. Bé chạm vào một hình, game đọc chậm
tên hình và màu, ví dụ "Hình vuông màu xanh dương", kèm hiệu ứng lấp lánh.
Không có thắng/thua.

Gồm `index.html` (HTML/CSS/JS thuần, hình vẽ bằng SVG) và thư mục `audio/`
chứa giọng đọc tên hình, tên màu (tạo bằng Google TTS).

Đây là một game con trong bộ game — xem cách deploy chung ở
[`../README.md`](../README.md).

## Chạy thử ngay trên máy

```bash
cd src/games/hinh-mau
python3 -m http.server 8000
# rồi mở http://localhost:8000
