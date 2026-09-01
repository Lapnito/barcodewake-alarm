---
title: Thuật ngữ BarcodeWake
lang: vi
app: barcodewake-alarm
page_type: glossary
updated: 2026-09-01
targets:
  - BarcodeWake terminology
facts_used:
  - core_measurement
  - data_storage
  - export_formats
---
# Thuật ngữ BarcodeWake

BarcodeWake sử dụng “mission” (nhiệm vụ) cho hành động cần thiết để tắt báo thức. Nhiệm vụ quét xác minh một mã vật lý đã đăng ký; nhiệm vụ thử thách xác minh một câu trả lời hoặc chuyển động; chia sẻ và sao lưu đề cập đến các định dạng trao đổi khác nhau.

## Thuật ngữ báo thức và nhiệm vụ

- Alarm (Báo thức): một sự kiện thức dậy được lên lịch với thời gian, các ngày hoạt động, âm thanh và cấu hình tắt.
- Mission (Nhiệm vụ): công việc phải hoàn thành trước khi tắt báo thức.
- Scan mission (Nhiệm vụ quét): nhiệm vụ dựa trên mã vạch, mã QR hoặc NFC, được so khớp với biểu diễn mã đã đăng ký.
- Challenge mission (Nhiệm vụ thử thách): nhiệm vụ toán, đánh máy, lắc hoặc bước.
- Single mode (Chế độ đơn): một nhiệm vụ đã cấu hình chạy cho báo thức.
- Chain mode (Chế độ chuỗi): các nhiệm vụ đã cấu hình chạy theo thứ tự đã chọn.
- Random mode (Chế độ ngẫu nhiên): một nhiệm vụ được chọn từ một tập hợp đã cấu hình.
- Difficulty (Độ khó): cài đặt nhiệm vụ thay đổi yêu cầu công việc; hiệu ứng chính xác phụ thuộc vào loại nhiệm vụ.

## Thuật ngữ về dữ liệu và độ tin cậy

- Registered code (Mã đã đăng ký): mã vạch, mã QR hoặc thẻ NFC vật lý liên kết với nhiệm vụ quét.
- Code hash (Băm mã): biểu diễn SHA‑256 một chiều được sử dụng bởi các đường dẫn lưu trữ và trao đổi hiện tại để so khớp các giá trị đã đăng ký.
- Local backup (Sao lưu cục bộ): biểu diễn đã xuất nhằm bảo toàn hoặc khôi phục dữ liệu ứng dụng.
- Setup QR (QR cài đặt): định dạng chia sẻ cấu hình hạn chế, không bao gồm mã đã đăng ký, định danh NFC, mã PIN và lịch sử.
- Reliability Doctor (Bác sĩ độ tin cậy): chẩn đoán trong ứng dụng dành cho quyền và cài đặt hệ thống có thể ảnh hưởng đến việc phát báo thức.
- Exact‑alarm access (Truy cập báo thức chính xác): quyền hoặc chính sách hệ thống Android cho phép lập lịch phụ thuộc thời gian.
- Battery optimisation (Tối ưu hóa pin): các điều khiển của hệ điều hành hoặc nhà cung cấp có thể hạn chế thực thi nền.

Để biết mối quan hệ tính năng đầy đủ, hãy xem [nhiệm vụ và chuỗi nhiệm vụ](features/missions.md). Để biết sự khác biệt giữa các định dạng xuất, hãy đọc [sao lưu và chia sẻ](guides/backup-and-sharing.md). Trang [thông tin thực tế](facts.md) định nghĩa những gì ứng dụng không tuyên bố đo lường.

