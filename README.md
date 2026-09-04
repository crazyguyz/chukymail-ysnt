# Chukymail YSNT — Công cụ tạo chữ ký email

Trang web tĩnh giúp nhân viên Công ty Cổ phần Yến Sào Nha Trang tự tạo chữ ký email
theo mẫu chuẩn của công ty, ngay trên trình duyệt — không cần cài đặt phần mềm.

## Dùng thử

Truy cập: https://crazyguyz.github.io/chukymail-ysnt/

## Tính năng

- Nhập: họ tên, chức danh, email, số ĐT di động, mã nhân viên
- Xem trước chữ ký trực tiếp (live preview)
- Tự chuẩn hóa số điện thoại Việt Nam: `0912 345 678`, `+84 912...`, `84912...` → `(+84) 912345678`
- Bỏ trống chức danh / SĐT → tự ẩn cụm tương ứng trên chữ ký
- Nút **Tải file .html**: lưu chữ ký thành `<mã nhân viên>.html`
- Nút **Copy HTML**: dán thẳng vào Outlook / Gmail (giữ nguyên định dạng, màu, logo)

## Cấu trúc

| File | Mô tả |
|------|-------|
| `index.html` | Trang web (1 file duy nhất, đã nhúng sẵn mẫu chữ ký + logo) |
| `signature-CTCP.html` | File mẫu chữ ký gốc (chứa placeholder `[username]`, `[job]`, `[mail]`, `[phone]`) |

## Chỉnh mẫu chữ ký

Sửa nội dung trong thẻ `<script type="text/plain" id="sigTemplate">` ở cuối file `index.html`
— đây là mẫu chữ ký gốc, giữ nguyên 4 placeholder để tool thay thế được.

## Triển khai

Đây là web tĩnh — upload toàn bộ thư mục lên bất kỳ hosting nào
(GitHub Pages, Netlify, Vercel, shared hosting...) là chạy. Không cần backend, không cần database.

---
© Công ty Cổ phần Yến Sào Nha Trang
