# Kiểm tra URL giả mạo GitHub

## 1. Phân tích

- URL thật: `https://github.com/login`
- URL giả: `https://githúb.com/login`
- Ký tự lạ: **ú** thay cho **u**.
- Đây là **Homograph Attack**: dùng ký tự Unicode dễ gây nhầm lẫn để đánh cắp thông tin đăng nhập.

## 2. Quy trình kiểm tra

1. Đọc kỹ **tên miền**, chú ý chữ có dấu hoặc ký tự lạ.
2. Không nhấn liên kết từ email đáng ngờ; tự nhập `github.com`.
3. Dùng Password Manager kiểm tra tên miền trước khi tự động điền, không cố điền khi không khớp.
4. Có thể dùng công cụ chuyển tên miền Unicode sang **Punycode** để phát hiện ký tự khác thường.

**Kết luận:** Không nhập mật khẩu vào trang nghi giả mạo. Biểu tượng HTTPS không chứng minh trang web là chính chủ.
