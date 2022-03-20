**Hướng dẫn cài đặt DirectAdmin**

Hôm nay mình sẽ hướng dẫn cài đặt DirectAdmin lên **VPS**/Server của bạn. Theo ý kiến cá nhân thì mình thấy DirectAdmin là một Control Panel rất tốt với chi phí duy trì không cao, hoạt động không chiếm nhiều tài nguyên và phù hợp chạy với các hệ thống vừa và nhỏ.

DirectAdmin là gì?

[*DirectAdmin*](https://www.directadmin.com/) là một trong rất nhiều bảng điều khiển (hay còn được gọi là Control Panel) dành cho những người quản trị Web Hosting với rất nhiều các tính năng từ cơ bản cho đến nâng cao mà bạn cần sử dụng. Tại Việt Nam DirectAdmin còn được gọi tắt là DA, DirectAdmin là một công cụ quản trị Web Hosting bản quyền và không có phiên bản miễn phí và được phát hành bởi hãn phần mềm JBMC Software. Tương thích tốt được các hệ điều hành sau:

- CloudLinux
- RedHat Enterprise / CentOS
- Debian
- FreeBSD
- Ubuntu (Sử dụng phiên bản **64-bit** dành cho Ubuntu)

Yêu cầu hệ thống khi cài đặt DirectAdmin

Tuy DirectAdmin sử dụng rất ít tài nguyên nhưng Direcadmin cũng khuyến chúng ta nên sử dụng bộ vi sử lý ít nhất là 500 Mhz và càng nhiều lõi càng tốt. Cần tối thiểu 1GB RAM (Tốt nhất nên sử dụng 2GB RAM trở lên), ít nhất 2GB SWAP. Riêng hệ thống sử dụng hệ điều hành CentOS 8 sẽ cần tối thiểu 2GB RAM (Tốt nhất nên sử dụng 4GB RAM trở lên).

Ổ cứng dung lượng trống ít nhất 2 Gigabytes  dung lượng sau khi đã cài đặt hệ điều hành. Trong trường hợp lượng truy cập của bạn cao có thể bạn sẽ cần nâng cấp thêm CPU và RAM sao cho phù hợp. Tất cả các dòng CPU Intel và AMD sẽ hoạt động tốt, CPU Solaris / Sparc sẽ không hoạt động được.

**Lưu ý:** Vui lòng không cài đặt các dịch vụ như Apache, PHP, MySQL, Ftp, Sendmail, v.v., vì trong quá trình cài đặt Directadmin sẽ làm điều này cho bạn. Tất cả những gì DirectAdmin cần là một VPS/Server cài mới hệ điều hành.
Không nên cài đặt DirectAdmin lên hệ thống đang chạy hiện tại, DirectAdmin sẽ không bảo toàn dữ liệu nếu bạn thao tác cài đè.

Hướng dẫn cài đặt DirectAdmin

Trong bài hướng dẫn cài đặt DirectAdmin này mình sẽ sử dụng một VPS chạy CentOS 7 và có CPU 5 lõi và 8GB RAM.
Để cài đặt DirectAdmin bạn cần có thông tin root của VPS/Server đồng thời dịch vụ SSH phải đang hoạt động để có thể sử dụng các lệnh cài đặt. Với VPS tại Azdigi mặc định đều SSH được sau khi cài đặt. Bạn nên tham khảo hướng dẫn sau nếu chưa nắm cách thức SSH:

Lưu ý: Để cài đặt bạn cần đăng ký bản quyền DirectAdmin cho IP thì mới có thể cài đặt được. Nếu không bạn sẽ gặp lỗi như sau khi cài đặt : Link ảnh

- Hướng dẫn đăng nhập vào VPS Linux với giao thức SSH

Trong trường hợp bạn muốn cài mới lại VPS của mình để sử dụng DirectAdmin thì có thể tham khảo hướng dẫn sau để khôi phục VPS về trạng thái như mới đăng ký:

- Hướng dẫn Reinstall lại OS khi sử dụng dịch vụ VPS tại AZDIGI

Bước 1: Cập nhật phiên bản hệ điều hành lên bản mới nhất

Bước đầu tiên trước khi cài đặt DirectAdmin bạn cần cập nhật hệ điều hành lên phiên bản mới nhất để mọi thứ hoạt động trơn tru nhất trong việc cài đặt.

Để cập nhật CentOS 7 bạn sử dụng lệnh sau:



yum update -y



Sau khi quá trình cập nhật xong và hiển thị tương tự hình sau thì chúng ta sử dụng lệnh reboot để khởi động lại VPS/Server và bắt đầu quá trình cài đặt ở bước 2.

Bước 2: Bắt đầu cài đặt DirectAdmin

Tại bước này ta sử dụng các lệnh sau để quá trình cài đặt được diễn ra:



AZDIGI Tutorial

wget -O setup.sh https://www.directadmin.com/setup.sh

chmod 755 setup.sh	

./setup.sh auto    

Giải thích các lệnh trên:

- Tải về tệp tin cài đặt
- Phân quyền tệp cài đặt vừa tải về
- Thực thi tệp cài đặt

Quá trình cài đặt diễn ra lâu hay nhanh sẽ tuỳ thuộc vào đường truyền quốc tế và hiệu năng VPS/Server của bạn. Thông thường nhanh nhất sẽ là 30 phút.

Sau khi quá trình cài đặt thành công bạn sẽ nhận được các thông tin quan trọng sau:

- Admin username: admin
- Admin password: ●●●●●●●●●●
- Admin email: admin@*hostname*
- To login now, follow this link: http://*IP*:2222

Dưới đây là hình ảnh minh hoạ:

Như vậy quá trình cài đặt DirectAdmin đã hoàn tất, bạn đã có thể truy cập vào đường dẫn quản trị DirectAdmin của mình theo dạng http://IP:2222 . Tuy nhiên bạn cần kích hoạt bản quyền DirectAdmin của mình theo bước 3 nữa nhé.

Bước 3: Kích hoạt DirectAdmin

Để kích hoạt DirectAdmin bạn chỉ cần có UID, LID và license này khớp với IP VPS/Server của bạn. Để kích hoạt ta sử dụng 3 lệnh sau:



cd /usr/local/directadmin/scripts

./getLicense.sh UID LID

service directadmin restart    

Tại đây bạn cần thay **UID** và **LID** thành số phù hợp với license DirectAdmin của bạn.

