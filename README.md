# Tâm Việt – Tờ khai thuế

Mã nguồn frontend React + Vite cho nền tảng hỗ trợ lập hồ sơ kê khai thuế bất động sản.

## Chạy tại máy tính
```bash
npm install
npm run dev
```

## Build để triển khai
```bash
npm run build
npm run preview
```
Thư mục đầu ra là `dist/`.

## Triển khai và gắn tên miền
Tên thương hiệu: **Tâm Việt – Tờ khai thuế**. Tên miền dự kiến: `tamviet-tokhaithue`; cần chọn phần mở rộng `.vn`, `.com` hoặc phần mở rộng khác và đăng ký tại nhà cung cấp tên miền.

- **Vercel:** import repository, framework Vite, build command `npm run build`, output directory `dist`. Sau khi deploy, thêm tên miền trong Project → Settings → Domains và cấu hình DNS theo thông tin Vercel.
- **Netlify:** import repository, build command `npm run build`, publish directory `dist`. Sau khi deploy, thêm tên miền trong Domain management và cấu hình DNS theo Netlify.
- Đã có `vercel.json` và `netlify.toml` để hỗ trợ định tuyến SPA.

**Lưu ý:** Mã nguồn này chưa tự đăng ký tên miền, chưa mua hosting và chưa triển khai lên Internet. Cần quyền quản trị tên miền và tài khoản hosting để đưa website lên địa chỉ công khai.

## Phạm vi kỹ thuật và dữ liệu
Phiên bản hiện tại là frontend. Hồ sơ lưu trên trình duyệt bằng IndexedDB/localStorage; dữ liệu không tự đồng bộ giữa nhiều thiết bị. OCR chạy phía trình duyệt và cần tải dữ liệu ngôn ngữ khi sử dụng. Các tệp Word hiện là phiếu tổng hợp dữ liệu làm việc, không mặc nhiên là mẫu tờ khai chính thức. Trước khi kê khai/nộp thuế, cần đối chiếu biểu mẫu, căn cứ tính thuế và quy định có hiệu lực tại ngày giao dịch.
