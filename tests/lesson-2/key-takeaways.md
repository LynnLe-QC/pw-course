# **Git**
### Các câu lệnh
1. git init - *dùng để khởi tạo git*
2. git config global user.name "name" - *dùng để cấu hình name cho 1 repo*
3. git config global user.email "email" - *dùng để cấu hình email cho 1 repo*
4. git config --global user.name "name" - *dùng để cấu hình default name cho hệ thống*
5. git config --global user.email "email" - *dùng để cấu hình default email cho hệ thống*
6. git config --list - *xem lại các cấu hình đã tạo*
7. git add<file_name> - *thêm <file_name> vào vùng Staging*
8. git add . - *thêm toàn bộ file vào vùng Staging*
9. git status - *xem trạng thái file:*
- *màu xanh (vùng staging)*
- *màu đỏ (vùng working)*
10. git commit -m "message" - *đưa file lên repostory, trong đó message là tùy chọn, dùng để quản lý phiên bản của mình*
*Quy tắc message:*
type: short_description
- *type: chore (sửa nhỏ lẻ, xóa file không dùng tới); feat (thêm tính năng hoặc testcase mới); fix (sửa lỗi test)*
- *short_description: max 50 kí tự, viết tiếng Anh hoặc tiếng Việt không dấu*
11. git log - *xem tên version, date, author của commit*

### Trình tự chạy các câu lệnh Git
1. git init
2. git config -*có thể bỏ qua nếu đã đặt git config --global trước đó*
3. git add
4. git commit
5. git push

# **Javascript**
### Đặt tên file
filename.js

### Các câu code
1. console.log("giá_trị"); - *hiển thị giá trị chuỗi hoặc của biến*
2. var tên_biến = "giá_trị" - c, có thể là data type bất kì*
3. let tên_biến = "giá_trị" - *để lưu trữ giá trị có thể thay đổi, có thể là data type bất kì* => nên dùng let hơn dùng var
4. const tên_biến = hằng_số = toán
_tử -*để lưu trữ giá trị không thể thay đổi*
5. if (điều_kiện) {//code} - *điều kiện để thực thi code*
6. for (khởi_tạo; điều_kiện_dừng; điều_kiện_tăng) {//code} -*thực thi code theo vòng lặp từ khởi_tạo đến điều_kiện_dừng theo logic của điều_kiện_tăng* 

__Code sẽ được chạy theo thứ tự từ trên xuống dưới__

### Các toán tử
1. Toán tử so sánh
- **>** - *lớn hơn*
- **<** - *nhỏ hơn*
- **==** - *bằng*
- **===** - *chưa học*
- **!=** - *khác*
- **!==** - *chưa học*
- **>=** - *lớn hơn hoặc bằng*
- **<=** - *nhỏ hơn hoặc bằng*
2. Toán tử số học
- **+** - *cộng*
- **-** - *trừ*
- **++** - *cộng thêm giống phía trên*
- **--** - *trừ thêm giống phía trên*

### Câu lệnh terminal để test code đã viết
node <path_file> -*path_file lấy bằng cách click chuột phải vào file rồi chọn Copy Path*

### Tips làm đẹp format code cho VSCode
ALt + Shift +F