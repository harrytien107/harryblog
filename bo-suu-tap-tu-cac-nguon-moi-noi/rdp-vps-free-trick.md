# RDP VPS free trick

Làm cách nào để tạo Google RDP miễn phí trong 48 giờ?

Hôm nay mình sẽ hướng dẫn mọi người về cách chúng ta có thể tạo Google RDP miễn phí trong 48 giờ để sử dụng tạm thời.

Yêu cầu:

tài khoản Gmail

Trước hết, hãy truy cập

[https://console.cloud.google.com/](https://console.cloud.google.com/)

Bây giờ, ở góc trên cùng bên phải, bạn sẽ thấy biểu tượng bảng điều khiển (activate cloud shell), hãy nhấp vào biểu tượng đó.

Đợi vài giây và bạn sẽ thấy bảng điều khiển đang chạy trong trang đó.

Sau đó, dán lệnh đã cho như sau:

docker run -p 6080:80 dorowu/ubuntu-desktop-lxde-vnc

và nhấn enter.

Nó sẽ bắt đầu tải xuống một số tệp, chỉ cần đợi trong vài giây.

Sau đó, nhấp vào nút xem trước web được cung cấp trên bảng điều khiển ở góc bên phải dọc theo nút cài đặt.

Thay đổi Port thành 6080 và nhấp vào change và preview

Nó sẽ chạy RDP VPS trong tab tiếp theo.

..............

Bây giờ, hãy mở terminal (LXTerminal)

gõ lệnh sudo su

Đừng gõ mật khẩu và nhấn enter ....

Tiếp tục chạy hệ thống.

Sau đó, cloud shell mà chúng tôi đã mở bị lỗi và bạn có thể sử dụng cùng thứ đó trong 48 giờ...
