# **NỘI DUNG TÀI LIỆU PHÂN QUYỀN NGƯỜI DÙNG** 

Nhóm người dùng tham gia vào hệ thống website thương mại điện tử D2C HOTMATE, bao gồm nhiệm vụ, phạm vi truy cập và quyền hạn tương ứng của từng vai trò. Việc phân quyền nhằm đảm bảo người dùng chỉ được thực hiện những thao tác phù hợp với chức năng của mình, bảo vệ dữ liệu cá nhân và duy trì tính an toàn trong quá trình vận hành hệ thống.

## **1. Bảng phân quyền người dùng**

Hệ thống HOTMATE gồm ba nhóm người dùng chính: Khách chưa đăng nhập (Guest), Khách hàng (Customer) và Quản trị viên (Admin).

| Vai trò | Nhiệm vụ chính | Quyền hạn |
| :---- | :---- | :---- |
| Khách chưa đăng nhập (Guest) | Truy cập website HOTMATE để xem trang chủ, câu chuyện thương hiệu và các danh mục thời trang nam thuộc hai dòng Basics và Smart Casual. Tìm kiếm, lọc sản phẩm theo tên, danh mục, khoảng giá và kích cỡ. Xem thông tin chi tiết sản phẩm, hình ảnh, chất liệu, bảng minh bạch cấu phần chi phí sản xuất, chính sách đổi trả 15 ngày và hướng dẫn chọn kích cỡ. | Chỉ được xem và truy cập dữ liệu sản phẩm công khai. Được sử dụng chức năng tìm kiếm, lọc và xem chi tiết sản phẩm. Không được thực hiện thao tác đặt hàng, xem lịch sử đơn hàng, truy cập thông tin cá nhân hoặc sử dụng các chức năng quản trị. Khi muốn thực hiện chức năng yêu cầu tài khoản, người dùng phải đăng nhập hoặc đăng ký trước. |
| Khách hàng (Customer) | Đăng ký, đăng nhập và quản lý thông tin tài khoản cá nhân. Tìm kiếm, lựa chọn sản phẩm theo kích cỡ, màu sắc; quản lý giỏ hàng; cung cấp thông tin giao hàng; lựa chọn phương thức thanh toán (COD hoặc Thanh toán trực tuyến qua Chuyển khoản QR Code, MoMo/VNPay), thực hiện đặt hàng và theo dõi quá trình xử lý đơn hàng.  | Được xem và cập nhật thông tin hồ sơ cá nhân; thêm, sửa số lượng, xóa sản phẩm trong giỏ hàng của chính mình; chọn phương thức thanh toán, thao tác chuyển hướng cổng thanh toán (nếu thanh toán trực tuyến) để tạo đơn hàng; xem danh sách và chi tiết các đơn hàng đã đặt. Áp dụng mã giảm giá (nếu có)  |
| Quản trị viên (Admin) | Quản lý hoạt động kinh doanh trên website, bao gồm danh mục, thông tin sản phẩm, biến thể kích cỡ và màu sắc, bảng minh bạch cấu phần chi phí sản xuất, số lượng tồn kho. Tiếp nhận, kiểm tra và xử lý đơn hàng; cập nhật trạng thái đơn hàng trong quá trình vận hành. | Được truy cập trang quản trị; thêm, sửa, xóa danh mục và sản phẩm; cập nhật hình ảnh, giá bán, chất liệu, kích cỡ, màu sắc, thông số chi phí sản xuất và tồn kho. Được xem danh sách, chi tiết toàn bộ đơn hàng và cập nhật trạng thái xử lý đơn. Không bị giới hạn trong phạm vi dữ liệu của một khách hàng như vai trò Customer. |

Lưu ý về quyền hạn: Các thao tác quản trị phải được kiểm tra quyền tại Backend, không chỉ ẩn hoặc hiện nút chức năng trên giao diện. Việc truy cập trực tiếp vào đường dẫn quản trị hoặc gọi API quản trị bằng tài khoản không đủ quyền đều phải bị từ chối.

## **2. Vai trò và trách nhiệm của các thành viên dự án**

| STT | Thành viên | Vai trò trong dự án | Trách nhiệm chính |
| :---- | :---- | :---- | :---- |
| 1 | Lữ Bích Hà | Trưởng nhóm / Business Analyst (BA) | Quản lý tiến độ, điều phối công việc qua GitHub Issues; khảo sát đối thủ, phân tích yêu cầu nghiệp vụ; kiểm soát phạm vi và tổng hợp báo cáo. |
| 2 | Phạm Thiện Thiên Thành Trình | UI/UX Designer | Khảo sát giao diện website thời trang tham khảo; thiết kế Sitemap, Wireframe, Mockup trên Figma; chuẩn bị hình ảnh, banner, icon và quy chuẩn màu sắc, font chữ. |
| 3 | Trần Hữu Thiện | Frontend Developer | Xây dựng giao diện bằng HTML5, CSS3 và JavaScript, phát triển các chức năng phía khách hàng như bộ lọc, chọn kích cỡ/màu sắc, giỏ hàng, tích hợp luồng chọn phương thức thanh toán / chuyển hướng cổng thanh toán, đặt hàng và tra cứu đơn hàng; đảm bảo Responsive . |
| 4 | Nguyễn Quỳnh Thiên An | Backend & Database Developer | Thiết kế cơ sở dữ liệu; xây dựng RESTful API; xử lý tìm kiếm, lọc sản phẩm, kiểm tra tồn kho, tính tổng tiền, lưu đơn hàng, cập nhật trạng thái và thiết lập xác thực, phân quyền. |
| 5 | Huỳnh Thị Huỳnh Như | QA / Integration & Documentation | Lập kế hoạch và kịch bản kiểm thử; phối hợp tích hợp Frontend – Backend; kiểm thử chức năng, giao diện, xử lý lỗi; quản lý tài liệu và nhật ký sử dụng AI. |

 

