# cyborgx0x.github.io

Trang cá nhân và blog công khai của cyborgx0x, phục vụ ngay tại địa chỉ gốc
**https://cyborgx0x.github.io/**. Trang được dựng bằng
[Hugo](https://gohugo.io/) với theme [PaperMod](https://github.com/adityatelange/hugo-PaperMod),
xuất bản qua GitHub Pages bằng GitHub Actions.

Đây là "nhà mới" của blog: toàn bộ nội dung trước đây nằm ở repo `cyborgx0x/blog`
(phục vụ tại đường dẫn con `/blog/`) đã được chuyển về đây để chính blog trở thành
trang chủ ở địa chỉ gốc.

## Nguyên tắc nội dung (quan trọng)

Nội dung ở đây được sao chép có chọn lọc từ một vault ghi chú cá nhân riêng tư.
Chỉ mang sang những bài thuộc khu vực tri thức tham khảo (Areas / Resources), và
**bắt buộc làm sạch mọi ngữ cảnh cá nhân** trước khi công khai:

- Không nhắc tới hoàn cảnh, sự việc hay quyết định cá nhân của tác giả.
- Không để lại liên kết tới ghi chú riêng tư (journal, dự án, tài chính...).
- Không xưng hô kiểu tư vấn cá nhân; trình bày dưới dạng tri thức khách quan.
- Giữ nguyên phần nguồn tham khảo học thuật để bảo đảm độ tin cậy.

## Cấu trúc

- `content/posts/` — các bài viết.
- `content/about.md` — trang giới thiệu.
- `content/search.md` — trang tìm kiếm (dùng index JSON của PaperMod).
- `hugo.toml` — cấu hình site (`baseURL` trỏ về địa chỉ gốc).
- `themes/PaperMod` — theme, dạng git submodule.
- `.github/workflows/hugo.yml` — build và deploy tự động khi push lên `main`.

## Chạy thử cục bộ

```bash
git clone --recurse-submodules <repo-url>
cd cyborgx0x.github.io
hugo server -D
```

Mở http://localhost:1313/.

## Thêm bài viết mới

```bash
hugo new posts/ten-bai-viet.md
```

Sửa nội dung, đặt `draft: false` (hoặc bỏ dòng `draft`), rồi push lên `main`.
GitHub Actions sẽ tự build và xuất bản.

## Kích hoạt GitHub Pages (làm một lần)

Trong repo trên GitHub: **Settings → Pages → Build and deployment → Source**
chọn **GitHub Actions**. Sau đó mỗi lần push lên `main` sẽ tự deploy.
