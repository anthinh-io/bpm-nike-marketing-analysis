# Mô hình hóa Quy trình Nghiệp vụ (BPMN 2.0)

## 1. Khái niệm & lý thuyết

- **BPMN** (Business Process Modeling Notation): ngôn ngữ ký hiệu trực quan chuẩn mở, giúp mọi bên liên quan (người dùng doanh nghiệp, BA, dev, kiến trúc sư dữ liệu) hiểu thống nhất cách vận hành quy trình.
- **Lợi ích:**
  - Ghi lại quy trình rõ ràng, nhất quán — tránh mỗi người diễn giải một kiểu.
  - Là cầu nối giao tiếp giữa đội thiết kế – vận hành – phát triển phần mềm (chuyển đổi số).
  - Hỗ trợ đào tạo nhân viên mới hiểu vai trò/thao tác của mình trong quy trình.
  - Giúp nhà phân tích tìm nút thắt (chi phí, thời gian, hiệu suất) để cải tiến quy trình.
- **Cấu trúc cốt lõi:** 3 lớp — Foundation (nền tảng), Services (dịch vụ), Common (phổ biến).

## 2. Các thành phần BPMN

- **Pool & Swimlane (Lane):** Pool = tổ chức/công ty/hệ thống (internal/external); Lane = phòng ban hoặc vai trò/nhân viên cụ thể bên trong Pool.
- **Activity:** hình chữ nhật bo tròn 4 góc; có dấu "+" nếu là hoạt động phức tạp chứa quy trình con.
- **Event:**
  - Start (nét đơn).
  - End (nét đậm).
  - Intermediate (vòng nét kép, có thể kèm biểu tượng gửi/nhận thông điệp hoặc theo thời gian lặp lại).
- **Gateway:**
  - *Exclusive/XOR* (dấu X): chỉ 1 trong các nhánh được chọn (như if/switch-case).
  - *Parallel/AND* (dấu +): tất cả nhánh phải chạy song song và hoàn tất mới đi tiếp (đồng bộ hóa).
  - *Inclusive/OR* (dấu O): một hoặc nhiều nhánh thỏa điều kiện, đi tiếp khi các nhánh đã chọn hoàn tất.
- **Data:** Data Object (file/hồ sơ), Collection Data (3 gạch dưới), Database (hình trụ).
- **Connecting Objects:** Sequence Flow (nét liền, nối trong cùng 1 Pool) vs. Message Flow (nét đứt, nối giữa các Pool khác nhau).

## 3. Ví dụ minh họa

- **XOR:** thanh toán trà sữa (1 trong 4 hình thức), đi Huế (tàu lửa/máy bay), kiểm tra hóa đơn lỗi.
- **AND:** mua hàng Tiki/Shopee, kiểm tra an ninh sân bay.
- **OR:** xử lý sự cố đi nhậu (hết xăng/kẹt xe/hết tiền — một hoặc nhiều điều kiện cùng lúc).
- **Swimlane:** quy trình xét duyệt tín dụng ngân hàng (nhân viên kinh doanh vs. bộ phận rủi ro).
- **Message Flow:** đặt Pizza, xét duyệt đơn mượn tiền (giữa khách hàng – lễ tân – đầu bếp).

## 4. Lưu ý quan trọng

- Message Flow (nét đứt) không dùng trong cùng 1 Pool; Sequence Flow (nét liền) không được cắt qua ranh giới Pool khác; không nối trực tiếp từ ngoài vào hoạt động bên trong sub-process.
- **Quy tắc đặt tên:**
  - Task = Động từ + Danh từ (tránh "xử lý", "ghi lại" chung chung).
  - Event = Danh từ + Động từ quá khứ.
  - Nhánh XOR/OR phải có label điều kiện.
