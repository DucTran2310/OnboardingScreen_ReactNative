# OnboardingScreen_ReactNative
AsyncStorage không an toàn cho dữ liệu nhạy cảm.

AsyncStorage chỉ đơn giản là lưu dữ liệu vào tài liệu trên ổ cứng của điện thoại và do đó bất kỳ ai có quyền truy cập vào hệ thống tệp của điện thoại đều có thể đọc dữ liệu đó.

Ít nhất là trên iOS, đúng là dữ liệu chỉ có sẵn cho ứng dụng đã viết nó, vì chính sách sandboxing của Apple. Điều này không ngăn chặn iPhone đã bẻ khóa với quyền truy cập root vào hệ thống tệp để nhận bất kỳ thứ gì họ muốn, vì AsyncStorage không mã hóa bất kỳ dữ liệu nào của nó.

Nhưng nói chung, không lưu dữ liệu nhạy cảm vào AsyncStorage, vì lý do tương tự bạn không nên mã hóa dữ liệu nhạy cảm trong mã javascript của bạn, vì nó có thể dễ dàng được biên dịch và đọc ngược lại.
<img src='./assets/anh1.png'>
<img src='./assets/anh2.png'>
<img src='./assets/anh3.png'>