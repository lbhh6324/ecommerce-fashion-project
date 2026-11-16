# **NỘI DUNG TÀI LIỆU ĐẶC TẢ YÊU CẦU (REQUIREMENTS)**

## **1. Mục tiêu dự án**

| Loại mục tiêu | Nội dung |
| :---- | :---- |
| Mục tiêu kinh doanh | Xây dựng nền tảng website thương mại điện tử trực tiếp đến người tiêu dùng (D2C) cho thương hiệu thời trang nam HOTMATE. Website tập trung trưng bày hai dòng sản phẩm chủ lực Basics và Smart Casual, hướng đến nhóm khách hàng nam giới từ 18–40 tuổi, bao gồm Gen Z, Millennials và nhân viên văn phòng. Dự án hướng đến việc mở rộng kênh bán hàng trực tuyến, chủ động thu thập dữ liệu khách hàng sơ cấp (First-party Data), chuẩn hóa quy trình quản lý sản phẩm, tồn kho và đơn hàng trên một hệ thống tập trung. |
| Giá trị mang lại cho khách hàng | Cung cấp nền tảng mua sắm trực tuyến thuận tiện, giúp khách hàng dễ dàng tìm kiếm và lựa chọn trang phục nam theo danh mục, khoảng giá, kích cỡ và màu sắc. Khách hàng có thể xem thông tin chất liệu, hướng dẫn chọn size, chính sách đổi trả trong 15 ngày và tra cứu minh bạch 100% cấu phần chi phí sản xuất của sản phẩm. Đồng thời, hệ thống hỗ trợ quản lý giỏ hàng, đặt hàng trực tuyến và theo dõi trạng thái đơn hàng. |
| Mục tiêu vận hành | Xây dựng hệ thống quản lý tập trung cho Admin, hỗ trợ quản lý danh mục, sản phẩm, biến thể kích cỡ/màu sắc, số lượng tồn kho và đơn hàng. Từng bước chuẩn hóa quy trình từ trưng bày sản phẩm, tiếp nhận đơn hàng đến xử lý và cập nhật trạng thái giao hàng. |
| Mục tiêu kỹ thuật | Phát triển website có cấu trúc rõ ràng, giao diện đáp ứng trên máy tính và điện thoại, có khả năng kết nối Frontend với Backend thông qua API và lưu trữ dữ liệu trong cơ sở dữ liệu. Đảm bảo các chức năng cốt lõi hoạt động thống nhất, dữ liệu được kiểm tra hợp lệ và quyền truy cập được kiểm soát theo vai trò. |

## **2. Phạm vi dự án**

Dự án được triển khai theo lộ trình Giai đoạn 1 – MVP (Minimum Viable Product), tập trung xây dựng những chức năng thiết yếu để kiểm chứng mô hình kinh doanh D2C của HOTMATE trên website. Phạm vi ưu tiên dòng thời trang nam, hai nhóm sản phẩm Basics và Smart Casual, cùng quy trình mua hàng và quản trị đơn hàng cơ bản.

### **2.1. Các chức năng trong phạm vi triển khai (MVP)**

