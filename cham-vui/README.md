# Chạm Vui - Bé Vui Chơi

Game siêu đơn giản cho bé 1-3 tuổi: chạm vào con vật/hoa quả/hình khối
đang bay trên màn hình, bé sẽ nghe gọi tên bằng tiếng Việt kèm hiệu ứng
pháo hoa vui mắt. Không có thắng/thua, không giới hạn thời gian.

Chỉ có `index.html` (HTML/CSS/JS thuần, không cần cài đặt gì) và một
thư mục `audio/` chứa sẵn 30 file mp3 giọng nữ đọc tên từng con vật/đồ
vật (tạo bằng Google TTS). Đây là một game con trong bộ game — xem
cách deploy chung ở [`../README.md`](../README.md).

## Chạy thử ngay trên máy

Mở thẳng file `index.html` bằng trình duyệt, hoặc chạy một server tĩnh
nhỏ (để giọng nói/âm thanh hoạt động ổn định hơn trên một số trình duyệt):

```bash
cd src/games/cham-vui
python3 -m http.server 8000
# rồi mở http://localhost:8000
```

## Ghi chú

- Giọng đọc tên là file mp3 thu sẵn (giọng nữ, phát âm chuẩn) trong
  `audio/`, nên nghe giống nhau trên mọi trình duyệt/thiết bị — không
  phụ thuộc trình duyệt có hỗ trợ đọc giọng nói hay không (Web Speech
  API của trình duyệt/OS thường chất lượng thấp, thậm chí im lặng trên
  một số trình duyệt như Brave/Edge trên Linux).
- Nếu vì lý do nào đó file mp3 không phát được, game tự động rơi về
  đọc bằng Web Speech API của trình duyệt (nếu có) như phương án dự phòng.
- Mỗi lần chạm cũng hiện chữ tên con vật/đồ vật trên màn hình, nên vẫn
  học được tên kể cả khi không nghe được âm thanh.
- Có nút loa ở góc trên bên phải để tắt/bật âm thanh.
- Hình ảnh con vật/đồ vật dùng bộ icon [Twemoji](https://github.com/twitter/twemoji)
  (CC-BY 4.0) tải qua CDN jsdelivr — chi tiết và nhất quán trên mọi máy,
  không phụ thuộc font emoji của từng hệ điều hành. Nếu tải ảnh lỗi
  (mất mạng), game tự động rơi về emoji chữ của trình duyệt.
- Cần internet lần đầu tải trang (để tải file mp3 + hình Twemoji); sau
  đó trình duyệt cache lại, không cần internet nữa.
