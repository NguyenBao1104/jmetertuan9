BÁO CÁO KIỂM THỬ HIỆU SUẤT JMETER

Ngày Kiểm Thử: 01/07/2025

Người Kiểm Thử: Nguyễn Công Bảo

1. Mục Tiêu Kiểm Thử

Sử dụng JMeter để kiểm tra hiệu năng trang web Qldt Phenikaa.

2. Môi Trường Kiểm Thử

Phần mềm Apache JMeter 5.6.3

3. Phương Pháp Kiểm Thử

Kiểm thử tự động với các kịch bản mô phỏng nhiều người dùng truy cập đồng thời.

4. Kịch Bản Kiểm Thử lần 1

Tên Kịch Bản: Kiểm thử tải trang chủ CTSV

Mục Đích: Đánh giá khả năng phản hồi của trang chủ khi có ít người truy cập

HTTP Request: https://qldtbeta.phenikaa-uni.edu.vn/congsinhvien/index.aspx#dashboard

Số lượng người dùng (Threads): 10

Ramp-up period (giây): 5

Loop-count: 5

Kết Quả Mong Đợi: Trang chủ phản hồi đầy đủ, không lỗi

Kết Quả Thực Tế: Đã gửi yêu cầu thành công, không phát sinh lỗi

Kết quả sau khi test:
![image](https://github.com/user-attachments/assets/60704fa2-76d5-48cc-acb3-29bfac9b61b0)


Thời gian phản hồi trung bình: 3.5 giây

Tỷ lệ yêu cầu thành công: 100%

5. Kịch Bản Kiểm Thử lần 2

Tên Kịch Bản: Kiểm thử chịu tải nhiều trang

Mục Đích: Kiểm tra khả năng chịu tải với nhiều người truy cập đồng thời vào các trang chức năng khác nhau

HTTP Request: https://qldtbeta.phenikaa-uni.edu.vn/congsinhvien/index.aspx#dashboard + Các trang chức năng phụ

Số lượng người dùng (Threads): 50

Ramp-up period (giây): 10

Loop-count: 10

Kết Quả Mong Đợi: Tất cả trang phản hồi đầy đủ, tốc độ chấp nhận được

Kết Quả Thực Tế: Có 1 số trang phản hồi chậm, tỷ lệ lỗi 2%

Kết quả sau khi test:
![image](https://github.com/user-attachments/assets/68733f44-18b6-4871-a918-482a35a18b7e)


Thời gian phản hồi trung bình: 6.2 giây

Tỷ lệ yêu cầu thành công: 98%

6. Kết luận

Trang web hoạt động tương đối ổn định, tuy nhiên cần tối ưu hiệu năng cho các trang chức năng khi lượng người dùng cao.