| STT | Nhóm chức năng | Nội dung triển khai |
| :---- | :---- | :---- |
| 1 | Trang chủ và danh mục | Xây dựng trang chủ giới thiệu thương hiệu HOTMATE, câu chuyện thương hiệu và các danh mục thời trang nam gồm: Áo thun Basics; Áo Polo và Sơ mi; Quần dài và Quần Short; Phụ kiện. Hỗ trợ người dùng điều hướng giữa các danh mục. |
| 2 | Hiển thị sản phẩm | Hiển thị danh sách sản phẩm theo trang chủ hoặc danh mục được lựa chọn. Mỗi sản phẩm có hình ảnh, tên, giá bán và thông tin chất liệu như Cotton, Upcycled Wool. Danh sách sản phẩm được cập nhật theo dữ liệu trong cơ sở dữ liệu. |
| 3 | Tìm kiếm và lọc sản phẩm | Cho phép tìm kiếm sản phẩm theo từ khóa tên sản phẩm; lọc theo danh mục, khoảng giá và kích cỡ. Kết quả phải phản ánh chính xác các điều kiện lọc và hiển thị thông báo khi không có sản phẩm phù hợp. |
| 4 | Chi tiết sản phẩm và minh bạch giá | Hiển thị hình ảnh, tên, giá bán, mô tả chất liệu, thông tin sản phẩm và các tùy chọn kích cỡ, màu sắc. Cung cấp bảng hướng dẫn chọn size, chính sách đổi trả 15 ngày và bảng minh bạch cấu phần chi phí sản xuất gồm vải, nhân công và vận chuyển. Cho phép khách hàng lựa chọn biến thể trước khi thêm sản phẩm vào giỏ hàng. |
| 5 | Tài khoản người dùng | Hỗ trợ đăng ký, đăng nhập và xác thực tài khoản. Hệ thống phân biệt quyền truy cập giữa Khách hàng và Quản trị viên; điều hướng người dùng đến giao diện phù hợp với vai trò sau khi đăng nhập thành công. |
| 6 | Giỏ hàng | Cho phép khách hàng thêm sản phẩm theo kích cỡ và màu sắc đã chọn, thay đổi số lượng, xóa sản phẩm và tự động tính tổng tiền. Giỏ hàng phải lưu đúng thông tin từng biến thể, đơn giá và số lượng sản phẩm, cho phép nhập mã giảm giá (voucher) hợp lệ để tính lại tổng tiền. |
| 7 | Đặt hàng | Cho phép khách hàng kiểm tra giỏ hàng, nhập họ tên, số điện thoại, email, địa chỉ nhận hàng, ghi chú và lựa chọn phương thức vận chuyển cùng phương thức thanh toán: Thanh toán khi nhận hàng (COD) hoặc Thanh toán trực tuyến (Chuyển khoản QR Code, Ví điện tử MoMo/VNPay). Với thanh toán trực tuyến, hệ thống chuyển hướng sang cổng thanh toán để hoàn tất giao dịch; sau đó kiểm tra thông tin, xác nhận tồn kho và tạo đơn hàng khi dữ liệu hợp lệ. |
| 8 | Theo dõi và quản lý đơn hàng | Cho phép khách hàng xem lịch sử mua hàng, thông tin chi tiết và trạng thái đơn hàng của chính mình. Khách hàng được hủy đơn khi đơn hàng còn ở trạng thái "Chờ xác nhận". Admin được xem toàn bộ đơn hàng và cập nhật trạng thái xử lý. |
| 9 | Quản trị hệ thống | Cung cấp giao diện quản trị cho Admin để thêm, sửa, xóa danh mục và sản phẩm; cập nhật hình ảnh, giá bán, chất liệu, biến thể kích cỡ/màu sắc, bảng minh bạch chi phí và số lượng tồn kho. Hỗ trợ xem chi tiết đơn hàng và cập nhật trạng thái xử lý đơn. |

### **2.2. Các chức năng ngoài phạm vi triển khai**

| STT | Chức năng | Lý do chưa triển khai trong đồ án |
| :---- | :---- | :---- |
| 1 | Hệ thống AI Smart Fit tư vấn kích cỡ | Thuộc lộ trình phát triển giai đoạn sau, đòi hỏi dữ liệu đo lường và lịch sử mua sắm đủ lớn, cùng mô hình trí tuệ nhân tạo vượt quá phạm vi và nguồn lực của học phần. |
| 2 | Hệ sinh thái hội viên HOTMATE Club và tích điểm Mate Cash | Là nhóm tính năng chăm sóc và giữ chân khách hàng nâng cao. Nhóm ưu tiên hoàn thiện quy trình mua hàng và quản lý đơn hàng cốt lõi trước. |
| 3 | Đồng bộ đa kênh qua API TikTok Shop, Shopee Mall và 04 showroom O2O | Yêu cầu tích hợp với các nền tảng bên thứ ba và đồng bộ dữ liệu bán hàng, tồn kho đa kênh. Nội dung này vượt quá phạm vi triển khai của đồ án. |
| 4 | Tích hợp API đơn vị vận chuyển thực tế (GHN, GHTK) | Việc giao nhận thực tế chỉ được ghi nhận qua trạng thái đơn hàng trên hệ thống, chưa đề xuất kết nối vận đơn tự động với đơn vị vận chuyển bên thứ ba. |
| 5 | Mở rộng danh mục thời trang nữ và Activewear | Không thuộc đối tượng sản phẩm trọng tâm của MVP. Dự án tập trung kiểm chứng mô hình kinh doanh với các dòng thời trang nam trước khi mở rộng danh mục. |

