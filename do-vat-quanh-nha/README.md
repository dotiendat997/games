# Đồ Vật Quanh Nhà - Bé Vui Chơi

Cùng cách chơi với [Chạm Vui](../cham-vui/) nhưng đổi bộ từ vựng sang
28 đồ vật quen thuộc hàng ngày (bình sữa, muỗng, bát, áo, quần, giày,
bàn chải, chìa khóa, điện thoại, ti vi, gấu bông, sách...) — phù hợp
bé đang tập nói (khoảng 15-24 tháng), vì đây là nhóm từ đầu tiên bé
thường gặp và dễ liên hệ với đồ vật thật quanh bé.

Bé chạm vào đồ vật đang bay trên màn hình, nghe gọi tên bằng tiếng
Việt kèm hiệu ứng pháo hoa vui mắt. Không có thắng/thua, không giới
hạn thời gian.

Gồm `index.html` (HTML/CSS/JS thuần) và thư mục `audio/` chứa sẵn 28
file mp3 giọng nữ đọc tên (tạo bằng Google TTS). Hình ảnh dùng bộ icon
Twemoji tải qua CDN jsdelivr, có chữ tên hiện kèm khi chạm, và tự rơi
về emoji chữ của trình duyệt nếu ảnh tải lỗi — xem chi tiết các cơ chế
này ở [`../cham-vui/README.md`](../cham-vui/README.md), vì hai game
dùng chung một khung game.

Đây là một game con trong bộ game — xem cách deploy chung ở
[`../README.md`](../README.md).

## Chạy thử ngay trên máy

```bash
cd src/games/do-vat-quanh-nha
python3 -m http.server 8000
# rồi mở http://localhost:8000
```
