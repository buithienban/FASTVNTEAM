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

 

 