Nguyên tắc xác định phạm vi: Các chức năng chưa được liệt kê trong phạm vi MVP không tự động được xem là yêu cầu bắt buộc. Mọi đề xuất mở rộng phải được nhóm xem xét và thống nhất trước khi triển khai.

## **3. Người dùng hệ thống**

Hệ thống phục vụ ba nhóm người dùng chính. Nhiệm vụ và quyền hạn chi tiết được quy định tại tài liệu docs/user-roles.md.

| STT | Vai trò | Mô tả |
| :---- | :---- | :---- |
| 1 | Khách chưa đăng nhập (Guest) | Là người truy cập website HOTMATE nhưng chưa đăng nhập tài khoản. Có thể xem trang chủ, danh mục, tìm kiếm, lọc sản phẩm và xem thông tin chi tiết, bao gồm chất liệu, bảng minh bạch chi phí và chính sách đổi trả. Không được thực hiện các chức năng yêu cầu tài khoản như đặt hàng và xem lịch sử đơn hàng. |
| 2 | Khách hàng (Customer) | Là người đã đăng ký và đăng nhập tài khoản trên hệ thống, thuộc nhóm khách hàng mục tiêu của HOTMATE. Có thể quản lý thông tin cá nhân, lựa chọn sản phẩm, quản lý giỏ hàng, đặt hàng, xem lịch sử và theo dõi trạng thái đơn hàng. Chỉ được truy cập dữ liệu gắn với tài khoản của mình. |
| 3 | Quản trị viên (Admin) | Là người phụ trách vận hành hệ thống HOTMATE. Có quyền quản lý danh mục, thông tin sản phẩm, biến thể kích cỡ/màu sắc, bảng minh bạch chi phí, tồn kho và toàn bộ đơn hàng. Chịu trách nhiệm cập nhật dữ liệu và trạng thái xử lý đơn hàng trên hệ thống. |

## **4. Yêu cầu chức năng (Functional Requirements)**

### **4.1. Bảng danh sách yêu cầu chức năng**

| Mã | Tên chức năng | Mô tả | Người sử dụng | Ưu tiên |
| :---- | :---- | :---- | :---- | :---- |
| F01 | Xem danh sách sản phẩm | Hiển thị danh sách sản phẩm thời trang nam trên trang chủ hoặc theo danh mục được lựa chọn. Mỗi sản phẩm cần có hình ảnh, tên, giá bán và thông tin chất liệu cơ bản. | Guest, Customer | Bắt buộc |
| F02 | Xem chi tiết sản phẩm | Hiển thị đầy đủ thông tin sản phẩm gồm hình ảnh, tên, giá bán, mô tả chất liệu, biến thể kích cỡ và màu sắc, bảng hướng dẫn chọn size, chính sách đổi trả 15 ngày và bảng minh bạch cấu phần chi phí sản xuất. | Guest, Customer | Bắt buộc |
| F03 | Tìm kiếm và lọc sản phẩm | Cho phép tìm kiếm sản phẩm theo tên và lọc kết quả theo danh mục, khoảng giá và kích cỡ. Kết quả phải được cập nhật theo điều kiện tìm kiếm và lọc của người dùng. | Guest, Customer | Bắt buộc |
| F04 | Đăng ký và đăng nhập | Cho phép người dùng tạo tài khoản, đăng nhập và xác thực danh tính. Hệ thống kiểm tra thông tin đầu vào, xác định vai trò và điều hướng đến giao diện tương ứng sau khi đăng nhập thành công. | Guest, Customer, Admin | Bắt buộc |
| F05 | Quản lý giỏ hàng | Cho phép khách hàng thêm sản phẩm theo biến thể kích cỡ, màu sắc; thay đổi số lượng, xóa sản phẩm, áp dụng mã giảm giá (voucher) cơ bản và tự động tính tổng giá trị giỏ hàng. | Customer, Guest (giỏ tạm) | Bắt buộc |
| F06 | Đặt hàng | Cho phép khách hàng xác nhận giỏ hàng, nhập thông tin người nhận, lựa chọn phương thức thanh toán được hỗ trợ (COD hoặc Thanh toán trực tuyến qua Chuyển khoản QR Code, Ví điện tử MoMo/VNPay) và tạo đơn hàng. Với đơn thanh toán trực tuyến, hệ thống chuyển hướng sang cổng thanh toán để hoàn tất giao dịch trước khi kiểm tra tính hợp lệ của thông tin, trạng thái tồn kho và lưu đơn hàng với trạng thái ban đầu. | Customer | Bắt buộc |
| F07 | Theo dõi và hủy đơn hàng | Cho phép khách hàng xem danh sách, chi tiết và trạng thái các đơn hàng đã đặt. Khách hàng chỉ được hủy đơn khi đơn hàng đang ở trạng thái "Chờ xác nhận". | Customer | Bắt buộc |
| F08 | Quản lý sản phẩm và danh mục | Cho phép Admin thêm, sửa, xóa danh mục và sản phẩm; cập nhật hình ảnh, giá bán, chất liệu, biến thể kích cỡ/màu sắc, bảng minh bạch chi phí sản xuất và số lượng tồn kho. | Admin | Bắt buộc |
| F09 | Quản lý đơn hàng | Cho phép Admin xem danh sách, chi tiết toàn bộ đơn hàng và cập nhật trạng thái xử lý. Trạng thái mới phải được đồng bộ để khách hàng có thể theo dõi trên tài khoản của mình. | Admin | Bắt buộc |

