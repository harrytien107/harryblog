# Google Colab

Anh em chia sẻ nội dung nhạy cảm, nội dung bản quyền hay bị soi, bị cảnh báo, bị ăn gậy thậm chí cho ngừng tài khoản. Những dự liệu này để yên thì không sao, nhưng bật share là dính đòn.

Vậy làm sao để share chúng đây. Giải pháp đưa ra là nén lại với mật khẩu, và đặt một cái tên khác đi rồi chia sẻ. Anh em nhận file rồi giải nén với mật khẩu là xem được.

Khổ nỗi file phim hơn chục GB, tải xuống rồi tải nên quá tội.

Tận dụng Colab để làm điều này trực tiếp trên Drive. Bộ đôi Drive + Colab có thể làm những điều mà OneDrive hay Dropbox chỉ dám mơ ước. Trong hai [bài trước](https://lucngoc.com/huong-dan-chuyen-du-lieu-giua-google-drive-va-onedrive/) thì Ngọc đã hướng dẫn cơ bản cách dùng rồi nên bài này Ngọc xin phép bỏ qua, anh em chịu khó đọc lại bài cũ.

Mở [Colab](https://colab.research.google.com/), tạo sổ tay mới, kết nối với Drive, cài rar

```
!apt install rar COPY
```

**I. NÉN**

Bạn đang đọc bài viết trên [lucngoc.com](https://lucngoc.com/huong-dan-ma-hoa-file-tren-google-drive/)

Giả sử trên Drive Ngọc có file Film.mp4 trong thư mục Downloads

```
.
└── Google Drive/
    └── Downloads/
        └── Film.mp4 COPY
```

Giờ cần nén file **Film.mp4** thành **Document.rar** với mật khẩu là **gicungduoc**

Ta chạy lệnh cd tới thư mục Downloads trên Drive

```
cd /content/drive/MyDrive/Downloads COPY
```

Chạy lệnh sau để nén, hệ thống sẽ hỏi mật khẩu nén, anh em nhập mật khẩu không dấu, không ký tự đặc biệt nhé (minh họa là gicungduoc):

```
!rar a -p Document.rar Film.mp4 COPY
```

```
Enter password (will not be echoed): ••••••••••
Reenter password: •••••••••• COPY
```

Anh em xem hình minh họa nhé:

<figure><img src="https://lucngoc.com/wp-content/uploads/2023/07/rar-drive-03.gif" alt="" height="591" width="966"><figcaption></figcaption></figure>

Vậy là xong, chia sẻ file Document.rar đi muôn nơi.

Trong một số tình huống hi hữu có thể bị lỗi hỏng file (rất ít), rủi ro rất nhỏ nhưng vẫn nhắc anh em. Quá trình đọc ghi vào Drive có giới hạn nhất định mỗi ngày.

**II. GIẢI NÉN**

Anh em nhận được link thì tạo bản sao vào Drive, cũng mở Colab, cd vào thư mục chứa bản sao đó (ở đây là thư mục gốc của Drive luôn):

```
!cd /content/drive/MyDrive COPY
```

Rồi chạy xả nén (ở đây gicungduoc là mật khẩu, anh em thay bằng mật khẩu được chia sẻ, nhớ không bỏ chữ p)

```
!unrar x -pgicungduoc Document.rar
```
