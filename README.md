# 🏫 Virtual Classroom: OpenGL Edition

### Dự án Mô Phỏng Lớp Học 3D (OpenGL & GLSL)

Dự án này là một ứng dụng đồ họa máy tính 3D mô phỏng không gian lớp học, được xây dựng bằng thư viện **OpenGL** và **FreeGLUT**. Ứng dụng tập trung vào việc áp dụng các kỹ thuật đồ họa 3D cơ bản và nâng cao, đặc biệt là **Shading** và **Tương tác Menu** phức tạp, để tạo ra một môi trường học tập ảo chi tiết và sinh động.

---

## ✨ Tính Năng Nổi Bật

* **Mô Hình Hóa Chi Tiết:** Mô hình hóa các đối tượng cơ bản của lớp học bao gồm bàn giáo viên, 8 bàn học sinh, bảng, cửa sổ và tủ đồ.
* **Chiếu sáng Phong Shading:**
    * Sử dụng **Fragment Shader (`fs.shader`)** để tính toán ánh sáng theo mô hình Phong, bao gồm ba thành phần: Ánh sáng Môi trường (Ambient), Ánh sáng Khuếch tán (Diffuse) và Ánh sáng Phản xạ (Specular).
    * Hỗ trợ **hai nguồn sáng độc lập** (`enable_light_1` và `enable_light_2`) để tăng tính thực tế của cảnh.
* **Hệ thống Menu Tương tác Đa cấp (GLUT):**
    * Sử dụng menu chuột phải (**GLUT Menu**) để tương tác với các đối tượng trong cảnh.
    * Menu con chi tiết cho phép lựa chọn và điều khiển các đối tượng riêng lẻ: **8 Bàn học sinh**, **9 Ngăn kéo** (Bàn GV + 8 Bàn HS), **6 Cửa sổ**, và **Tủ đồ**.
    * Cho phép người dùng **thay đổi trạng thái** (ví dụ: mở/đóng ngăn kéo) và **tùy chỉnh màu sắc** của các đối tượng thông qua menu.
* **Quản lý Màu sắc và Vertex:** Sử dụng **Vertex Shader (`vs.shader`)** để tính toán ma trận biến đổi và gán màu sắc động cho các đỉnh dựa trên tham số `uniform int color`, giúp dễ dàng thay đổi màu sắc của vật thể trong thời gian chạy.

---

## 🛠️ Yêu Cầu Hệ Thống và Công Nghệ

| Công nghệ | Vai trò | Tệp liên quan |
| :--- | :--- | :--- |
| **OpenGL/GLSL** | API đồ họa cốt lõi và Ngôn ngữ Shader. | `vs.shader`, `fs.shader` |
| **FreeGLUT** | Quản lý cửa sổ, xử lý sự kiện đầu vào và Menu. | `main.cpp` |
| **GLEW** | Quản lý và tải các extension của OpenGL. | `main.cpp` |
| **C++** | Ngôn ngữ lập trình chính. | `main.cpp` |

## 🧑‍💻 👤 Tác Giả & Cộng Tác

Dự án này được phát triển bởi một nhóm sinh viên như một phần của môn học Đồ họa Máy tính.

* **Đóng góp chính của cá nhân tôi:** Tìm hiểu **OpenGL**, tạo cấu trúc cơ bản của dự án (Base), thiết lập **Vertex Shader (`vs.shader`)** và **Fragment Shader (`fs.shader`)** cho hiệu ứng chiếu sáng, và mô hình hóa một số vật thể ban đầu.
* **Các thành viên khác:** Đã đóng góp vào việc mô hình hóa đối tượng, phát triển hệ thống menu tương tác, và tối ưu hóa mã nguồn.

---