## **3. Nguyên tắc kiểm soát truy cập**

| STT | Nguyên tắc | Mô tả hoạt động |
| :---- | :---- | :---- |
| 1 | Xác thực trước khi mua hàng | Khách chưa đăng nhập được phép xem, tìm kiếm sản phẩm và thêm sản phẩm vào giỏ hàng. Tuy nhiên, khi thực hiện các chức năng yêu cầu định danh như tiến hành thanh toán, chọn phương thức thanh toán (COD/Trực tuyến) hoặc xem lịch sử đơn hàng, hệ thống bắt buộc người dùng phải đăng nhập hoặc đăng ký tài khoản trước khi tiếp tục.  |
| 2 | Phân quyền theo vai trò | Hệ thống xác định quyền truy cập dựa trên vai trò Guest, Customer và Admin. Mỗi vai trò chỉ được phép thực hiện những chức năng đã được quy định; các yêu cầu không thuộc quyền hạn phải bị từ chối. |
| 3 | Bảo vệ dữ liệu cá nhân (First-party Data) | Mỗi khách hàng chỉ được phép xem và cập nhật hồ sơ, giỏ hàng và lịch sử đơn hàng gắn với tài khoản của chính mình. Hệ thống không cho phép khách hàng truy cập dữ liệu của tài khoản khác thông qua việc thay đổi mã người dùng hoặc mã đơn hàng trên URL hay API. |
| 4 | Phân tách khu vực quản trị | Chỉ tài khoản có vai trò Admin mới được phép truy cập trang quản trị và thực hiện các chức năng quản lý danh mục, sản phẩm, tồn kho và đơn hàng. Guest và Customer không được truy cập các chức năng này. |
| 5 | Kiểm soát trạng thái đơn hàng | Khách hàng chỉ được hủy đơn khi đơn hàng đang ở trạng thái "Chờ xác nhận". Khi đơn đã được chuyển sang trạng thái xử lý tiếp theo, chức năng hủy đơn không còn khả dụng đối với Customer. |
| 6 | Kiểm soát tồn kho theo biến thể | Số lượng tồn kho được quản lý theo từng biến thể kích cỡ và màu sắc. Hệ thống phải kiểm tra tồn kho trước khi tạo đơn hàng, không cho phép đặt vượt quá số lượng hiện có và cập nhật số lượng tồn kho theo kết quả xử lý đơn. |
| 7 | Bảo vệ thông tin xác thực | Mật khẩu phải được băm trước khi lưu vào cơ sở dữ liệu. Thông tin đăng nhập và dữ liệu nhạy cảm không được hiển thị công khai hoặc lưu trực tiếp trong mã nguồn. |

## **4. Tóm tắt luồng phân quyền hệ thống**

| Nhóm người dùng | Phạm vi chức năng chính | Mức độ quyền hạn |
| :---- | :---- | :---- |
| Khách chưa đăng nhập (Guest) | Xem trang chủ, duyệt danh mục, tìm kiếm, lọc sản phẩm, xem chi tiết sản phẩm, bảng minh bạch chi phí và chính sách đổi trả. | Chỉ xem (View Only) |
| Khách hàng (Customer) | Quản lý tài khoản cá nhân, quản lý giỏ hàng, đặt hàng, xem lịch sử, theo dõi và hủy đơn khi còn chờ xác nhận. | Mua hàng (Customer Access) |
| Quản trị viên (Admin) | Quản lý danh mục, sản phẩm, biến thể, thông số chi phí, tồn kho; xem và cập nhật trạng thái toàn bộ đơn hàng. | Quản trị hệ thống (Admin Access) |

## **5. Quy định kiểm soát quyền theo chức năng**

| Chức năng | Guest | Customer | Admin |
| :---- | :---- | :---- | :---- |
| Xem trang chủ và danh mục | Được phép | Được phép | Được phép |
| Xem danh sách và chi tiết sản phẩm | Được phép | Được phép | Được phép |
| Tìm kiếm và lọc sản phẩm | Được phép | Được phép | Được phép |
| Đăng ký và đăng nhập | Được phép đăng ký/đăng nhập | Được phép đăng nhập | Được phép đăng nhập |
| Quản lý thông tin cá nhân | Không được phép | Chỉ tài khoản của mình | Theo phạm vi quản trị được cấp |
| Quản lý giỏ hàng | Được phép thao tác giỏ tạm (thêm, sửa số lượng, xóa)  | Chỉ giỏ hàng của mình (bao gồm nhập mã giảm giá) | Không thuộc nghiệp vụ mua hàng của Admin |
| Đặt hàng | Không được phép | Được phép | Không thuộc nghiệp vụ mua hàng của Admin |
| Xem lịch sử và theo dõi đơn hàng | Không được phép | Chỉ đơn hàng của mình | Toàn bộ đơn hàng |
| Hủy đơn hàng | Không được phép | Chỉ đơn ở trạng thái Chờ xác nhận | Được xử lý theo nghiệp vụ quản trị |
| Quản lý danh mục và sản phẩm | Không được phép | Không được phép | Được phép |
| Quản lý biến thể và tồn kho | Không được phép | Không được phép | Được phép |
| Quản lý bảng minh bạch chi phí | Không được phép chỉnh sửa | Chỉ được xem | Được phép cập nhật |
| Cập nhật trạng thái đơn hàng | Không được phép | Không được phép | Được phép |
