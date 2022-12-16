![](img/11.png)
### Giải quyết
- Sau khi đăng nhập, truy cập trang admin và nhận được thông báo ` Admin interface only available to local users `
- Thay đổi HTTP method, đến TRACE method trả về response chứa 1 custom HTTP header
![](img/12.png)
- Giờ đã biết header cần sử dụng, thiết lập nó để được gửi cùng mỗi request bên tab Proxy.
![](img/13.png)
- Truy cập lại trang admin và xóa tài khoản carlos.
![](img/14.png)
###### Solved!