### **4.2. Tiêu chí nghiệm thu (Acceptance Criteria)**

| Mã | Tiêu chí nghiệm thu |
| :---- | :---- |
| F01 | Hệ thống hiển thị tối thiểu 8 sản phẩm trên mỗi trang. Mỗi sản phẩm phải có hình ảnh, tên và giá bán. Khi người dùng chọn danh mục như Áo thun, Polo và Sơ mi, Quần hoặc Phụ kiện, danh sách phải cập nhật đúng các sản phẩm thuộc danh mục tương ứng. |
| F02 | Khi chọn một sản phẩm, hệ thống phải mở đúng trang chi tiết và hiển thị chính xác tên, giá bán, hình ảnh, chất liệu, chính sách đổi trả 15 ngày và bảng minh bạch cấu phần chi phí sản xuất. Trang phải có tùy chọn kích cỡ S, M, L, XL; màu sắc; bảng hướng dẫn chọn size và nút thêm vào giỏ hàng. Người dùng phải lựa chọn biến thể hợp lệ trước khi thêm sản phẩm. |
| F03 | Hệ thống cho phép tìm kiếm bằng từ khóa tên sản phẩm và lọc kết quả theo danh mục, khoảng giá và kích cỡ. Thời gian phản hồi kết quả tìm kiếm/lọc dưới 2 giây trong điều kiện kiểm thử của dự án. Khi không có kết quả phù hợp, hệ thống hiển thị thông báo rõ ràng. |
| F04 | Người dùng đăng ký thành công khi cung cấp email hợp lệ và mật khẩu đáp ứng độ dài tối thiểu theo quy định của hệ thống. Hệ thống thông báo lỗi khi email không hợp lệ, thông tin đăng nhập không chính xác hoặc trường bắt buộc bị bỏ trống. Sau khi đăng nhập thành công, người dùng được xác định đúng vai trò và điều hướng đến giao diện tương ứng. Mật khẩu không được lưu dưới dạng văn bản thuần trong cơ sở dữ liệu. |
| F05 | Sản phẩm trong giỏ hàng phải hiển thị đúng tên, kích cỡ, màu sắc, đơn giá và số lượng. Khi người dùng thay đổi số lượng hoặc xóa sản phẩm, tổng giá trị giỏ hàng phải được tính toán và cập nhật chính xác. Không cho phép số lượng nhỏ hơn 1 hoặc vượt quá số lượng tồn kho của biến thể tương ứng. Khi khách hàng nhập mã giảm giá hợp lệ, hệ thống tự động trừ số tiền ưu đãi tương ứng vào tổng giá trị giỏ hàng; nếu mã không hợp lệ hoặc hết hạn thì hiển thị thông báo lỗi và lúc này tổng giá trị giỏ hàng không thay đổi.  |
| F06 | Hệ thống không cho phép đặt hàng khi giỏ hàng trống hoặc thiếu họ tên, số điện thoại và địa chỉ giao hàng. Nếu khách hàng chọn thanh toán trực tuyến (Chuyển khoản QR Code, Ví điện tử MoMo/VNPay), hệ thống chuyển hướng sang cổng thanh toán để xử lý giao dịch; trường hợp thanh toán thất bại sẽ hiển thị thông báo lỗi và yêu cầu thử lại. Khi giao dịch thanh toán thành công (hoặc chọn COD), hệ thống kiểm tra lại số lượng tồn kho của từng biến thể; nếu hợp lệ và đủ hàng thì tạo mã đơn hàng, lưu thông tin sản phẩm, số lượng, đơn giá, phí vận chuyển, tổng tiền, thông tin giao hàng và phương thức thanh toán với trạng thái ban đầu là "Chờ xác nhận". Giỏ hàng được làm trống sau khi tạo đơn thành công và số lượng tồn kho được trừ tương ứng. |
| F07 | Hệ thống chỉ hiển thị các đơn hàng thuộc tài khoản đang đăng nhập, bao gồm mã đơn, ngày đặt, danh sách sản phẩm, tổng tiền và trạng thái xử lý. Khách hàng được hủy đơn khi trạng thái là "Chờ xác nhận". Khi đơn bị hủy thành công, trạng thái phải được cập nhật và số lượng tồn kho đã trừ phải được hoàn lại theo đúng biến thể sản phẩm. Không cho phép khách hàng hủy đơn đã chuyển sang giai đoạn xử lý tiếp theo. |
| F08 | Admin có thể thêm, sửa, xóa danh mục và sản phẩm; cập nhật giá bán, hình ảnh, chất liệu, kích cỡ, màu sắc, thông số bảng minh bạch chi phí và tồn kho. Dữ liệu sau khi cập nhật phải được đồng bộ trên giao diện khách hàng. Hệ thống không cho phép lưu sản phẩm khi thiếu tên, giá bán không hợp lệ hoặc số lượng tồn kho âm. Tài khoản không có vai trò Admin không được thực hiện các thao tác này. |
| F09 | Admin xem được danh sách và chi tiết toàn bộ đơn hàng, bao gồm thông tin người nhận, sản phẩm, biến thể, số lượng và tổng tiền. Admin có thể cập nhật trạng thái đơn hàng theo quy trình xử lý. Khi trạng thái thay đổi, thông tin mới phải được lưu trong hệ thống và hiển thị đồng bộ trên trang theo dõi đơn hàng của khách hàng. Người dùng không có quyền Admin không được gọi chức năng cập nhật trạng thái đơn hàng. |

