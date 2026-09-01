---
title: Nhiệm vụ và chuỗi nhiệm vụ của BarcodeWake
lang: vi
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - how do BarcodeWake missions work
facts_used:
  - what_it_is
  - core_measurement
  - hardware_requirements
  - known_limitations
---
# Nhiệm vụ và chuỗi nhiệm vụ của BarcodeWake

Một nhiệm vụ BarcodeWake là điều kiện dùng để tắt báo thức. Nguồn hiện tại hỗ trợ mã vạch, mã QR, toán học, gõ phím, lắc và bước đi, với NFC đã đăng ký được xử lý qua đường quét mã. Các nhiệm vụ có thể chạy đơn lẻ, theo thứ tự hoặc chọn ngẫu nhiên.

## Các nhiệm vụ quét tạo ra khoảng cách vật lý

Nhiệm vụ mã vạch hoặc QR so sánh một quét camera trực tiếp với mã đã đăng ký khi thiết lập. Mã có thể được đặt trên một vật thể ngoài tầm với: đồ dùng nhà tắm trong phòng tắm, một món ăn sáng trong bếp, hoặc một vật ổn định khác ở nơi có đủ ánh sáng. NFC cũng tuân theo cùng một nguyên tắc chung với thẻ tương thích và thiết bị. Ứng dụng lưu trữ một biểu diễn băm trong các đường dẫn hiện tại thay vì cần mã gốc để so sánh thông thường.

Chọn một vật thể sẽ vẫn có sẵn khi báo thức kêu. Bao bì có thể bị vứt đi, nhãn phai mờ và hành trình thay đổi môi trường. Đăng ký mã trên hộp thuốc duy nhất mà bạn có thể cần thay thế sẽ kém bền vững hơn so với việc sử dụng nhãn bền. [Hướng dẫn cài đặt báo thức](../guides/set-up-an-alarm.md) đề cập đến vị trí và kiểm tra.

## Các nhiệm vụ thử thách đánh đổi chuyển động lấy nỗ lực

Toán học và gõ phím yêu cầu đầu vào tập trung. Lắc và bước đi yêu cầu chuyển động thể chất và cảm biến được hỗ trợ. Cài đặt độ khó và mục tiêu thay đổi mức độ công việc mong đợi, nhưng nhiệm vụ khó hơn không tự động tốt hơn. Ma sát quá mức có thể khuyến khích tắt báo thức hoàn toàn, trong khi một nhiệm vụ dễ có thể trở nên tự động sau khi lặp lại.

Phù hợp nhiệm vụ với chế độ thất bại. Nếu bạn tắt báo thức khi còn nửa ngủ, quét ở phòng khác tạo ra khoảng cách hữu ích. Nếu truy cập camera không tiện lợi, một nhiệm vụ gõ ngắn hoặc toán học có thể thực tế hơn. Nếu có vấn đề về khả năng vận động, thăng bằng hoặc khả năng tiếp cận, tránh các nhiệm vụ dựa trên chuyển động và chọn nhiệm vụ có thể hoàn thành an toàn.

## Chế độ đơn, chuỗi và ngẫu nhiên

Chế độ đơn yêu cầu một nhiệm vụ đã cấu hình. Chế độ chuỗi chạy một số nhiệm vụ đã cấu hình theo thứ tự. Chế độ ngẫu nhiên chọn từ một tập hợp đã cấu hình, giảm khả năng một tương tác đã ghi nhớ trở thành tự động. Các chế độ này xuất hiện trong nguồn đã kiểm tra mới hơn; [tính khả dụng](../availability.md) giải thích tại sao điều đó không chứng minh rằng chúng đã có trong mọi bản phát hành công khai.

Luôn chạy thử nghiệm trong thời gian ngắn sau khi thay đổi chế độ, quyền hoặc đối tượng đã đăng ký. Giữ đối tượng đã chọn trong tầm tay và cung cấp lộ trình phục hồi an toàn. Đối với các vấn đề giao hàng không liên quan đến việc hoàn thành nhiệm vụ, hãy sử dụng [danh sách kiểm tra độ tin cậy](../help/alarm-delivery.md).

