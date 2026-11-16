# AI Usage Log – Dự án Website Thương mại Điện tử Thời trang HOTMATE

---

## Lần sử dụng 1: Phân tích nghiệp vụ và đề xuất yêu cầu hệ thống

### Công cụ

- **Tên công cụ AI:** Google Gemini

### Mục đích

- Phân tích bài toán kinh doanh, đề xuất mục tiêu, phạm vi dự án, phân quyền người dùng, danh sách yêu cầu chức năng/phi chức năng, quy trình nghiệp vụ và rủi ro triển khai cho website thời trang **HOTMATE**.

### Prompt

```text
Bạn là chuyên gia phân tích nghiệp vụ cho dự án thương mại điện tử.
Thông tin dự án:
- Tên dự án: Website thương mại điện tử thời trang HOTMATE (ecommerce-fashion-project)
- Sản phẩm hoặc dịch vụ: Kinh doanh các sản phẩm thời trang ứng dụng tối giản cho Nam giới (Basics và Smart Casual) theo định hướng thời trang bền vững và minh bạch chi phí sản xuất. Có tích hợp bán lẻ và bán combo.
- Khách hàng mục tiêu: Nam giới văn phòng trẻ (25–40 tuổi) ưu tiên tối giản, chất liệu bền bỉ và tiện lợi; Sinh viên & Gen Z (18–24 tuổi) nhạy bén công nghệ, thích minh bạch và mua combo.
- Vấn đề kinh doanh: Quần áo qua trung gian đội giá cao; khách băn khoăn form dáng dẫn đến e ngại chốt đơn/đổi trả nhiều; khách khó biết cấu thành chi phí thực sự và nguồn gốc chất liệu.
- Website tham khảo: Yody (yody.vn), Routine (routine.vn), Uniqlo (uniqlo.com)
- Thời gian thực hiện: 1 học phần (khoảng 10–12 tuần)
- Quy mô nhóm: 5 thành viên

Hãy đề xuất:
1. Mục tiêu và phạm vi dự án.
2. Các nhóm người dùng và quyền hạn.
3. Danh sách chức năng cần có.
4. Quy trình nghiệp vụ chính.
5. Yêu cầu phi chức năng.
6. Các chức năng nên hoàn thành ở phiên bản đầu tiên.
7. Các chức năng nâng cao có thể bổ sung.
8. Rủi ro khi triển khai và cách giảm thiểu.

Phân biệt rõ: Yêu cầu bắt buộc, Yêu cầu có thể phát triển sau, Đề xuất cần nhóm xác minh thêm. Không giả định nhóm có đủ thời gian hoặc năng lực để triển khai tất cả chức năng. Hãy giải thích cơ sở của từng đề xuất.
```

### Kết quả đề xuất

1. **Mục tiêu & Phạm vi:** Xây dựng website D2C **HOTMATE** giúp khách hàng mua trang phục nam, lọc sản phẩm theo màu/size, xem thông tin minh bạch chất liệu/chi phí; tích hợp công cụ chọn size và đặt hàng trực tuyến; hỗ trợ quản trị viên quản lý danh mục, biến thể và đơn hàng.
2. **Nhóm người dùng & Quyền hạn:**
   - _Khách chưa đăng nhập (Guest):_ Xem trang chủ, tìm kiếm/lọc, xem chi tiết sản phẩm, đọc Giới thiệu/Blogs.
   - _Khách hàng (Customer):_ Đăng ký/đăng nhập, lưu thông số đo, đặt hàng, áp dụng voucher, theo dõi đơn hàng.
   - _Quản trị viên (Admin):_ Quản lý danh mục, sản phẩm & biến thể, xử lý trạng thái đơn hàng.
3. **Danh sách chức năng đề xuất:**
   - _Yêu cầu bắt buộc (Core):_ Phân loại danh mục; Tìm kiếm từ khóa; Bộ lọc (Giá, Màu sắc, Kích cỡ); Xem chi tiết sản phẩm & chọn biến thể; Bảng minh bạch chi phí; Quản lý giỏ hàng; Đăng ký/đăng nhập; Đặt hàng (COD, chuyển khoản); Quản trị sản phẩm và đơn hàng.
   - _Yêu cầu mở rộng / Nâng cao:_ Công cụ gợi ý size AI (Smart Fit); Tính năng mua theo gói Combo (Bundles); Chuyên mục Blog (_HOTMATE Journal_); Tích điểm thành viên (_Mate Cash_ / _HOTMATE Club_); Đồng bộ đa kênh (Shopee, TikTok); Cổng thanh toán trực tuyến (VNPay/MoMo).
