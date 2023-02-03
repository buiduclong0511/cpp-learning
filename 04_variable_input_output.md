## Biến (variable) là gì?
- Biến (variable) đại diện cho **vùng nhớ** lưu trữ dữ liệu của chương trình, biến được dùng để đọc/ghi dữ liệu.
- Cách sử dụng biến:
    - Trước khi sử dụng phải khai báo biến
    - Cú pháp khai báo: `<Kiểu dữ liệu> <Tên biến>;` hoặc `<Kiểu dữ liệu> <Tên biến 1>, <Tên biến 2>,...;`

```c
#include <iostream>

int main()
{
    int x; // Khai báo biến x có kiểu dữ liệu số nguyên (integer)
    float y; // Khai báo biến y có kiểu dữ liệu số thực (float)
    char c; // Khai báo biến c có kiểu dữ liệu ký tự (character)

    return 0;
}
```

## Cách đặt tên biến
- Không đặt tên biến trùng với từ khóa (void, for, while, do, delete,...)
- Tên biến không chứa khoảng trắng hoặc ký tự đặc biệt
- Ký tự đầu tiên của tên biến phải là chữ cái

## Nhập xuất dữ liệu
- Để nhập xuất dữ liệu trong C++, chúng ta sử dụng thư viện `iostream`. Thư viện này cung cấp cho chúng ta những thứ được định nghĩa sẵn để sử dụng.
    - `std::cout`: In dữ liệu ra console
    ```c
        #include <iostream>

        int main()
        {
            std::cout << "Hello World!"; // In ra console chuỗi "Hello World!"

            return 0
        }
    ```
    Kết quả:
    ```
    Hello World!
    ```
    - `std::cin`: Đọc dữ liệu từ bàn phím và gán dữ liệu cho biến được chỉ định. Dùng cho thao tác nhập dữ liệu.
    ```c
        #include <iostream>

        int main()
        {
            int x;
            std::cout << "Type value of x: ";
            std::cin >> x; // Nhập vào giá trị của x

            std::cout << "Value of x: " << x; // In ra console giá trị của x

            return 0;
        }
    ```
    Kết quả:
    ```
    Type value of x: 10
    Value of x: 10
    ```
    - `std::endl`: Ngắt dòng khi hiển thị dữ liệu trên console, có thể dùng ký tự `\n` để thay thế.
    ```c
        #include <iostream>

        int main()
        {
            std::cout << "Hello World!" << std::endl;
            std::cout << "CPP" << std::endl << "Learing!" << std::endl;
            std::cout << "Full\nStack";

            return 0;
        }
    ```
    Kết quả:
    ```
    Hello World!
    CPP 
    Learning!
    Full 
    Stack
    ```