### **4.3. Quy định trạng thái đơn hàng**

Để thống nhất giữa chức năng đặt hàng, quản lý đơn hàng và theo dõi đơn hàng, hệ thống sử dụng các trạng thái sau:

| Trạng thái | Ý nghĩa | Quyền cập nhật |
| :---- | :---- | :---- |
| Chờ xác nhận | Đơn hàng vừa được tạo thành công và đang chờ Admin tiếp nhận, xác nhận. | Hệ thống tự động tạo; Customer được phép hủy. |
| Đang chuẩn bị hàng | Đơn hàng đã được Admin xác nhận và đang trong quá trình chuẩn bị sản phẩm. | Admin |
| Đang giao hàng | Đơn hàng đã được bàn giao cho đơn vị vận chuyển hoặc chuyển sang bước giao hàng mô phỏng. | Admin |
| Giao thành công | Đơn hàng đã hoàn tất quá trình giao hàng. | Admin |
| Đã hủy | Đơn hàng đã bị hủy theo quy trình được hệ thống cho phép. | Customer khi đơn còn Chờ xác nhận; Admin theo nghiệp vụ quản trị. |

Luồng trạng thái chính:

Chờ xác nhận → Đang chuẩn bị hàng → Đang giao hàng → Giao thành công.

Trường hợp hủy: Chờ xác nhận → Đã hủy.

