# BÁO CÁO BÀI TẬP LỚN
## MÔN: PHÁT TRIỂN ỨNG DỤNG TRÊN THIẾT BỊ DI ĐỘNG - TEE0419

## Thông tin sinh viên
- **Họ và tên:** Phạm Linh  
- **Mã sinh viên:** K225480106102  

---

# 1. Giới thiệu bài tập lớn

Bài tập lớn môn **Phát triển ứng dụng trên thiết bị di động - TEE0419** yêu cầu xây dựng ứng dụng bằng **MIT App Inventor** và **Android Studio**, đồng thời ghi lại toàn bộ quá trình thực hiện bằng file Markdown để upload lên GitHub.

Các yêu cầu chính:
- Thiết kế ứng dụng bằng MIT App Inventor gồm 3 Screen.
- Xây dựng APP1 trên Android Studio sử dụng dữ liệu trong Assets.
- Xây dựng APP2 Android Studio tương đương MIT App Inventor.
- Tích hợp API và WebView.
- Viết báo cáo mô tả quá trình thực hiện.

---

# 2. Xây dựng ứng dụng bằng MIT App Inventor

## 2.1 Tạo project mới

Đầu tiên truy cập vào MIT App Inventor và tiến hành tạo project mới. Sau khi tạo xong, đặt tên project và chuẩn bị xây dựng giao diện theo yêu cầu đề bài.

### Ảnh 1
![Ảnh 1](images/1.png)

---

## 2.2 Thiết kế Screen About

Tạo màn hình đầu tiên dùng để giới thiệu thông tin cá nhân.

Các thành phần được sử dụng:
- Label hiển thị họ tên và mã sinh viên.
- Button chuyển sang màn hình giải toán.
- Button chuyển sang màn hình WebView.

Tiến hành chỉnh các thuộc tính như:
- Font chữ
- Màu nền
- Kích thước chữ
- Căn giữa nội dung

### Ảnh 2
![Ảnh 2](images/2.png)

### Ảnh 3
![Ảnh 3](images/3.png)

---

## 2.3 Thiết kế Screen giải toán

Tiến hành tạo giao diện giải toán đơn giản.

Các thành phần sử dụng:
- TextBox nhập dữ liệu.
- Button thực hiện tính toán.
- Label hiển thị kết quả.

Ứng dụng thực hiện giải bài toán đơn giản như:
- Tính tổng hai số
- Hoặc giải phương trình

### Ảnh 4
![Ảnh 4](images/4.png)

### Ảnh 5
![Ảnh 5](images/5.png)

---

## 2.4 Thiết kế Screen WebView

Tạo Screen thứ ba sử dụng **WebViewer** để hiển thị website hỗ trợ giao diện điện thoại.

Website sử dụng:

`https://k58kmt.tdh.io.vn`

Sau đó điều chỉnh giao diện phù hợp với thiết bị di động.

### Ảnh 6
![Ảnh 6](images/6.png)

### Ảnh 7
![Ảnh 7](images/7.png)

---

## 2.5 Thiết kế Block xử lý chức năng

Sau khi hoàn thiện giao diện, tiến hành kéo thả các Block để xử lý logic chương trình.

Các chức năng thực hiện:
- Chuyển Screen khi click Button.
- Thực hiện phép tính.
- Hiển thị kết quả.
- Mở website bằng WebViewer.

### Ưu điểm:
- Dễ sử dụng.
- Không cần viết nhiều code.
- Trực quan.

### Nhược điểm:
- Khó mở rộng ứng dụng lớn.
- Hạn chế hơn so với Android Studio.

### Ảnh 8
![Ảnh 8](images/8.png)

### Ảnh 9
![Ảnh 9](images/9.png)

---

# 3. Xây dựng APP1 bằng Android Studio (Dữ liệu Assets)

## 3.1 Tạo project Android Studio

Tiến hành mở Android Studio và tạo project mới bằng mẫu **Empty Activity**.

Sau khi tạo project, tổ chức lại cấu trúc thư mục và chuẩn bị dữ liệu.

