# SkinSync - AI-Powered Skincare Ecosystem 🧴✨

<div align="center">

![.NET](https://img.shields.io/badge/.NET-9.0-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-Mobile-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![React](https://img.shields.io/badge/React-Vite-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![AI Powered](https://img.shields.io/badge/AI-Smart%20Dermatology-FF6F00?style=for-the-badge)
![PayOS](https://img.shields.io/badge/Payment-PayOS-00C853?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

**Nền tảng chăm sóc da cá nhân hóa đa nền tảng: Kiểm tra xung đột thành phần mỹ phẩm & Trợ lý ảo AI**

</div>

---

## 🌸 1. Giới thiệu Dự án (Project Overview)

**SkinSync** là một hệ sinh thái chăm sóc da toàn diện kết hợp giữa **Mobile App (Flutter)**, **Web Portal (React/Vite)** và **Backend API (.NET 9)**. Dự án giải quyết các vấn đề nan giải của người dùng khi sử dụng mỹ phẩm: lo sợ kích ứng do dùng chung các hoạt chất xung đột, không biết cách xây dựng chu trình dưỡng da (routine) khoa học và khó khăn trong việc theo dõi tiến trình hồi phục của làn da theo thời gian.

Với sự hỗ trợ của mô hình **Trí tuệ nhân tạo (AI Engine)** và thuật toán đối soát thành phần chuyên sâu, SkinSync đóng vai trò như một chuyên gia da liễu số đồng hành 24/7 cùng người dùng.

---

## ⚡ 2. Các Tính năng Đột phá (Core Capabilities)

### 🔬 1. Kiểm tra Xung đột Thành phần Mỹ phẩm (Ingredient Conflict Checker)
- Tự động phân tích danh sách thành phần hoạt tính trong các sản phẩm skincare.
- Cảnh báo các cặp hoạt chất kỵ nhau có nguy cơ gây bỏng rát, kích ứng hoặc triệt tiêu hiệu quả (ví dụ: AHA/BHA với Retinoids, Vitamin C với Niacinamide ở độ pH không tương thích...).

### 🤖 2. Trợ lý Ảo Da liễu AI & Lời nhắc Thông minh (AI Chat & Smart Reminder)
- Chatbot tư vấn chuyên sâu về các vấn đề da (mụn, thâm, lão hóa, nhạy cảm).
- Đặt lịch nhắc nhở chu trình skincare buổi sáng/tối tự động dựa theo thói quen sinh hoạt.

### 📈 3. Theo dõi Tiến trình Sức khỏe Da (Skin Progress & Health Scoring)
- Đánh giá và chấm điểm mức độ nghiêm trọng của từng vấn đề da (*Skin Health & Concern Severity Scores*).
- Nhật ký hình ảnh theo dõi tiến trình cải thiện làn da qua từng tuần.
- Xuất báo cáo tình trạng da chuyên nghiệp định dạng PDF (`ReportPdfService.cs`).

### 📦 4. Xây dựng Chu trình Tự động (Routine & Regimen Builder)
- Thuật toán chấm điểm và gợi ý sản phẩm phù hợp nhất với loại da (da dầu, da khô, da hỗn hợp).
- Sắp xếp thứ tự thoa sản phẩm chuẩn y khoa (từ lỏng đến đặc, cân bằng độ pH).

### 💳 5. Tích hợp Thanh toán PayOS & Xác thực Supabase
- Cổng thanh toán trực tuyến qua ngân hàng / mã VietQR thông qua cổng **PayOS** (hỗ trợ Webhook tự động).
- Hệ thống quản lý tài khoản bảo mật và phân quyền linh hoạt qua **Supabase Auth**.

---

## 🛠 3. Kiến trúc Đa nền tảng (Multi-Platform Architecture)

```
SkinSync/
├── BE_SkinSync/                 # Backend Web API (.NET 9, EF Core, SQL Server)
│   ├── AI/ & AIPlatform/        # Module AI Platform Core & Chatbot
│   ├── Auth/                    # Supabase Authentication & Role authorization
│   ├── Entities/ & Dtos/        # Data Models & Schema Migrations
│   ├── Recommendations/         # Thuật toán gợi ý & kiểm tra xung đột thành phần
│   └── Services/                # PayOS Payment, Skin Service, PDF Exporter
├── FE_skinsync/                 # Web Portal dành cho Quản trị viên & Bác sĩ (React + Vite)
├── mobile_skinsync/             # Ứng dụng Di động cho Người dùng cuối (Flutter + Dart)
└── filter_skinsafe_for_skinsync.py # Data pipeline thu thập và làm sạch dữ liệu mỹ phẩm
```

---

## ⚙️ 4. Công nghệ Cốt lõi (Tech Stack)

| Thành phần | Công nghệ chính | Ghi chú |
| :--- | :--- | :--- |
| **Backend Core** | **ASP.NET Core 9.0 Web API** | Hiệu năng cao, kiến trúc dịch vụ module hóa |
| **Mobile App** | **Flutter / Dart** | Giao diện hiện đại, tối ưu cho cả iOS & Android |
| **Web Client** | **React 18 + Vite + TypeScript** | Web Portal quản trị và đối chiếu dữ liệu |
| **Database & ORM** | **SQL Server / Supabase + EF Core** | Quản lý dữ liệu quan hệ, bảng thành phần mỹ phẩm |
| **Payment Gateway** | **PayOS Webhook Service** | Tích hợp thanh toán QR ngân hàng tự động |
| **Data Processing** | **Python (Pandas, BeautifulSoup)** | Cào dữ liệu sản phẩm & chuẩn hóa danh mục mỹ phẩm |

---

## 🚀 5. Hướng dẫn Khởi chạy Hệ thống (Quick Start)

### 1. Khởi chạy Backend API (.NET 9):
```bash
cd BE_SkinSync
dotnet restore
dotnet ef database update
dotnet run
# Swagger UI: https://localhost:5001/swagger
```

### 2. Khởi chạy Mobile App (Flutter):
```bash
cd mobile_skinsync
flutter pub get
flutter run
```

### 3. Khởi chạy Web Portal (React):
```bash
cd FE_skinsync
npm install
npm run dev
# Truy cập tại: http://localhost:5173
```

---

## 👥 6. Tác giả & Đóng góp (Credits)

- **Dự án phát triển bởi:** Đội ngũ phát triển SkinSync.
- **Thành viên đóng góp:** Trung Kiên ([@tkiennt](https://github.com/tkiennt)):
  - Đóng góp hơn **42 commits** vào nhánh tính năng cốt lõi.
  - Xây dựng và đồng bộ giao diện Mobile App, tối ưu hóa trải nghiệm người dùng trên thiết bị di động.
  - Phối hợp kết nối các API dịch vụ da liễu và quy trình xác thực dữ liệu người dùng.
