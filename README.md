# Games

Bộ game nhỏ cho con, mỗi game là một thư mục riêng, chạy được ngay bằng
HTML/CSS/JS thuần (không cần build) và deploy chung qua GitHub Pages
từ một repo duy nhất.

## Danh sách game

- [`cham-vui/`](cham-vui/) — Chạm Vui: bé chạm vào con vật/hoa quả bay
  trên màn hình, nghe gọi tên tiếng Việt. Dành cho bé 1-3 tuổi.
- [`tho-vuot-rao/`](tho-vuot-rao/) — Thỏ Vượt Rào: bé vẽ đường cầu vồng
  bằng tay để chặn đàn thỏ đang đi qua, thỏ tự tìm cách nhảy/chui/vòng
  qua đường vẽ.
- [`do-vat-quanh-nha/`](do-vat-quanh-nha/) — Đồ Vật Quanh Nhà: giống
  Chạm Vui nhưng đổi bộ từ sang đồ vật hàng ngày (bình sữa, muỗng,
  giày, bàn chải...), hợp bé đang tập nói.
- [`hoc-so/`](hoc-so/) — Học Số: chạm số 1-9, nghe tên số và thấy đúng
  số lượng đồ vật hiện ra.
- [`mau-sac/`](mau-sac/) — Màu Sắc: chạm ô màu, nghe tên màu và thấy các
  đồ vật cùng màu xuất hiện.
- [`dem-so/`](dem-so/) — Đếm Số: chạm số 1-9, game đếm từng đồ vật một
  và đọc số đếm kèm tên đồ vật.

`index.html` ở thư mục gốc là trang chọn game, link tới từng thư mục con.

## Thêm game mới

1. Tạo thư mục mới, ví dụ `src/games/ten-game-moi/`, với `index.html`
   riêng của game đó.
2. Thêm một thẻ link vào `index.html` ở gốc để game xuất hiện trong
   danh sách chọn.

## Deploy lên GitHub Pages (deploy một lần, dùng chung cho mọi game)

1. Tạo một repo mới trên GitHub (public), ví dụ đặt tên `games`.
2. Từ thư mục `src/games` này:
   ```bash
   git init
   git add .
   git commit -m "Add games collection"
   git branch -M main
   git remote add origin https://github.com/<username>/games.git
   git push -u origin main
   ```
3. Trên GitHub: vào **Settings → Pages**, mục "Build and deployment"
   chọn **Deploy from a branch**, branch **main**, folder **/ (root)** → Save.
4. Sau 1-2 phút:
   - Trang chọn game: `https://<username>.github.io/games/`
   - Game Chạm Vui: `https://<username>.github.io/games/cham-vui/`

Từ giờ mỗi khi thêm game mới, chỉ cần `git add`, `git commit`,
`git push` — không cần lặp lại bước tạo repo/bật Pages.
