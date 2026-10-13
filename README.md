# Bài tập: Tái cấu trúc CSS Landing Page sang SASS

## Nguồn tham khảo

Dựa trên landing page đã làm tại: https://github.com/kien335/codegym-career-landing-page

- Dùng lại phong cách đỏ/trắng, nội dung hero, các lợi ích và hai khóa học CGC JAVA / CGC PHP từ bài cũ.
- **Đây là bản triển khai lại rút gọn**, không phải bản sao pixel-perfect của toàn bộ repo cũ. Repo cũ chưa có phần thống kê riêng; bài này thêm một khối thống kê minh họa để đáp ứng đề bài mới.
- Các con số trong thống kê chỉ mô tả cấu trúc nội dung mẫu, **không phải thành tích hay số liệu vận hành của CodeGym**.
- `original-style.css`: CSS gốc từ repo đã làm, lưu để đối chiếu.

## Các phần đã làm

1. Navigation và Header (`scss/layout/_header.scss`)
2. Sản phẩm nổi bật / khóa học (`scss/components/_cards.scss`)
3. Số liệu thống kê (`scss/components/_stats.scss`)
4. Footer (`scss/layout/_footer.scss`)

## Kỹ thuật SASS

- Variables: `scss/abstracts/_variables.scss`
- Mixins: `scss/abstracts/_mixins.scss` (container, card-surface, on-mobile)
- Nesting: selectors trong các partials
- Partials và `@use`: `scss/main.scss`
- Responsive: media query bằng mixin `on-mobile`

## Cách chạy

Cài Sass CLI một lần: `npm.cmd install -g sass`

Trên Windows PowerShell, tại thư mục dự án:

```powershell
sass.cmd scss/main.scss style.css
```

Nếu muốn CSS tự cập nhật khi sửa SCSS:

```powershell
sass.cmd scss/main.scss style.css --watch
```

Mở `index.html` bằng trình duyệt. Đã kèm `style.css` đầu ra để chạy ngay cả khi chưa có Sass trên thiết bị.

## Nộp bài

Đưa `index.html`, `scss/`, `style.css`, `original-style.css`, `README.md` lên GitHub và dán link repository vào CodeGym.
