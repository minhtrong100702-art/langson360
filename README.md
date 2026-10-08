# Lạng Sơn 360 - AI Guide

**Ứng dụng web giới thiệu du lịch, văn hóa và đặc sản tỉnh Lạng Sơn**

Lạng Sơn 360 - AI Guide là một ứng dụng web được xây dựng theo hướng trực quan, tương tác và thân thiện với học sinh. Ứng dụng hỗ trợ khám phá các địa danh, đặc sản, văn hóa và lịch sử của Lạng Sơn, đồng thời tích hợp chức năng "AI Guide" dạng xử lý từ khóa bằng JavaScript để gợi ý nội dung phù hợp với câu hỏi của người dùng.

## 1. Mục tiêu

- Giới thiệu vẻ đẹp, văn hóa, lịch sử và ẩm thực Lạng Sơn.
- Hỗ trợ học sinh tìm hiểu địa phương thông qua hình thức trực quan và tương tác.
- Ứng dụng công nghệ web và JavaScript để tạo trải nghiệm khám phá.
- Có thể sử dụng làm sản phẩm STEM, sản phẩm học tập hoặc công cụ giới thiệu du lịch địa phương.

## 2. Công nghệ sử dụng

Ứng dụng được xây dựng dưới dạng **một file HTML duy nhất**, bao gồm:

- HTML5
- CSS3
- JavaScript
- Font Awesome
- Google Maps Embed
- Web Speech API / Speech Synthesis
- LocalStorage
- Hệ thống xử lý câu hỏi "AI Guide" bằng JavaScript và từ khóa

Không sử dụng:

- Node.js / npm
- Backend server
- Cơ sở dữ liệu
- API key
- File `.env`
- Framework bắt buộc như React, Vue hoặc Angular

## 3. Cấu trúc dự án

```text
LangSon360/
├── index.html
├── README.md
└── .gitignore
```

### `index.html`

File chính của ứng dụng. Toàn bộ giao diện, CSS và JavaScript được tích hợp trong cùng một file.

### `README.md`

Tài liệu giới thiệu dự án và hướng dẫn sử dụng/triển khai.

### `.gitignore`

Danh sách các file/thư mục không cần đưa lên GitHub.

## 4. Chạy ứng dụng trên máy tính

Không cần cài đặt phần mềm lập trình.

Chỉ cần:

1. Tải hoặc sao chép `index.html`.
2. Nhấp đúp vào file.
3. Mở bằng trình duyệt Chrome, Edge hoặc trình duyệt hiện đại khác.

## 5. Đưa ứng dụng lên GitHub Pages

### Bước 1: Tạo repository

Tạo một repository mới trên GitHub, ví dụ:

```text
langson360
```

### Bước 2: Tải file lên repository

Đưa các file sau vào thư mục gốc:

```text
index.html
README.md
.gitignore
```

### Bước 3: Bật GitHub Pages

Vào:

```text
Settings → Pages
```

Chọn:

```text
Source: Deploy from a branch
Branch: main
Folder: / (root)
```

Nhấn **Save**.

Sau khi GitHub Pages hoàn tất triển khai, website sẽ có dạng:

```text
https://TEN-TAI-KHOAN.github.io/langson360/
```

Trong đó `TEN-TAI-KHOAN` là tên tài khoản GitHub của bạn.

## 6. Lưu ý về kết nối Internet

Phiên bản hiện tại có một số thành phần sử dụng tài nguyên bên ngoài, vì vậy **chưa phải phiên bản offline hoàn toàn**.

Các thành phần có thể cần Internet:

- Một số hình ảnh được tải từ ImgBB.
- Font Awesome được tải từ CDN.
- Bản đồ Google Maps được nhúng từ Google Maps.
- Một số chức năng liên quan đến nội dung trực tuyến có thể phụ thuộc vào trình duyệt/kết nối mạng.

Phần giao diện và logic JavaScript chính vẫn nằm trong `index.html`.

## 7. Chức năng AI Guide

Chức năng "AI Guide" trong phiên bản hiện tại được triển khai bằng JavaScript phía trình duyệt.

Hệ thống phân tích câu hỏi dựa trên các từ khóa và nhóm chủ đề, sau đó trả về nội dung phù hợp.

Ví dụ các nhóm câu hỏi:

- Lịch trình 1 ngày
- Ẩm thực
- Đặc sản
- Di tích
- Lịch sử
- Văn hóa
- Ná Nhèm
- Giá tham khảo

Đây là **AI dạng xử lý logic/từ khóa cục bộ**, không sử dụng API AI bên ngoài và không yêu cầu API key.

## 8. Bộ đếm lượt truy cập

Ứng dụng sử dụng `localStorage` để lưu bộ đếm trên trình duyệt.

Do đó, bộ đếm hiện tại mang tính **cục bộ trên thiết bị/trình duyệt**, không phải hệ thống thống kê lượt truy cập toàn cầu của website.

Nếu cần thống kê lượt truy cập thực tế trên Internet, có thể tích hợp thêm một dịch vụ thống kê hoặc cơ sở dữ liệu trực tuyến ở phiên bản sau.

## 9. Quyền riêng tư

Ứng dụng không yêu cầu người dùng tạo tài khoản và không yêu cầu nhập mật khẩu.

Các dữ liệu cục bộ như bộ đếm truy cập được lưu bằng `localStorage` trên trình duyệt của người dùng.

## 10. Định hướng phát triển

Các phiên bản tiếp theo có thể phát triển:

- Bản đồ tương tác nâng cao.
- Tìm kiếm địa điểm.
- Lọc địa danh theo huyện/chủ đề.
- Lịch trình du lịch tự động.
- Quiz kiến thức về Lạng Sơn.
- Trò chơi hóa hoạt động khám phá địa phương.
- Tích hợp AI hội thoại thực sự thông qua API.
- Chuyển toàn bộ hình ảnh và tài nguyên sang dạng nhúng để tăng khả năng chạy offline.
- Hệ thống thống kê truy cập trực tuyến.

## 11. Sử dụng trong giáo dục STEM

Sản phẩm có thể được sử dụng làm sản phẩm STEM/giáo dục địa phương với các nội dung:

- Xác định vấn đề thực tiễn.
- Nghiên cứu văn hóa và du lịch địa phương.
- Thiết kế giao diện web.
- Lập trình HTML/CSS/JavaScript.
- Ứng dụng AI và công nghệ số.
- Kiểm thử và cải tiến sản phẩm.
- Trình bày sản phẩm trước hội đồng.

## 12. Tác giả / Nhóm thực hiện

**Sản phẩm:** Lạng Sơn 360 - AI Guide

**Đơn vị:** Trường PTDTNT THCS&THPT Bình Gia - Lạng Sơn

---

> Đây là phiên bản web hiện tại của dự án. Khi phát triển phiên bản mới, nên cập nhật README để phản ánh chính xác các tính năng và công nghệ được sử dụng.
