## Các kiểu dữ liệu thường gặp
- Các kiểu dữ liệu thường gặp trong C++: 
    - Integer (int): Kiểu số nguyên (`1`, `2`, `3`)
    - Float (float): Kiểu số thực (`1.2`, `1.3`, `3.14`,...)
    - Double (double): Kiểu số thực (có giới hạn lưu trữ lớn hơn so với float)
    - Boolean (bool): 1/0 (True/False)
    - Character (char): Kiểu ký tự (`'a'`, `'b'`, `'c'`,...)
- Ngoài ra còn có các kiểu dữ liệu khác: `long`, `long long`, `unsigned long`, `short`, `unsigned short`,...

    ```c
    #include <iostream>

    int main()
    {
        int a = 1;
        
        float b = 1.4;
        
        double c = 3.14;
        
        char d = 'a';
        
        bool e = true;
        bool f = 1;

        return 0;
    }
    ```

## Giới hạn lưu trữ
- Ngoài việc lưu trữ các loại dữ liệu khác nhau, mỗi kiểu dữ liệu lại có các giới hạn lưu trữ khác nhau

    Ví dụ:
    - Kiểu `int` có thể lưu trữ 4 byte (-2,147,483,648 tới 2,147,483,647)
    - Kiểu `short` có thể lưu trữ 2 byte (-32,768 tới 32,767)
- Sử dụng các macro sau đây để kiểm tra giá trị lớn nhất hoặc nhỏ nhất mà 1 kiểu dữ liệu có thể lưu trữ
    - `INT_MAX`: Giá trị lớn nhất mà kiểu `int` có thể lưu trữ.
    - `INT_MIN`: Giá trị nhỏ nhất mà kiểu `int` có thể lưu trữ.
    - `SHRT_MAX`: Giá trị nhất mà kiểu `short` có thể lưu trữ.
    - `SHRT_MIN`: Giá trị nhỏ nh mà kiểu `short` có thể lưu trữ.
    - `LONG_MAX`: Giá trị nhất mà kiểu `long` có thể lưu trữ.
    - `LONG_MIN`: Giá trị nhỏ nh mà kiểu `long` có thể lưu trữ.
    - `FLT_MAX`: Giá trị nhất mà kiểu `float` có thể lưu trữ.
    - `FLT_MIN`: Giá trị nhỏ nh mà kiểu `float` có thể lưu trữ.
    - `DBL_MAX`: Giá trị nhất mà kiểu `double` có thể lưu trữ.
    - `DBL_MIN`: Giá trị nhỏ nh mà kiểu `double` có thể lưu trữ.

    Ví dụ:
    ```c
    #include <iostream>

    int main()
    {
        std::cout << "Min int: " << INT_MIN << std::endl;
        std::cout << "Max int: " << INT_MAX << std::endl;
        std::cout << "Min short: " << SHRT_MIN << std::endl;
        std::cout << "Max short: " << SHRT_MAX << std::endl;

        return 0;
    }
    ```
- Sử dụng `sizeof` để xác định số lượng byte mà một kiểu dữ liệu có thể lưu trữ

    Ví dụ:
    ```c
    #include <iostream>

    int main()
    {
        std::cout << "Int: " << sizeof(int) << std::endl; // 4
        std::cout << "Float: " << sizeof(float) << std::endl; // 4
        std::cout << "Double: " << sizeof(double) << std::endl; // 8
        std::cout << "Bool: " << sizeof(bool) << std::endl; // 1
        std::cout << "Char: " << sizeof(char) << std::endl; // 1
        std::cout << "Long: " << sizeof(long) << std::endl; // 4

        return 0;
    }
    ```
