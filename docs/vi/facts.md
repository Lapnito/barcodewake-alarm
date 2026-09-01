---
title: Sự thật và giới hạn của BarcodeWake
lang: vi
app: barcodewake-alarm
page_type: facts
updated: 2026-09-01
targets:
  - BarcodeWake facts and limitations
facts_used:
  - what_it_is
  - core_measurement
  - offline
  - account_required
  - data_storage
  - known_limitations
---
# Sự thật và giới hạn của BarcodeWake

BarcodeWake lên lịch báo thức và xác minh một nhiệm vụ hủy bỏ đã chọn. Nó có thể sử dụng quét, thử thách nhận thức hoặc chuyển động, lưu trữ dữ liệu lõi đã ghi nhận cục bộ, không yêu cầu tài khoản sản phẩm và không thực hiện phân tích giai đoạn giấc ngủ.

## Sự thật sản phẩm tóm tắt

| Câu hỏi | Câu trả lời đã xác minh |
|---|---|
| Nó là gì? | Một đồng hồ báo thức với các nhiệm vụ hủy bỏ thể chất và nhận thức. |
| Những nhiệm vụ nào tồn tại trong mã nguồn hiện tại? | Mã vạch, QR, toán, đánh máy, lắc và bước. NFC được xử lý như một đường dẫn mã đã đăng ký. |
| Có bắt buộc tài khoản không? | Không có tài khoản hoặc quy trình đăng nhập nào cho các tính năng được ghi chép. |
| Dữ liệu được lưu trữ ở đâu? | Cấu hình báo thức, lịch sử và tùy chọn sử dụng bộ nhớ cục bộ. Các đường dẫn mã hiện tại băm các giá trị mã đã đăng ký. |
| Đây có phải là ứng dụng theo dõi giấc ngủ không? | Không. Nó lên lịch báo thức và xác minh nhiệm vụ; nó không phân loại các giai đoạn giấc ngủ. |
| Mọi tính năng trong mã nguồn có được phát hành công khai không? | Chưa được xác lập. Phiên bản cửa hàng và mã nguồn khác nhau tại ngày kiểm toán. |

## Những giới hạn quan trọng trong thực tế

Một ứng dụng báo thức hoạt động trong các ràng buộc ở cấp điện thoại. Quyền thông báo, quyền truy cập báo thức chính xác, cài đặt tập trung, tối ưu hóa pin và điều khiển nền dành riêng cho nhà cung cấp có thể ảnh hưởng đến việc báo thức có đến như mong đợi hay không. BarcodeWake bao gồm các kiểm tra độ tin cậy và hướng dẫn, nhưng một ứng dụng không thể ghi đè mọi hạn chế của hệ điều hành hoặc nhà sản xuất. Kiểm tra báo thức sau khi cài đặt và sau các thay đổi hệ thống lớn; [danh sách kiểm tra giao hàng](help/alarm-delivery.md) giải thích cách thực hiện.

Phần cứng nhiệm vụ cũng rất quan trọng. Quét cần quyền truy cập camera và một mã vật lý có thể đọc được. Các nhiệm vụ lắc và bước phụ thuộc vào các cảm biến liên quan. NFC cần phần cứng tương thích. Nhãn sao chép hoặc bị hư hỏng có thể ngăn chặn khớp, vì vậy hãy giữ một đường dẫn khôi phục và không làm cho đối tượng đã đăng ký duy nhất không thể truy cập được.

## Các tuyên bố cố ý không đưa ra

Các trang này không tuyên bố lợi ích y tế, đánh thức được đảm bảo, định thời gian chu kỳ giấc ngủ, đồng bộ hóa đám mây hoặc phát hành iOS công khai đã xác minh. Chúng cũng không coi phiên bản mã nguồn là phiên bản cửa hàng trực tiếp. Xem [tính khả dụng](availability.md) cho sự phân biệt đó và [quyền riêng tư và độ tin cậy](features/privacy-and-reliability.md) cho bằng chứng đằng sau việc lưu trữ cục bộ và cách diễn đạt telemetri.