Việc cập nhật trạng thái phải được kiểm soát để tránh chuyển trạng thái không hợp lệ. Khi đơn hàng bị hủy và tồn kho đã được trừ, hệ thống phải hoàn lại số lượng cho đúng biến thể sản phẩm.

### **4.4. Bảng phân nhóm chức năng theo nghiệp vụ**

| Nhóm nghiệp vụ | Đối tượng phục vụ | Mã chức năng tương ứng |
| :---- | :---- | :---- |
| Nhóm 1: Trưng bày và tìm kiếm sản phẩm | Guest và Customer | F01, F02, F03 |
| Nhóm 2: Tài khoản và mua hàng | Customer; Guest ở bước đăng ký/đăng nhập | F04, F05, F06, F07 |
| Nhóm 3: Quản trị hệ thống | Admin | F08, F09 |

### **4.5. Luồng nghiệp vụ cốt lõi**

Luồng mua hàng của khách hàng:

1\. 	Khách truy cập website và xem danh sách sản phẩm (F01).

2\. 	Tìm kiếm hoặc lọc sản phẩm theo nhu cầu (F03).

3\. 	Chọn sản phẩm và xem thông tin chi tiết, bảng minh bạch chi phí (F02).

4\. 	Chọn kích cỡ, màu sắc và thêm sản phẩm vào giỏ hàng (F05).

5\. 	Đăng nhập hoặc đăng ký tài khoản nếu chưa xác thực (F04).

6\. 	Kiểm tra giỏ hàng, nhập thông tin giao hàng, chọn phương thức thanh toán (COD hoặc Thanh toán trực tuyến qua Chuyển khoản QR Code, Ví điện tử MoMo/VNPay) và xác nhận đặt hàng (F06).

7\. 	Nếu thanh toán trực tuyến, hệ thống chuyển hướng sang cổng thanh toán để hoàn tất giao dịch; khi thanh toán thành công (hoặc chọn COD), hệ thống kiểm tra tồn kho, lưu đơn hàng vào cơ sở dữ liệu với trạng thái "Chờ xác nhận", trừ tồn kho và gửi thông báo/Email xác nhận mã đơn hàng.

8\. 	Admin tiếp nhận và xử lý đơn hàng, cập nhật trạng thái (F09).

9\. 	Khách hàng theo dõi trạng thái đơn hàng trên tài khoản cá nhân (F07).

Luồng quản trị đơn hàng:

1\. 	Admin đăng nhập vào hệ thống.

2\. 	Truy cập danh sách đơn hàng và xem chi tiết đơn.

3\. 	Kiểm tra thông tin sản phẩm, biến thể, số lượng và thông tin người nhận.

4\. 	Cập nhật trạng thái xử lý đơn theo quy trình.

5\. 	Hệ thống lưu trạng thái mới và đồng bộ thông tin để khách hàng theo dõi.

## **5. Yêu cầu phi chức năng (Non-Functional Requirements)**

