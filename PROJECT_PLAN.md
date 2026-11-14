# **PROJECT PLAN**

**Dự án:** Website bán hàng quần áo thời trang \- Hotmate  
**Mục tiêu:** Lập kế hoạch phân công vai trò, lộ trình triển khai, danh sách công việc chi tiết và phương án quản trị rủi ro cho dự án phát triển ứng dụng Web/TMĐT.

## **1\. Thành viên và vai trò**

Nhóm áp dụng nguyên tắc phân công rõ ràng: mỗi nhiệm vụ có một người chịu trách nhiệm chính, có sản phẩm đầu ra cụ thể và các thành viên phối hợp hỗ trợ nhau trong suốt quá trình tích hợp, kiểm thử.

| STT | Họ và tên | Vai trò chính | Trách nhiệm cụ thể |
| :---- | :---- | :---- | :---- |
| 1 | **Lữ Bích Hà** | **Trưởng nhóm / Business Analyst (BA)** | \- Quản lý tiến độ chung của dự án và điều phối công việc qua GitHub Issues. \- Khảo sát đối thủ, phân tích yêu cầu nghiệp vụ (REQUIREMENTS.md) và quy trình đặt hàng (docs/business-workflow.md). \- Kiểm soát phạm vi dự án và tổng hợp báo cáo. |
| 2 | **Huỳnh Thị Huỳnh Như** | **UI/UX Designer** | \- Khảo sát giao diện các website thời trang tham khảo (docs/competitor-analysis.md). \- Thiết kế Sitemap, Wireframe và Mockup trên Figma (Trang chủ, Danh sách sản phẩm, Chi tiết sản phẩm kèm Bảng size, Giỏ hàng, Thanh toán, Trang Admin). \- Chuẩn bị tài nguyên hình ảnh sản phẩm quần áo, banner, icon và quy chuẩn màu sắc/font chữ. |
| 3 | **Phạm Thiện Thiên Thành Trình** | **Frontend Developer** | \- Xây dựng cấu trúc giao diện bằng HTML5, CSS3 (Tailwind CSS / Bootstrap) và JavaScript. \- Lập trình giao diện tương tác phía khách hàng: bộ lọc quần áo, chọn biến thể (Màu sắc/Kích cỡ S, M, L, XL), giỏ hàng động, form đặt hàng (Checkout) và tra cứu đơn. \- Đảm bảo giao diện hiển thị tốt trên cả máy tính và điện thoại (Responsive Web Design). |
| 4 | **Trần Hữu Thiện** | **Backend & Database Developer** | \- Thiết kế cơ sở dữ liệu (ERD) quản lý Danh mục, Sản phẩm, Biến thể (Size/Màu/Tồn kho), Đơn hàng và Người dùng. \- Xây dựng RESTful API xử lý nghiệp vụ: tìm kiếm/lọc sản phẩm, kiểm tra tồn kho theo Size/Màu, tính tổng tiền/voucher, lưu đơn hàng và cập nhật trạng thái đơn. \- Thiết lập cơ chế xác thực, phân quyền (Khách hàng / Quản trị viên) và bảo mật dữ liệu. |
| 5 | **Nguyễn Quỳnh Thiên An** | **QA / Integration & Documentation** | \- Lập kế hoạch kiểm thử (Test Plan) và viết kịch bản kiểm thử (Test Cases) bám sát luồng mua hàng và xử lý đơn. \- Phối hợp tích hợp giữa Frontend và Backend; kiểm thử chức năng, giao diện và xử lý lỗi. \- Quản lý nhật ký sử dụng AI (AI\_USAGE\_LOG.md), quy tắc AI (AGENTS.md) và rà soát tài liệu dự án trước khi nộp. |

## **2\. Các giai đoạn**

Dự án được chia thành 6 giai đoạn tuần tự gắn liền với tiến độ các buổi học thực hành:

### **Giai đoạn 1: Khảo sát và xác định yêu cầu (Tuần 1 \- Buổi 1\)**

