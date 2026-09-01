---
title: Tại sao báo thức BarcodeWake có thể không kêu
lang: vi
app: barcodewake-alarm
page_type: help
updated: 2026-09-01
targets:
  - why did my BarcodeWake alarm not ring
facts_used:
  - accuracy_limits
  - hardware_requirements
  - known_limitations
---
# Tại sao báo thức BarcodeWake có thể không kêu

Một báo thức đã lưu vẫn có thể bị chặn bởi cài đặt thông báo, quyền truy cập báo thức chính xác, chế độ focus hoặc im lặng, âm lượng thấp, hạn chế pin, tạm dừng ứng dụng hoặc điều khiển nền của nhà cung cấp. Kiểm tra việc gửi riêng biệt với quét nhiệm vụ, sau đó chạy thử nghiệm trên màn hình khóa.

## Đầu tiên tách biệt việc gửi khỏi việc bỏ qua

Tạo một báo thức thử nghiệm gần với một nhiệm vụ đơn giản và để ứng dụng ở chế độ nền. Khóa màn hình. Nếu không có màn hình báo thức hoặc âm thanh xuất hiện, vấn đề nằm ở việc gửi; thay đổi mã vạch đã đăng ký sẽ không khắc phục được. Nếu báo thức xuất hiện nhưng nhiệm vụ không thể hoàn thành, việc gửi hoạt động và vấn đề nằm ở camera, cảm biến, so khớp mã hoặc cấu hình nhiệm vụ.

Xác nhận báo thức được bật, ngày đã lên lịch đúng và múi giờ của điện thoại khớp với lịch trình dự định. Kiểm tra âm lượng phương tiện và báo thức thay vì chỉ dựa vào trạng thái nút bên. Xem lại các quy tắc không làm phiền hoặc focus, thiết bị âm thanh đã kết nối và liệu điện thoại đã được khởi động lại sau khi tạo báo thức.

## Xem xét các cổng quyền của hệ điều hành

Cho phép thông báo và bất kỳ quyền truy cập báo thức chính xác hoặc báo thức toàn màn hình nào được yêu cầu bởi bản dựng đã cài đặt. Xóa BarcodeWake khỏi các danh sách tối ưu hóa pin hung hăng hoặc ngủ tự động khi nhà cung cấp thiết bị cung cấp các điều khiển đó. Mở chẩn đoán độ tin cậy trong ứng dụng và làm theo các cài đặt dành riêng cho thiết bị mà nó xác định. Trang [quyền riêng tư và độ tin cậy](../features/privacy-and-reliability.md) giải thích tại sao các phụ thuộc hệ thống này vẫn tồn tại ngay cả khi dữ liệu ứng dụng được lưu trữ cục bộ.

Sau khi thay đổi một cài đặt, lặp lại thử nghiệm trên màn hình khóa. Thay đổi một số cài đặt cùng lúc khiến nguyên nhân khó xác định hơn. Các bản cập nhật hệ thống có thể đặt lại hoặc diễn giải lại quyền, vì vậy hãy thử nghiệm lại sau bản cập nhật lớn hoặc cài đặt lại ứng dụng.

## Chẩn đoán việc hoàn thành nhiệm vụ riêng biệt

Đối với các nhiệm vụ mã vạch và QR, hãy làm sạch ống kính camera, cải thiện ánh sáng và xác nhận đối tượng đã đăng ký không thay đổi. Cấp quyền camera. Đối với NFC, hãy xác minh hỗ trợ thiết bị và giữ thẻ gần vị trí ăng-ten đúng. Các nhiệm vụ lắc và bước phụ thuộc vào cảm biến chuyển động hoặc bước chân và có thể hoạt động khác khi các chế độ tiết kiệm pin hạn chế việc gửi cảm biến.

Nếu một nhiệm vụ được cấu hình như một phần của chuỗi, mọi bước bắt buộc phải hoàn thành. Xem lại [hành vi nhiệm vụ](../features/missions.md) và, nếu cần, tạo thử nghiệm mới bằng [quy trình thiết lập](../guides/set-up-an-alarm.md).

## Biết khi nào điện thoại là giới hạn

BarcodeWake không thể ghi đè thiết bị đã tắt nguồn, pin cạn kiệt, phần cứng âm thanh bị hỏng hoặc mọi trình killer tác vụ của nhà sản xuất. Nó không phải là dịch vụ thông báo khẩn cấp. Giữ một phương pháp báo thức khác cho các tình huống có hậu quả cao và báo cáo các lỗi có thể tái tạo với mẫu thiết bị, phiên bản hệ thống, phiên bản ứng dụng và các điều kiện thử nghiệm chính xác.

