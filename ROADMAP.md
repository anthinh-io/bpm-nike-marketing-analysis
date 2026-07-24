# Roadmap

## 1. Rubric chấm điểm (5 tiêu chí)

| #   | Tiêu chí                      | Yêu cầu cụ thể                                                                                                                                                                                                                                 | Điểm trừ / lưu ý                                                                  |
| --- | ----------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| 1   | Liệt kê & phân loại quy trình | Tối thiểu **10 quy trình**, chia đều 3 cấp (Quản lý / Cốt lõi / Hỗ trợ), mỗi cấp ≥3, một cấp sẽ có 4. Vẽ sơ đồ kiến trúc quy trình tổng thể.                                                                                                   | —                                                                                 |
| 2   | Mô tả quy trình               | Mô tả bằng lời cho **10 quy trình**: bước thực hiện, actor (ai kích hoạt / ai hưởng lợi), kịch bản thành công & thất bại.                                                                                                                      | —                                                                                 |
| 3   | Mô hình hóa BPMN              | Tối thiểu **6 quy trình** (2 Quản lý + 2 Cốt lõi + 2 Hỗ trợ), dùng **BPMN 2.0** (Lucidchart). Điểm theo số gateway: >7 cổng = 1đ, >5 = 0.75đ, 4–5 = 0.5đ, <3 = 0.25đ, 0 cổng = 0đ.                                                             | Sai ký hiệu/tên/quy tắc vẽ: **-0.25đ/lỗi**                                        |
| 4   | Phân tích quy trình           | Phân tích tối thiểu **2 quy trình** (tối đa cả 6). Định tính: VA/BVA/NVA + tối thiểu 4 loại lãng phí (Move, Hold, Over-processing, Defects), bảng 3 cột (mô tả – phân loại – khắc phục), đánh dấu trên sơ đồ. Định lượng: thời gian + chi phí. | —                                                                                 |
| 5   | Trình bày báo cáo             | Theo mẫu khóa luận của trường: mục lục nội dung/hình/bảng/từ viết tắt, font size 12, đen trắng nhất quán. Nhãn bảng ở trên, nhãn hình ở dưới.                                                                                                  | Lỗi chính tả: **-1đ/lỗi** (dễ mất trắng cả tiêu chí). Sai vị trí nhãn: -1 đến -2đ |

## 2. Mốc thời gian

| Tuần                | Khoảng ngày    | Việc cần làm theo giảng viên                                                                                                            | Trạng thái      |
| ------------------- | -------------- | --------------------------------------------------------------------------------------------------------------------------------------- | --------------- |
| 1–2                 | 06/07 – 19/07  | Lập nhóm (≥4 người), chọn công ty và lĩnh vực, tạo repo GitHub, thêm email giảng viên, phân chia công việc ban đầu                      | ✅ Hoàn tất     |
| 3–5                 | 20/07 – 09/08  | Rải công việc từng tuần: liệt kê quy trình, mô tả, bắt đầu mô hình hóa                                                                  | ⏳ Đang bắt đầu |
| 6–7                 | 10/08 – 23/08  | Chuẩn bị **slide báo cáo cuối kỳ**: mỗi cấp (quản lý/cốt lõi/hỗ trợ) chọn 1 quy trình tiêu biểu để trình bày, nhận góp ý từ giảng viên  | ⏳ Sắp tới      |
| +1 tuần sau báo cáo | ~24/08 – 30/08 | Chỉnh sửa theo góp ý, hoàn thiện toàn bộ báo cáo Word (10 quy trình mô tả, 6 sơ đồ BPMN, phân tích, đề xuất), nộp file Word + PDF slide | ⏳ Sắp tới      |

## 3. Bài học rút ra từ báo cáo mẫu

|                          | CellphoneS                                 | FUTA Bus Lines                                                                       | Áp dụng cho nhóm                                                                                   |
| ------------------------ | ------------------------------------------ | ------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------- |
| Số quy trình mô hình hóa | 6                                          | 9 (vượt yêu cầu tối thiểu)                                                           | Làm đúng tối thiểu 6 trước, dư sức thì mở rộng                                                     |
| Cấu trúc chương          | Gộp mô hình hóa + phân tích chung 1 chương | Tách riêng: Chương 2 chỉ mô hình hóa, Chương 3 chỉ phân tích                         | **Nên theo FUTA** — tách bạch giúp rubric tiêu chí 3 và 4 dễ chấm riêng, dễ tự rà soát điểm        |
| Độ sâu phân tích         | Chỉ bảng VA/BVA/NVA + lãng phí cơ bản      | Có thêm Stakeholder Analysis, Issue Register (cột giải pháp cụ thể), Pareto, Why-Why | Làm tối thiểu 2 quy trình theo chuẩn FUTA (Issue Register có cột "khắc phục") để tối ưu tiêu chí 4 |
| Đề xuất cải tiến         | Gộp chung, chung chung ở phần Kết luận     | Cụ thể theo từng vấn đề, có người phụ trách/thời hạn                                 | Làm bảng đề xuất riêng cho từng lãng phí phát hiện                                                 |

