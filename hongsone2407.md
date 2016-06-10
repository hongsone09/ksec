#**I.TÌM HIỂU VỀ MÔ HÌNH OSI VÀ TCP/IP**
##**1. MÔ HÌNH OSI**
<ul>
<li>Mô hình OSI(Open Systems Interconnection Reference Model) nghĩa là Mô hình tham chiếu kết nối các hệ thống mở dựa vào nguyên lý tầng cấp, lý giải một cách trừu tượng kỹ thuật kết nối truyền thông giữa các máy vi tính và thiết kế giao thức mạng giữa chúng.
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
 **1.1 Tầng Physical**
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
 **1.2 Tầng Datalink**
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
 **1.3 Tầng Network**
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
 **1.4 Tầng Transport**
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
 </ul>
 **1.5 Tầng Session**
 <ul>
 <li>Thiết lập, quản lí, duy trì phiên thông tin giao dịch giữa 2 hệ thống.
 </li>
 </ul>
 <ul>
 <li>Giải quyết những vấn đề về đồng bộ hóa. Sử dụng các giao thức: NFS(network file system), X-window system, ASP
 </li>
 </ul>
 **1.6 Tầng Presentation**
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
 **1.7 Tầng Application**
 <ul>
 <li>Quy định giao diện người dùng và môi trường OSI.
 </li>
 </ul>
 <ul>
 <li>Cung cấp các phương tiện cho người sử dụng. Lớp đưa ra các giao thức:HTTP.FTP,SMTP,POP3,Telnet
 </li>
 </ul>
 **2. Mô hình TCP/IP**
 <img src="http://www.ittraining.vn/wp-content/uploads/2016/02/mo-hinh-OSI-v%C3%A0-TCP.png">
 <ul>
 <li>TCP/IP có cấu trúc tương tự mô hình OSI,tuy nhiên để đảm bảo tính tương thích giữa các mạng và sự tin cậy của việc truyền thông tin trên mạng, bộ giao thức TCP/IP được chia thành 2 phần riêng biệt:giao thức IP sử dụng cho việc kết nối mạng và giao thức TCP để đảm bảo việc truyền dữ liệu một cách tin cậy.
 Mô hình TCP/IP gồm 4 tầng:

 </li>
 </ul>
 **2.1 Tầng ứng dụng**
 <ul>
 <li>Là nơi các chương trình mạng thường dùng làm việc nhằm liên lạc với các nút trong mạng.Giao tiếp xảy ra trong tầng này tùy theo các ứng dụng cụ thể và dữ liệu được truyền từ chương trình, trong định dạng được sử dụng nội bộ và được đóng gói theo một giao thức tầng giao vận.
 </li>
 </ul>
 **2.2 Tầng giao vận**
 <ul>
 <li>Kết hợp các khả năng truyền thông điệp trực tiếp không phụ thuộc vào mạng bên dưới,kèm theo kiểm soát lỗi, phân mảnh và điều khiển lưu lượng.
 </li>
 </ul>
 <ul>
 <li>Cung cấp dịch vụ kết nối các ứng dụng với nhau thông qua việc sử dụng các cổng TCP và UDP.
 </li>
 </ul>
 **2.3 Tầng mạng**
 <ul>
 <li>Dẫn đường cho dữ liệu từ mạng nguồn đến mạng đích. Nhiệm vụ này thường đòi hỏi việc định tuyến cho gói tin qua một mạng lưới các mạng máy tính, đó là liên mạng.
 </li>
 </ul>
 **2.4 Tầng liên kết**
 <ul>
 <li>Chuyển các gói tin từ tầng mạng tới các máy chủ khác nhau. Tầng liên kết còn có thể là tầng nơi các gói tin được chặn để gửi qua một mạng riêng ảo.
 </li>
 </ul>
 <ul>
 <li>Tầng liên kết còn có thể được xem là bao gồm cả tầng vật lý-tầng là kết hợp các thành phần mạng vật lý và các thiết bị nối mạng có liên quan và các đặc tả mức thấp về các tín hiệu.
 </li>
 </ul>
 **II.MỘT SỐ GIAO THỨC LỚP ỨNG DỤNG TRONG MÔ HÌNH TCP/IP**
 **1. Dịch vụ đăng nhập từ xa TELNET**
 <ul>
 <li>Telnet là ứng dụng sử dụng telnet cho phép người dùng có thể đăng nhập vào một hệ thống ở xa và làm việc giống như đang sư dụng nội bộ máy tính vậy. Người sử dụng dùng chương trình Telnet Client thực hiện một số kết nối TCP với một Telnet Server ở cổng 23.
 </li>
 </ul>
 **2. Dịch vụ truyền file FTP**
 <ul>
 <li>Dịch vụ truyền File là một trong những dịch vụ sớm nhất ứng dụng giao thức TCP/IP. FTP cho phép người dùng thực hiện các chức năng sao chép, đổi tên, xóa file, tạo thư mục... ở một hệ thống ở xa.
 </li>
 </ul>
 <ul>
 <li>Hệ thống FTP ở xa thường yêu cầu người dùng cung cấp định danh ID và mật khẩu trước khi truy nhập hệ thống.
 </li>
 </ul>
 <ul>
 <li>FTP sử dụng cổng TCP ở lớp Transport để truyền file một cách tin cậy.Tại FTP Server thì sẽ được gán các cổng cố định là 20,21 còn ở Client thì sẽ được gán giá trị bất kỳ lớn hơn 1023. Để có thể hoạt động FTP thiết lập 2 kết nối. Một cho login và theo đó là giao thức Telnet. Hai là cho quản lý dữ liệu.
 **3. Trivial File Transfer Protocol(TFTP)**
 <ul>
 <li>Mặc dù FTP là giao thức truyền tập tin tổng quát trong bộ giao thức TCP/IP nhưng lại rất phức tạp. Nhiều ứng dụng không cần đến tất cả các tính năng mà FTP cung cấp. Do đó người ta đưa ra một giao thức thứ hai cung cấp dịch vụ ít tốn kém và không phức tạp được gọi là TFTP.
 </li>
 </ul>
 <ul>
 <li>Giao thức này không cần đến những tương tác phức tạp giữa client và server. TFTP giới hạn thao tác chỉ trong việc truyền tập tin và không cung cấp việc xác minh. Không giống như FTP, TFTP không cần dịch vụ chuyển tin đáng tin cậy. Nó sử dụng giao thức UDP của tầng Transport có sử dụng timeout và việc truyền lại để đảm bảo dữ liệu được truyền đến nới. Bên gửi truyền một tập tin theo những khối kích thước cố định(512 byte) và đợi lời đã nhận trước khi gửi tiếp. Bên phía nhận gửi lời đã nhận được mỗi khối.
 </li>
 </ul>
 **4. Network File System(NFS)**
 <ul>
 <li>Được phát triển đầu tiên bởi công ty Sun Microsoft, hệ tập tin mạng(Network File System- NFS) cung cấp việc truy xuất trực tuyến các tập tin dùng chung. Người sử dụng có thể thực hiện một chuông trình ứng dụng bất kỳ và sử dụng bất kỳ một tập tin nào trong việc xuất nhập. Bản thân tên các tập tin không cho biết chúng cục bộ hay ở xa. NFS là một RPC(Remote Procedure Call)
 </li>
 </ul>
 **5. Simple Mail Transfer Protocol(SMTP)**
 <ul>
 <li>Giao thức SMTP là giao thức tiêu chuẩn trên Internet cho việc truyền thư điện tử giữa các máy tính. SMTP được thiết kế để chuyển giao những thông điệp text và cùng hỗ trợ những ứng dụng multimedia. SMTP thực hiện bên trên một phiên kết nối Telnet NVT.
 <img src="http://cs.lmu.edu/~ray/images/smtp.gif">
 </li>
 </ul>
 <ul>
 <li>Có hai thành phần chính trong SMTP: nơi gửi và nơi nhận. Nơi gửi được coi như là mấy khách thực hiện lập một kết nối TCP với nơi nhận đóng vai trò là máy chủ. Cổng tiêu chuẩn để thực hiện kết nối TCP là 25. Trong một phiên của SMTP, nơi gửi và nhận trao đổi một chuỗi các lệnh và trả lời.
 </li>
 </ul>
 **6. Simple Network Management Protocol(SNMP)**
 <ul>
 <li>Giao thức quản lý mạng chuẩn của TCP/IP là SNMP định nghĩa giao thức quản lý cấp để quản lý hai thao tác cơ sở: trích giá trị từ một biến và lưu trữ giá trị một biến.
 </li>
 </ul>
 **7. Domain Name Service(DNS)**
 <ul>
 <li>Đối với những người truy cập Internet, việc nhớ nhiều địa chỉ IP cùng một lúc là rất khó. Do đó các nhà thiết kế tạo nên những tên dễ nhớ như www.youtube.com, www.innisfree.com.vn,....Người dùng muốn truy cập đến địa chỉ nào thì chỉ cần gõ bàn phím tới tên đó.
 </li>
 </ul>
 <ul>
 <li>Tuy nhiên giao thức lớp mạng IP chỉ có thể hiểu và làm việc được với địa chỉ IP. Do vậy cần có sự chuyển đổi qua lại giữa tên và địa chỉ IP. Việc chuyển đổi tên thành địa chỉ được thực hiện qua hệ thống miền (Domain Name System_DNS).
 Hệ thống DNS thực chất là những cơ sở dữ liệu chứa tên và địa chỉ tương ứng cùng với các thông tin khác đi kèm.
 </li>
 </ul>
 **8. Dynamic Host Configuration Protocol(DHCP)/BootP(Bootstrap Protocol)**
 <ul>
 <li>Giao thức Bootstrap gọi là BOOTP cung cấp một cách khác với RARP cho máy tính nào cần xác định địa chỉ IP của nó. 
 </li>
 <ul>
 <ul>
 <li>BOOTP tổng quát hơn RARP vì nó sử dụng UDP nên có thể mở rộng việc bootstrap đi qua bộ định tuyến.
 </li>
 </ul>
 <ul>
 <li>BOOTP cũng cho phép máy tính xác định địa chỉ của bộ định tuyến, địa chỉ server và tên của chương trình mà máy tính phải chạy. BOOTP thiết kế đủ nhỏ và để chứa trong bootstrap ROM.
 </li>
 </ul>
 <ul>
 <li>BOOTP hiệu quả hơn RARP bởi vì thông điệp BOOTP xác định nhiều dữ liệu cần thiết vào lúc khởi động, bao gồm địa chỉ IP của máy tính, địa chỉ bộ định tuyến và địa chỉ server.
 </li>
 </ul>
 <ul>
 <li>DHCP là sự mở rộng của BOOTP. DHCP cho phép server cấp phát địa chỉ IP một cách động. Việc cấp phát động là cần thiết đối với những môi trường mạng không dây, trong đó máy tính có thể kết nối và tách ra khỏi mạng một cách nhanh chóng.
 </li>
 </ul>
 **III. MÔ HÌNH TCP/IP 5 LỚP**
 <ul>
 <li>Ngày nay đa phần các giao thức đều chạy trên chồng giao thức TCP/IP, thế nhưng trong việc học tập, giảng dạy cũng như làm việc thì luôn đối chiếu vào mô hình OSI. Chính vì thế để đáp ứng sự cần thiết của mô hình OSI cũng như rút ngắn các tầng không quan trọng lắm người ta nghĩ ra mô hình 5 lớp.
 </li>
 </ul>
 <li>Mô hình 5 lớp gồm các lớp:
 </li>
 <ul>
 <li>Application
 </li>
 </ul>
 <ul>
 <li>Transport
 </li>
 </ul>
 <ul>
 <li>Network
 </li>
 </ul>
 <ul>
 <li>Datalink
 </li>
 </ul>
 <ul>
 <li>Physical
 </li>
 </ul>
 <ul>
 <li>5 lớp này được quan tâm nhất khi cấu hình và troubleshoot hệ thống mạng
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