* Chốt đề tài "Website bán hàng quần áo thời trang \- Hotmate", xác định khách hàng mục tiêu và vấn đề kinh doanh.  
* Khảo sát tối thiểu 3 website thời trang đối thủ để rút ra bài học thiết kế và chức năng.  
* Xác định vai trò người dùng (docs/user-roles.md), quy trình nghiệp vụ mua hàng & xử lý đơn (docs/business-workflow.md).  
* Khởi tạo GitHub Repository dùng chung và hoàn thiện bộ tài liệu khởi tạo dự án (README.md, REQUIREMENTS.md, PROJECT\_PLAN.md, AGENTS.md, AI\_USAGE\_LOG.md).

### **Giai đoạn 2: Thiết kế giao diện (Tuần 2\)**

* Xây dựng sơ đồ cấu trúc website (Site Map) cho phân hệ Khách hàng và Quản trị viên.  
* Thiết kế khung bố cục (Wireframe) và giao diện chi tiết (UI Mockup) cho các màn hình chính.  
* Chuẩn hóa bộ quy tắc thiết kế (Design System): bảng màu thương hiệu Hotmate, typography, hệ thống lưới (Grid) và thu thập hình ảnh mẫu quần áo thời trang.

### **Giai đoạn 3: Xây dựng các chức năng frontend (Tuần 3 \- Tuần 4\)**

* Thiết lập cấu trúc thư mục Frontend và CSS dùng chung (common.css, Header, Footer, Navigation).  
* Cắt ghép giao diện tĩnh và lập trình tương tác JavaScript cho các trang của Khách hàng: Trang chủ, Danh mục & Bộ lọc sản phẩm, Chi tiết sản phẩm (chọn Size, Màu sắc, xem Bảng quy đổi kích cỡ), Giỏ hàng và Thanh toán (Checkout).  
* Xây dựng giao diện trang Quản trị (Admin Dashboard): Quản lý sản phẩm, kiểm tra tồn kho và cập nhật trạng thái đơn hàng.

### **Giai đoạn 4: Phát triển backend và cơ sở dữ liệu (Tuần 4 \- Tuần 5\)**

* Thiết kế lược đồ cơ sở dữ liệu (Database Schema) đáp ứng bài toán biến thể sản phẩm thời trang (1 mẫu áo/quần có nhiều Size và Màu sắc với số lượng tồn kho riêng).  
* Khởi tạo máy chủ Backend, cấu hình kết nối cơ sở dữ liệu và tạo dữ liệu mẫu (Seed data).  
* Xây dựng các API cốt lõi: API Danh mục & Sản phẩm, API Kiểm tra tồn kho & Đặt hàng (trừ tồn kho khi tạo đơn), API Tra cứu & Cập nhật trạng thái đơn hàng (Chờ xác nhận $\rightarrow$ Đang chuẩn bị hàng $\rightarrow$ Đang giao hàng $\rightarrow$ Giao thành công), API Đăng nhập/Đăng ký.

### **Giai đoạn 5: Tích hợp và kiểm thử (Tuần 6\)**

* Kết nối giao diện Frontend với các API Backend (thay thế dữ liệu tĩnh bằng dữ liệu động từ CSDL).  
* Thực hiện kiểm thử tích hợp toàn bộ luồng nghiệp vụ chính (Customer Order Workflow & Admin Order Fulfillment Workflow).  
* Kiểm thử các trường hợp ngoại lệ (hết size/màu, nhập sai thông tin nhận hàng, giỏ hàng trống, lỗi thanh toán) và sửa lỗi (Bug fixing).

### **Giai đoạn 6: Triển khai và hoàn thiện (Tuần 7 \- Cuối kỳ)**

* Tối ưu hóa hiệu năng, giao diện Responsive và rà soát bảo mật cơ bản (ẩn biến môi trường, kiểm tra dữ liệu đầu vào).  
* Triển khai (Deploy) ứng dụng lên môi trường chạy thực tế hoặc đóng gói hoàn chỉnh trên GitHub.  
* Hoàn thiện tài liệu báo cáo cuối kỳ, cập nhật đầy đủ AI\_USAGE\_LOG.md và chuẩn bị slide thuyết trình bảo vệ đồ án.

## **3\. Công việc**

Bảng phân công và theo dõi chi tiết các hạng mục công việc (mapping với GitHub Issues):

