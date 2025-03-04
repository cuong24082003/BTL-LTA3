# Xây dựng ứng dụng Android sử dụng MIT APP INVENTOR
---
### Author: Nguyễn Tuấn Anh
### Class: K57KMT
### ID Student: K215480106003
#### Video quay toàn bộ quá trình làm (3 hour): [Here](https://youtu.be/89Vu26tkhlA)
----
## Yêu cầu:
1. Tìm hiểu và xây dựng một app android cơ bản
2. Giao diện ứng dụng hiển thị thông tin cá nhân: Họ tên, mã sinh viên, ảnh, video,..
3. Thiết kế giao diện giải bài tìm nghiệm phương trình bậc 2
-----

![images](https://github.com/user-attachments/assets/94283c37-a4e7-4964-88af-281b405b1c9d)

### Demo


https://github.com/user-attachments/assets/c490f04e-2ee6-494a-b509-331b8b62f681


------
### Khi vào màn hình chính của ứng dụng, sẽ có 2 lựa chọn, hiển thị thông tin cá nhân hoặc giải phương tình bậc 2
![image](https://github.com/user-attachments/assets/8b00c35a-77a4-410b-8fcc-2db42d105dc5)
### Hiển thị thông tin cá nhân bảo gồm: tên sinh viên, Class, ID Sudent, Ảnh cá nhân, video
----------
![image](https://github.com/user-attachments/assets/83ef5d56-8ee8-4fb3-bb11-6c2dc5eeb78f)

### Bài toán tính các nghiệm của phương trình bậc 2
-----------
![image](https://github.com/user-attachments/assets/b66949dc-a37c-4f74-9767-77d266cba65a) ![image](https://github.com/user-attachments/assets/f337569b-f320-4d8f-917b-4e20eab67fe8)

### Một số hình ảnh về phần thiết kế ứng dụng

#### Màn hình chính
![image](https://github.com/user-attachments/assets/db92741c-e60d-400e-8003-03b4c044a9b0)

![image](https://github.com/user-attachments/assets/95da43dd-a1e2-4b81-82c4-fbf9edc887bc)

#### Màn hình 2

![image](https://github.com/user-attachments/assets/cc60c91a-9f10-4e27-999b-da93e47afb5e)

![image](https://github.com/user-attachments/assets/54165c24-a9d7-49e5-a61d-1c1f78c26794)

#### Màn hình 3

![image](https://github.com/user-attachments/assets/6bab8da0-66b6-477e-abba-6b75a34a3795)

![image](https://github.com/user-attachments/assets/7ac1627a-0e6a-4c49-bf0e-f592eda7c562)

# README - Ứng dụng Android cơ bản với MIT App Inventor

## Giới thiệu
Ứng dụng Android được xây dựng bằng MIT App Inventor nhằm phục vụ mục đích học tập và thực hành phát triển phần mềm di động. Ứng dụng bao gồm các chức năng hiển thị thông tin cá nhân và giải phương trình bậc 2.

## Chức năng chính
### 1. Giao diện thông tin cá nhân
Giao diện cung cấp các thông tin cá nhân của người dùng, bao gồm:
- Họ và tên: Nguyễn Văn A
- Mã sinh viên: K215480106003
- Ảnh đại diện (Hỗ trợ định dạng .jpg, .png)
- Video giới thiệu bản thân (Hỗ trợ định dạng .mp4)

#### Logic chương trình
- Thành phần giao diện: 
  - Label: Hiển thị tiêu đề và thông tin cá nhân
  - ImagePicker: Chọn ảnh từ thư viện thiết bị
  - Player: Phát video giới thiệu
  - Button: Điều khiển các chức năng như chọn ảnh, phát video

#### Code
- Sử dụng khối lệnh `when ImagePicker.AfterPicking` để hiển thị ảnh đã chọn:
```blocks
when ImagePicker1.AfterPicking
  set Image.Picture to ImagePicker1.Selection
```
- Sử dụng khối lệnh `when Button_PlayVideo.Click` để phát video:
```blocks
when Button_PlayVideo.Click
  call Player1.Start
```

### 2. Giải phương trình bậc 2
Ứng dụng cung cấp giao diện nhập liệu và tính toán nghiệm của phương trình bậc 2 có dạng: 
```
ax² + bx + c = 0
```

#### Logic chương trình
- Người dùng nhập các hệ số `a`, `b`, `c`
- Sử dụng công thức tính delta:
```
Δ = b² - 4ac
```
- Xác định nghiệm dựa vào giá trị của delta:
  - Δ < 0: Vô nghiệm
  - Δ = 0: Nghiệm kép
  - Δ > 0: Hai nghiệm phân biệt

#### Code
- Khối lệnh tính delta:
```blocks
set delta to (b * b) - (4 * a * c)
```
- Khối lệnh tính nghiệm:
```blocks
if delta > 0 then
  set x1 to (-b + sqrt(delta)) / (2 * a)
  set x2 to (-b - sqrt(delta)) / (2 * a)
else if delta = 0 then
  set x1 to -b / (2 * a)
else
  set result to "Vô nghiệm"
```

## Công nghệ sử dụng
- MIT App Inventor 2
- Ngôn ngữ lập trình: Block-Based Programming

## Môi trường phát triển
- Trình duyệt: Google Chrome
- Phần mềm giả lập: MIT AI2 Companion

## Hướng dẫn cài đặt
1. Tải ứng dụng về điện thoại dưới định dạng `.apk`.
2. Cài đặt ứng dụng trên thiết bị Android.
3. Mở ứng dụng và sử dụng các chức năng.

## Tác giả
- Họ tên: Nguyễn Tuấn Anh
- Mã sinh viên: K215480106003









