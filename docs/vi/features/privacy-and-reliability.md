---
title: Quyền riêng tư và độ tin cậy của BarcodeWake
lang: vi
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - is BarcodeWake private and reliable
facts_used:
  - offline
  - account_required
  - ads_tracking
  - data_storage
  - accuracy_limits
---

# Quyền riêng tư và độ tin cậy của BarcodeWake

BarcodeWake giữ cấu hình báo thức và dữ liệu nhiệm vụ đã ghi nhận trên thiết bị và không yêu cầu tài khoản ứng dụng. Các đường dẫn mã hiện tại băm (hash) các giá trị mã đã đăng ký. Telemetry tùy chọn được mô tả là bị tắt theo mặc định, trong khi việc phát báo thức vẫn phụ thuộc vào quyền hệ thống và kiểm soát của nhà cung cấp.

## Dữ liệu cục bộ không loại bỏ phụ thuộc hệ thống

Lưu trữ cục bộ có nghĩa là việc thiết lập báo thức thông thường không yêu cầu tài khoản đám mây BarcodeWake. Các bản ghi báo thức, lịch sử và tùy chọn được xử lý thông qua lớp dữ liệu cục bộ của ứng dụng. Các giá trị mã vạch, QR và NFC đã đăng ký được biểu diễn bằng hash SHA-256 trong các đường dẫn lưu trữ và nhập hiện tại, điều này tránh việc giữ lại giá trị thô thông thường để so khớp.

Việc băm (hash) không giống như mã hóa mọi bản ghi của ứng dụng, và lưu trữ cục bộ không phải là bản sao lưu. Người có quyền truy cập vào thiết bị đã mở khóa vẫn có thể xem tên báo thức, lịch trình hoặc lịch sử qua ứng dụng. Điện thoại bị mất hoặc khôi phục cũng có thể mất dữ liệu cục bộ trừ khi người dùng đã thực hiện xuất. Xem [sao lưu và chia sẻ](../guides/backup-and-sharing.md) để biết các định dạng và mục đích khác nhau của chúng.

Chính sách quyền riêng tư cho biết telemetry tùy chọn được tắt theo mặc định và mô tả cách xử lý tổng hợp nếu được bật. Tài liệu này do đó không đưa ra tuyên bố rộng hơn rằng ứng dụng không thể giao tiếp qua mạng. Nó nêu rõ các sự thật đã được xác minh hẹp hơn: hoạt động cốt lõi và dữ liệu là cục bộ, không yêu cầu tài khoản sản phẩm, và không có phụ thuộc SDK quảng cáo trong dự án đã kiểm tra.

## Độ tin cậy là trách nhiệm chia sẻ

BarcodeWake có thể lên lịch và hiển thị báo thức, nhưng hệ điều hành quyết định khi nào công việc nền có thể chạy và những gián đoạn nào được phép. Quyền thông báo, quyền truy cập báo thức chính xác, chế độ im lặng hoặc tập trung, tối ưu hóa pin, tạm ngưng ứng dụng tự động và trình quản lý tác vụ của nhà sản xuất đều có thể ảnh hưởng. Công cụ độ tin cậy trong ứng dụng có thể xác định rủi ro cấu hình và hướng dẫn người dùng đến cài đặt; nó không thể ghi đè chính sách hệ thống.

Sau khi cài đặt, hãy thử nghiệm với màn hình khóa và điện thoại ở chế độ nguồn giống như khi qua đêm. Lặp lại bài kiểm tra đó sau khi cập nhật hệ thống, thay đổi tiết kiệm pin hoặc cài lại ứng dụng. Giữ thiết bị được sạc, âm lượng phù hợp và nhiệm vụ đã chọn có sẵn vật lý. Thực hiện [khắc phục lỗi phát báo thức](../help/alarm-delivery.md) khi bài kiểm tra thất bại.

## Những gì quyền riêng tư và độ tin cậy không đảm bảo

BarcodeWake không phải thiết bị y tế, dịch vụ cảnh báo khẩn cấp hay ứng dụng theo dõi giấc ngủ. Không có ứng dụng báo thức nào có thể đảm bảo việc thức dậy hoặc bồi thường cho thiết bị không khả dụng. Trang [thông tin và giới hạn](../facts.md) liệt kê các giới hạn này, trong khi [tính khả dụng](../availability.md) phân biệt bằng chứng từ cửa hàng công khai với khả năng của mã nguồn mới hơn.

