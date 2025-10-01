# DEMO MICROSERVICE:

Một hệ thống microservices demo được xây dựng bằng Spring Boot, minh họa kiến trúc microservices với các service độc lập

## Kiến trúc hệ thống:

Hệ thống bao gồm các service chính:
**service-discovery** (eureka-server): Quản lý đăng ký và khám phá service
**gateway-service** 
**product-service**
**user-service**

## Cách chạy ứng dụng:

**Bước 1** : Đóng gói eureka-server (cd registry -> docker-compose up --build)

**Bước 2** : Chạy các service còn lại (nếu muốn chạy bằng lệnh thì cần packaging service và sử dụng câu lệnh .\mvnw spring-boot:run (maven) hoặc .\gradle bootRun (gradle))

**Bước 3** : Truy cập http://localhost:8761 để kiểm tra xem đã tồn tại các service chưa

## Lưu ý:

-  Cần chú ý sự tương thích giữa phiên bản SpringBoot và SpringCloud
-  Cần có annotation @EnableEurekaServer ở file Application
