![](img/1.png)
### Giải quyết
- Phân tích ứng dụng web:
    - Trang web công khai là 1 trang mua sắm chỉ có chức năng đăng nhập và kiểm tra số lượng mặt hàng còn lại
    ![](img/2.png)
    - Khi sử dụng chức năng kiểm tra mặt hàng: Có vẻ như tham số stockApi đang yêu cầu HTTP/URL, điều này có thể dẫn đến lỗ hổng SSRF nếu các biện pháp kiểm soát phòng ngừa chưa được triển khai đúng cách. 
    ![](img/3.png)
- Khai thác:
    - Thử attack vào chính server ứng dụng web (thông qua loopback network interface với hostname kiểu 127.0.0.1 hoặc localhost)
    ![](img/4.png)
    - Xuất hiện `Admin panel`, thử request đến `Admin panel`
    ![](img/5.png)
    - Tiếp theo thử kiểm tra thấy liên kết để xóa tài khoản carlos 
    ![](img/6.png)
    - Sửa URL để gửi request xóa tài khoản carlos.
    ![](img/7.png)
    - Request được gửi thành cô, có thể quay lại `Admin panel` để kiểm tra.
    ![](img/8.png)
###### Solved!
