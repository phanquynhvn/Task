**Tạo và chạy site trên Localhost IIS Windows Server 2019**


`  `Vào biểu tượng tìm kiếm gõ **inetmgr >> Enter** 

![ảnh](https://user-images.githubusercontent.com/101308077/158891700-134fa04a-f6ca-496b-9cd2-c6306aed2639.png)

Xuất hiện màn hình **internet information services (iis) manager**. Bấm chuột phải tại **Default Web Site >>** chọn **Explore**

![ảnh](https://user-images.githubusercontent.com/101308077/158891727-ebd48029-cd93-4d70-9427-a215a398ea95.png)

Tại thư mục **wwwroot** bấm chuột phải tạo *1 thư mục chứa Site*

![ảnh](https://user-images.githubusercontent.com/101308077/158891748-648cdbd4-c6cb-49fa-acc4-f4a11307e8e9.png)

Tạo 1 file .txt trong thư mục vừa tạo bằng cách bấm phải chuột chọn **New >>text Document**

![ảnh](https://user-images.githubusercontent.com/101308077/158891799-edae8ba3-dce2-4e65-b140-8691d97cf6af.png)

Vào **View >> File name extensions** để hiển thị phần mở rộng của file vừa tạo

![ảnh](https://user-images.githubusercontent.com/101308077/158891818-14ff8688-2759-47ae-8817-85f20076ea69.png)

Đổi tên file vừa tạo thành **index.html**

![ảnh](https://user-images.githubusercontent.com/101308077/158891842-88317f68-d1f5-4b28-893e-42af50d25885.png)

Thêm nội dung file: Chọn file và click chuột phải chọn **Open with >> Notepad** 

![ảnh](https://user-images.githubusercontent.com/101308077/158891866-bf478793-07ad-4223-b4cb-d8fe198a970b.png)

Quay lại màn hình **internet information services (iis) manager** chọn **Sites** và bấm phải chuột chọn **Add Website**

![ảnh](https://user-images.githubusercontent.com/101308077/158891890-284acee0-57dd-46a2-9b7e-23bac94807c6.png)

Xuất hiện hộp thoại:  Tại ô **Site name**: điền tên website, tại ô **Physical path** nhấn vào dấu “**…** “tìm đường dẫn đến thư mục chứa site. Điền thông tin host tại ô **Host name** 

![ảnh](https://user-images.githubusercontent.com/101308077/158892066-1d5c0a5a-bc34-4ca6-8c5a-141983409b0a.png)

Tiếp theo thêm website vào host local:

- Vào thư mục chứa file **hosts** ( Đường dẫn: *C:/Windows/System32/drivers/etc*)
- Chọn file hosts và bấm phải chuột **>> Open with** >> **Notepad** và khai báo domain đã tạo trước đó và lưu file.

![ảnh](https://user-images.githubusercontent.com/101308077/158892026-460f5695-104b-4941-bfe9-4cadcf36f2a8.png)

Mở trình duyệt *Internet Explore* chạy domain để kiểm tra tiến trình cài đặt.

![ảnh](https://user-images.githubusercontent.com/101308077/158892001-ee9e0aae-4e91-4e1f-8ad3-b2d832aa2371.png)

Màn hình báo đã thêm site thành công.