| Mã công việc | Tên công việc | Người phụ trách | Kết quả cần đạt (Deliverables) | Thời hạn | Trạng thái |
| :---- | :---- | :---- | :---- | :---- | :---- |
| **TASK-01** | Khảo sát website đối thủ ngành thời trang | Bích Hà, Huỳnh Như | File docs/competitor-analysis.md phân tích tối thiểu 3 website thời trang. | Buổi 1 (Tuần 1\) | Đã hoàn thành |
| **TASK-02** | Xác định vai trò người dùng và yêu cầu hệ thống | Bích Hà | Hoàn thiện file REQUIREMENTS.md và docs/user-roles.md. | Buổi 1 (Tuần 1\) | Đã hoàn thành |
| **TASK-03** | Mô tả quy trình nghiệp vụ mua hàng & xử lý đơn | Thành Trình, Thiên An | Hoàn thiện file docs/business-workflow.md kèm sơ đồ Flowchart & Sequence Diagram. | Buổi 1 (Tuần 1\) | Đã hoàn thành |
| **TASK-04** | Thiết lập GitHub Repo và bộ tài liệu khởi tạo | Bích Hà, Hữu Thiện, Thiên An | Public Repo gồm README.md, PROJECT\_PLAN.md, AGENTS.md, AI\_USAGE\_LOG.md, .gitignore và tạo các GitHub Issues ban đầu. | Buổi 1 (Tuần 1\) | Đang thực hiện |
| **TASK-05** | Thiết kế Sitemap, Wireframe và UI Kit cho Hotmate | Huỳnh Như | Bản vẽ Figma gồm Sitemap, Wireframe các trang chính và thư mục tài nguyên hình ảnh quần áo mẫu. | Tuần 2 | Chưa bắt đầu |
| **TASK-06** | Thiết kế CSDL (Database Schema) & Khởi tạo Backend | Hữu Thiện | Sơ đồ CSDL (quản lý sản phẩm, biến thể Size/Màu, đơn hàng), cấu trúc thư mục backend/ và dữ liệu mẫu. | Tuần 3 | Chưa bắt đầu |
| **TASK-07** | Xây dựng giao diện Khung dùng chung, Trang chủ & Danh mục | Huỳnh Như, Thành Trình | Các trang index.html, products.html, thanh tìm kiếm, bộ lọc theo giá/size/màu và CSS dùng chung. | Tuần 3 | Chưa bắt đầu |
| **TASK-08** | Xây dựng giao diện Chi tiết sản phẩm, Giỏ hàng & Checkout | Thành Trình | Các trang product-detail.html (chọn Size/Màu, bảng size), cart.html, checkout.html và order-tracking.html. | Tuần 4 | Chưa bắt đầu |
| **TASK-09** | Xây dựng giao diện Quản trị viên (Admin Dashboard) | Huỳnh Như, Thành Trình | Phân hệ admin/ gồm trang quản lý sản phẩm/tồn kho và trang quản lý, cập nhật trạng thái đơn hàng. | Tuần 4 | Chưa bắt đầu |
| **TASK-10** | Phát triển API Sản phẩm, Danh mục & Kiểm tra tồn kho | Hữu Thiện | Các API lấy danh sách sản phẩm, lọc theo danh mục/size/màu, xem chi tiết và kiểm tra số lượng tồn kho. | Tuần 4 | Chưa bắt đầu |
| **TASK-11** | Phát triển API Đặt hàng, Quản lý đơn & Xác thực | Hữu Thiện | API tạo đơn hàng (trừ tồn kho), áp dụng voucher, tra cứu trạng thái đơn và API Admin duyệt/hủy đơn. | Tuần 5 | Chưa bắt đầu |
| **TASK-12** | Tích hợp Frontend \- Backend và Kiểm thử hệ thống | Thiên An (chủ trì), Cả nhóm | Website hoạt động xuyên suốt luồng đặt hàng; danh sách Test Cases và biên bản sửa lỗi. | Tuần 6 | Chưa bắt đầu |
| **TASK-13** | Triển khai (Deploy), đóng gói tài liệu & Báo cáo cuối kỳ | Cả nhóm | Link sản phẩm chạy ổn định, mã nguồn sạch trên GitHub, hoàn tất tài liệu và slide báo cáo. | Tuần 7 | Chưa bắt đầu |

## **4\. Rủi ro**

