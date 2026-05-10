# Môn: Phát triển ứng dụng với mã nguồn mở
nguyễn lam sơn_K225480106076
# Bài làm
## TỔ CHỨC CSDL CHO HỆ THỐNG QUẢN LÝ TIỆM CẦM ĐỒ: viết tay ra giấy, lấy điện thoại chụp lại, upload ảnh lên github (đã nói về các nghiệp vụ trên lớp, ghi bảng)
# 
## 1.SỬ DỤNG DOCKER TRÊN UBUNTU ĐỂ:
Mariadb : chứa csdl của hệ thống này
Phpmyadmin: để soi được csdl (chỉ để xem, ko cần tạo bảng từ đây, django sẽ làm hết)
Django: build 1 docker container (dùng Dockerfile): trên nền python, sử dụng django, nhớ mount thư mục để dễ edit, edit dùng: sudo nano ten_file
## <img width="359" height="149" alt="image" src="https://github.com/user-attachments/assets/249a4c0d-5f1b-49d2-aba6-940e5c683421" />
## <img width="865" height="751" alt="image" src="https://github.com/user-attachments/assets/f270eee1-bff7-47bf-9e4b-2973427b13ff" />
## <img width="1113" height="967" alt="image" src="https://github.com/user-attachments/assets/f4302f09-4217-44d8-aa97-cab840c181f8" />
## Khởi động bằng lệnh:
docker compose build
docker compose up -d
Kiểm tra bằng docker ps
## <img width="1110" height="617" alt="image" src="https://github.com/user-attachments/assets/8a59216f-1e7e-4436-a56d-d743badd9721" />
## <img width="566" height="111" alt="image" src="https://github.com/user-attachments/assets/7e02bf74-38db-41c1-b297-fcf0dc8e4e9d" />
## <img width="1088" height="369" alt="image" src="https://github.com/user-attachments/assets/c33aa539-60d4-485e-982c-b3c033e9c11c" />
# 2. Khởi tạo Code Django & Cấu hình
# Tạo Project và App:
khởi tạo 
## <img width="1049" height="89" alt="image" src="https://github.com/user-attachments/assets/8b76832d-83a2-4af6-b3de-c7812dbab58e" />
Sau khi chạy sẽ sinh thêm các Components mới:
## <img width="364" height="360" alt="image" src="https://github.com/user-attachments/assets/571b5f0d-d17c-46e0-85c5-f27f6639d25c" />
# Sửa file config/settings.py
Cấp phép truy cập: ALLOWED_HOSTS = ['*']
## <img width="656" height="122" alt="image" src="https://github.com/user-attachments/assets/51bbe60d-502b-44e0-a3fb-e50f18baae97" />
Kết nối DB: Sửa khối DATABASES thành:
## <img width="620" height="251" alt="image" src="https://github.com/user-attachments/assets/d6693961-a102-43b6-af5b-d6aaaf144b1b" />
# Tạo Bảng và Giao diện Admin
a) Viết Models (pawnshop/models.py):
## <img width="1544" height="1020" alt="image" src="https://github.com/user-attachments/assets/bb0a07e1-bea6-44c5-9c16-41e2d479487a" />
## <img width="1520" height="1066" alt="image" src="https://github.com/user-attachments/assets/ef142f9b-354f-4942-94f0-013552745d63" />
b) Cấu hình Admin (pawn_app/admin.py):
## <img width="1505" height="1079" alt="image" src="https://github.com/user-attachments/assets/ee836771-7a09-4944-9198-3e101cd63756" />
## <img width="1491" height="447" alt="image" src="https://github.com/user-attachments/assets/bcac2f68-14a8-48c4-9147-63d9b5b1ae66" />
## <img width="1118" height="941" alt="image" src="https://github.com/user-attachments/assets/91075a2d-0242-4f3a-9747-d792e1ce2612" />
Tạo trang "Con Nợ Đến Hạn"
## ![Uploading image.png…]()

