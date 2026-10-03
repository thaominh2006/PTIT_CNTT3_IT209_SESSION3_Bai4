# Bài 4: Nginx chạy song song nhiều cổng (Virtual Hosts)

## Môi trường
- VPS của AZVPS (thay cho DigitalOcean Droplet), IP: 165.101.46.72
- Nginx, UFW

## Cấu trúc
- multi-port.conf: cấu hình 2 server block (cổng 8080 và 8090)
- beta-app/index.html: trang Beta App (cổng 8080)
- internal-app/index.html: trang Internal App (cổng 8090)

## Tường lửa
- UFW: đã mở 8080/tcp và 8090/tcp
- Cloud Firewall: AZVPS không dùng Cloud Firewall riêng, truy cập từ internet thành công sau khi mở UFW

## Kết quả
Xem các ảnh chụp trong thư mục images/.