---
title: Tình trạng phân phối và phiên bản của BarcodeWake
lang: vi
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# Tình trạng phân phối và phiên bản của BarcodeWake

BarcodeWake có danh sách công khai đã xác minh trên Google Play cho Android. Vào ngày kiểm toán, Google Play hiển thị phiên bản 1.0.0, trong khi dự án mã nguồn đã kiểm tra khai báo phiên bản 2.0.0+2. Không có danh sách App Store công khai nào được xác minh.

## Phân phối công khai đã xác minh

Gói Android được liệt kê công khai dưới dạng [BarcodeWake: No Cheat Alarm trên Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). Ảnh chụp nhanh của cửa hàng được chụp cho tài liệu này ghi nhận phiên bản 1.0.0 và ngày cập nhật lần cuối vào tháng 3 năm 2026. Ảnh chụp nhanh đó là bằng chứng về danh sách tại một thời điểm, không phải là lời hứa rằng mọi khu vực đều thấy cùng một bản phát hành hoặc rằng danh sách sẽ không thay đổi.

Cây mã nguồn chứa các dự án nền tảng Android và iOS. Mã nguồn nền tảng không chứng minh việc đăng tải trên cửa hàng. Vì không có trang App Store nào được xác minh, các tài liệu này mô tả các mục liên quan đến iOS chỉ là hỗ trợ mã nguồn và không cho người đọc biết rằng BarcodeWake hiện có thể tải xuống từ Apple.

## Tại sao hai số phiên bản xuất hiện

Kho lưu trữ `pubspec.yaml` khai báo phiên bản mã nguồn 2.0.0+2 và nhật ký thay đổi của nó mô tả một hệ thống nhiệm vụ rộng hơn so với danh sách công khai đã chụp. Việc phát hành trên cửa hàng có thể chậm hơn so với nhánh phát triển, được phân giai đoạn theo khu vực, hoặc đơn giản là chưa được phát hành. Nếu không có bản ghi cửa hàng phù hợp, phát biểu an toàn là hẹp: khả năng tồn tại trong mã nguồn đã kiểm tra, trong khi tính khả dụng công khai chỉ được chứng minh cho phiên bản cửa hàng đã chụp.

Khi một trang tính năng nói "mã nguồn hiện tại", cách diễn đạt đó là cố ý. Trước khi dựa vào chuỗi nhiệm vụ, chia sẻ cài đặt hoặc khả năng mới hơn khác, hãy kiểm tra phiên bản của ứng dụng đã cài đặt và các điều khiển hiển thị. Bắt đầu với [hành vi nhiệm vụ](features/missions.md), sau đó chỉ sử dụng [hướng dẫn cài đặt](guides/set-up-an-alarm.md) cho các tùy chọn mà bản dựng đã cài đặt thực sự hiển thị.

## Yêu cầu thiết bị và kiểm tra cài đặt

Quét yêu cầu quyền camera. Các nhiệm vụ NFC, chuyển động và bước đi cần phần cứng thiết bị tương ứng. Việc phân phối báo thức trên Android có thể yêu cầu quyền thông báo và truy cập báo thức chính xác, với các cài đặt pin bổ sung trên một số nhà sản xuất. Cài đặt từ danh sách cửa hàng đã xác minh, tạo báo thức thử nghiệm trong thời gian gần, khóa màn hình và xác nhận cả âm thanh và nhiệm vụ đã chọn trước khi phụ thuộc vào nó cho một cuộc thức dậy quan trọng.

Để có danh sách ranh giới ngắn gọn, hãy đọc [sự thật sản phẩm](facts.md). Nếu báo thức thử nghiệm không hoạt động, hãy làm theo [khắc phục sự cố phân phối báo thức](help/alarm-delivery.md) thay vì tạo lại báo thức nhiều lần.

