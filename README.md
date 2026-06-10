# BÁO CÁO BÀI TẬP LỚN
## MÔN: PHÁT TRIỂN ỨNG DỤNG TRÊN THIẾT BỊ DI ĐỘNG - TEE0419

## Thông tin sinh viên
- **Họ và tên:** Nguyễn Thị Kim Huệ  
- **Mã sinh viên:** K225480106

---

# 1. Giới thiệu bài tập lớn

Bài tập lớn môn **Phát triển ứng dụng trên thiết bị di động - TEE0419** yêu cầu sinh viên xây dựng ứng dụng bằng **MIT App Inventor** và **Android Studio**, đồng thời ghi lại toàn bộ quá trình thực hiện bằng file Markdown để upload lên GitHub.

Yêu cầu chính của bài tập gồm:
- Thiết kế ứng dụng bằng MIT App Inventor gồm 3 Screen.
- Xây dựng APP1 trên Android Studio sử dụng dữ liệu chuẩn bị trước trong thư mục Assets.
- Xây dựng APP2 trên Android Studio tương đương với ứng dụng MIT App Inventor.
- Tích hợp API gửi dữ liệu và WebView hiển thị website.
- Viết báo cáo mô tả chi tiết quá trình thực hiện.

---

# 2. Tìm hiểu yêu cầu đề bài

Trước khi bắt đầu thực hiện, tiến hành đọc kỹ đề bài để xác định rõ các yêu cầu cần làm.

Các nội dung chính cần hoàn thành gồm:

## 2.1 MIT App Inventor
Ứng dụng cần có **3 Screen**:
- Screen giới thiệu bản thân (About)
- Screen giải bài toán đơn giản
- Screen sử dụng WebView để hiển thị website

Ngoài ra cần tìm hiểu:
- Cách kéo thả giao diện.
- Cách chỉnh thuộc tính của component.
- Cách sử dụng Block để xử lý sự kiện.
- Ưu điểm và nhược điểm của lập trình kéo thả.

### Ảnh 1
![Ảnh 1](images/1.png)

### Ảnh 2
![Ảnh 2](images/2.png)

---

# 3. Xây dựng ứng dụng bằng MIT App Inventor

## 3.1 Tạo project mới

Đầu tiên truy cập trang MIT App Inventor và tạo một project mới.

Sau khi tạo project, tiến hành đặt tên ứng dụng và chuẩn bị xây dựng các màn hình theo yêu cầu đề bài.

### Ảnh 3
![Ảnh 3](images/3.png)

---

## 3.2 Thiết kế Screen About

Tại màn hình đầu tiên, tiến hành tạo giao diện giới thiệu thông tin cá nhân.

Các thành phần được sử dụng:
- **Label** để hiển thị thông tin cá nhân.
- **Button** để chuyển sang Screen giải toán.
- **Button** để chuyển sang Screen WebView.

Sau đó thay đổi các thuộc tính như:
- Font chữ
- Kích thước chữ
- Màu sắc
- Căn giữa nội dung bằng Alignment

### Ảnh 4
![Ảnh 4](images/4.png)

### Ảnh 5
![Ảnh 5](images/5.png)

---

## 3.3 Thiết kế Screen giải toán

Tiến hành tạo giao diện nhập dữ liệu để giải toán đơn giản.

Các thành phần sử dụng:
- **TextBox** để nhập dữ liệu đầu vào.
- **Button** để thực hiện tính toán.
- **Label** để hiển thị kết quả.

Ví dụ:
- Giải phương trình bậc 2.
- Tính tổng hai số.
- Tính diện tích hình học.

### Ảnh 6
![Ảnh 6](images/6.png)

### Ảnh 7
![Ảnh 7](images/7.png)

---

## 3.4 Thiết kế Screen WebView

Tạo thêm một Screen chứa thành phần **WebViewer** để hiển thị website hỗ trợ giao diện điện thoại.

Website sử dụng:

`https://k58kmt.tdh.io.vn`

Sau đó thiết lập kích thước hiển thị phù hợp với màn hình điện thoại.

### Ảnh 8
![Ảnh 8](images/8.png)

### Ảnh 9
![Ảnh 9](images/9.png)

---

## 3.5 Thiết kế Block xử lý sự kiện

Sau khi hoàn thiện giao diện, tiến hành kéo thả các Block để xử lý chức năng.

Các Block thực hiện:
- Click Button chuyển Screen.
- Xử lý tính toán.
- Hiển thị kết quả.
- Mở website bằng WebViewer.

### Ưu điểm của Block:
- Không cần viết code quá nhiều.
- Dễ học và trực quan.
- Phù hợp với người mới bắt đầu.

### Nhược điểm:
- Khó mở rộng ứng dụng lớn.
- Thiếu tính linh hoạt so với viết code.

