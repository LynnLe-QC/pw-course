# **Git**

## Các bước thay đổi commit message
1. chạy `git commit --amend` 
2. gõ `i` - *vào chế độ insert*
3. gõ `esc` - *thoát chế độ insert*
4. gõ `:wq` - *write and quit*

hoặc chỉ chạy ` git commit --amend -m"message"` - *chỉnh sửa message mà không mở chế độ insert*

Sau khi change thì có thể chạy lệnh `git log` để check các thay đổi

## Undo commit từ Staging về Working
- chạy lệnh `git restore --staged <path_file>`
- Sau khi undo thì chạy lệnh `git status` để check hiện trạng các file

## Undo commit từ Repostory về Working
- chạy lệnh `git reset HEAD~1` - *trong đó 1 có thể thay đổi, là số lượng commit*
- Sau khi undo thì chạy lệnh `git status` để check hiện trạng các file
- Chạy lại `git log` để kiểm tra các commit

## Branching model
- Dùng để config các nhánh của repo
- Tạo ra vùng làm việc mới để không gây ảnh hưởng đến các vùng đang hoạt động khác
1. Chạy lệnh `git branch <ten_nhanh>` - *tạo branch mới*
2. Chạy lệnh `git checkout <ten_nhanh>` - *thực hiện copy code từ nhánh đang ở sang nhánh mới vừa tạo*

Hoặc chỉ Chạy lệnh `git checkout -b <ten_nhanh>` - *câu này là gộp của 2 câu trên*

## Git ignore
- Dùng để bỏ qua những file không muốn git theo dõi
- Đặt tên file: `.gitignore`
- Cách viết: viết vào trong file:
  - `tên file` - *format: tên folder/tên file*

  - `tên folder`

## Checkout về 1 revision
- dùng câu lệnh `git log` lấy được danh sách các commit, trong đó có dãy kí tự kiểu `070745d6c000d2a90740dcf97ee5db3f9418cc1f` - *đây là commit hash hay còn gọi là revision*
- dùng câu lệnh `git checkout <revision>` - *xem lại code của mình trong quá khứ có những gì*

# Javascript
## Convention
- Là các quy tắc code theo format cho dễ nhìn, dễ đọc
- Cách đặt tên  
  - `snake_case_now_now` - *ít khi dùng, hiện tại chưa dùng nên chưa học*
  - `kebab-case-now-now` - *hay dùng, để đặt tên file*
  - `camelCaseNowNow` - * hay dùng, để đặt tên biến*
  - `PascalCaseNowNow` - *để đặt tên class*

## Cách cộng chuỗi
let <tên biến> = <giá trị>
console.log(`${tên biến}`)

VD: let name = "Linh";
    console.log(`Tôi là ${name}`);

## Data type: Object
- dùng để lưu trữ tập hợp các giá trị vào cùng 1 biến hoặc 1 hằng số

   `let/const <tên obj> = {<thuoc tinh1>:<gia tri>,<thuoc tinh2>:<gia tri>}`

- thuoc tinh = tên biến
- giá trị = giống biến hoặc có thể là 1 object khác
- VD: let student = {
          name = "Linh",
          age = 32,
          job = Mom
       };
- Truy xuất giá trị object:
    - cách 1: console.log(`Student name: ${student.name}`};
    - cách 2: console.log(`Student name: ${student["name"]}`};

- Sửa/Thêm thuộc tính vào object:
     - Cách 1: `tên biến.thuộc tính = giá trị;`
        VD: let a = {
               name = "A",
               age = 1
            } 
            a.class = 3; - *thêm thuộc tính vào object*
     - Cách 2: `tên biến["thuộc tính"] = giá trị;` 
        VD: let a = {
               name = "A",
               age = 1
            } 
            a["class"] = 3; - *thêm thuộc tính vào object* 

- Xóa thuộc tính khỏi object:
     - `delete tên biến.thuộc tính;`
     - VD: let a = {
               name = "A",
               age = 1
            } 
            delete a.name; - *xóa thuộc tính name khỏi object*

## Data type: Array

- Là mảng các giá trị
- Có thể chứa nhiều kiểu dữ liệu
- VD: 
   - let studenArr = ["Han","Yen", "Linh"]
   - let studenArr = [{name:1,age:2},{name:2,age:3},]
- Đếm số index (phần tử): 
     `const count = studenArr.length;`
- In số số lượng phần tử:
     `console.log (count)`
- Tìm  giá trị của phần tử qua index:
     `console.log studentArr[số index])`         
- Tìm index qua giá trị:
     `console.log studentArr.indexOf("giá trị"))` - *nếu không có giá trị nào thỏa mãn thì nó trả ra -1*
     
## Toán tử logic
1. 2 vế đều đúng: `&&`
2. 1 trong 2 vế đúng: `||`
3. đảo ngược giá trị mệnh đề: `!`
4. VD:
let a = true;
let b = false;
let c = a && b;
let d = a || b;
console.log(c) - *in ra false*
consolde.log(d) - *in ra true*

## Hàm/Function
- Dùng để thực hiện 1 nhiệm vụ cụ thể
- Giúp tái sử dụng code mà không cần viết lại nhiều lần
- VD: 
   - function helloworld(){console.log("hello world!")}
helloworld(); - *in ra Helloworld, nếu không có dòng `helloworld()` thì không in ra được gì*
   - function printStundentName(studentName) {console.log(`Ten hoc vien: ${studentName}`)};
   printStudentName("Linh") - *in ra: Ten hoc vien: Linh*
   - function caculate(a, b) {
    const sum = a + b;
    return sum;
    };
    const total = caculate(5, 6);
    console.log(total); - *in ra 11*

## Function Kết hợp với array:
VD:  let studenArr = ["Han","Yen", "Linh"];
    function printArrChar(studentArr){
    for (let i=0; 1 < studentArr.length; i++) {
        console.log(studentArr[i]);
        }
        }
        printArrChar{studentArr}; - *in ra danh sách giá trị của array từ 0 đến max*    

## Object kết hợp với Const
- const không thể thay đổi được
- object không thể thay đổi toàn bộ object, nhưng có thể thay đổi thuộc tính
  VD:  const student = {“name”: “alex”, “age”: 20}
       student = {“name”: “Nagi”, “age”: 18} // lỗi
       student.name = "Nga"; // Hợp lệ
