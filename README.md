# BÁO CÁO GIỚI THIỆU SẢN PHẨM

## HỆ THỐNG QUẢN LÝ TÀI SẢN VÀ TÀI CHÍNH DOANH NGHIỆP TÍCH HỢP AI CHATBOT

**Phiên bản:** 1.0  
**Nền tảng:** Odoo ERP 15.0  
**Nhóm phát triển:** Hoàng Phương Huế - Nguyễn Lê Việt Hoàng - Nguyễn Trung Thành

---

## MỤC LỤC

1. [Tổng quan sản phẩm](#1-tổng-quan-sản-phẩm)
2. [Chức năng chi tiết các module](#2-chức-năng-chi-tiết-các-module)
3. [Ưu điểm vượt trội của sản phẩm](#3-ưu-điểm-vượt-trội-của-sản-phẩm)
4. [Công nghệ sử dụng](#4-công-nghệ-sử-dụng)

---

## 1. TỔNG QUAN SẢN PHẨM

### 1.1. Giới thiệu

Hệ thống Quản lý Tài sản và Tài chính là giải pháp ERP toàn diện được phát triển trên nền tảng Odoo, tích hợp công nghệ Trí tuệ nhân tạo (AI) tiên tiến. Sản phẩm được thiết kế nhằm số hóa và tự động hóa toàn bộ quy trình quản lý tài sản cố định, công cụ dụng cụ và các nghiệp vụ tài chính liên quan trong doanh nghiệp.

### 1.2. Mục tiêu sản phẩm

- **Số hóa toàn diện:** Chuyển đổi quy trình quản lý tài sản từ thủ công sang điện tử
- **Tự động hóa thông minh:** Giảm thiểu thao tác thủ công, tối ưu hiệu suất làm việc
- **Ra quyết định nhanh chóng:** Cung cấp dữ liệu realtime qua Dashboard trực quan
- **Hỗ trợ 24/7:** Tích hợp AI Chatbot hỗ trợ người dùng mọi lúc mọi nơi
- **Tuân thủ chuẩn mực:** Đáp ứng các quy định kế toán về khấu hao và quản lý tài sản

### 1.3. Đối tượng sử dụng

| Đối tượng | Vai trò trong hệ thống |
|-----------|------------------------|
| Nhân viên | Đăng ký mượn/trả tài sản, tra cứu thông tin |
| Trưởng phòng | Phê duyệt đơn mượn, quản lý tài sản phòng ban |
| Quản lý tài sản | Kiểm kê, bảo trì, điều chuyển, thanh lý tài sản |
| Kế toán/Tài chính | Quản lý khấu hao, hạch toán, lập báo cáo tài chính |
| Ban lãnh đạo | Giám sát tổng quan qua Dashboard, phê duyệt mua sắm |

### 1.4. Kiến trúc hệ thống

```
┌─────────────────────────────────────────────────────────────────┐
│                    GIAO DIỆN NGƯỜI DÙNG (WEB)                   │
├─────────────────────────────────────────────────────────────────┤
│  ┌─────────────┐  ┌─────────────────┐  ┌─────────────────────┐  │
│  │ q_trang_chu │  │ quan_ly_tai_san │  │ quan_ly_tai_chinh   │  │
│  │ Dashboard & │  │ Quản lý         │  │ Quản lý             │  │
│  │ AI Chatbot  │  │ Tài sản         │  │ Tài chính           │  │
│  └─────────────┘  └─────────────────┘  └─────────────────────┘  │
├─────────────────────────────────────────────────────────────────┤
│                    ODOO ERP PLATFORM (v15.0)                    │
├─────────────────────────────────────────────────────────────────┤
│  ┌─────────────────┐              ┌─────────────────────────┐   │
│  │ PostgreSQL DB   │              │ Google Gemini AI API    │   │
│  │ (Dữ liệu)       │              │ (Xử lý ngôn ngữ tự nhiên)│   │
│  └─────────────────┘              └─────────────────────────┘   │
└─────────────────────────────────────────────────────────────────┘
```

---

## 2. CHỨC NĂNG CHI TIẾT CÁC MODULE

### 2.1. Module Trang chủ & AI Chatbot (`q_trang_chu`)

#### 2.1.1. Dashboard Tổng quan

| Chức năng | Mô tả |
|-----------|-------|
| **Thống kê KPI realtime** | Hiển thị tổng số tài sản, giá trị tài sản, số đơn chờ duyệt, tài sản đang mượn |
| **Biểu đồ trực quan** | Phân tích tài sản theo danh mục, xu hướng mượn trả theo thời gian |
| **Thông báo quan trọng** | Cảnh báo tài sản quá hạn, đơn cần phê duyệt, lịch bảo trì |
| **Thao tác nhanh** | Shortcut đến các chức năng thường dùng (Tạo đơn mượn, Duyệt đơn, Kiểm kê...) |
| **Hoạt động gần đây** | Timeline các hoạt động mới nhất trong hệ thống |

#### 2.1.2. AI Chatbot Assistant

| Chức năng | Mô tả |
|-----------|-------|
| **Hỗ trợ 24/7** | Trợ lý ảo hoạt động liên tục, sẵn sàng hỗ trợ người dùng mọi lúc |
| **Hướng dẫn quy trình** | Giải thích từng bước quy trình mượn/trả, kiểm kê, thanh lý tài sản |
| **Tra cứu thông tin** | Truy vấn nhanh thông tin bảo hành, vị trí, trạng thái tài sản |
| **Kiểm tra lịch mượn** | Xem tài sản có sẵn để mượn, đơn mượn của bản thân |
| **Giải đáp thắc mắc** | Trả lời các câu hỏi về quy định, chính sách quản lý tài sản |
| **Gợi ý thông minh** | Đề xuất hành động tiếp theo dựa trên ngữ cảnh hội thoại |

**Luồng xử lý Chatbot:**

```
Người dùng gửi tin nhắn
        ↓
Phát hiện ý định (Intent Detection)
        ↓
Thu thập dữ liệu ngữ cảnh từ Database (RAG)
        ↓
Gọi Gemini AI API sinh câu trả lời
        ↓
Trả về kết quả + Gợi ý hành động
```

---

### 2.2. Module Quản lý Tài sản (`quan_ly_tai_san`)

#### 2.2.1. Quản lý Danh mục & Hồ sơ Tài sản

| Chức năng | Mô tả |
|-----------|-------|
| **Danh mục tài sản** | Phân loại tài sản theo nhóm (Máy tính, Nội thất, Phương tiện...) |
| **Hồ sơ tài sản chi tiết** | Lưu trữ thông tin: Tên, Mã, Nguyên giá, Ngày mua, Nhà cung cấp, Thông số kỹ thuật |
| **Quản lý bảo hành** | Theo dõi ngày bắt đầu, kết thúc bảo hành, nhà cung cấp dịch vụ |
| **Lịch sử biến động** | Ghi nhận toàn bộ thay đổi: Điều chuyển, sửa chữa, nâng cấp |
| **Mã QR/Barcode** | Hỗ trợ in mã định danh cho từng tài sản |

#### 2.2.2. Quy trình Mượn - Trả Tài sản

| Chức năng | Mô tả |
|-----------|-------|
| **Tạo đơn mượn** | Nhân viên đăng ký mượn tài sản qua form điện tử |
| **Phê duyệt đa cấp** | Trưởng phòng → Quản lý tài sản xét duyệt đơn mượn |
| **Bàn giao tài sản** | Ghi nhận biên bản bàn giao khi cho mượn |
| **Theo dõi hạn trả** | Cảnh báo tự động khi tài sản sắp đến hạn hoặc quá hạn trả |
| **Thu hồi tài sản** | Ghi nhận tình trạng tài sản khi nhận lại |
| **Lịch sử mượn trả** | Truy xuất toàn bộ lịch sử mượn/trả của từng tài sản |

**Quy trình mượn tài sản:**

```
Tạo đơn mượn → Gửi duyệt → Trưởng phòng duyệt → Quản lý TS duyệt 
     → Bàn giao tài sản → Sử dụng → Trả tài sản → Hoàn thành
```

#### 2.2.3. Kiểm kê Tài sản

| Chức năng | Mô tả |
|-----------|-------|
| **Lập kế hoạch kiểm kê** | Tạo đợt kiểm kê theo định kỳ (tháng/quý/năm) |
| **Phân công kiểm kê** | Giao nhiệm vụ kiểm kê cho từng nhân viên/phòng ban |
| **Ghi nhận kết quả** | Đối chiếu số liệu thực tế với sổ sách |
| **Xử lý chênh lệch** | Báo cáo thừa/thiếu, đề xuất xử lý |
| **Báo cáo kiểm kê** | Xuất báo cáo tổng hợp kết quả kiểm kê |

#### 2.2.4. Bảo trì & Sửa chữa

| Chức năng | Mô tả |
|-----------|-------|
| **Lịch bảo trì định kỳ** | Thiết lập lịch bảo dưỡng cho từng loại tài sản |
| **Yêu cầu sửa chữa** | Nhân viên báo hỏng, đề xuất sửa chữa |
| **Theo dõi tiến độ** | Cập nhật trạng thái xử lý yêu cầu |
| **Lịch sử kỹ thuật** | Ghi nhận toàn bộ lịch sử bảo trì, sửa chữa |

#### 2.2.5. Điều chuyển & Thanh lý

| Chức năng | Mô tả |
|-----------|-------|
| **Luân chuyển nội bộ** | Điều chuyển tài sản giữa các phòng ban |
| **Đề xuất thanh lý** | Lập đề xuất thanh lý tài sản hết khấu hao/hư hỏng |
| **Phê duyệt thanh lý** | Quy trình xét duyệt thanh lý tài sản |
| **Ghi nhận thanh lý** | Cập nhật trạng thái, giá trị thu hồi |

---

### 2.3. Module Quản lý Tài chính (`quan_ly_tai_chinh`)

#### 2.3.1. Quản lý Khấu hao Tài sản

| Chức năng | Mô tả |
|-----------|-------|
| **Thiết lập phương pháp** | Khấu hao đường thẳng, số dư giảm dần, theo sản lượng |
| **Tính khấu hao tự động** | Chạy tính khấu hao định kỳ (tháng/quý/năm) |
| **Bảng khấu hao chi tiết** | Xem lịch khấu hao của từng tài sản |
| **Bút toán khấu hao** | Tự động sinh bút toán kế toán khấu hao |
| **Điều chỉnh khấu hao** | Xử lý các trường hợp điều chỉnh đặc biệt |

**Công thức khấu hao đường thẳng:**
```
Mức khấu hao năm = (Nguyên giá - Giá trị thu hồi) / Số năm sử dụng
```

#### 2.3.2. Phê duyệt Mua sắm Tài sản

| Chức năng | Mô tả |
|-----------|-------|
| **Đề xuất mua sắm** | Các phòng ban lập đề xuất mua tài sản mới |
| **Kiểm soát ngân sách** | Đối chiếu với ngân sách được phân bổ |
| **Phê duyệt đa cấp** | Quy trình phê duyệt theo mức giá trị |
| **Theo dõi thực hiện** | Cập nhật tiến độ mua sắm sau khi được duyệt |

#### 2.3.3. Hạch toán Kế toán

| Chức năng | Mô tả |
|-----------|-------|
| **Bút toán tăng tài sản** | Tự động sinh bút toán khi nhập mới tài sản |
| **Bút toán giảm tài sản** | Ghi nhận khi thanh lý, nhượng bán tài sản |
| **Bút toán khấu hao** | Hạch toán chi phí khấu hao định kỳ |
| **Bút toán sửa chữa** | Ghi nhận chi phí bảo trì, sửa chữa lớn |

#### 2.3.4. Báo cáo Tài chính

| Loại báo cáo | Mô tả |
|--------------|-------|
| **Báo cáo tổng hợp tài sản** | Thống kê toàn bộ tài sản theo danh mục, phòng ban |
| **Báo cáo khấu hao** | Chi tiết khấu hao lũy kế, giá trị còn lại |
| **Báo cáo tăng/giảm tài sản** | Biến động tài sản trong kỳ |
| **Báo cáo chi phí bảo trì** | Tổng hợp chi phí sửa chữa, bảo dưỡng |
| **Báo cáo theo phòng ban** | Phân bổ giá trị tài sản theo đơn vị sử dụng |

---

## 3. ƯU ĐIỂM VƯỢT TRỘI CỦA SẢN PHẨM

### 3.1. Tích hợp AI Chatbot Thông minh

✅ **Hỗ trợ 24/7** - Trợ lý ảo sẵn sàng hỗ trợ bất kỳ lúc nào, giảm tải cho bộ phận IT/Hành chính

✅ **Xử lý ngôn ngữ tự nhiên** - Hiểu và phản hồi bằng tiếng Việt tự nhiên nhờ Gemini AI

✅ **Truy vấn dữ liệu realtime** - Tra cứu thông tin tài sản, bảo hành, lịch mượn trực tiếp từ hệ thống

✅ **Gợi ý thông minh** - Đề xuất hành động phù hợp dựa trên ngữ cảnh

### 3.2. Dashboard Trực quan & Realtime

✅ **Giao diện hiện đại** - Thiết kế UI/UX theo xu hướng mới, dễ sử dụng

✅ **Dữ liệu realtime** - Cập nhật tức thời, không cần refresh trang

✅ **Biểu đồ đa chiều** - Phân tích dữ liệu trực quan bằng Chart.js

✅ **Thao tác nhanh** - Truy cập chức năng thường dùng chỉ với 1 click

### 3.3. Quy trình Số hóa Hoàn chỉnh

✅ **Paperless** - Loại bỏ hoàn toàn giấy tờ, biểu mẫu thủ công

✅ **Phê duyệt điện tử** - Quy trình duyệt online, có thể thực hiện từ xa

✅ **Truy xuất nguồn gốc** - Lịch sử đầy đủ, minh bạch, dễ kiểm toán

✅ **Thông báo tự động** - Email/Notification khi có việc cần xử lý

### 3.4. Tự động hóa Nghiệp vụ

✅ **Tính khấu hao tự động** - Chạy định kỳ, không cần thao tác thủ công

✅ **Sinh bút toán tự động** - Kế toán không cần nhập liệu thủ công

✅ **Cảnh báo thông minh** - Nhắc nhở tài sản quá hạn, bảo hành sắp hết

✅ **Báo cáo tự động** - Xuất báo cáo theo mẫu chuẩn

### 3.5. Khả năng Mở rộng & Tích hợp

✅ **Nền tảng Odoo** - Dễ dàng tích hợp với các module khác (Kế toán, Nhân sự, Mua hàng...)

✅ **API mở** - Kết nối với hệ thống bên ngoài qua REST API

✅ **Tùy biến linh hoạt** - Có thể điều chỉnh theo đặc thù doanh nghiệp

✅ **Đa người dùng** - Hỗ trợ nhiều user đồng thời, phân quyền chi tiết

### 3.6. Bảo mật & An toàn Dữ liệu

✅ **Phân quyền chi tiết** - Kiểm soát truy cập theo vai trò, chức năng

✅ **Audit Trail** - Ghi log toàn bộ thao tác của người dùng

✅ **Backup tự động** - Sao lưu dữ liệu định kỳ

✅ **Mã hóa dữ liệu** - Bảo vệ thông tin nhạy cảm

---

## 4. CÔNG NGHỆ SỬ DỤNG

### 4.1. Nền tảng & Framework

| Công nghệ | Phiên bản | Mục đích sử dụng |
|-----------|-----------|------------------|
| **Odoo ERP** | 15.0 | Nền tảng ERP chính, cung cấp framework phát triển |
| **Python** | 3.8+ | Ngôn ngữ lập trình backend chính |
| **PostgreSQL** | 12+ | Hệ quản trị cơ sở dữ liệu |
| **JavaScript/OWL** | ES6+ | Xây dựng giao diện frontend động |
| **XML/QWeb** | - | Template engine cho views và reports |
| **SCSS/CSS3** | - | Styling giao diện người dùng |

### 4.2. Trí tuệ Nhân tạo (AI)

| Công nghệ | Mục đích |
|-----------|----------|
| **Google Gemini 2.0 Flash** | Xử lý ngôn ngữ tự nhiên (NLP), sinh câu trả lời thông minh |
| **RAG (Retrieval-Augmented Generation)** | Bổ sung context từ database để trả lời chính xác hơn |
| **Intent Detection** | Phân loại ý định người dùng để xử lý phù hợp |

### 4.3. Visualization & UI

| Công nghệ | Mục đích |
|-----------|----------|
| **Chart.js** | Vẽ biểu đồ thống kê, phân tích dữ liệu |
| **Font Awesome** | Bộ icon hệ thống |
| **Bootstrap 4** | CSS framework responsive |
| **Moment.js** | Xử lý định dạng ngày giờ |

### 4.4. Kiến trúc Hệ thống

```
┌─────────────────────────────────────────────────────────────┐
│                      CLIENT LAYER                           │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐       │
│  │ Web Browser  │  │ Mobile App   │  │  API Client  │       │
│  └──────────────┘  └──────────────┘  └──────────────┘       │
└─────────────────────────────────────────────────────────────┘
                            │
                            ▼
┌─────────────────────────────────────────────────────────────┐
│                    APPLICATION LAYER                        │
│  ┌──────────────────────────────────────────────────────┐   │
│  │                  Odoo Web Server                      │   │
│  │  • HTTP/HTTPS • Session Management • Authentication   │   │
│  └──────────────────────────────────────────────────────┘   │
│  ┌──────────────────────────────────────────────────────┐   │
│  │              Custom Odoo Modules                      │   │
│  │  • q_trang_chu • quan_ly_tai_san • quan_ly_tai_chinh │   │
│  └──────────────────────────────────────────────────────┘   │
│  ┌──────────────────────────────────────────────────────┐   │
│  │              Odoo Core Modules                        │   │
│  │  • base • web • mail • account • hr                   │   │
│  └──────────────────────────────────────────────────────┘   │
└─────────────────────────────────────────────────────────────┘
                            │
                            ▼
┌─────────────────────────────────────────────────────────────┐
│                      DATA LAYER                             │
│  ┌──────────────────────┐  ┌────────────────────────────┐   │
│  │   PostgreSQL DB      │  │   External Services        │   │
│  │   • Master Data      │  │   • Gemini AI API          │   │
│  │   • Transaction      │  │   • Email Server           │   │
│  │   • Attachments      │  │   • File Storage           │   │
│  └──────────────────────┘  └────────────────────────────┘   │
└─────────────────────────────────────────────────────────────┘
```

### 4.5. Yêu cầu Hệ thống

#### Server Requirements:

| Thành phần | Yêu cầu tối thiểu | Khuyến nghị |
|------------|-------------------|-------------|
| **CPU** | 2 cores | 4+ cores |
| **RAM** | 4 GB | 8+ GB |
| **Storage** | 50 GB SSD | 100+ GB SSD |
| **OS** | Ubuntu 20.04 LTS | Ubuntu 22.04 LTS |

#### Client Requirements:

| Thành phần | Yêu cầu |
|------------|---------|
| **Browser** | Chrome/Firefox/Edge (phiên bản mới nhất) |
| **Kết nối mạng** | Ổn định, tốc độ ≥ 5 Mbps |
| **Độ phân giải** | ≥ 1366x768 pixels |

---

## KẾT LUẬN

Hệ thống Quản lý Tài sản và Tài chính tích hợp AI Chatbot là giải pháp toàn diện giúp doanh nghiệp:

- **Tiết kiệm thời gian** nhờ tự động hóa quy trình và hỗ trợ AI 24/7
- **Giảm sai sót** nhờ số hóa và kiểm soát quy trình chặt chẽ
- **Ra quyết định nhanh** nhờ dữ liệu realtime và báo cáo trực quan
- **Tối ưu chi phí** nhờ quản lý khấu hao và bảo trì hiệu quả
- **Nâng cao trải nghiệm** người dùng với giao diện hiện đại và AI Chatbot thông minh

---

*Tài liệu được tạo bởi Nhóm phát triển - 02/2026*
