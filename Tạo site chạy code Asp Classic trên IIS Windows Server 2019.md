**Tạo site chạy code Asp Classic trên IIS Windows Server 2019**

Bước 1: Chọn **Add roles and features** trong *Server Manager/Dashboash*

![ảnh](https://user-images.githubusercontent.com/101308077/159037873-cb7260b5-0c58-4efe-8264-ee6e24290e62.png)

Bước 2: tích vào các hạng mục hỗ trợ ASP, ASP.NET sau đó bấm **next** và tiến hành cài đặt.

![ảnh](https://user-images.githubusercontent.com/101308077/159038362-32c50b9f-2512-4bef-8cc8-3666203c1374.png)

Bước 3: Vào đường dẫn (*C:\interpub\wwwroot*) tạo một thư mục chứa website.

![ảnh](https://user-images.githubusercontent.com/101308077/159039941-0dbcd3c6-0ecc-440f-9468-91a2704bb462.png)

Bước 4:  tạo 1 file.asp trong thư mục vừa tạo

![ảnh](https://user-images.githubusercontent.com/101308077/159040325-e10ac16f-80ee-4228-bf26-65f38d6f0855.png)

Bước 5: tạo dòng lệnh Asp hiển thị nội dung và lưu lại.

![ảnh](https://user-images.githubusercontent.com/101308077/159040774-86012835-90e1-4568-a71d-a0450f852fa9.png)

Bước 6: Tiếp theo vào trình quản trị của IIS Server **Internet Infomation Services (IIS) Manager** bằng cách bấm vào biểu tượng tìm kiếm trong thanh *task bar* gõ **inetmgr>> Enter**

![ảnh](https://user-images.githubusercontent.com/101308077/159042243-4b6452e0-fd0e-4235-94cf-49c489e78e01.png)

Bước 7: chọn **Site** và chuột phải chọn **Add Website**

![ảnh](https://user-images.githubusercontent.com/101308077/159042581-441d3c7c-54aa-409b-901d-8a4ee00cc6c5.png)

Bước 8: Tại ô **site name:** điền tên domain, Tại **Physical path** >> click vào dấu **"..."** tìm đến đường dẫn tới thư mục chứa website, Tại **Host name** điền tên host >> **OK**

![ảnh](https://user-images.githubusercontent.com/101308077/159043414-c831c481-1651-47a5-b916-500c58dbadac.png)

Bước 9: add website vừa tạo lên hosts (*C:\Windows\System32\drivers\etc\hosts*). chọn file hosts và bấm chuột phải >> **Open With >> Notepad**

![ảnh](https://user-images.githubusercontent.com/101308077/159044642-a00b1e16-8fba-4c37-847a-f0ad134d8c6c.png)

Bước 10: Khai báo domain vừa tạo 

![ảnh](https://user-images.githubusercontent.com/101308077/159045036-9e300819-9be5-4912-ab20-87f06b69b8a7.png)

Bước 11: Mở trình duyệt và kiểm tra lại tiến trình cài đặt

![ảnh](https://user-images.githubusercontent.com/101308077/159045868-aa732f8e-ad49-4be4-8ba8-ef196ca9e199.png)

Tiếp tục cài đặt SQL Server để kết nối cơ sở dữ liệu

Lưu ý: <p>- Set Permissions cho thư mục chứa website</p>
       <p>- Set Default Document cho site ví dụ index.asp.</p>