## 4. Kế hoạch công việc chi tiết theo tuần (từ hiện tại)

### Tuần 3 (20–26/07) — Chốt danh sách quy trình

- [ ] Rà lại 20 quy trình ứng viên trong `docs/01` → ánh xạ vào 3 cấp **Quản lý / Cốt lõi / Hỗ trợ** (hiện đang phân theo nhóm chuỗi giá trị, chưa theo cấp BPM)
- [ ] Chốt tối thiểu **10 quy trình chính thức** (loại các mục [không rõ] như 7.2, 9.x trừ khi có nguồn bổ sung)
- [ ] Vẽ sơ đồ **Kiến trúc quy trình tổng thể** (Lucidchart)
- [ ] Phân công 4 thành viên phụ trách theo nhóm quy trình hoặc theo chương

### Tuần 4 (27/07–02/08) — Mô tả quy trình

- [ ] Mô tả bằng lời cả 10 quy trình: bước thực hiện, actor kích hoạt/hưởng lợi, kịch bản thành công/thất bại
- [ ] Soạn bộ câu hỏi khảo sát: 10 định tính + 10 định lượng / quy trình (ưu tiên 6 quy trình sẽ mô hình hóa trước)

### Tuần 5 (03–09/08) — Mô hình hóa BPMN

- [ ] Vẽ BPMN cho 6 quy trình đã chọn (2 Quản lý + 2 Cốt lõi + 2 Hỗ trợ), mỗi sơ đồ hướng tới **>7 gateway** để đạt điểm tối đa
- [ ] Rà soát ký hiệu/quy tắc đặt tên/quy tắc vẽ trước khi chốt (mỗi lỗi -0.25đ)

### Tuần 6 (10–16/08) — Phân tích + chuẩn bị báo cáo

- [ ] Phân tích định tính (VA/BVA/NVA, 4 loại lãng phí, bảng 3 cột) cho tối thiểu 2 quy trình
- [ ] Phân tích định lượng (thời gian, chi phí)
- [ ] Chuẩn bị slide: mỗi cấp 1 quy trình tiêu biểu, kiểm tra thời lượng, chuẩn bị bật camera cho tất cả thành viên

### Tuần 6–7 (~17–23/08) — Báo cáo

- [ ] Thuyết trình trước lớp, ghi nhận góp ý của giảng viên

### Tuần sau báo cáo (~24–30/08) — Hoàn thiện & nộp

- [ ] Hoàn thiện phân tích còn thiếu, thêm bảng đề xuất cải tiến (vấn đề – mô tả – đề xuất) theo từng lãng phí
- [ ] Format báo cáo cuối theo mẫu khóa luận trường: mục lục, mục lục hình, mục lục bảng, danh mục viết tắt
- [ ] Soát chính tả kỹ (mỗi lỗi -1đ), kiểm tra nhãn bảng ở trên / nhãn hình ở dưới, font nhất quán size 12 đen trắng
- [ ] Nộp file Word + PDF slide

## 5. Nguyên tắc xuyên suốt (để không bị 0 điểm)

- Mỗi thành viên **tự commit phần việc của mình** hàng tuần (không dồn, không nhờ người khác commit hộ) — đúng CONTRIBUTING.md hiện có.
- Không để 3 tuần liên tiếp không có hoạt động GitHub nào.
- Dùng AI hỗ trợ ý tưởng/chuẩn hóa câu hỏi/làm đẹp sơ đồ, không giao toàn bộ việc vẽ BPMN và phân tích cho AI.

## 6. Các điểm cần làm rõ

- Ngày báo cáo cuối kỳ chính xác (hiện chỉ suy ra "tuần 6–7" từ lời giảng viên, cần chốt ngày cụ thể).
- Có bao gồm mục 7.2 (marketing tổng thể) và mục 9 (kế toán/thuế) trong danh sách 10 quy trình chính thức không, hay thay bằng quy trình khác có nguồn rõ ràng hơn?
- Cách lấy số liệu định lượng (thời gian, chi phí) cho phân tích — hiện `docs/01` chỉ có dữ liệu định tính từ nguồn công khai, chưa có cách tiếp cận cho phần định lượng (ước tính giả định vs. tìm thêm nguồn).
- Chưa chốt cụ thể 6/10 quy trình nào sẽ được chọn để mô hình hóa BPMN.
- Chưa phân công lại công việc theo 4 thành viên.
