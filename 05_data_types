## Các kiểu dữ liệu thường gặp
- Các kiểu dữ liệu thường gặp trong C++: 
    - Integer (int): Kiểu số nguyên (`1`, `2`, `3`)
    - Float (float): Kiểu số thực (`1.2`, `1.3`, `3.14`,...)
    - Double (double): Kiểu số thực (có không gian lưu trữ lớn hơn so với float)
    - Boolean (bool): True/False
    - Character (char): Kiểu ký tự (`'a'`, `'b'`, `'c'`,...)
- Ngoài ra còn có các kiểu dữ liệu khác: `long`, `long long`, `unsigned long`, `short`, `unsigned short`,...

## Giới hạn lưu trữ
- Ngoài việc lưu trữ các loại dữ liệu khác nhau, mỗi kiểu dữ liệu lại có các giới hạn lưu trữ khác nhau

    Ví dụ:
    - Kiểu `int` có thể lưu trữ 4 byte (-2,147,483,648 tới 2,147,483,647)
    - Kiểu `short` có thể lưu trữ 2 byte (-32,768 tới 32,767)
- Sử dụng `sizeof` để xác định số lượng byte mà một kiểu dữ liệu có thể lưu trữ

    Ví dụ:
    ```c
    #include <iostream>

    int main()
    {
        std::cout << sizeof(int); // 4
        std::cout << sizeof(float); // 4
        std::cout << sizeof(double); // 8

        return 0;
    }
    ```
- Sử dụng các biến sau đây để kiểm tra giá trị max/min mà 1 kiểu dữ liệu có thể lưu trữ
    - `INT_MAX`: Giá trị max của kiểu `int`
    - `INT_MIN`: Giá trị min của kiểu `int`
    - `SHRT_MAX`: Giá trị max của kiểu `short`
    - `SHRT_MIN`: Giá trị min của kiểu `short`
    - `LONG_MAX`: Giá trị max của kiểu `long`
    - `LONG_MIN`: Giá trị min của kiểu `long`
    - `FLT_MAX`: Giá trị max của kiểu `float`
    - `FLT_MIN`: Giá trị min của kiểu `float`
    - `DBL_MAX`: Giá trị max của kiểu `double`
    - `DBL_MIN`: Giá trị min của kiểu `double`

    Ví dụ:
    ```c
    #include <iostream>

    int main()
    {
        std::cout << "Giá trị max của kiểu int: " << INT_MAX;

        retunr 0;
    }
    ```
