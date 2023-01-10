![](img/7.png)
### Giải quyết
- Từ mô tả và qua thử nghiệm chức năng `Check stock`,khi thử inject 1 payload khác thì kết quả trả về không có gì ngoài `Invalid product ID`
![](img/8.png)
` => Blind xxe => Kiểm tra bằng cách sử dụng OAST gửi 1 http request đến doamin Burp Collaborator `
![](img/9.png)
###### Solved!