Dưới đây là danh sách các rủi ro tiềm ẩn khi triển khai dự án website thời trang **Hotmate** cùng phương án phòng ngừa và xử lý của nhóm:

| Mã rủi ro | Mô tả rủi ro | Mức độ ảnh hưởng | Phương án phòng ngừa và xử lý |
| :---- | :---- | :---- | :---- |
| **RISK-01** | **Lan man phạm vi dự án (Scope Creep):** Nhóm ôm đồm quá nhiều tính năng phức tạp (như tích hợp API giao hàng thực tế GHN/GHTK, cổng thanh toán thật, livestream, gợi ý size bằng AI) dẫn đến không kịp tiến độ. | Cao | \- Bám sát phạm vi phiên bản đầu tiên (MVP) đã chốt trong REQUIREMENTS.md và docs/business-workflow.md. \- Chỉ mô phỏng bước thanh toán online và ghi nhận trạng thái vận chuyển trên hệ thống; ưu tiên hoàn thiện luồng cốt lõi trước khi làm tính năng nâng cao. |
| **RISK-02** | **Phức tạp khi xử lý biến thể sản phẩm (Size & Màu sắc) và lệch tồn kho:** Ngành thời trang yêu cầu quản lý tồn kho theo từng cặp (Màu \+ Size). Dễ xảy ra lỗi khách đặt vượt quá số lượng tồn hoặc quên trừ/cộng lại kho khi đặt/hủy đơn. | Cao | \- Thiết kế bảng biến thể sản phẩm (Product\_Variants) tách biệt rõ ràng trong CSDL ngay từ Giai đoạn 2 & 4\. \- Kiểm tra tồn kho ở cả 2 bước: khi thêm vào giỏ hàng và khi bấm "Xác nhận đặt hàng" ở Backend. Viết Test Case kỹ cho trường hợp hết hàng. |
| **RISK-03** | **Chậm trễ khi tích hợp giữa Frontend và Backend:** Dữ liệu trả về từ API không khớp với cấu trúc hiển thị ở giao diện hoặc lỗi CORS, làm tắc nghẽn Giai đoạn 5\. | Trung bình \- Cao | \- Thành Trình (Frontend) và Hữu Thiện (Backend) thống nhất cấu trúc dữ liệu JSON (API Contract) ngay từ đầu Giai đoạn 3\. \- Frontend sử dụng dữ liệu giả lập (Mock JSON) đúng cấu trúc đã hẹn trong lúc chờ Backend hoàn thiện API. |
| **RISK-04** | **Xung đột mã nguồn (Git Merge Conflicts) và mất dữ liệu:** Các thành viên sửa chung một file trên GitHub mà không đồng bộ trước, dẫn đến ghi đè code của nhau. | Trung bình | \- Phân chia file/thư mục rõ ràng cho từng thành viên; làm việc trên các nhánh (branch) riêng theo từng tính năng/Issue. \- Thực hiện git pull trước khi code và tạo Pull Request để Trưởng nhóm/QA review trước khi gộp vào nhánh chính (main). |
| **RISK-05** | **Phụ thuộc quá mức vào AI hoặc lộ thông tin nhạy cảm:** Thành viên giao phó toàn bộ việc viết code cho AI mà không hiểu bản chất, hoặc vô tình đẩy mật khẩu CSDL, API key lên Public Repository. | Cao | \- Tuân thủ nghiêm ngặt quy định trong AGENTS.md và ghi chép đầy đủ vào AI\_USAGE\_LOG.md; mọi đoạn code do AI gợi ý đều phải có thành viên đọc hiểu, kiểm tra và giải thích được. \- Cấu hình file .gitignore ngay từ đầu để loại trừ file .env, thư mục node\_modules và tuyệt đối không hard-code thông tin bảo mật. |
| **RISK-06** | **Chênh lệch khối lượng công việc và tiến độ cá nhân:** Một số thành viên bận lịch thi/học môn khác dẫn đến trễ hạn công việc phụ trách. | Trung bình | \- Chia nhỏ công việc theo từng tuần trên GitHub Issues; họp nhóm ngắn (15 phút/tuần) để cập nhật tiến độ. \- Áp dụng cơ chế hỗ trợ chéo (Pair Programming) khi có thành viên gặp khó khăn về kỹ thuật. |

