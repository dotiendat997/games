# Màu Sắc - Bé Vui Chơi

Một ô màu nhảy trên màn hình. Bé chạm vào, game đọc tên màu bằng giọng
nữ tiếng Việt (Đỏ, Cam, Vàng, Xanh lá, Xanh dương, Tím, Hồng) rồi hiện
các đồ vật có đúng màu đó (táo đỏ, cá xanh dương, bông hoa hồng...).
Không có thắng/thua.

Gồm `index.html` (HTML/CSS/JS thuần) và thư mục `audio/` chứa 7 file mp3
tên màu (tạo bằng Google TTS). Hình đồ vật dùng bộ icon Twemoji tải qua
CDN jsdelivr.

Đây là một game con trong bộ game — xem cách deploy chung ở
[`../README.md`](../README.md).

## Chạy thử ngay trên máy

```bash
cd src/games/mau-sac
python3 -m http.server 8000
# rồi mở http://localhost:8000
```
