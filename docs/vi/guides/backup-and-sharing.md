---
title: Sao lưu và chia sẻ báo thức BarcodeWake một cách an toàn
lang: vi
app: barcodewake-alarm
page_type: guide
updated: 2026-09-01
targets:
  - how to back up or share BarcodeWake alarms
facts_used:
  - export_formats
  - data_storage
  - known_limitations
---
# Sao lưu và chia sẻ báo thức BarcodeWake một cách an toàn

Sử dụng xuất JSON khi cần giữ hoặc di chuyển dữ liệu ứng dụng của bạn, mã vạch sao lưu PDF có thể in để phục hồi, và chia sẻ mã QR cài đặt khi người khác chỉ cần cấu trúc báo thức. Việc chia sẻ cố tình bỏ qua các bí mật đã đăng ký và lịch sử.

## Chọn định dạng phù hợp cho công việc

Nguồn hiện tại cung cấp các con đường trao đổi khác nhau vì sao lưu và chia sẻ không phải là cùng một thao tác. Bản sao lưu JSON nhằm mục đích truyền dữ liệu có cấu trúc và phục hồi. Bản sao lưu PDF chuyển tài liệu phục hồi thành tài liệu mã vạch có thể in. Mã QR cài đặt được thiết kế hẹp hơn: nó có thể truyền cấu hình báo thức giới hạn mà không mang theo giá trị mã vạch đã đăng ký, định danh NFC, mã PIN hoặc lịch sử.

Không coi mã QR cài đặt như một bản sao lưu thiết bị đầy đủ. Người nhận phải đăng ký mã vật lý của riêng họ và kiểm tra quyền cục bộ. Việc chia sẻ cài đặt hiện tại cũng giới hạn số lượng báo thức mà nó mang theo, vì vậy hãy xác minh kết quả nhập thay vì cho rằng mọi lịch trình đã được chuyển. [Thông tin sản phẩm](../facts.md) ghi lại các giới hạn này.

## Tạo và bảo vệ bản sao lưu cá nhân

Sử dụng hành động xuất có sẵn trong bản dựng đã cài đặt, chọn JSON hoặc bản sao lưu có thể in theo kế hoạch phục hồi, và lưu kết quả ở nơi bạn kiểm soát. Bản sao lưu có thể tiết lộ tên báo thức, lịch trình và các cấu hình khác ngay cả khi các giá trị mã thô đã đăng ký được bảo vệ hoặc bỏ qua. Xử lý nó như dữ liệu thường nhật cá nhân: tránh liên kết công khai, máy in chia sẻ và các kênh nhắn tin không đáng tin cậy.

Sau khi xuất, hãy xác nhận rằng tệp có thể được tìm thấy và dấu thời gian của nó khớp với bản sao lưu dự định. Không xóa dữ liệu ứng dụng gốc chỉ vì lệnh xuất báo cáo thành công. Kiểm tra khôi phục là cách kiểm tra đáng tin cậy duy nhất, nhưng hãy thực hiện trên thiết bị an toàn hoặc sau khi tạo bản sao thứ hai để bản thân bài kiểm tra không trở thành sự kiện mất mát.

## Chia sẻ cấu hình mà không chia sẻ bí mật

Tạo mã QR cài đặt chỉ cho các báo thức mà người nhận nên nhận. Người nhận quét mã đó, kiểm tra lịch trình đã nhập và cung cấp mã, thẻ NFC hoặc chi tiết phục hồi của riêng họ. Thiết kế này ngăn cấu hình được chia sẻ chuyển giao âm thầm khóa vật lý để tắt báo thức của người khác.

Sau khi nhập, mỗi người nên chạy [kiểm tra cài đặt báo thức](set-up-an-alarm.md) đầy đủ. Quyền, cảm biến và các hạn chế của hệ điều hành không được chuyển trong mã QR. Nếu báo thức đã nhập không xuất hiện khi bị khóa, hãy làm theo [khắc phục sự cố giao báo thức](../help/alarm-delivery.md).

Phiên bản nguồn và cửa hàng khác nhau trong quá trình kiểm tra này, vì vậy bản dựng công khai đã cài đặt có thể không hiển thị mọi tùy chọn trao đổi được mô tả ở đây. [Tính khả dụng](../availability.md) giải thích cách diễn giải các khả năng chỉ có trong mã nguồn.

