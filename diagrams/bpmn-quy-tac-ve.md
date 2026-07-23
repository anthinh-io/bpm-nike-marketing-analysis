**Chuẩn & thứ tự**
- Bắt buộc **BPMN 2.0** (không flowchart/UML thuần).
- **Mô tả bằng lời trước** (actors, customer, tasks theo thứ tự, outcome +/−) → **mới vẽ**.
- Tool gợi ý: **Lucidchart** (hoặc tool BPMN tương đương).

**Pool / Lane**
- Pool: tổ chức / đối tác; Lane: vai trò, nhân viên, **hệ thống** (ERP, CRM…).
- Activity nằm **trên lane của người/bộ phận thực hiện**.
- Phân **internal / external** rõ (VD customer external; NV/bếp internal).
- Mỗi phòng 1 pool **hoặc** 1 pool tổ chức + nhiều lane (nếu gộp phải thể hiện tổ chức bao trùm).
- Giao tiếp **giữa pool**: **message flow** (nét đứt), không dùng sequence flow xuyên pool.

**Flow elements**
- **Activity**: chữ nhật bo góc; tên **động từ + danh từ** (Check stock, Reject order…).
- **Event** (start / intermediate / end): đặt tên rõ theo quy ước, **không mơ hồ**; End gắn **outcome thật** (fulfilled / rejected…), không end “giữa chừng” gây hiểu nhầm.
- **Subprocess**: activity có dấu **+**; đóng gói thì nối vào khung; mở rộng thì **activity trong không nối thẳng** ra process cha.
- **Start**: tròn nét đơn (**1 start** / sơ đồ đơn giản).
- **End**: tròn nét đậm; **nhiều end** theo nhánh +/−.
- **Intermediate**: tròn nét đôi; **Timer** khi chờ/lặp theo thời hạn.
- **1 hình ≈ 1 quy trình**; QT lớn → chia nhỏ / subprocess.

**Gateway (XOR / AND / OR)**
- **XOR**: đúng **1** nhánh (if/switch).
- **AND** (dấu +): **song song**, join khi **tất cả** nhánh xong.
- **OR**: một hoặc nhiều nhánh theo điều kiện.
- **Split phải join** (trừ nhánh end ngay sau split). Quên join = lỗi nặng.
- Gắn **label điều kiện** trên từng nhánh ra.

**Connecting objects & data**
- **Sequence flow**: nét liền + mũi tên, trong cùng pool/process.
- **Message flow**: nét đứt **chỉ giữa pool** (PO, invoice, thông báo…); không thay sequence trong cùng pool; không sequence xuyên pool.
- **Association**: gắn data / annotation.
- Data object (file), collection (3 gạch), data store (hình trụ); mũi tên **rỗng = input**, **đặc = output**.

**Khi vẽ**
- Luôn có nhánh **Positive / Negative** → gateway + end tương ứng.
- Sơ đồ phải **khớp mô tả/workshop** đã viết.
- Lỗi hay gặp khi vẽ: sai ký hiệu / pool-lane / đặt tên / đường vẽ; **split không join** = lỗi nặng.