| STT | Nhóm yêu cầu | Nội dung chi tiết |
| :---- | :---- | :---- |
| 1 | Giao diện đáp ứng đa thiết bị (Responsive) | Website phải hiển thị rõ ràng, cân đối và phù hợp với nhận diện thương hiệu thời trang nam HOTMATE. Các trang chủ, danh sách sản phẩm, chi tiết sản phẩm, giỏ hàng, thanh toán và trang quản trị phải sử dụng được trên máy tính (Desktop) và điện thoại (Mobile), không bị vỡ bố cục hoặc che khuất nội dung quan trọng. |
| 2 | Kiểm tra dữ liệu đầu vào (Validation) | Các biểu mẫu đăng ký, đăng nhập, đặt hàng, thêm và chỉnh sửa sản phẩm phải kiểm tra tính hợp lệ trước khi lưu. Dữ liệu cần kiểm tra gồm email đúng định dạng, số điện thoại hợp lệ, trường bắt buộc không được bỏ trống, giá bán và số lượng tồn kho phải là số hợp lệ, không âm. Hệ thống phải hiển thị thông báo rõ ràng khi dữ liệu không hợp lệ. |
| 3 | Bảo mật và phân quyền | Chỉ tài khoản Admin được phép truy cập các chức năng quản trị F08 và F09. Khách hàng chỉ được xem và thao tác trên dữ liệu thuộc tài khoản của mình. Mật khẩu phải được băm an toàn trước khi lưu vào cơ sở dữ liệu. Các API cần kiểm tra xác thực và quyền truy cập; không công khai mật khẩu, API Key, thông tin kết nối cơ sở dữ liệu hoặc dữ liệu nhạy cảm trên repository GitHub. |
| 4 | Tổ chức mã nguồn và khả năng bảo trì | Cấu trúc dự án phải được phân chia rõ ràng giữa giao diện (Frontend), xử lý nghiệp vụ (Backend) và cơ sở dữ liệu. Các module và file cần được đặt tên nhất quán, hạn chế code trùng lặp, thuận tiện cho việc kiểm thử, tích hợp và bảo trì. Các thành viên phải tuân thủ quy tắc trong file AGENTS.md. |

## **6. Giới hạn và giả định (Constraints và Assumptions)**

### **6.1. Giới hạn của dự án**

| Loại giới hạn | Nội dung |
| :---- | :---- |
| Thời gian và nguồn lực | Dự án được thực hiện bởi nhóm 5 thành viên trong khuôn khổ thời gian của một học phần. Các thành viên đảm nhiệm những vai trò chính gồm Business Analyst, UI/UX Designer, Frontend Developer, Backend và Database Developer và QA/Integration và Documentation. Vì vậy, nhóm tập trung hoàn thiện phiên bản MVP, ưu tiên các chức năng mua hàng và quản trị cốt lõi thay vì triển khai toàn bộ hệ sinh thái HOTMATE trong dài hạn. |
| Công nghệ | Hệ thống được xây dựng bằng HTML5, CSS3 và JavaScript cho giao diện, kết hợp Backend và cơ sở dữ liệu phù hợp với năng lực của nhóm. Backend cung cấp các API phục vụ truy xuất sản phẩm, kiểm tra tồn kho, xác thực, đặt hàng và cập nhật trạng thái đơn. Công nghệ hoặc framework cụ thể được thực hiện theo thống nhất của nhóm và cấu hình thực tế trong repository. |
| Phạm vi nghiệp vụ | Dự án tập trung vào thời trang nam thuộc hai dòng Basics và Smart Casual. Không triển khai các chức năng mở rộng như AI Smart Fit, hệ thống hội viên, đồng bộ đa kênh, showroom O2O và tích hợp API đơn vị vận chuyển thực tế. |
| Môi trường giao dịch | Hệ thống hỗ trợ luồng thanh toán COD và thanh toán trực tuyến qua cổng thanh toán (Chuyển khoản QR Code, Ví điện tử MoMo/VNPay) trong môi trường học tập, phục vụ mô phỏng và kiểm thử quy trình nghiệp vụ. Việc giao nhận vận chuyển được ghi nhận thông qua cập nhật trạng thái đơn hàng trên hệ thống. |
| Tích hợp hệ thống | Frontend và Backend cần thống nhất cấu trúc dữ liệu trao đổi qua API. Việc tích hợp phải được thực hiện theo từng giai đoạn để hạn chế lỗi không tương thích dữ liệu và ảnh hưởng đến tiến độ chung. |

### **6.2. Các giả định của dự án**

