# ChatApp
Đây là phần mềm đơn gian hỗ trợ chat nhiều người dùng. Người dùng có thể chat với nhau trong cùng mạng LAN (local). Ngoài ra, nó có cơ chế đăng kí, đăng nhập để lưu tin nhắn của người dùng trong các phiên sử dụng

### Sản phẩm bao gồm: 
* Client.jar: Client (máy khách) để người dùng tương tác với Server, sử dụng các tính năng để có thể chat với người dùng khác trong mạng LAN
* Server.jar: Server (máy chủ) là nơi tiếp nhận các kết nối từ các Client (máy khách) và nó có nhiệm vụ xử lý và chuyển tiếp các gói tin từ Client đến nếu cần thiết. Một Server có thể có nhiều Server con chạy đa luồng phục vụ độc lập cho từng Client.

### Để có thể chạy chương trình máy tính của bạn phải có môi trường để chạy Java, bạn có thể tải:
- Java development kit (JDK) phiên bản 1.8 trở lên
- Java runtime environment (JRE) phiên bản 8 trở lên

### Cách sử dụng:
- Tải các file *.jar cần thiết ở mục **Releases**
- Khởi tạo Server nếu chưa có (các máy tình trong mạng LAN có thể sử dụng chung):
    + Mở Terminal/CMD
    + Sử dụng lệnh `cd` để di chuyển đến thư mục chứa file Server.jar:
        + `cd <path to Server.jar>`
    + Sử dụng lệnh để chạy Server.jar
        + `java -jar Server.jar`
- Khởi tạo Client:
    + Mở cửa sổ Terminal/CMD mới:
    + Sử dụng lệnh `cd` để di chuyển đến thư mục chứa file Client.jar:
        + `cd <path to Client.jar>`
    + Sử dụng lệnh để chạy Client.jar (nếu Server đặt ở máy khác trong mạng LAN, ta cần truyền vào IP của máy chạy Server trong mạng LAN, ví dụ như: 192.168.1.5)
        + `java -jar Client.jar <IP máy chạy Server>`
    + Đăng kí, đăng nhập để tiếp tục
    + Chọn người dùng trên danh sách online và bắt đầu chat (bạn cũng có thể chọn Server để chat với Server)
