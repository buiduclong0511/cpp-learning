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

- Đọc/ghi dữ liệu
```c
#include <iostream>

int main()
{
    int x; // Khai báo biến x có kiểu dữ liệu số nguyên (integer)
    float y; // Khai báo biến y có kiểu dữ liệu số thực (float)
    char c; // Khai báo biến c có kiểu dữ liệu ký tự (character)

    std::cin >> x;
    std::cin >> y;
    std::cin >> c;

    std::cout << x;
    std::cout << y;
    std::cout << c;

    return 0;
}
```
## Cách đặt tên biến
- Không đặt tên biến trùng với từ khóa (void, for, while, do, delete,...)
- Tên biến không chứa khoảng trắng hoặc ký tự đặc biệt
- Ký tự đầu tiên của tên biến phải là chữ cái
