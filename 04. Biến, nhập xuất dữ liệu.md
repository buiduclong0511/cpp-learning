## Biến (variable) là gì?
- Biến là thứ được dùng để lưu trữ dữ liệu của chương trình và nó mang ý nghĩa có thể thay đổi được.
- Cách sử dụng biến:
    - Trước khi sử dụng phải khai báo biến
    - Cú pháp khai báo: `<Kiểu dữ liệu> <Tên biến>;` hoặc `<Kiểu dữ liệu> <Tên biến 1>, <Tên biến 2>,...;`

    ```c
    #include <iostream>

    int main()
    {
        int i; // Khai báo biến i có kiểu dữ liệu số nguyên (integer)
        float f; // Khai báo biến f có kiểu dữ liệu số thực (float)
        char c; // Khai báo biến c có kiểu dữ liệu ký tự (character)

        int a, b; // Khai báo 2 biến a, b có kiểu dữ liệu số nguyên (integer)

        int d = 1; // Khai báo biến d và gán (assign) cho biến d giá trị 1

        std::cout << d;

        return 0;
    }
    ```
    Kết quả:
    ```
    1
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

        return 0;
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
        std::cout << "x = ";
        std::cin >> x; // Nhập vào giá trị của x

        std::cout << "Value of x: " << x; // In ra console giá trị của x

        return 0;
    }
    ```
    Kết quả:
    ```
    x = 10
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
