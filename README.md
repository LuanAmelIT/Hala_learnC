Sử dụng thư viện #include <stdio.h>  thư viện giao tiếp với màn hinhd console. Tức là những giao tiếp với máy tính của mình. Trong lập trình nhúng ta không sử dụng thư viện này.

1.Biến
  + Biến gồm có các kiểu dữ liệu nguyên thủy như : Int , Float , double ....
    Dưới đây là kích thước và phạm vi giá trị của tất cả các kiểu dữ liêu:
    ![kieu du lieu](https://github.com/LuanAmelIT/Hala_learnC/assets/150274175/2c638789-0cbe-46b8-b804-03991152c42c)
    ![kieu du lieu 1](https://github.com/LuanAmelIT/Hala_learnC/assets/150274175/0812c7fa-c189-4685-97f3-659ebdba4968)


  + Trong ngành nhúng sử dụng thư viện #include <stdint.h>. Trong thư viện này có nhưng biến được định nghĩa lại VD: UInt8,UIint16,UInt32.
    Tất cả các biến nguyên thủy điều có kích thước khác nhau.
    
    
+ Vậy vì sao ngành nhúng không sử dụng kiểu dữ liêu nguyên thủy ? . Do vi điều khiển phạm vi vùng nhớ rất chi là nhỏ. Vi thế nên cần tiết kiệm phạm vi đó để hệ thống hoặt động tốt.
  Đơn cử như nếu chúng ta đọc từ cảm biến nhiệt độ LM35 về Arduino,ta chỉ cần giá trị của nó chỉ lấy 2 chữ số thập phân nếu dùng Int thì dẫn điến phí vùng dữ liệu. Giải pháp tốt nhất
  là nên chọn kiểu dữ liệu phù hợp với phạm vi của cảm biến theo manual của cảm biến và phạm vi miền dữ liệu của vi điều khiển.

+ Hàm printf dùng để in ra màm hình console.Hàm này thường đi chung với chổi định dạng nhập xuất theo C.
 
  ![chuoi_dinh_dang](https://github.com/LuanAmelIT/Hala_learnC/assets/150274175/630d869b-580e-4a48-82b1-30dd1de26ed5)
    
