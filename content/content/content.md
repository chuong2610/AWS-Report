
![alt text](image.png)
![alt text](image-1.png)
![alt text](image-2.png)
![alt text](image-3.png)
![alt text](image-4.png)
![alt text](image-5.png)
![alt text](image-6.png)
![alt text](image-7.png)
![alt text](image-8.png)
![alt text](image-9.png)
![alt text](image-10.png)
![alt text](image-11.png)
![alt text](image-12.png)
# EV Rental AI Agent - Hướng dẫn triển khai

## 📖 Tổng quan

### Giới thiệu
**EV Rental AI Agent** là một chatbot thông minh được xây dựng để hỗ trợ khách hàng trong hệ thống cho thuê xe điện VinFast. Agent sử dụng AI để:
- Trả lời câu hỏi tự nhiên bằng tiếng Việt
- Tự động tìm kiếm thông tin từ nhiều nguồn
- Hiển thị dữ liệu dạng card trực quan trên giao diện chat

### Công nghệ sử dụng

| Thành phần | Công nghệ | Vai trò |
|------------|-----------|---------|
| **AI Model** | AWS Bedrock - Claude 3.5 Sonnet | Xử lý ngôn ngữ tự nhiên, sinh response |
| **Agent Framework** | Strands Agent SDK | Tự động chọn và gọi tools phù hợp |
| **Backend API** | FastAPI (Python) | REST API server |
| **Database** | PostgreSQL | Lưu trữ chat history |
| **Frontend** | React + Chakra UI | Giao diện người dùng |
| **Knowledge Base** | AWS Bedrock Knowledge Base | Lưu trữ tài liệu, chính sách, FAQ |

---

## 🎯 Chức năng chính

### 1. **Tìm kiếm thông tin từ Knowledge Base**

**Khách hàng hỏi:**
- "Chính sách thuê xe của bạn là gì?"
- "Giá thuê xe VF8 bao nhiêu?"
- "Quy trình đặt xe như thế nào?"
- "Có cần đặt cọc không?"

**Agent sẽ:**
- Tự động tìm kiếm trong Knowledge Base (chứa tài liệu PDF, văn bản chính sách)
- Tổng hợp thông tin liên quan
- Trả lời bằng tiếng Việt với format Markdown

**Ví dụ response:**
```markdown
## 📋 Chính sách thuê xe VinFast

Để thuê xe điện VinFast, bạn cần:

### 📄 Giấy tờ cần thiết:
- ✅ CMND/CCCD gốc (còn hiệu lực)
- ✅ Bằng lái xe hạng B1 trở lên
- ✅ Hộ khẩu hoặc sổ tạm trú

### 💰 Chi phí:
- **VF8**: 1,500,000 VNĐ/ngày
- **VF9**: 2,000,000 VNĐ/ngày
- **Đặt cọc**: 10,000,000 VNĐ

### 📝 Quy trình:
1. Đặt xe online hoặc tại văn phòng
2. Cung cấp giấy tờ và thanh toán
3. Ký hợp đồng và nhận xe
4. Trả xe đúng hạn và hoàn cọc
```

---

### 2. **Tra cứu xe available**

**Khách hàng hỏi:**
- "Xe nào đang có sẵn?"
- "Tìm xe ở Hà Nội từ 10/12 đến 15/12"
- "VF8 có sẵn không?"

**Agent sẽ:**
- Gọi API backend lấy danh sách xe
- Lọc theo tiêu chí (thành phố, ngày tháng, loại xe)
- Hiển thị dưới dạng **Vehicle Cards** với đầy đủ thông tin

**Response format:**
```json
{
  "response": "Hiện có **3 xe VF8** đang available...",
  "data": {
    "type": "vehicles",
    "items": [
      {
        "id": "VF001",
        "name": "VinFast VF8 Plus",
        "model": "VF8",
        "battery_capacity": 87.7,
        "range": 420,
        "price_per_day": 1500000,
        "status": "available"
      }
    ]
  }
}
```

**Frontend hiển thị:**
```
┌────────────────────────┐
│ 🚗 VinFast VF8 Plus   │
│ ✅ Available           │
│ ⚡ 87.7 kWh            │
│ 🔋 420 km              │
│ 💰 1,500,000 VNĐ/ngày  │
└────────────────────────┘
```

---

### 3. **Tìm trạm sạc gần đây**

**Khách hàng hỏi:**
- "Các trạm sạc hiện có"
- "Trạm sạc gần tôi"
- "Trạm sạc ở Hà Nội"

**Agent sẽ:**
- Gọi API lấy danh sách trạm sạc
- Tính khoảng cách (nếu có tọa độ)
- Hiển thị **Station Cards** với địa chỉ, trạng thái

**Response format:**
```json
{
  "response": "Có **2 trạm sạc** gần bạn...",
  "data": {
    "type": "stations",
    "items": [
      {
        "id": "ST001",
        "name": "Trạm Hà Nội Central",
        "address": "123 Láng Hạ, Ba Đình, Hà Nội",
        "status": "active",
        "available_chargers": 5,
        "total_chargers": 8,
        "distance": 2.5
      }
    ]
  }
}
```