4. **Quy trình nghiệp vụ chính:** Mua hàng 9 bước (Truy cập website → Tìm kiếm/lọc → Xem chi tiết & chọn biến thể → Thêm giỏ hàng → Kiểm tra giỏ → Nhập thông tin giao hàng & chọn thanh toán → Xác nhận đơn → Lưu hệ thống & trừ tồn kho → Theo dõi trạng thái đơn).
5. **Yêu cầu phi chức năng:** Giao diện Responsive; kiểm tra validation form; mã hóa mật khẩu; phân quyền trang quản trị.
6. **Rủi ro & Giảm thiểu:** Rủi ro phình to phạm vi do nhiều tính năng tích hợp (Smart Fit, đồng bộ kênh, tích điểm); rủi ro sai lệch tồn kho theo biến thể màu/size.

### Người kiểm tra

- Trần Hữu Thiện

---

## Lần sử dụng 2: Phản biện độc lập danh sách yêu cầu dự án

### Công cụ

- **Tên công cụ AI:** GitHub Copilot (Copilot Fusion)

### Mục đích

- Đánh giá độc lập, phản biện tính khả thi, phát hiện các chức năng dư thừa, vượt phạm vi đồ án sinh viên và rủi ro triển khai từ bản đề xuất của Google Gemini.

### Prompt

```text
Bạn là người phản biện độc lập cho đồ án website thương mại điện tử HOTMATE (nhóm 5 sinh viên, làm trong 1 học phần).
Bối cảnh: Bán thời trang nam D2C, giải quyết vấn đề khách khó chọn size, muốn biết chi phí thực và giá rẻ.
AI thứ nhất đề xuất:
1. Bắt buộc: Danh mục, tìm kiếm, lọc (giá, màu, size), chi tiết sản phẩm, bảng minh bạch chi phí, giỏ hàng, đặt hàng (COD/chuyển khoản), đăng ký/đăng nhập, quản trị sản phẩm/biến thể và đơn hàng.
2. Mở rộng: Công cụ gợi ý size AI (Smart Fit), mua theo gói Combo (Bundles), Blog (HOTMATE Journal), điểm Mate Cash/Club, đồng bộ đa kênh (Shopee/TikTok), thanh toán VNPay.
Các website tham khảo: Yody, Routine, Uniqlo.

Hãy phản biện ngắn gọn theo 6 khía cạnh:
1. Có giải quyết đúng vấn đề kinh doanh không?
2. Yêu cầu nào trùng lặp hoặc không cần thiết?
3. Chức năng nào vượt quá phạm vi nhóm sinh viên?
4. Có thiếu chức năng cơ bản hoặc bước nghiệp vụ nào không?
5. Rủi ro dữ liệu, bảo mật, quyền riêng tư là gì?
6. Yêu cầu nào chưa đủ rõ để lập trình và kiểm thử?
```

### Kết quả phản biện (Từ GitHub Copilot)

1. **Mức độ giải quyết vấn đề kinh doanh:** Bảng minh bạch chi phí giải quyết tốt yêu cầu công khai giá. Tuy nhiên, việc dùng AI để giải quyết khó khăn chọn size (Smart Fit) là quá phức tạp so với nguồn lực thực tế, dễ làm dự án đi chệch hướng khỏi mục tiêu xây dựng quy trình mua bán cốt lõi.
2. **Trùng lặp / Không cần thiết:** Tính năng bán theo gói Combo (Bundles) và hệ thống tích điểm Mate Cash hiện chưa thiết yếu trong giai đoạn đầu, sẽ làm phức tạp quy trình tính toán tổng tiền và trừ tồn kho.
3. **Vượt phạm vi nhóm sinh viên:** Công cụ AI Smart Fit, tích hợp đồng bộ đa kênh (Shopee, TikTok, API vận chuyển GHN) và cổng thanh toán VNPay đòi hỏi dữ liệu huấn luyện lớn, giấy phép merchant và thời gian tích hợp dài, hoàn toàn vượt quá thời lượng 1 học phần. Đề xuất: Loại bỏ hoặc chỉ làm ở mức hiển thị bảng Size Guide tĩnh.
4. **Chức năng / Bước nghiệp vụ còn thiếu:** Chưa nêu rõ luồng kiểm tra số lượng tồn kho theo từng cặp biến thể trước khi cho phép đặt hàng; thiếu nghiệp vụ xử lý đổi trả hàng và quản lý trạng thái giao hàng chi tiết (_Chờ xác nhận → Đang chuẩn bị hàng → Đang giao hàng → Giao thành công_).
5. **Rủi ro dữ liệu, bảo mật:** Việc lưu trữ "chỉ số cơ thể khách hàng" (nếu làm Smart Fit) làm phát sinh rủi ro về quyền riêng tư.
6. **Chưa đủ rõ để lập trình và kiểm thử:** Cần chuẩn hóa công thức trừ tồn kho cho hàng Combo (nếu giữ) và tiêu chí xác định dữ liệu cho Bảng minh bạch chi phí.

