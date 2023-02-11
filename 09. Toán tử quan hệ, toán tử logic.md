##  Toán tử quan hệ
- Là các phép toán để thực hiện việc so sánh: `>`, `<`, `>=`, `<=`, `==`, `!=`.
- Các phép toán này trả về giá trị boolean.

    Ví dụ:
    ```c
    #include <iostream>

    int main()
    {
        std::cout << (3 > 2) << std::endl; // 1 - true
        std::cout << (1 > 2) << std::endl; // 0 - false

        int a = 3;
        int b = 3;
        std::cout << (a == b) << std::endl; // 1 - true
        std::cout << (a != b) << std::endl; // 0 - false

        bool c = a < b;
        std::cout << c << std::endl; // 0 - false

        return 0;
    }
    ```
    Kết quả:
    ```
    1
    0
    1
    0
    0
    ```
- Lưu ý: 2 giá trị tham gia vào phép so sánh phải có cùng kiểu dữ liệu.

##  Toán tử logic
-  Các toán tử logic trong C++: `AND (&&)`, `OR (||)`, `NOT (!)`
    - AND: Nếu 2 vế đều là `true` thì kết quả trả về là `true`, các trường hợp còn lại thì trả về `false`.
    - OR: Nếu 2 vế đều là `false` thì kết quả trả về là `false`, các trường hợp còn lại thì trả về `true`.
    - NOT: Trả về giá trị phủ định.

    Ví dụ:
    ```c
    #include <iostream>

    int main()
    {
        // AND
        std::cout << (true && true) << std::endl; // 1 - true
        std::cout << (true && false) << std::endl; // 0 - false
        std::cout << (false && true) << std::endl; // 0 - false
        std::cout << (false && false) << std::endl; // 0 - false

        // OR
        std::cout << (true || true) << std::endl; // 1 - true
        std::cout << (true || false) << std::endl; // 1 - true
        std::cout << (false || true) << std::endl; // 1 - true
        std::cout << (false || false) << std::endl; // 0 - false

        // NOT
        std::cout << !true << std::endl; // 0 - false
        std::cout << !false << std::endl; // 1 - true

        return 0;
    }
    ```
- Sử dụng kết hợp với toán tử quan hệ.

    Ví dụ:
    ```c
    #include <iotream>

    int main()
    {
        int a = 1, b = 2, c = 3;

        bool d = (a < b) && (b > c); // true && false
        bool e = (a < b) || (b > c); // true || false

        std::cout << d << std::endl; // 0 - false
        std::cout << e << std::endl; // 1 - true

        return 0;
    }
    ```
