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
3. Tóa tử chia dư(%)
*dùng để trả về phần dư của phép tính*
VD: 3%3 =0 hay 3%2 = 1
dùng trong ứng dụng:
- Tìm số chẵn: x%2 = 0
- Tìm số lẻ: x%2 = 1

### In kết hợp
1. In kết hợp giá trị chuỗi và biến 
- **console.log("message")** - *in giá trị kiểu chuỗi*
- **console.log(<variable_name>")** -*in giá trị của biến*
- **console.log("message:"+<variable_name>")** - *kết hợp*
- **console.log("message:",<variable_name>")** - *kết hợp*
2. Nối chuỗi với toán tử (+)
  **console.log(bieesn1 + biến2)**
  VD: const s1 = "H"
      const s2 = "M"
      console.log(s1+s2)  => in ra: "HM"


### Câu lệnh terminal để test code đã viết
node <path_file> -*path_file lấy bằng cách click chuột phải vào file rồi chọn Copy Path*

### Tips làm đẹp format code cho VSCode
ALt + Shift +F

# **File markdown**
1. Tên file
- filename.md
- Dùng để định dạng văn bản
2. Tiêu đề
- Dùng #, ##, ### + tiêu đề
- Càng nhiều dấu # thì tiêu đề càng nhỏ
3. Chữ in đậm
- Cách 1: Thêm ** + text + **
- Cách 2: Thêm __ + text + __
4. Chữ in nghiêng
- Cách 1: Thêm * + text + *
- Cách 2: Thêm _ + text + _
5. Danh sách
- Hiển thị danh sách có thứ tự: 
      1. mục 1
      2. mục 2
- Hiển thị danh sách không có thứ tự:
    - mục a
    - mục b
6. Chèn liên kết
   [text](link)  
7. Chèn hình ảnh
   ![text](link)

