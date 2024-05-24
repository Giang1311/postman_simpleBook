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
  