### Ảnh 10
![Ảnh 10](images/10.png)

---

## 3.2 Tạo thư mục Assets

Tiến hành tạo thư mục **assets** để lưu dữ liệu chuẩn bị trước.

Lợi ích:
- File đi theo ứng dụng sau khi build.
- Có thể truy cập offline.
- Không cần internet.

Ví dụ:
- File văn bản hướng dẫn.
- Nội dung dữ liệu có sẵn.

### Ảnh 11
![Ảnh 11](images/11.png)

### Ảnh 12
![Ảnh 12](images/12.png)

---

## 3.3 Đọc dữ liệu từ Assets

Tiến hành đọc dữ liệu bằng `AssetManager`.

Ví dụ cú pháp:

```java
InputStream inputStream = getAssets().open("data.txt");
```

Sau khi đọc:
- Chuyển đổi dữ liệu.
- Xử lý nếu cần.
- Hiển thị lên giao diện.

### Ảnh 13
![Ảnh 13](images/13.png)

### Ảnh 14
![Ảnh 14](images/14.png)

---

# 4. Xây dựng APP2 bằng Android Studio

## 4.1 Activity About

Tiến hành xây dựng màn hình giới thiệu thông tin sinh viên.

Màn hình gồm:
- Họ tên
- Mã sinh viên
- Button chuyển sang màn hình giải toán
- Button chuyển sang màn hình WebView

Để chuyển màn hình sử dụng **Intent**.

### Ảnh 15
![Ảnh 15](images/15.png)

### Ảnh 16
![Ảnh 16](images/16.png)

![Ảnh 26](images/26.png)

![Ảnh 27](images/27.png)

---

## 4.2 Activity giải toán

Tiến hành xây dựng giao diện giải toán.

Quy trình:
1. Nhập dữ liệu.
2. Thực hiện tính toán.
3. Hiển thị kết quả.
4. Gửi API sau khi tính toán.

API sử dụng:

`https://k58kmt.tdh.io.vn/api`

### Ảnh 17
![Ảnh 17](images/17.png)

### Ảnh 18
![Ảnh 18](images/18.png)

### Ảnh 19
![Ảnh 19](images/19.png)

---

## 4.3 Kết nối API

Sau khi tính toán hoàn tất, ứng dụng gửi dữ liệu tới API bằng phương thức POST.

Dữ liệu gửi bao gồm:
- Mã sinh viên
- Input
- Output

Ứng dụng nhận phản hồi JSON từ server.

### Ảnh 20
![Ảnh 20](images/20.png)

### Ảnh 21
![Ảnh 21](images/21.png)

---

## 4.4 Activity WebView

Tiến hành tạo Activity sử dụng WebView.

Website sử dụng:

`https://k58kmt.tdh.io.vn?masv=K225480106102`

Mục tiêu:
- Hiển thị website trong ứng dụng.
- Tương thích điện thoại.
- Không cần mở trình duyệt ngoài.

### Ảnh 22
![Ảnh 22](images/22.png)

### Ảnh 23
![Ảnh 23](images/23.png)

---

# 5. Chạy thử và hoàn thiện ứng dụng

Sau khi hoàn thiện các chức năng, tiến hành chạy thử ứng dụng trên máy ảo hoặc điện thoại thật để kiểm tra.

Các nội dung kiểm tra:
- Chuyển màn hình hoạt động đúng.
- Giải toán chính xác.
- API gửi thành công.
- WebView hiển thị đúng.

Sau khi kiểm tra tiến hành sửa lỗi và tối ưu giao diện.

### Ảnh 24
![Ảnh 24](images/24.png)

### Ảnh 25
![Ảnh 25](images/25.png)

---

# 6. Kết luận

Qua bài tập lớn này, em đã hiểu hơn về quy trình phát triển ứng dụng trên thiết bị di động bằng **MIT App Inventor** và **Android Studio**, đồng thời biết cách sử dụng **Assets**, **API**, **WebView** và xử lý giao diện trên Android.
