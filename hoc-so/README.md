# Học Số - Bé Vui Chơi

Bé chạm vào một số từ 1 đến 9: số to hiện giữa màn hình, game đọc tên
số bằng giọng nữ tiếng Việt ("Ba"...), rồi lần lượt hiện đúng số lượng
đồ vật (táo, sao, bóng bay, hoa) kèm tiếng "tách" nhẹ, giúp bé gắn số
với số lượng thật. Không có thắng/thua.

Gồm `index.html` (HTML/CSS/JS thuần) và thư mục `audio/` chứa 9 file mp3
đọc tên số (tạo bằng Google TTS). Hình đồ vật dùng bộ icon Twemoji tải
qua CDN jsdelivr.

Đây là một game con trong bộ game — xem cách deploy chung ở
[`../README.md`](../README.md).

## Chạy thử ngay trên máy

```bash
cd src/games/hoc-so
python3 -m http.server 8000
# rồi mở http://localhost:8000
```
