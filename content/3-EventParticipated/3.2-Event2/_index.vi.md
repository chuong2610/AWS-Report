---
title: "Event 2"
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

# Báo Cáo Tổng Kết: AWS Cloud Mastery Series #1
**Chủ đề:** GENERATIVE AI, RAG & AWS AGENTIC AI

## 1. Mục Tiêu Chính Của Sự Kiện

Sự kiện tập trung vào việc trang bị kiến thức toàn diện để xây dựng các ứng dụng AI hiện đại trên nền tảng AWS:

* **Tối ưu hóa tương tác:** Nâng cao kỹ năng *Prompt Engineering* để điều khiển mô hình AI chính xác.
* **Ứng dụng nhanh:** Sử dụng các *AWS Pretrained AI Services* để tích hợp trí tuệ nhân tạo mà không cần training model từ số 0.
* **Làm chủ dữ liệu:** Triển khai kiến trúc *RAG (Retrieval-Augmented Generation)* để cập nhật kiến thức riêng cho AI và loại bỏ hiện tượng ảo giác (hallucination).
* **Chuyển đổi sang Agentic AI:** Tìm hiểu cách đưa AI Agent từ giai đoạn thử nghiệm (POC) ra thực tế (Production) bằng *Amazon Bedrock AgentCore*.
* **Giao tiếp thời gian thực:** Tiếp cận *Pipecat Framework* để tạo ra các trợ lý ảo giọng nói với độ trễ cực thấp.

## 2. Diễn Giả Tham Gia

* **Anh Lâm Tuấn Kiệt** (Sr DevOps Engineer - FPT Software): Chia sẻ góc nhìn chuyên sâu về vận hành hệ thống.
* **Bạn Danh Hoàng Hiếu Nghị** (AI Engineer - Renova Cloud): Chuyên gia về các giải pháp và mô hình AI.
* **Anh Đinh Lê Hoàng Anh** (Cloud Engineer Trainee - First Cloud AI Journey): Đại diện cho góc nhìn của người mới bắt đầu hành trình Cloud AI.

---

## 3. Nội Dung Chuyên Sâu

### 3.1. Prompt Engineering & Foundation Models: Nền Móng Vững Chắc

Sự kiện nhấn mạnh nguyên tắc "Input tốt tạo ra Output tốt". Để làm việc hiệu quả với các Foundation Models trên Bedrock, cần nắm vững:

* **Zero-shot / Few-shot Prompting:** Kỹ thuật cung cấp ngữ cảnh hoặc ví dụ mẫu để định hướng AI trả kết quả đúng định dạng mong muốn.
* **Chain of Thought (CoT):** Kỹ thuật yêu cầu AI "tư duy từng bước", giúp giải quyết các bài toán suy luận logic phức tạp và giảm thiểu sai sót.

### 3.2. Hệ Sinh Thái AWS AI Services (Pretrained)

Giải pháp API giúp các lập trình viên tích hợp tính năng thông minh vào ứng dụng một cách nhanh chóng:

* **Vision:** *Amazon Rekognition* (Phân tích ảnh/video, kiểm duyệt nội dung).
* **Language:** *Amazon Translate* (Dịch thuật), *Comprehend* (Phân tích ngữ nghĩa), *Textract* (Trích xuất văn bản từ tài liệu).
* **Audio:** *Amazon Polly* (Text-to-Speech) và *Transcribe* (Speech-to-Text).

### 3.3. RAG - Giải Pháp Cho Dữ Liệu Doanh Nghiệp

RAG là chìa khóa để AI hiểu được dữ liệu nội bộ mà không cần fine-tuning tốn kém:

* **Cơ chế:** Sử dụng *Amazon Titan Text Embeddings V2* để vector hóa dữ liệu, cho phép tìm kiếm theo ngữ nghĩa (semantic search).
* **Knowledge Bases for Amazon Bedrock:** Dịch vụ quản lý trọn gói quy trình RAG: từ cắt nhỏ tài liệu (Chunking), lưu trữ Vector, truy xuất (Retrieval) đến sinh câu trả lời (Generation).

### 3.4. Bước Tiến Lên Agentic AI (AI Tác Vụ)

Xu hướng GenAI đang dịch chuyển mạnh mẽ từ "Hỏi - Đáp" sang "Hành động":

* **Phân cấp:** Từ *Assistant* (tác vụ đơn lẻ) -> *Agents* (hướng mục tiêu, biết dùng công cụ) -> *Agentic Systems* (đa tác nhân, tự chủ).
* **Thách thức "Prototype to Production":** Nhiều dự án Agent thất bại khi ra thực tế do vấn đề về tốc độ xử lý, rủi ro an toàn dữ liệu và khả năng duy trì ngữ cảnh (Memory) kém.

### 3.5. Amazon Bedrock AgentCore: Hạ Tầng Cho AI Agent

AgentCore giải quyết các bài toán hóc búa để doanh nghiệp tự tin triển khai Agent:

* **Kiểm soát:** Quản lý định danh (Identity) và quyền hạn chặt chẽ.
* **Khả năng thực thi:** Tích hợp *Code Interpreter* (Sandbox chạy Python an toàn) để xử lý tính toán chính xác.
* **Giám sát (Observability):** Cho phép theo dõi luồng suy luận của Agent để debug và tối ưu hóa.
* **Bộ nhớ:** Duy trì ngữ cảnh qua các phiên hội thoại dài.

### 3.6. Pipecat Framework: Tương Lai Của Voice AI

Giải pháp mã nguồn mở cho các ứng dụng giao tiếp đa phương thức (Multimodal) thời gian thực:

* **Ưu điểm:** Độ trễ (Latency) cực thấp, tạo cảm giác hội thoại tự nhiên.
* **Quy trình Pipeline:** Xử lý song song các luồng WebRTC -> STT -> LLM -> TTS để đảm bảo phản hồi tức thì.

---

## 4. Bài Học Và Suy Ngẫm Cá Nhân

Qua buổi workshop, tôi đã hệ thống hóa được lộ trình phát triển công nghệ và rút ra những điểm sáng:

1.  **Tư duy Agentic AI:** AI không còn là công cụ tra cứu thụ động mà đã trở thành "nhân viên số" biết lập kế hoạch và hành động. Bedrock AgentCore chính là mảnh ghép quan trọng để hiện thực hóa điều này.
2.  **Vượt qua rào cản Production:** Những chia sẻ về "hố sâu ngăn cách" giữa bản demo và thực tế rất giá trị. Các tính năng bảo mật và giám sát của AWS giúp giải quyết nỗi lo về an toàn khi trao quyền cho AI.
3.  **Tiềm năng của Giao tiếp không chạm:** Pipecat mở ra cơ hội lớn cho các ứng dụng thực tế như Tổng đài AI, Luyện thi ảo hay Phỏng vấn tự động nhờ khả năng phản hồi thời gian thực ấn tượng.

## 5. Kết Luận

Sự kiện **"Generative AI & Agentic AI on AWS"** đã vẽ nên một bức tranh rõ ràng:

* **Hiện tại:** Tối ưu hóa RAG và Prompt Engineering.
* **Tương lai:** Chuyển dịch sang các hệ thống Agent tự chủ (Autonomous Agents).

Với sự hỗ trợ từ hệ sinh thái AWS (Bedrock, AgentCore) và cộng đồng Open Source (Pipecat), rào cản kỹ thuật đã được hạ thấp, tạo đà cho sự bùng nổ của các giải pháp nghiệp vụ sáng tạo.



