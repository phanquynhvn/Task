**Tạo user trên Directadmin**

Trong bài viết hôm nay, mình sẽ hướng dẫn các bạn tạo user trên DirectAdmin.

I. Tổng quan

Ở bài viết trước, mình đã hướng dẫn các bạn [cài đặt DirectAdmin], nên trong bài này mình sẽ hướng dẫn các bạn cách để tạo một user trên DirectAdmin. Từ đó thì chúng ta mới có thể phân phối đến cho khách hàng của chúng ta và tạo được website ở trên đó.

**Lưu ý:** Để tạo user trên DirectAdmin, các bạn cần phải có quyền Admin hoặc Reseller thì mới được nhé.

II. Tạo user trên Directadmin

Để tạo user trên Directadmin chúng ta cần đi qua 3 bước sau.

Bước 1: Đăng nhập vào DirectAdmin

Đầu tiên chúng ta sẽ cần đăng nhập vào giao diện DirectAdmin với đường dẫn như sau:


http://ip:2222


Trong đó các bạn thay ip thành IP địa chỉ máy chủ DirectAdmin của các bạn. Dưới đây là giao diện đăng nhập DirectAdmin mới nhất hiện tại.

![ảnh](https://user-images.githubusercontent.com/101308077/159183579-f88510d3-b19b-40be-940f-50260a2efdcd.png)
*Giao diện đăng nhập DirectAdmin.*

Sau đó các bạn cần đăng nhập với tài khoản admin hoặc tài khoản reseller của mình.

Bước 2: Tạo user package trên DirectAdmin

Sau khi đăng nhập ở bước một xong, chúng ta tiếp tục tạo một **user package**, đây chính là các gói hosting tạo ra theo ý của các bạn.

Các bạn rê chuột vào khu vực **Account Manager** và chọn **Manage User Packages**.

![ảnh](https://user-images.githubusercontent.com/101308077/159183592-2e0878de-4f52-4dc8-9be0-67d5d7bb92e4.png)

Tại đây các bạn chọn nút Add Package như hình bên dưới.

![ảnh](https://user-images.githubusercontent.com/101308077/159183614-df5672f7-07b8-4fbb-9f66-e44ddc94377a.png)

Sau đó các bạn sẽ tùy chỉnh các thông số Package này sao cho phù hợp với nhu cầu của các bạn.

![ảnh](https://user-images.githubusercontent.com/101308077/159183621-3f7db380-3400-4404-8d83-4039c80fabfe.png)

Theo ý kiến cá nhân của mình thì những thông số các bạn nên để không giới hạn đó là:

- Bandwidth.
- Inode.
- Sub-Domains.
- MySQL Databases.
- Domain Pointers.
- FTP Accounts.

Những thông số khác các bạn cứ tùy chỉnh theo nhu cầu của các bạn nhé. Và bạn hoàn toàn có thể tạo ra nhiều gói cao thấp khác nhau để phân phối cho những phân khúc khách hàng khác nhau của mình.

Bước 3: Tạo User trên DirectAdmin với một Package

Sau khi bạn đã tạo một vài Package ở bước 2 thì chúng ta mới bắt đầu tạo user ở bước này. Các bạn cũng thao tác tương như như ở bước 2, nhưng sẽ chọn **Add New User**.

![ảnh](https://user-images.githubusercontent.com/101308077/159183626-b1544d80-4e97-44e3-832b-a829de4af1f1.png)

Sau đó các bạn cần điền một số thông tin cho user đó nữa là có thể tạo được. Các bạn nên lưu lại thông tin **Username/Password** nhé.

![ảnh](https://user-images.githubusercontent.com/101308077/159183630-450a72b7-3edd-478f-87af-4d0f43b55636.png)

Sau khi đã điền hết thông tin cần thiết, và lựa chọn User Package phù hợp, các bạn chọn **SUBMIT**.

