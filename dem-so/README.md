# Đếm Số - Bé Vui Chơi

Hàng số 1 đến 9 ở trên cùng. Bé chạm vào một số, game đọc "Số ba", rồi
lần lượt hiện từng đồ vật (bong bóng, bông hoa, ngôi sao, quả táo, con
cá — mỗi lần chơi một loại) và đọc số đếm kèm tên: "Một bông hoa", "Hai
bông hoa", "Ba bông hoa". Cuối cùng đọc "Có ba bông hoa".

Gồm `index.html` (HTML/CSS/JS thuần) và thư mục `audio/` chứa giọng đọc
số, tên đồ vật (tạo bằng Google TTS). Hình đồ vật dùng bộ icon Twemoji
tải qua CDN jsdelivr.

Đây là một game con trong bộ game — xem cách deploy chung ở
[`../README.md`](../README.md).

## Chạy thử ngay trên máy

```bash
cd src/games/dem-so
python3 -m http.server 8000
# rồi mở http://localhost:8000
```
