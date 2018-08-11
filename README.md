# TGS Salt Identification
Build an algorithm that automatically and accurately identifies if a subsurface target is salt or not.

This is a contest in Kaggle's community. Total prize is 100 000 $. In this repo, we only discuss about analytics and synthetic problem 

## Mô tả:
Có một số khu vực trên trái đất với sự tích tụ một lượng lớn dầu mỏ và khí đốt cũng có một lượng muối khổng lồ nằm phía dưới bề mặt.

Nhưng thật không may mắn, để biết chính xác nơi có lượng muối lớn tốt là rất khó khăn. Hình ảnh địa chấn chuyên nghiệp vấn đòi hỏi về chuyên môn cao của các chuyên gia về khu vực muối tốt. Nhưng vẫn còn nhiều điều chủ quan và có sự biến đổi cao. Đáng báo động hơn là nó còn dẫn những nguy cơ tiềm tàng cho những giàn khoan.

Để tạo ra các hình ảnh địa chấn và kết xuất 3D chính xác nhất, TGS (công ty dữ liệu địa lý hàng đầu thế giới) hy vọng cộng đồng học máy của Kaggle sẽ có thể xây dựng một thuật toán tự động và xác định chính xác nếu mục tiêu dưới mặt là muối hay không.

## Dữ liệu:

Dữ liệu địa chấn được thu thập bằng cách sử dụng những phản xạ địa chấn. Phương pháp này đòi hỏi một nguồn năng lượng địa chấn được kiểm soát, chẳng hạn như khí nén hoặc máy rung địa chấn, và các cảm biến ghi lại sự phản xạ từ các sự rung chuyển bên dưới bề mặt. Dữ liệu được ghi lại sau đó được xử lý để tạo chế độ xem 3D về nội thất của trái đất. Phản xạ địa chấn tương tự như X-ray, sonar và echolocation.

Một hình ảnh địa chấn được tạo ra từ những hình ảnh phản xạ của sự rung chuyển vật chất. Những hình ảnh địa chấn cho thấy ranh giới khác nhau giữa những loại chuyển động vật chất. Về lý thuyết, sức mạnh của sự phản chiếu tỷ lệ thuận với sự khác biệt về tính chất vật lý giữa các bề mặt. Trong khi hình ảnh địa chấn cho thấy ranh giới cũng như giới hạn của sự rung chuyển, họ không nói nhiều về những sự chuyển động vật chất; một số loại rung chuyển vật chất dễ xác định trong khi một số thì khó.

Có một vài khu vực trên thế giới có lượng muối lớn dưới bề mặt. Một trong những thách thức của hình ảnh địa chấn là xác định muối ở bên dưới bề mặt. Mật độ của muối luôn là 2.14 g/cc thấp hơn so với vật chất xung quanh. Vận tốc địa chấn của muối là 4,5 km/s, thường nhanh hơn các loại đá xung quanh. Sự khác biệt này tạo ra một sự phản chiếu sắc nét tại giao diện trầm tích muối. Thông thường muối là một loại chất rắn vô định hình không có nhiều cấu trúc bên trong. Điều này có nghĩa rằng thường không có nhiều phản xạ bên trong muối, trừ khi có những trầm tích bị mắc kẹt bên trong nó. Vận tốc địa chấn cao bất thường của muối có thể tạo ra các vấn đề với hình ảnh địa chấn.

Dữ liệu là tập hợp các hình ảnh được chọn tại các vị trí khác nhau ngẫu nhiên ở lớp dưới mặt của hình ảnh địa chấn. Các hình ảnh có kích thước 101 x 101 pixel và mỗi pixel được phân loại là muối hoặc trầm tích. Ngoài các hình ảnh địa chấn, độ sâu của vị trí được chụp ảnh được cung cấp cho mỗi hình ảnh. Mục tiêu của cuộc thi là phân khúc các khu vực có chứa muối.

![](http://pcable.com/uc/wr/motion01/comp_01-pcable_2d.jpg)
## Đánh giá
