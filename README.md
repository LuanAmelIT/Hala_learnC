- Sử dụng thư viện #include <stdio.h>  thư viện giao tiếp với màn hinhd console. Tức là những giao tiếp với máy tính của mình. Trong lập trình nhúng ta không sử dụng thư viện này.
- Trong ngành nhúng sử dụng thư viện #include <stdint.h>. Trong thư viện này có nhưng biến được định nghĩa lại VD: UInt8,UIint16,UInt32.

1.Biến
  + Biến gồm có các kiểu dữ liệu nguyên thủy như : Int , Float , double ....
    Dưới đây là kích thước và phạm vi giá trị của tất cả các kiểu dữ liêu:
    ![unit8](https://github.com/LuanAmelIT/Hala_learnC/assets/150274175/97a60f65-4d2b-4911-b8d8-5a110fa91245)
    ![kieu du lieu 1](https://github.com/LuanAmelIT/Hala_learnC/assets/150274175/0812c7fa-c189-4685-97f3-659ebdba4968)
    
  + Kiểu dữ liệu Enum trong ngôn ngữ C hay còn gọi là kiểu dữ liệu cố định, kiểu liệt kê. Giá trị của một Enum chỉ có thể nhận giá trị là một số các số nguyên cho trước.
  +  Kiểu void dùng xác định không có giá trị nào (không phải là null).
  +  Kiểu dữ liệu Boolean là một kiểu dữ liệu có chỉ có thể nhận một trong hai giá trị như đúng/sai (true/false, yes/no, 1/0) nhằm đại diện cho hai giá trị thật (truth value).
  +  Kiểu dữ liệu Bool trong lập trình C, thực chất bool chính là kiểu integer (0 tức là false, khác 0 tức là true).

+ Vậy vì sao ngành nhúng không sử dụng kiểu dữ liêu nguyên thủy ? . Do vi điều khiển phạm vi vùng nhớ rất chi là nhỏ. Vi thế nên cần tiết kiệm phạm vi đó để hệ thống hoặt động tốt.
  Đơn cử như nếu chúng ta đọc từ cảm biến nhiệt độ LM35 về Arduino,ta chỉ cần giá trị của nó chỉ lấy 2 chữ số thập phân nếu dùng Int thì dẫn điến phí vùng dữ liệu. Giải pháp tốt nhất
  là nên chọn kiểu dữ liệu phù hợp với phạm vi của cảm biến theo manual của cảm biến và phạm vi miền dữ liệu của vi điều khiển.

+ Hàm printf dùng để in ra màm hình console.Hàm này thường đi chung với chổi định dạng nhập xuất theo C.
 
  ![chuoi_dinh_dang](https://github.com/LuanAmelIT/Hala_learnC/assets/150274175/630d869b-580e-4a48-82b1-30dd1de26ed5)
    
+ Để biết kích thước của 1 biến ta dùng như sau:

  
  ![TESTHAHA1](https://github.com/LuanAmelIT/Hala_learnC/assets/150274175/bbe104f2-8b20-4372-ae6e-53b85395fe8a)
+ Như vậy kích thước của biến trên là bằng 1 byte.Uint8 , Uint16, Uint32 thì nhìn vào con số sau mỗi kiểu dữ liệu ta có thể nhận biết được số Bit và Byte của kiểu dữ liệu đó, Unit chữ U có nghĩa là unsigned tức là số nguyên dương, trường hợp không có thì có phạm vi cả nguyên dương và nguyên âm để tìm phạm vi giá trị của 2 miền này thì ta chia cho 2.Việc đặt biến để sử dụng lớn hơn phạm vi giá trị của kiểu dữ liệu sẽ xảy ra hiện tượng tràn bộ nhớ và dữ liệu sẽ bị sai. Tính phạm vi giá trị bằng 2^8 hoặc 16 hoặc ....Như vậy đoií với 2^8 bằng  256 từ (0 - 255) thì sẽ có 256 ô lưu.Cũng giống như PLC , ở đây nói về PLC mitsubishi thì khi biến được đưa giá trị vào thì buffert memory sẽ lấy giá trị số đó đưa vào các ô nhớ theo dạng mã nhị phân.
  ![btplc](https://github.com/LuanAmelIT/Hala_learnC/assets/150274175/5616211c-c15a-4223-8971-a831cf6a6350)

  









  
