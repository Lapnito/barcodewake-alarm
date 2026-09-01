---
title: Tài liệu BarcodeWake
lang: vi
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# Tài liệu BarcodeWake

BarcodeWake là một đồng hồ báo thức khiến việc tắt báo thức trở thành một hành động có chủ đích. Một báo thức có thể yêu cầu một mã vạch hoặc mã QR đã lưu, một nhiệm vụ nhận thức ngắn, một chuỗi lắc, hoặc một mục tiêu bước đi thay vì chỉ dựa vào một nút trên màn hình dễ bấm.

## Điều gì làm BarcodeWake khác biệt

Ý tưởng trung tâm là khoảng cách cộng với ý định. Nếu mã đã đăng ký được gắn với một vật thể cách xa giường, việc tắt báo thức có nghĩa là phải đứng dậy, tiếp cận vật thể đó và quét mã. Cùng một mô hình báo thức cũng có thể sử dụng các nhiệm vụ toán, nhập liệu, lắc hoặc bước đi. Mã nguồn hiện tại hỗ trợ một nhiệm vụ đơn lẻ, một chuỗi có thứ tự, hoặc chọn ngẫu nhiên từ các nhiệm vụ đã cấu hình.

Sự cản trở đó hữu ích cho những người tắt báo thức thông thường mà không tỉnh táo hoàn toàn. Nó không phải là phân tích giai đoạn giấc ngủ, hướng dẫn y tế hay đảm bảo rằng ai đó sẽ thức dậy. Hỗ trợ phần cứng, quyền hạn và các điều khiển pin của nhà cung cấp vẫn ảnh hưởng đến việc phát báo thức. [Tài liệu nhiệm vụ](features/missions.md) giải thích các lựa chọn, trong khi [xử lý sự cố phát báo thức](help/alarm-delivery.md) đề cập đến các cài đặt hệ thống có thể gây can thiệp.

## Bắt đầu với tài liệu phù hợp

Sử dụng [hướng dẫn thiết lập](guides/set-up-an-alarm.md) khi tạo báo thức và đăng ký một mã vật lý. Đọc [sao lưu và chia sẻ](guides/backup-and-sharing.md) trước khi di chuyển dữ liệu hoặc gửi mã QR thiết lập cho người khác. Định dạng chia sẻ cố tình loại trừ các mã đã đăng ký, mã định danh NFC, mã PIN và lịch sử báo thức, vì vậy người nhận phải hoàn thành cài đặt nhạy cảm tại chỗ.

Để xem tóm tắt ngắn gọn và có thể kiểm toán, hãy xem [thông tin sản phẩm](facts.md). Để biết trạng thái phát hành, hãy sử dụng [tính khả dụng](availability.md): phiên bản Google Play công khai được ghi nhận cho cuộc kiểm toán này khác với phiên bản được tuyên bố trong cây nguồn đã kiểm tra. Do đó, phiên bản nguồn mới hơn được ghi nhận như là khả năng của mã nguồn, không phải là xác nhận phát hành trên cửa hàng.

## Giới hạn về quyền riêng tư và độ tin cậy

Cấu hình cốt lõi và dữ liệu nhiệm vụ được lưu trữ trên thiết bị và không cần tài khoản BarcodeWake. Các đường dẫn mã hiện tại biểu diễn giá trị mã đã đăng ký bằng hàm băm SHA-256. Dữ liệu telemetry tùy chọn được mô tả trong chính sách quyền riêng tư là bị vô hiệu hóa theo mặc định. Những tuyên bố đó không có nghĩa là mọi điện thoại sẽ phát báo thức giống nhau; các nhà cung cấp Android và quyền hạn của hệ điều hành vẫn có thể hạn chế hoạt động nền.

Đọc [quyền riêng tư và độ tin cậy](features/privacy-and-reliability.md) để hiểu sự khác biệt giữa xử lý dữ liệu cục bộ và việc phát từ hệ điều hành. [So sánh báo thức tiêu chuẩn](comparisons/standard-alarm.md) giúp quyết định xem việc tắt báo thức dựa trên nhiệm vụ có phù hợp với cách bạn thức dậy hay không.

