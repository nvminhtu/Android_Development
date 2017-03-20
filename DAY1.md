# Day 1
### Android Operating System: (AOS)
* Là 1 hệ điều hành xây dựng dựa trên nhân Linux.
* Open Source
* Được tạo bởi Google.

### Cấu trúc Android Operating System:
* Tầng Applications: Là các ứng dụng của chúng ta (ví dụ như: Home, Contacts, Phone, Browsers,,...)
* Tầng Application Framewrok (Quản lý các Activity, Window, Package,...)
* Tầng thư viện:
Bao gồm Libraries và Runtime
Libraries: chứa các thư viện hỗ trợ cho app: có thể kể đến như: data storage, web browsing.
Runtime: chứa Davik M, Các thư viện Core Java giúp cho việc chạy App Android.
* Tầng Linux Kernel: Giúp cho việc làm việc với phần cứng: phần hiển thị, Camera, Flash, Wifi, hay Audio,...

### Phiên bản Android:
* Có thể tham khảo trên trang chính của Android để biết được version là bao nhiêu.
* Version mới nhất là Nougat (7.0 - 7.1.1)
* Theo như thị phần điện thoại, thì bây giờ có thể làm app support từ version 5.x trở lên, vì các máy thấp hơn hiện không còn được sử dụng nhiều nữa.
* Thêm vào đó Webview cũng được nâng cấp trên các phiên bản mới -> mượt mà hơn.

### Android Application:
* App của chúng ta có thể hiểu là 1 phần được cài đặt và chạy hoàn toàn độc lập.
* Bao gồm nhiều file cấu hình, code Java, và những file tài nguyên (resources).
* Trong file config - chúng ta có thể xác định và cấu hình cho các component liên quan:
* ---------- Component --------------
* Application

* Activity
Điều khiển UI và xử lý tương tác với người dùng.
* Service
Xử lý các tiến trình background - khi chúng ta làm ta gắn kết vào ứng dụng của chúng ta.
* Broadcast receiver
Chúng xử lý giao tiếp giữa Android OS và các ứng dụng
(Giúp phản hồi các thông điệp từ ứng dụng khác hoặc từ hệ thống. Một Broadcast Receiver được triển khai như là 1 lớp con của Broadcast Receiver - mỗi thông điệp được coi như là 1 Intent)
* Content Provider
Chúng xử lý dữ liệu và quản lý cơ sở dữ liệu

=> Lướt qua phần này vì chỉ cần biết khi cần sẽ lấy ra xài thôi.

### Defining the user Interface
Một phần hiển thị ra cho user của 1 Activity được xác định bởi fragments, views và layout managers.
* Các thành phần này được xác định thông qua file định dạng cho layout là XML.
* Views: là 1 user interface Widget (ví dụ như: Button hay text fields.)

* Fragment (phần này sẽ tìm hiểu kĩ hơn sau): có thể hiểu nó là 1 sub Activiy cũng được - Giúp thiết kế activity có nhiều modules.
[Ví dụ Fragment]

### Context
Quái Context là gì?
* Gặp nhiều trong code - chúng ta có thể hiểu tạm là bối cảnh
* Hiểu chung là khi muốn gọi 1 cái gì đó từ tài nguyên hay bối cảnh hiện tại ta dùng nó.
Ví dụ: nếu ta gọi this - thì this chính là context của màn hình hiện tại, nếu activty của chúng ta gọi bị destroy thì context này không tồn tại thế thôi.

### Android Developer Tools và Android Studio
* Google cung cấp IDE: Android Studio.
* Code Logic của ứng dụng thì được viết bằng ngôn ngữ lập trình Java.
* 1 Ứng dựng Android thì yêu cầu rất nhiều file cấu hình cụ thể.
* Công cụ của Android Studio giúp chúng ta chuyển đổi các file sang 1 file chạy ứng dụng duy nhất (Compile, package, deploy và khởi tạo ứng dụng) => Cái này chúng ta gọi là Gradle và (Android Software Development Kit) - (Android SDK)
* Ngoài ra Android SDK còn chứa ADB (giúp tạo máy ảo.)
* Cài đặt công cụ và các tools cần thiết. Quá dễ không bàn tới (có thể Google).

### Tăng tốc khi build và chạy cho Android nếu máy có sử dụng Chip Intel
* Chúng ta vào Android SDK -> chọn X86 System Image Android 22 - vài cài đặt.
* Hoặc trong Android SDK -> Chọn Extra -> chọn Intel x86 Emulator Accelerator (HAXM) - tăng tốc cho máy ảo.

**Free Software, Hell Yeah!**

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

[Vogella Android Operating System]: <http://www.vogella.com/tutorials/Android/article.html#android-versions>
[Ví dụ Fragment]: <https://laptrinhtuduy.wordpress.com/2014/04/29/fragment-trong-android/>