**Frontend hiển thị:**
```
┌──────────────────────────┐
│ ⚡ Trạm Hà Nội Central   │
│ ✅ Đang hoạt động         │
│ 📍 123 Láng Hạ, Ba Đình  │
│ ⚡ 5/8 trạm khả dụng      │
│ 📏 Cách 2.5 km           │
└──────────────────────────┘
```

---



---

## 🏗️ Kiến trúc hệ thống

```
┌─────────────────┐
│  React Frontend │  ← User Interface
│  (Port 3000)    │
└────────┬────────┘
         │ HTTP POST /chat
         ↓
┌─────────────────┐
│  FastAPI        │  ← REST API
│  (Port 8000)    │
└────────┬────────┘
         │
    ┌────┴────┐
    ↓         ↓
┌─────────┐ ┌──────────────┐
│Strands  │ │ PostgreSQL   │
│Agent SDK│ │ (Chat History)│
└────┬────┘ └──────────────┘
     │
     ├─────→ AWS Bedrock (Claude 3.5 Sonnet)
     │
     ├─────→ AWS Bedrock Knowledge Base
     │
     └─────→ Backend API (Port 8080)
              ├─ Vehicles
              ├─ Stations
              └─ Bookings
```

---

## 🚀 Hướng dẫn triển khai

### Bước 1: Chuẩn bị môi trường AWS

#### 1.1. Tạo AWS Account
- Truy cập: https://aws.amazon.com
- Đăng ký account mới (cần thẻ tín dụng)

#### 1.2. Tạo IAM User để sử dụng trong code

**Bước 1: Tạo IAM User**
1. Vào **AWS Console → IAM → Users → Create User**
2. User name: `bedrock-app-user`
3. ✅ Chọn: **Provide user access to the AWS Management Console** (optional)
4. ✅ Chọn: **I want to create an IAM user**
5. Click **Next**

**Bước 2: Gán quyền (Permissions)**
1. Chọn: **Attach policies directly**
2. Tìm và chọn các policies sau:
   - ✅ `AmazonBedrockFullAccess` - Quyền sử dụng Bedrock
   - ✅ (Optional) `AmazonS3ReadOnlyAccess` - Nếu dùng Knowledge Base với S3
3. Click **Next** → **Create User**

**Bước 3: Tạo Access Keys**
1. Click vào user vừa tạo: `bedrock-app-user`
2. Tab **Security credentials**
3. Scroll xuống **Access keys** → Click **Create access key**
4. Chọn use case: **Application running outside AWS**
5. Click **Next** → **Create access key**
6. ⚠️ **QUAN TRỌNG**: Copy và lưu lại:
   - `Access key ID` (ví dụ: `AKIAIOSFODNN7EXAMPLE`)
   - `Secret access key` (chỉ hiển thị 1 lần, ví dụ: `wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY`)
7. Click **Done**

**⚠️ Lưu ý bảo mật:**
```bash
# Lưu vào .env file (KHÔNG commit lên Git)
AWS_ACCESS_KEY_ID=YOUR_ACCESS_KEY_ID_HERE
AWS_SECRET_ACCESS_KEY=YOUR_SECRET_ACCESS_KEY_HERE
AWS_REGION=us-west-2
```

---

### Bước 2: Setup AWS Bedrock

#### 2.1. Enable Model Access (QUAN TRỌNG)

**Lưu ý:** Phải enable model access trước khi sử dụng, nếu không sẽ bị lỗi `ValidationException`.

1. Vào **AWS Console → Services → Bedrock**
2. Ở sidebar bên trái, click **Model access** (ở mục Foundation models)
3. Click nút **Manage model access** (màu cam)
4. Tìm và chọn các models:
   - ✅ **Anthropic - Claude 3.5 Sonnet v2** (anthropic.claude-3-5-sonnet-20241022-v2:0)
   - ✅ **Amazon - Titan Embeddings G1 - Text** (nếu dùng Knowledge Base)
5. Click **Request model access** (ở góc dưới bên phải)
6. Đợi approval:
   - **Instant access models**: Available ngay lập tức (màu xanh ✅)
   - **Other models**: Chờ 5-30 phút (status sẽ đổi từ "In progress" → "Access granted")

**Kiểm tra model đã enable:**
```bash
# Dùng AWS CLI (nếu đã cài)
aws bedrock list-foundation-models --region us-west-2

# Hoặc check trên Console:
# Bedrock → Model access → Status phải là "Access granted"
```

#### 2.2. Tạo Knowledge Base (Optional)

**Nếu muốn sử dụng chức năng tìm kiếm chính sách/FAQ:**

1. Vào **Bedrock → Knowledge Bases → Create**
2. Chọn tên: `ev-rental-knowledge-base`
3. Data source:
   - **S3 bucket**: Upload các file PDF/TXT chứa:
     - Chính sách thuê xe
     - Bảng giá
     - FAQ
     - Quy trình đặt xe
4. Embeddings model: **Titan Embeddings G1 - Text**
5. Vector database: **Bedrock managed (OpenSearch Serverless)**
6. Sync data → Đợi indexing hoàn tất
7. Copy **Knowledge Base ID** (dạng `89CI1JSSE4`)

---

