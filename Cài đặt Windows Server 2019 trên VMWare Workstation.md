**Cài đặt Windows Server 2019 trên VMWare Workstation**

Sau khi tải về ISO Windows Server và cài đặt VMWare Workstation vào máy tính, chúng ta cùng bắt đầu quá trình cài đặt Windows Server 2019 với việc khởi động VMWare Workstation và chọn **“Create a New Virtual Machine”**

![ảnh](https://user-images.githubusercontent.com/101308077/158881462-75428816-ef13-4972-8beb-581402b7c2d1.png)

Tiếp đến, nếu bạn là người mới thao tác với VMWare Workstation thì tôi khuyến nghị lựa chọn **Typical** ở cửa sổ tiếp theo

![ảnh](https://user-images.githubusercontent.com/101308077/158881483-8ec8c1bf-46d8-45ad-9c64-d15eee998ee2.png)

Lựa chọn mục thứ 3 để thêm ISO sau cùng vì nếu như bạn thêm ISO ở bước này, hệ thống sẽ bắt chúng ta khai báo một vài thông tin về tài khoản.

![ảnh](https://user-images.githubusercontent.com/101308077/158881521-7a711039-6ef3-4c40-8ef0-b674a070d964.png)

Lựa chọn hệ điều hành cài đặt ở bước tiếp theo, ở đây tôi sẽ chọn **Microsoft** và **Windows Server 2019**  (về cơ bản 2016 và 2019 là tương tự nên không lo lắng, do tôi sử dụng version VMWare cũ nên chưa được cập nhật)

![ảnh](https://user-images.githubusercontent.com/101308077/158881561-00c05ff8-86eb-486b-bd61-7337d1a9be76.png)

Tiếp đến, chúng ta cần đặt tên cho máy ảo Windows Server 2019 để phân biệt với các máy ảo khác và nơi lưu trữ máy ảo

![ảnh](https://user-images.githubusercontent.com/101308077/158881592-7f25f53b-c49f-4674-8af9-42402b486e8c.png)

Khai báo thông số dung lượng ổ đĩa trên máy ảo khi tạo ra (mặc định sẽ là **60GB**) và lựa chọn **“Single virtual disk as a single file”**

![ảnh](https://user-images.githubusercontent.com/101308077/158881661-ce95b17c-a21e-4d40-883a-b1d376ebf728.png)

Ấn **Finish** để hoàn tất

![ảnh](https://user-images.githubusercontent.com/101308077/158881718-145c12e7-785b-4d00-836d-b7b2fb703dcd.png)

Ở màn hình mới, lựa chọn “**Customize Hardware”** để thêm ISO vào trước khi bật máy ảo

![ảnh](https://user-images.githubusercontent.com/101308077/158881743-b1bc2f80-3c64-46d1-9584-710bbde9251f.png)

Lựa chọn **CD/DVD (SATA)**, phần Use ISO image file và lựa chọn nơi lưu trữ ISO Windows Server 2019, sau đó ấn **OK** để hoàn tất.

![ảnh](https://user-images.githubusercontent.com/101308077/158881766-8370f3b6-64bf-4496-b94a-4ce00138cd49.png)

Đến bước này, khởi chạy máy ảo lên bằng việc chọn **Power on this virtual machine**

Hệ thống được khởi động, chọn ngôn ngữ và thời gian và bàn phím sau đó ấn **Next**

![ảnh](https://user-images.githubusercontent.com/101308077/158881972-1a82a8fb-b8fb-4497-a733-0d3c6bff95db.png)

Chọn **Install now**

![ảnh](https://user-images.githubusercontent.com/101308077/158881993-5a1ccd02-f95e-4a65-9ef5-f8f7a896fd78.png)

Lựa chọn hệ điều hành muốn cài đặt. Vì ở đây là cài đặt để lab nên tôi sẽ lựa chọn phiên bản cao cấp nhất **(Datacenter Evaluation có giao diện)** và ấn **Next**

![ảnh](https://user-images.githubusercontent.com/101308077/158882009-15258907-a07b-4210-b093-0dec7c10d664.png)

đồng thời đồng ý với **các điều khoản của Mcirosoft**

![ảnh](https://user-images.githubusercontent.com/101308077/158882031-f5cc54b4-f513-423b-8538-1d922178223a.png)

Lựa chọn **Custom: Install Windows only (advanced)**

![ảnh](https://user-images.githubusercontent.com/101308077/158882067-6aea40ab-f876-466b-abfc-0bdd98922645.png)

Tiếp đến lựa chọn phân vùng để bung bộ cài đặt Windows Server 2019, vì ở đây có một ổ đĩa nên tôi sẽ ấn **Next** 

![ảnh](https://user-images.githubusercontent.com/101308077/158882090-d428e1dd-fda6-47b4-9538-1bd4e17e8986.png)

Quá trình cài đặt sẽ tiếp tục diễn ra, tùy thuộc vào cấu hình của máy và ổ đĩa, thời gian sẽ diễn ra khoảng 10 phút.

![ảnh](https://user-images.githubusercontent.com/101308077/158882113-06a30d2b-b538-4044-b142-694bfe5490f2.png)

Sau khi quá trình cài đặt tự động hoàn tất và khởi động lại, bạn sẽ phải khai báo mật khẩu cho tài khoản Administrator ngay trước khi đăng nhập vào hệ điều hành (khác với Windows client sẽ có lựa chọn không cần tạo mật khẩu)

![ảnh](https://user-images.githubusercontent.com/101308077/158882150-2817ca35-d1a0-4702-b5f8-b18ccde13491.png)

Ấn **Finish** và đăng nhập vào hệ thống, sử dụng **Ctrl + Alt + Del** để unlock. Khi bạn sử dụng VMWare thì tổ hợp phím sẽ là **Ctrl + Alt + Insert**.

![ảnh](https://user-images.githubusercontent.com/101308077/158882174-90801694-c23a-4629-bf82-1f882573dfcb.png)

Màn hình hiển thị Windows Server 2019 trên VMWare.

