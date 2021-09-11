__*Mô tả phương thức kiểm thử ứng dụng web theo chuẩn OWASP và giải thích cách kiểm thử ứng dụng web bằng các biện pháp kiểm thử bảo mật.*__

### What is Web Application Security Testing?

  Kiểm thử bảo mật là một phương pháp đánh giá độ bảo mật của một hệ thống hoặc mạng máy tính bằng cách xác thực hoặc xác minh tính hiệu quả của các biện pháp bảo mật ứng dụng. Pentest Webapp chỉ tập chung vào đánh giá tính bảo mật của ứng dụng web. 
  Quá trình này bao gồm việc phân tích ứng dụng để tìm các điểm yếu, sai sót kỹ thuật hoặc các lỗ hổng bảo mật. Bất kì vấn đề bảo mật nào được phát hiện sẽ được báo cáo lại với chủ hệ thống cùng với đánh giá mức độ ảnh hưởng và đề xuất giải pháp giảm thiểu và ngăn chặn rủi ro.
  
### What is a Vulnerability?

Lỗ hổng bảo mật là một sai sót hoặc điểm yếu trong thiết kế, triển khai, vận hành hoặc quản lý của hệ thống có thể bị khai thác để xâm phạm các mục tiêu bảo mật của hệ thống

### What is a Threat?

Mối đe dọa là bất kì thứ gì ( attacker, internnal user, một hệ thống không ổnđịnh, etc..) có thể gây hại cho tài sản của chủ sở hữu của ứng dụng( tài nguyên có giá trị như dữ liệu trong DB hoặc các file hệ thống) bằng cách khai thác một lỗ hổng.

### What is OWASP Testing Methodology?

Kiểm tra bảo mật là một kỹ thuật để kiểm tra tính bảo mật của các ứng dụng web trong một số trường hợp nhất định. Phương pháp kiểm tra bảo mật webapp OWASP dựa trên phương pháp Black Box.

Kiểm thử có thể đượcphân loại thành __bị động__ hoặc __chủ động__:

__Passive Testing__

Trong quá trình kiểm thử thụ động, một người kiểm thử có gắng hiểu tính logic của ứng dụng và khám phá ứng dụng như một người dùng.

Các công cụ có thể sử dụng để thu thập thông tin. Ví dụ, một HTTP proxy có thể được sử dụng để quan sát tất cả các HTP request và reponses.
Người kiểm thử thường phải hiểu tất cả điểm truy cập và tính năng của hệ thống ( HTTP headers, các tham số , cookie , APIs, các công nghệ sử dụng,  etc..)
Chi tiết sẽ được đề cập sau ở phần __Information Gatherthing__.

Ví dụ, Tester có thể tìm thấy một trang có URL: __https://spider.com/login/?a=1&b=1

Trong trường hợp này, ứng dụng hiển thị 2 access points là 2 tham số a và b. Tất cả những input đầu vào trong giai đoạn này đại diện cho một mục tiêu để kiểm tra

__Active Testing__

Tập hợp các phương thức kiểm thử được chia làm 12 thể loại:

- Information Gatherthing 
- Configuration and Deployment Management Testing 
- Identify Management Testing 
- Authentication Testing 
- Authorization Testing
- Sesion management Testing 
- Input validation testing 
- Error Handling 
- Cryptography
- Business Logic testing
- Client-side Testing
- API testing
