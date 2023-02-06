## Biến cục bộ và biến toàn cục

1. Phạm vi cục bộ
- Trong 1 chương trình sẽ có các phạm vi (scope), mỗi 1 phạm vi sẽ được thể hiện bằng dấu `{}`.
- Biến khai báo ở phạm vi nào thì chỉ được sử dụng ở trong phạm vi đó (đó được gọi là các biến cục bộ).

    Ví dụ:
    ```cpp
    #include <iostream> 

    int main()
    {
        int main_var = 0;
        std::cout << main_var << std::endl;

        { // Phạm vi 1
            int scope_var_1 = 1;
            std::cout << scope_var_1 << std::endl;

            {
                std::cout << scope_var_1 << std::endl;
            }
        }

        { // Phạm vi 2
            int scope_var_2 = 2;
            std::cout << scope_var_2 << std::endl;
            std::cout << scope_var_1 << std::endl; // Lỗi: scope_var_1 was not declared in this scope
        }

        return 0;
    }
    ```
- Khi có 1 biến ở phạm vi bên trong trùng tên với 1 biến ở phạm vi bên ngoài, chương trình sẽ ưu tiên lấy giá trị của biến ở phạm vi gần nhất tính từ trong ra ngoài.

    Ví dụ:
    ```cpp
    #include <iostream>

    int main()
    {
        int main_var = 0;

        {
            int main_var = 1;
            std::cout << main_var; // 1
        }

        std::cout << main_var; // 0

        return 0;
    }
    ```
2. Phạm vi toàn cục
- Các biến được khai báo ở bên ngoài chương trình được gọi là biến toàn cục có thể được sử dụng ở bất cứ nơi nào trong chương trình.

    Ví dụ:
    ```cpp
    #include <iostream>

    int global_var = 1;

    int main()
    {
        std::cout << "Main scope: " << global_var << std::endl;

        { // Phạm vi 1
            std::cout << "Scope 1: " << global_var << std::endl;
        }

        { // Phạm vi 2
            std::cout << "Scope 2: " << global_var << std::endl;
        }

        return 0;
    }
    ```
