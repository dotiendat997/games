# Chạm Vui - Bé Vui Chơi

Game siêu đơn giản cho bé 1-3 tuổi: chạm vào con vật/hoa quả/hình khối
đang bay trên màn hình, bé sẽ nghe gọi tên bằng tiếng Việt kèm hiệu ứng
pháo hoa vui mắt. Không có thắng/thua, không giới hạn thời gian.

Chỉ có 1 file `index.html` (HTML/CSS/JS thuần, không cần cài đặt gì).
Đây là một game con trong bộ game — xem cách deploy chung ở
[`../README.md`](../README.md).

## Chạy thử ngay trên máy

Mở thẳng file `index.html` bằng trình duyệt, hoặc chạy một server tĩnh
nhỏ (để giọng nói/âm thanh hoạt động ổn định hơn trên một số trình duyệt):

```bash
cd src/games/cham-vui
python3 -m http.server 8000
# rồi mở http://localhost:8000
```

## Ghi chú

- Giọng đọc tên (tiếng Việt) dùng Web Speech API của trình duyệt —
  máy/trình duyệt nào không có giọng vi-VN thì sẽ tự động im lặng phần
  đó, phần chạm/âm thanh chuông vẫn hoạt động bình thường.
- Có nút loa ở góc trên bên phải để tắt/bật âm thanh.
- Không cần internet sau khi tải trang xong (không phụ thuộc thư viện
  ngoài, không cần ảnh/âm thanh tải riêng).
