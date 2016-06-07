#**I. TÌM HIỂU VỀ MÔ HÌNH OSI VÀ TCP/IP**
##**1. MÔ HÌNH OSI**
<ul>
<li>**Mô hình OSI** (Open Systems Interconnection Reference Model) nghĩa là Mô hình tham chiếu kết nối các hệ thống mở dựa vào nguyên lý tầng cấp, lý giải một cách trừu tượng kỹ thuật kết nối truyền thông giữa các máy vi tính và thiết kế giao thức mạng giữa chúng.
 </li>
</ul> 
 <ul>
 <li>**Mục đích**: Mô hình OSI phân chia chức năng của một giao thức ra thành một chuỗi các tầng. Mỗi một tầng cấp có một đặc tính là nó chỉ sử dụng chức năng của tầng dưới nó, đồng thời cho phép tầng trên sử dụng các chức năng của mình. Một hệ thống cài đặt các giao thức bao gồm một chuỗi các tầng nói trên gọi là "chồng giao thức".
 </li>
 </ul>
 <ul>
 <li>**Ưu điểm của mô hình OSI**: Chia hoạt động thông tin mạng thành những phần nhỏ và đơn giản hơn. Chuẩn hóa các thành phần mạng để dễ dàng phát triển. Chuẩn hóa giao diện giữa các tầng. Dễ dàng truyền dữ liệu.
 </li>
 <ul>
 <ul>
 <li>Mô hình OSI là một cấu trúc phả hệ có 7 tầng, nó xác định các yêu cầu cho sự giao tiếp giữa hai máy tính. Mô hình này đã được định nghĩa bởi ISO. Mô hình cho phép tất cả các thành phần của mạng hoạt động hòa đồng, bất kể thành phần ấy do ai tạo dựng.
 <img src="http://www.vnpro.vn/wp-content/uploads/2015/11/Osi-model-jb.png">
 </li>
 </ul>
 ###**1.1 Tầng Physical**
 <ul>
 <li>Có liên quan tới việc truyền và nhận dòng cấu trúc nguyên bit trên một phương tiện vật lý.
 </li>
 </ul>
 <ul>
 <li> Thiết lập hoặc ngắt mạch kết nối điện với một môi trường truyền dẫn.
 </li>
 </ul>
 <ul>
 <li>Cung cấp các chuẩn về điện, dây cáp, tốc độ truyền. Quy định khoảng cách máy gửi và máy nhận.
 </li>
 </ul>
 ###**1.2 Tầng Datalink**
 <li>Lớp liên kết dữ liệu cung cấp khung truyền dữ liệu không có lỗi từ nút này tới nút khác trong lớp vật lý, cho phép các lớp phía trên thực hiện truyền ảo không lỗi trên liên kết. Để thực hiện việc này, lớp liên kết dữ liệu cung cấp:
</li> 
 <ul>
 <li>Thiết lập và kết thúc liên kết hợp lý giữa hai nút.
 </li>
 </ul>
 <ul>
 <li>Kiểm soát lưu lượng truy cập khung yêu cầu nút truyền "trở lại" khi không có bộ đệm khung nào.
 </li>
 </ul>
 <ul>
 <li>Truyền, nhận khung. Đặt giới hạn khung. Kiểm tra lỗi khung.
 </li>
 </ul>
 <ul>
 <li>Quản lý truy cập phương tiện: xác định khi nút "có quyền" sử dụng các phương tiện vật lý.
 </li>
 </ul>
 ###**1.3 Tầng Network**
 <ul>
 <li>Xác định chuyển hướng, vạch đường đi cho các gói tin trên mạng.
 </li>
 </ul>
 <ul>
 <li>Quyết định đường đi từ máy nguồn tới máy đích.
 </li>
 </ul>
 <ul>
 <li>Quản lý lưu lượng, định tuyến, kiểm soát sự tắc nghẽn của dữ liệu. Các giao thức:IP,IPX,RIP...
 </li>
 </ul>
 ###**1.4 Tầng Transport**
 <ul>
 <li>Xác định địa chỉ và cách thức truyền gói tin.
 </li>
 </ul>
 <ul>
 <li>Phân đoạn hệ thống giữa các máy truyền và tái lập dữ liệu máy nhận.
 </li>
 </ul>
 <ul>
 <li>Đảm bảo việc truyền thông tin là đáng tin cậy(end to end). Các giao thức: TCP,UDP,SPX
 </li>
 <ul>
 ###**1.5 Tầng Session**
 <ul>
 <li>Thiết lập, quản lí, duy trì phiên thông tin giao dịch giữa 2 hệ thống.
 </li>
 </ul>
 <ul>
 <li>Giải quyết những vấn đề về đồng bộ hóa. Sử dụng các giao thức: NFS(network file system), X-window system, ASP
 </li>
 </ul>
 ###**1.6 Tầng Presentation**
 <ul>
 <li>Phân tán và định dạng dữ liệu cho tầng ứng dụng.
 </li>
 </ul>
 <ul>
 <li>Chuyển đổi thông tin từ cú pháp của người sử dụng sang cú pháp để truyền dữ liệu.
 </li>
 </ul>
 <ul>
 <li>Định dạng dữ liệu từ lớp 7 đưa xuống, gửi đi bản sao để bên thu có thể hiểu được dữ liệu bên phát.
 </li>
 </ul>
 ###**1.7 Tầng Application**
 <ul>
 <li>Quy định giao diện người dùng và môi trường OSI.
 </li>
 </ul>
 <ul>
 <li>Cung cấp các phương tiện cho người sử dụng. Lớp đưa ra các giao thức:HTTP.FTP,SMTP,POP3,Telnet
 ##**2. Mô hình TCP/IP**
 
 
 
 
 
 
 
 
 