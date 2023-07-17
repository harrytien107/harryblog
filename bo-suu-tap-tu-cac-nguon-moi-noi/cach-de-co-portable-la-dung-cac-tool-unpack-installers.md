# Cách để có Portable là dùng các tool unpack installers

Các phần mềm sẽ thường đóng gói bằng các trình cài đặt như InstallShield , Inno Setup , .....

thì chúng ta sẽ xài các tool unpack installers tuỳ theo các trình cài đặt đó

ví dụ gần nhất là TreeSize , được đóng gói bằng Inno Setup

chúng ta có tool là Innoextract ([https://constexpr.org/innoextract/](https://constexpr.org/innoextract/))

chỉ cần xài cmd -> innoextract.exe -e -Treesize "TreeSize-Setup.exe"

là chúng ta đã có Portable , cũng có thể coi đây là một cách crack app đơn giản vì không cần nhập key từ thằng cài đặt
