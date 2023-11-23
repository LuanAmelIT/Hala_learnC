Sử dụng thư viện #include <stdio.h> // thư viện giao tiếp với màn hinhd console. Tức là những giao tiếp với máy tính của mình. Trong lập trình nhúng ta không sử dụng thư viện này.
1.Biến
  + Biến gồm có các kiểu dữ liệu nguyên thủy như : Int , Float , double ....
  + Trong ngành nhúng sử dụng thư viện #include <stdint.h>. Trong thư viện này có nhưng biến được định nghĩa lại VD: UInt8,UIint16,UInt32.
    Tất cả các biến nguyên thủy điều có kích thước khác nhau.
    Char 1 byte	-128 tới 127 hoặc 0 tới 255.
    Unsigned char	1 byte	0 tới 255.
    Signed char	1 byte	-128 tới 127.
    Int	2 hoặc 4 bytes	-32,768 tới 32,767 hoặc -2,147,483,648 tới 2,147,483,647.
    Unsigned int	2 hoặc 4 bytes	0 tới 65,535 hoặc 0 tới 4,294,967,295.
    Short	2 bytes	-32,768 tới 32,767.
    Unsigned short	2 bytes	0 tới 65,535.
    long	4 bytes	-2,147,483,648 tới 2,147,483,647.
    Unsigned long	4 bytes	0 tới 4,294,967,295.
    ...
+ Vậy vì sao ngành nhúng không sử dụng kiểu dữ liêu nguyên thủy ? . Do vi điều khiển phạm vi vùng nhớ rất chi là nhỏ. Vi thế nên cần tiết kiệm phạm vi đó để hệ thống hoặt động tốt.
  Đơn cử như nếu chúng ta đọc từ cảm biến nhiệt độ LM35 về Arduino,ta chỉ cần giá trị của nó chỉ lấy 2 chữ số thập phân nếu dùng Int thì dẫn điến phí vùng dữ liệu. Giải pháp tốt nhất
  là nên chọn kiểu dữ liệu phù hợp với phạm vi của cảm biến theo manual của cảm biến và phạm vi miền dữ liệu của vi điều khiển.

+ Hàm printf dùng để in ra màm hình console.Hàm này thường đi chung với chổi định dạng nhập xuất theo C.
  %c	char	Xuất ra một ký tự
  %s	char *	Xuất ra một chuỗi ký tự
  ![chuoi_dinh_dang](https://github.com/LuanAmelIT/Hala_learnC/assets/150274175/630d869b-580e-4a48-82b1-30dd1de26ed5)
    
