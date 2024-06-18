# FASTVNTEAM

 Mã nguồn được cung cấp phát triển công khai miễn phí từ các thành viên của FASTVNTEAM

 # CÀI ĐẶT & HỖ TRỢ

 ``Mã nguồn mở của chúng tôi hỗ trợ các phần mềm php 7.4-.8.2 and nignx 1.20.00>=, Docker new version``

 Cài đặt mã nguồn
```bash
  https://btbfast.com/fastvnteam/source/new.zip
```
Thiết lập Nignx
```bash
  location ~* (runtime|application)/{    
    return 403;
}
location / {
    if (!-e $request_filename){
        rewrite  ^(.*)$  /index.php?s=$1  last;   break;
    }
}
```
# Quan trọng

1. Sau khi cài đặt chương trình, bạn sẽ nhận được liên kết tải xuống mã nguồn. Tải nó về thư mục gốc của trang web và giải nén nó.

2. Sao chép tệp cấu hình ``.example.env``, đổi tên thành ``.env`` và điền thông tin cài đặt

3. Nếu bạn là người dùng phiên bản cá nhân (ủy quyền ngoại tuyến), vui lòng viết chứng chỉ trước để tiếp tục thao tác.

4. Chuyển đến cài đặt PHP, xóa chức năng vô hiệu hóa các hàm ``putenv`` và ``proc_open``, đồng thời cài đặt phần mở rộng ``fileinfo`` và ``ioncube``
# Cài đặt svh
```bash
wget https://getcomposer.org/installer -O composer.phar
php composer.phar
php composer.phar install
```
# Lệnh khởi động dtb
```bash
php think migrate:run
```

# Lệnh tạo docker
```bash
bash <(curl -Ls https://btbfast.com/docker/install.sh)
```

## Tác giả
- [@FASTVNTEAM](https://github.com/buithienban)
- [@buithienban](https://t.me/buithienban)


 

 