| STT | Giả định | Nội dung |
| :---- | :---- | :---- |
| 1 | Dữ liệu sản phẩm | Hình ảnh trang phục nam, tên sản phẩm, giá bán, mô tả chất liệu, kích cỡ, màu sắc và số liệu bảng minh bạch cấu phần chi phí sản xuất được sử dụng là dữ liệu mẫu phục vụ phát triển và kiểm thử. |
| 2 | Dữ liệu người dùng | Tài khoản khách hàng và quản trị viên sử dụng dữ liệu giả lập. Không sử dụng thông tin cá nhân thật của khách hàng bên ngoài trong quá trình phát triển và kiểm thử. |
| 3 | Dữ liệu giao dịch | Các đơn hàng được tạo trong quá trình kiểm thử là dữ liệu mô phỏng. Mã đơn hàng, thông tin người nhận, trạng thái và chi tiết sản phẩm được lưu nhằm đánh giá luồng đặt hàng và quản lý đơn. |
| 4 | Thanh toán | Hệ thống hỗ trợ phương thức thanh toán khi nhận hàng (COD) và thanh toán trực tuyến qua cổng thanh toán (Chuyển khoản QR Code, Ví điện tử MoMo/VNPay) phục vụ vận hành và kiểm thử quy trình nghiệp vụ. Hệ thống nhận kết quả phản hồi trạng thái giao dịch (thành công/thất bại) từ cổng thanh toán ở môi trường kiểm thử và không lưu trữ trực tiếp dữ liệu thanh toán nhạy cảm của khách hàng. |
| 5 | Tồn kho | Số lượng tồn kho ban đầu được thiết lập bằng dữ liệu mẫu. Mỗi biến thể sản phẩm theo kích cỡ và màu sắc có số lượng tồn kho riêng để phục vụ việc kiểm tra khả năng đặt hàng và cập nhật tồn kho. |
| 6 | Người vận hành | Admin là tài khoản được nhóm cấp quyền để thực hiện các chức năng quản trị trong môi trường đồ án. Việc cấp và thay đổi quyền quản trị phải được kiểm soát, không cho phép người dùng tự nâng quyền tài khoản. |

## **7. Tổng kết yêu cầu dự án**

| Hạng mục | Nội dung tổng hợp |
| :---- | :---- |
| Mục tiêu dự án | Xây dựng website thương mại điện tử D2C HOTMATE nhằm trưng bày sản phẩm thời trang nam, hỗ trợ mua sắm trực tuyến, thu thập dữ liệu khách hàng sơ cấp và quản lý đơn hàng tập trung. |
| Phạm vi triển khai | Phiên bản MVP tập trung vào hai dòng sản phẩm Basics và Smart Casual, bao gồm trưng bày sản phẩm, tìm kiếm/lọc, tài khoản, giỏ hàng, đặt hàng, theo dõi đơn và quản trị hệ thống. |
| Quy mô đặc tả | Gồm 09 yêu cầu chức năng (F01–F09), 03 nhóm người dùng, 03 nhóm nghiệp vụ chính và 04 nhóm yêu cầu phi chức năng. |
| Nhóm người dùng | Khách chưa đăng nhập (Guest), Khách hàng (Customer) và Quản trị viên (Admin). |
| Nhóm chức năng nghiệp vụ | Nhóm 1: Trưng bày và tìm kiếm sản phẩm; Nhóm 2: Tài khoản và mua hàng; Nhóm 3: Quản trị hệ thống. |
| Luồng nghiệp vụ cốt lõi | Xem danh sách sản phẩm (F01) → Tìm kiếm và lọc (F03) → Xem chi tiết và minh bạch chi phí (F02) → Đăng ký/đăng nhập (F04) → Quản lý giỏ hàng (F05) → Đặt hàng và kiểm tra tồn kho (F06) → Admin xử lý đơn hàng (F09) → Khách hàng theo dõi đơn hàng (F07). |
| Nguyên tắc bảo mật | Phân quyền theo vai trò, xác thực trước khi thực hiện chức năng yêu cầu tài khoản, bảo vệ dữ liệu cá nhân, kiểm soát quyền truy cập trang quản trị và bảo vệ thông tin xác thực. |
| Cơ sở nghiệm thu | Đối chiếu kết quả triển khai với mô tả chức năng, tiêu chí nghiệm thu F01–F09, yêu cầu phi chức năng và các luồng nghiệp vụ đã xác định. |

Đây là cơ sở để nhóm triển khai thiết kế giao diện, xây dựng cơ sở dữ liệu, phát triển Frontend và Backend, tích hợp hệ thống và thực hiện kiểm thử. Mọi chức năng phát sinh cần được đối chiếu với phạm vi MVP và thống nhất trước khi đưa vào triển khai.