### Ảnh 10
![Ảnh 10](images/10.png)

### Ảnh 11
![Ảnh 11](images/11.png)

---

# 4. Xây dựng APP1 bằng Android Studio (Dữ liệu trong Assets)

## 4.1 Tạo project Android Studio

Tiến hành mở Android Studio và tạo project mới bằng mẫu **Empty Activity**.

Sau khi tạo xong project, tiến hành tổ chức thư mục dự án và chuẩn bị dữ liệu cho ứng dụng.

### Ảnh 12
![Ảnh 12](images/12.png)

---

## 4.2 Tạo thư mục Assets

Trong Android Studio, tiến hành tạo thư mục **assets** để lưu dữ liệu có sẵn trong ứng dụng.

Khi ứng dụng được build:
- Tất cả file trong Assets sẽ đi theo ứng dụng.
- Có thể sử dụng offline.
- Không cần internet để truy cập dữ liệu.

Ví dụ ứng dụng:
- App hướng dẫn học tập.
- App từ điển mini.
- App đọc dữ liệu cài sẵn.

### Ảnh 13
![Ảnh 13](images/13.png)

### Ảnh 14
![Ảnh 14](images/14.png)

---

## 4.3 Đọc dữ liệu từ Assets

Tiến hành đọc dữ liệu bằng `AssetManager`.

Ví dụ cú pháp:

```java
InputStream inputStream = getAssets().open("data.txt");
```

Sau khi đọc dữ liệu:
- Chuyển đổi thành chuỗi ký tự.
- Xử lý dữ liệu nếu cần.
- Hiển thị lên giao diện.

### Ảnh 15
![Ảnh 15](images/15.png)

### Ảnh 16
![Ảnh 16](images/16.png)

---

# 5. Xây dựng APP2 bằng Android Studio

## 5.1 Activity About

Tạo màn hình giới thiệu thông tin sinh viên.

Màn hình gồm:
- Thông tin cá nhân.
- Nút chuyển sang Activity giải toán.
- Nút chuyển sang Activity WebView.

Để chuyển màn hình sử dụng **Intent**.

### Ảnh 17
![Ảnh 17](images/17.png)

### Ảnh 18
![Ảnh 18](images/18.png)

---

## 5.2 Activity giải toán

Tiến hành xây dựng chức năng giải toán đơn giản.

Quy trình thực hiện:
1. Người dùng nhập dữ liệu.
2. Ứng dụng xử lý phép tính.
3. Hiển thị kết quả.
4. Gửi dữ liệu lên API.

API sử dụng:

`https://k58kmt.tdh.io.vn/api`

Dữ liệu gửi đi dạng JSON.

### Ảnh 19
![Ảnh 19](images/19.png)

### Ảnh 20
![Ảnh 20](images/20.png)

### Ảnh 21
![Ảnh 21](images/21.png)

---

## 5.3 Kết nối API

Sau khi giải toán thành công, ứng dụng tiến hành gửi dữ liệu tới API.

Dữ liệu bao gồm:
- Mã sinh viên
- Input
- Output

Ứng dụng nhận lại kết quả JSON từ server.

### Ảnh 22
![Ảnh 22](images/22.png)

### Ảnh 23
![Ảnh 23](images/23.png)

---

## 5.4 Activity WebView

Tiến hành tạo WebView để truy cập website:

`https://k58kmt.tdh.io.vn?masv=K225480106102`

Mục tiêu:
- Hiển thị website trong ứng dụng.
- Tối ưu hiển thị cho điện thoại.
- Không cần mở trình duyệt ngoài.

### Ảnh 24
![Ảnh 24](images/24.png)

### Ảnh 25
![Ảnh 25](images/25.png)

---

# 6. Chạy thử và hoàn thiện ứng dụng

Sau khi hoàn thiện các chức năng, tiến hành chạy thử ứng dụng trên điện thoại hoặc máy ảo Android để kiểm tra.

Các nội dung kiểm tra:
- Giao diện hiển thị.
- Chức năng chuyển màn hình.
- Giải toán chính xác.
- Gửi API thành công.
- WebView hoạt động đúng.

Sau quá trình kiểm tra, tiến hành sửa lỗi và tối ưu giao diện.

### Ảnh 26
![Ảnh 26](images/26.png)

### Ảnh 27
![Ảnh 27](images/27.png)

---

# 7. Kết luận

Qua bài tập lớn này, em đã hiểu rõ hơn về quy trình phát triển ứng dụng di động bằng **MIT App Inventor** và **Android Studio**, đồng thời học được cách sử dụng **Assets**, **API**, **WebView**, xử lý sự kiện và thiết kế giao diện trên nền tảng Android.

