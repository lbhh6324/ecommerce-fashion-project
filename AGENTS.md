# **Project Instructions for AI**

Tài liệu này quy định các nguyên tắc, phạm vi và quy trình làm việc bắt buộc dành cho các công cụ Trí tuệ Nhân tạo (AI Assistants / Coding Agents) khi hỗ trợ nhóm phát triển dự án **Hotmate**.

## **1\. Project context**

* Đây là dự án website thương mại điện tử của sinh viên nhóm 9 thuộc học phần **Phát triển ứng dụng Web/TMĐT**.

* **Tên dự án:** Website bán hàng quần áo thời trang \- Hotmate.

* **Đặc thù nghiệp vụ cốt lõi:** Quản lý danh mục quần áo thời trang, quản lý biến thể sản phẩm theo cặp **Màu sắc (Color)** và **Kích cỡ (Size: S, M, L, XL)** kèm bảng quy đổi kích cỡ (Size chart), kiểm tra tồn kho theo phân loại, quản lý giỏ hàng, đặt hàng trực tuyến (Checkout) và xử lý trạng thái đơn hàng (Chờ xác nhận $\rightarrow$ Đang chuẩn bị hàng $\rightarrow$ Đang giao hàng $\rightarrow$ Giao thành công).

* **Định hướng công nghệ & Kiến trúc:**

  * **Frontend:** HTML5, CSS3 (Tailwind CSS / Bootstrap), JavaScript.

  * **Backend & Database:** RESTful API kết nối Cơ sở dữ liệu quản lý Danh mục, Sản phẩm, Biến thể (Product\_Variants), Đơn hàng và Người dùng.

* **Mục tiêu học tập:** Mỗi thành viên trong nhóm (BA, UI/UX, Frontend, Backend, QA) đều phải tự đọc hiểu, kiểm soát và giải thích được toàn bộ phần mã nguồn hoặc tài liệu do mình phụ trách vào cuối học phần.

## **2\. Scope**

* Chỉ triển khai các chức năng đã được nhóm thống nhất trong REQUIREMENTS.md và quy trình nghiệp vụ trong docs/business-workflow.md.

* **Phân biệt rõ trong mọi đề xuất:**

  * **Yêu cầu bắt buộc (MVP):** Tìm kiếm/lọc quần áo, xem chi tiết & bảng size, chọn biến thể Size/Màu, thêm vào giỏ hàng, kiểm tra tồn kho, áp dụng mã giảm giá (voucher), đặt hàng (COD hoặc mô phỏng thanh toán Online), theo dõi và cập nhật trạng thái đơn hàng phía Khách hàng & Quản trị viên (Admin).

  * **Yêu cầu có thể phát triển sau (Out of current scope):** Không tự ý triển khai tích hợp API đơn vị vận chuyển thực tế (GHN, GHTK), cổng thanh toán thật yêu cầu giấy phép doanh nghiệp, chatbot AI phức tạp, gợi ý size bằng AI hoặc tính năng livestream bán hàng.

  * **Đề xuất cần nhóm xác minh thêm:** Bất kỳ tính năng phụ trợ nào chưa có trong tài liệu đều phải hỏi ý kiến nhóm trước.

* Không giả định nhóm có đủ thời gian hoặc năng lực để triển khai tất cả chức năng nâng cao.

## **3\. Coding principles**

* **Giữ mã nguồn dễ đọc và dễ bảo trì:**

  * Đặt tên biến, hàm, class, file và API endpoint rõ nghĩa, nhất quán.

  * Viết chú thích (comments) ngắn gọn bằng tiếng Việt hoặc tiếng Anh ở các đoạn xử lý nghiệp vụ quan trọng (như kiểm tra tồn kho theo Size/Màu, tính tổng tiền đơn hàng, cập nhật trạng thái đơn) để sinh viên dễ nắm bắt.

* **Không thay đổi kiến trúc lớn khi chưa được nhóm đồng ý:**

  * Giữ nguyên cấu trúc tách biệt giữa giao diện (frontend/ hoặc các trang HTML/CSS/JS) và máy chủ (backend/), không tự ý cài đặt thêm thư viện/framework nặng khi chưa được xác nhận.