### Bảng tổng hợp đối chiếu và Quyết định cuối cùng của nhóm

| Nội dung / Chức năng                                       | AI thứ nhất đề xuất | AI thứ hai (Copilot) phản biện                | Quyết định của nhóm                                | Lý do quyết định                                                                                                                                                        |
| :--------------------------------------------------------- | :------------------ | :-------------------------------------------- | :------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **1. Trưng bày danh mục, Lọc & Tìm kiếm sản phẩm**         | Đề xuất (Bắt buộc)  | Đồng ý                                        | **Giữ lại (Trong phạm vi MVP)**                    | Chức năng cốt lõi của E-commerce.                                                                                                                                       |
| **2. Bảng minh bạch chi phí sản xuất**                     | Đề xuất (Bắt buộc)  | Đồng ý                                        | **Giữ lại (Trong phạm vi MVP)**                    | Khớp với định vị thương hiệu và vấn đề kinh doanh của nhóm.                                                                                                             |
| **3. Chọn biến thể (Màu/Size) & Quản lý giỏ hàng**         | Đề xuất (Bắt buộc)  | Cần kiểm tra tồn kho nghiêm ngặt.             | **Giữ lại & Bổ sung logic (Trong phạm vi MVP)**    | Bắt buộc kiểm tra tồn kho từng biến thể trước khi thêm giỏ.                                                                                                             |
| **4. Đặt hàng (COD, Chuyển khoản) & Trạng thái đơn**       | Đề xuất (Bắt buộc)  | Cần chuẩn hóa các bước trạng thái.            | **Giữ lại (Trong phạm vi MVP)**                    | Giới hạn ở COD và chuyển khoản mô phỏng; trạng thái: _Chờ xác nhận, Đang chuẩn bị hàng, Đang giao hàng, Giao thành công, Đã hủy_.                                       |
| **5. Công cụ tư vấn size AI (Smart Fit)**                  | Đề xuất (Mở rộng)   | Quá phức tạp, rủi ro quyền riêng tư.          | **Loại bỏ khỏi MVP (Ngoài phạm vi)**               | Thay bằng hiển thị bảng hướng dẫn chọn kích cỡ (Size Guide) tĩnh.                                                                                                       |
| **6. Bán hàng theo Combo (Bundles) & Tích điểm Mate Cash** | Đề xuất (Mở rộng)   | Làm phức tạp logic giỏ hàng và trừ tồn kho.   | **Loại bỏ khỏi MVP (Ngoài phạm vi)**               | Tập trung hoàn thiện quy trình bán lẻ từng món (Basics, Smart Casual).                                                                                                  |
| **7. Đồng bộ đa kênh (Shopee, TikTok) & Thanh toán VNPay** | Đề xuất (Mở rộng)   | Vượt quá năng lực và thời gian của sinh viên. | **Loại bỏ kết nối thật (Chỉ mô phỏng thanh toán)** | Chỉ làm website độc lập, không đồng bộ sàn ngoài; không tích hợp API cổng thanh toán tiền thật (chỉ mô phỏng luồng thanh toán QR/MoMo/VNPay trong môi trường kiểm thử). |
| **8. Blog (HOTMATE Journal)**                              | Đề xuất (Mở rộng)   | Không nên làm hệ thống CMS phức tạp.          | **Điều chỉnh – Làm giao diện tĩnh**                | Chỉ cắt HTML/CSS để đảm bảo thẩm mỹ cho trang, không làm tính năng đăng bài động.                                                                                       |

### Người kiểm tra

- Trần Hữu Thiện (Người thực hiện)
- Lữ Bích Hà (Trưởng nhóm xác nhận)
