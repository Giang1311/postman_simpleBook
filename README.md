# postman_simpleBook

# Kiểm thử API với Postman

## Giới thiệu
Mục tiêu của bài tập này là thực hành kiểm thử API bằng cách sử dụng Postman. Bài tập bao gồm các bước từ việc lựa chọn một API thực tế, phân tích tài liệu API, viết các trường hợp kiểm thử, thực hiện kiểm thử và ghi lại kết quả kiểm thử.

## API Được Chọn
API được lựa chọn cho bài tập này là **Simple Books API**, một API cho phép người dùng lưu trữ sách.

## Phân Tích Tài Liệu API
Để hiểu rõ các chức năng và điểm cuối của OpenWeatherMap API, tài liệu API đã được tham khảo:
- **Điểm cuối chính**: `https://simple-books-api.glitch.me`
- 1 vài endpoint:
  - 'GET /books': Returns a list of books.
  - 'GET /books/:bookId': Retrieve detailed information about a book.
  - 'POST /orders': Allows you to submit a new order. Requires authentication.
 
## Các Trường Hợp Kiểm Thử
## Kiểm thử thành công
1. Kiểm thử lấy thông tin danh sách Books
   - Mô tả: Kiểm thử API với lấy danh sách Books với type là non-fiction.
   - **Phương thức: GET
   - Endpoint: `https://simple-books-api.glitch.me/books/`
   - Mong đợi: HTTP Status 200, thông tin về Books type non-fiction
   - ![image]![Screenshot (45)](https://github.com/Giang1311/postman_simpleBook/assets/96896545/937612f9-fe2d-41e4-9e41-d30016cc513a)
2. **Kiểm thử lấy thông tin Books bằng ID**
   - Mô tả: Kiểm thử API với ID Books hợp lệ.
   - Phương thức: GET
   - Endpoint: `https://simple-books-api.glitch.me/books/`
   - Mong đợi: HTTP Status 200, thông tin về Books cụ thể (ví dụ Book có ID là 5).
   - ![image]![Screenshot (46)](https://github.com/Giang1311/postman_simpleBook/assets/96896545/36ba776c-fd8e-4191-b527-d80c6a665a9b)
## Kiểm thử thất bại
1. Kiểm thử với Books không hợp lệ
   - Mô tả: Kiểm thử API khi sai type của Books.
   - Phương thức: GET
   - Mong đợi: HTTP Status 404, thông báo lỗi "Not Found".
   - ![image]![failed1](https://github.com/Giang1311/postman_simpleBook/assets/96896545/4e969dec-2565-45e3-b745-814469d1b7b6)
2. Kiểm thử với ID Books không hợp lệ
   - Mô tả: Kiểm thử API khi sai ID của Books.
   - Phương thức: GET
   - Mong đợi: HTTP Status 404, thông báo lỗi "Not Found".
   - ![image]![failed2](https://github.com/Giang1311/postman_simpleBook/assets/96896545/2e04fe77-49e5-46e4-bc7b-84b0ae1ac51f)


## Báo Cáo Kiểm Thử Chi Tiết

**Mục Tiêu Kiểm Thử:**
- Xác định và xác thực các phản hồi của Simple Books API dựa trên các truy vấn khác nhau.

**Phạm Vi Kiểm Thử:**
- Các điểm cuối liên quan đến việc lấy dữ liệu của các loại Book.

**Kết Quả Kiểm Thử:**
- Tất cả các trường hợp kiểm thử được thực hiện và kết quả phù hợp với mong đợi.
- API hoạt động đúng với thành phố hợp lệ và xử lý các lỗi một cách thích hợp khi cung cấp dữ liệu không hợp lệ hoặc thiếu API key.

**Khuyến Nghị:**
- API hoạt động tốt và xử lý các lỗi đúng cách. Khuyến nghị duy trì tài liệu chi tiết và cung cấp các ví dụ cụ thể để hỗ trợ người dùng API.