* **Không tự ý xóa chức năng đang hoạt động:**

  * Khi sửa lỗi hoặc nâng cấp một thành phần (ví dụ: trang Giỏ hàng hoặc API Đặt hàng), phải đảm bảo không làm hỏng các luồng liên quan đã chạy ổn định.

* **Ưu tiên thay đổi nhỏ, có thể kiểm tra:**

  * Chia nhỏ mã nguồn theo từng bước (incremental changes) gắn với từng nhiệm vụ trong PROJECT\_PLAN.md để nhóm có thể chạy thử và kiểm chứng ngay trên trình duyệt hoặc công cụ test API.

## **4\. Workflow**

### **Trước khi sửa mã nguồn:**

1. **Đọc các tài liệu liên quan:** Tham chiếu kỹ REQUIREMENTS.md, docs/business-workflow.md, PROJECT\_PLAN.md và cấu trúc code hiện tại của dự án.

2. **Phân tích hiện trạng:** Xác định rõ nguyên nhân lỗi hoặc vị trí các file cần thêm mới/chỉnh sửa; kiểm tra sự tương thích giữa dữ liệu Frontend và API Backend.

3. **Đề xuất phương án:** Trình bày ngắn gọn hướng giải quyết, giải thích cơ sở của đề xuất và liệt kê các file dự kiến sẽ tác động.

4. **Chờ nhóm xác nhận:** Chỉ tiến hành viết hoặc sửa mã nguồn sau khi thành viên phụ trách xác nhận đồng ý với phương án.

### **Sau khi sửa mã nguồn:**

1. **Giải thích các thay đổi:** Tóm tắt logic vừa triển khai một cách dễ hiểu để thành viên phụ trách nắm rõ bản chất kỹ thuật.

2. **Nêu file đã sửa:** Liệt kê danh sách chính xác đường dẫn các file đã tạo mới hoặc cập nhật.

3. **Hướng dẫn chạy và kiểm thử:** Cung cấp các bước cụ thể để chạy thử trên máy cục bộ (Localhost/Browser) và các kịch bản kiểm thử (ví dụ: thử chọn Size M \- Màu Đen khi còn hàng và khi hết hàng).

4. **Báo cáo các giới hạn còn tồn tại:** Nêu rõ các trường hợp biên (edge cases) chưa xử lý hoặc những điểm nhóm cần tự kiểm tra lại (phục vụ việc ghi nhận vào AI\_USAGE\_LOG.md).

## **5\. Security**

* **Không đưa mật khẩu, API key hoặc token vào mã nguồn:**

  * Tuyệt đối không hard-code chuỗi kết nối CSDL (Database connection string), secret key, mật khẩu quản trị vào các file code đẩy lên GitHub Public Repository.

  * Luôn sử dụng biến môi trường qua file .env và nhắc nhóm kiểm tra file .gitignore để loại trừ .env, node\_modules/.

* **Không tự ý vô hiệu hóa kiểm tra bảo mật:**

  * Luôn duy trì kiểm tra dữ liệu đầu vào (validation) ở cả Frontend và Backend (thông tin người nhận, số lượng đặt mua $\geq 1$, kiểm tra tồn kho hợp lệ, phân quyền Admin/Customer).

  * Mật khẩu người dùng trong CSDL bắt buộc phải được mã hóa (hash) chứ không lưu dưới dạng văn bản thuần (plain text).

* **Không sử dụng dữ liệu cá nhân thật khi chưa được phép:**

  * Toàn bộ dữ liệu sản phẩm quần áo, tài khoản khách hàng và đơn hàng dùng để phát triển/kiểm thử phải là dữ liệu mẫu giả lập (Mock/Seed data).

## **6\. Communication**

* **Nếu yêu cầu chưa rõ, hãy hỏi lại trước khi triển khai:** Khi prompt của thành viên thiếu thông tin (ví dụ: chưa rõ cấu trúc JSON trả về, chưa rõ quy tắc tính phí vận chuyển hay trạng thái đơn hàng), AI phải đặt câu hỏi làm rõ thay vì tự suy đoán.

* **Phong cách phản hồi:** Rõ ràng, có cấu trúc, mang tính hướng dẫn học thuật để hỗ trợ sinh viên hiểu sâu kiến thức phát triển ứng dụng Web/TMĐT.

