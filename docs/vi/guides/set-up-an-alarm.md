---
title: Cách thiết lập báo thức BarcodeWake
lang: vi
app: barcodewake-alarm
page_type: guide
updated: 2026-09-01
targets:
  - how to set up a BarcodeWake alarm
facts_used:
  - what_it_is
  - hardware_requirements
  - accuracy_limits
---

# Cách thiết lập báo thức BarcodeWake

Trước tiên hãy tạo lịch trình, chọn một nhiệm vụ an toàn và thực tế, cấp các quyền cần thiết, sau đó chạy một bài kiểm tra khóa màn hình trong thời gian gần. Đối với các nhiệm vụ quét, đăng ký một đối tượng bền bỉ sẽ khả dụng và có thể đọc được khi báo thức kêu.

## Chọn nhiệm vụ trước khi đối tượng

Quyết định hành động nào sẽ phân biệt giữa thức dậy và tắt báo. Một mã vạch ở phòng khác tạo ra khoảng cách vật lý. Toán hoặc gõ thêm vào sự tập trung mà không cần camera. Lắc hoặc bước đi thêm chuyển động nhưng phụ thuộc vào cảm biến và có thể không phù hợp với mọi người hoặc môi trường. [Tài liệu tham khảo nhiệm vụ](../features/missions.md) giải thích các sự đánh đổi giữa các chế độ đơn, chuỗi và ngẫu nhiên.

Nếu sử dụng mã vạch, mã QR hoặc thẻ NFC, hãy chọn thứ gì đó bền bỉ. Tránh bao bì dùng một lần, một đối tượng mà thành viên khác trong gia đình có thể di chuyển, hoặc mã sẽ không thể tiếp cận được khi đi du lịch. Kiểm tra xem camera có thể lấy nét trong điều kiện ánh sáng dự kiến hay không. NFC cần một điện thoại và thẻ tương thích.

## Cấu hình lịch trình và quy tắc tắt báo

Mở trình chỉnh sửa báo thức, đặt thời gian mong muốn và các ngày hoạt động, sau đó chọn nhiệm vụ được hiển thị bởi bản dựng đã cài đặt. Cấu hình độ khó hoặc mục tiêu một cách thận trọng cho bài kiểm tra đầu tiên. Nếu phiên bản đã cài đặt hỗ trợ chuỗi, sắp xếp các nhiệm vụ theo thứ tự có thể hoàn thành an toàn mà không vội vàng qua cầu thang hoặc rời khỏi khu vực an toàn.

Đăng ký mã vật lý từ quy trình thiết lập nhiệm vụ. Đặt cho báo thức một nhãn xác định thói quen dự định thay vì tiết lộ thông tin nhạy cảm. Xem lại âm lượng, rung và bất kỳ tùy chọn theo dõi sau khi thức dậy nào được hiển thị trong bản dựng đã cài đặt. Các điều khiển khả dụng có thể khác nhau vì [phiên bản công khai và mã nguồn](../availability.md) không giống nhau tại ngày kiểm toán.

## Cấp quyền có mục đích

Cho phép thông báo và quyền truy cập liên quan đến báo thức cần thiết cho việc giao. Cấp quyền truy cập camera chỉ khi sử dụng nhiệm vụ quét, và quyền truy cập cảm biến khi nhiệm vụ đã chọn cần nó. Trên Android, xem lại cài đặt exact-alarm và pin nếu kiểm tra độ tin cậy của ứng dụng đánh dấu chúng. Không cho rằng việc lưu báo thức chứng minh rằng giao trong nền được phép.

## Kiểm tra toàn bộ đường dẫn qua đêm

Đặt một bài kiểm tra trước vài phút. Khóa màn hình, để BarcodeWake ở chế độ nền và đặt điện thoại vào cùng trạng thái âm thanh và nguồn như kế hoạch qua đêm. Xác nhận rằng báo thức xuất hiện, âm thanh có thể nghe được và nhiệm vụ đã chọn có thể hoàn thành chính xác. Sau đó lặp lại sau khi di chuyển đối tượng đã đăng ký đến vị trí thực tế của nó.

Nếu giao báo thức thất bại, hãy sử dụng [danh sách kiểm tra giao báo thức](../help/alarm-delivery.md). Nếu thành công, hãy cân nhắc tạo [sao lưu cục bộ](backup-and-sharing.md) sau khi thiết lập ổn định.

