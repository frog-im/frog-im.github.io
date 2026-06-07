---
title: Chính sách quyền riêng tư | TimeBack
description: Chính sách quyền riêng tư của TimeBack
lang: vi
last_updated: 2026-06-06
---

# Chính sách bảo mật (TimeBack)

- **Tên ứng dụng:** TimeBack
- **Nhà phát triển:** frog-im
- **Liên hệ:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Ngày có hiệu lực:** 2026-06-03
- **Cập nhật lần cuối:** 2026-06-06

Chính sách quyền riêng tư này dựa trên việc triển khai hiện tại của ứng dụng TimeBack. TimeBack cung cấp tính năng đánh giá thời gian sử dụng thiết bị, mục tiêu hàng ngày, bản ghi thời gian đã lấy lại, phản ánh, thử thách, thông báo, chia sẻ và các tính năng quảng cáo.

## 1. Tính năng

TimeBack cung cấp các tính năng sau:

- Đánh giá thời gian sử dụng ứng dụng thông qua quyền truy cập sử dụng Android
- Mục tiêu sử dụng hàng ngày, lời nhắc và thông báo sử dụng trên thanh trạng thái
- Thông báo cảnh báo giới hạn cứng và hiển thị lớp phủ
- Lựa chọn ứng dụng ngoại lệ lớp phủ
- Bản ghi hoạt động theo thời gian được thu hồi
- Hồ sơ phản ánh hàng ngày
- Thử thách tiến độ và quản lý danh sách kiểm tra
- Chia sẻ hình ảnh chỉ số sử dụng
- Quảng cáo Google AdMob và các tùy chọn bảo mật dựa trên UMP

## 2. Thông tin chúng tôi xử lý

### 2-1. Quyền truy cập đọc qua thông tin sử dụng

Nếu người dùng cấp quyền `PACKAGE_USAGE_STATS` cho Android, ứng dụng có thể đọc thông tin sau từ thiết bị:

- Tên gói ứng dụng
- Tên ứng dụng
- Thời gian sử dụng ứng dụng
- Phạm vi ngày và giờ được sử dụng để tổng hợp mức sử dụng

Thông tin này được sử dụng để cung cấp số liệu thống kê sử dụng và so sánh việc sử dụng với mục tiêu của người dùng.

### 2-2. Thông tin được người dùng nhập hoặc định cấu hình

- Mục tiêu sử dụng hàng ngày
- Trạng thái và khoảng thời gian kích hoạt lời nhắc sử dụng
- Cài đặt hiển thị sử dụng thanh trạng thái
- Danh mục hoạt động có thời gian được lấy lại, tiêu đề, thời gian bắt đầu và thời lượng
- Văn bản phản ánh hàng ngày
- Tiến trình thử thách và các mục trong danh sách kiểm tra
- Danh sách ứng dụng ngoại lệ lớp phủ

### 2-3. Thông tin được lưu trữ trên thiết bị

Ứng dụng có thể lưu trữ thông tin sau trong cơ sở dữ liệu SQLite cục bộ hoặc SharedPreferences:

- Bản ghi thời gian sử dụng ứng dụng
- Mục tiêu và cài đặt hàng ngày
- Bản ghi hoạt động theo thời gian được thu hồi
- Hồ sơ phản ánh hàng ngày
- Tiến trình thử thách và trạng thái danh sách kiểm tra
- Trạng thái hoàn tất quá trình giới thiệu
- Các cài đặt như lời nhắc sử dụng, cảnh báo giới hạn cứng, hiển thị thanh trạng thái và các ứng dụng ngoại lệ lớp phủ
- Sự đồng ý của quảng cáo địa phương và trạng thái tùy chọn quyền riêng tư

Dựa trên cách triển khai hiện tại, các bản ghi cục bộ này không được tự động tải lên máy chủ frog-im.

### 2-4. Dữ liệu về quảng cáo và sự đồng ý

Khi Quảng cáo trên thiết bị di động của Google SDK (AdMob) và UMP được sử dụng, Google hoặc các đơn vị liên kết của Google có thể xử lý thông tin như:

- Giá trị nhận dạng quảng cáo, chẳng hạn như Android AD_ID
- IP địa chỉ và thông tin mạng
- Thông tin thiết bị, phiên bản OS và thông tin ứng dụng
- Số lần hiển thị quảng cáo, số lần nhấp chuột, dữ liệu đo lường và tín hiệu lỗi
- Trạng thái đồng ý với quảng cáo và tùy chọn quyền riêng tư
- Vị trí gần đúng

## 3. Mục đích xử lý

Ứng dụng xử lý thông tin cho các mục đích sau:

- Đọc thời gian sử dụng, hiển thị số liệu thống kê và so sánh mức sử dụng với mục tiêu
- Lưu trữ các bản ghi phản ánh và thời gian được lấy lại do người dùng nhập
- Quản lý tiến trình thử thách
- Cung cấp lời nhắc và thông báo trên thanh trạng thái
- Cung cấp thông báo cảnh báo giới hạn cứng, hiển thị lớp phủ và xử lý ngoại lệ lớp phủ
- Chia sẻ hình ảnh thống kê sử dụng khi người dùng yêu cầu
- Phân phát quảng cáo, đo lường hiệu suất quảng cáo và áp dụng các lựa chọn đồng ý với quảng cáo
- Duy trì sự ổn định của ứng dụng và phản hồi các lỗi

## 4. Lưu trữ cục bộ và xử lý bên ngoài

### 4-1. Bộ nhớ cục bộ

TimeBack lưu trữ dữ liệu người dùng chủ yếu trong bộ nhớ trong của ứng dụng trên thiết bị. Dựa trên cách triển khai hiện tại, hồ sơ sử dụng, mục tiêu, phản ánh và thông tin thử thách không được tự động tải lên máy chủ frog-im.

Bộ nhớ cục bộ có thể bao gồm những thứ sau.

| Kho | Các mục được lưu trữ | Mục đích | Phương pháp xóa |
|---|---|---|---|
| SQLcơ sở dữ liệu nhỏ | Bản ghi sử dụng ứng dụng, tên gói, tên ứng dụng, thời gian sử dụng, tổng hợp dựa trên ngày | Hiển thị số liệu thống kê sử dụng và so sánh việc sử dụng với mục tiêu | Tính năng xóa trong ứng dụng, xóa dữ liệu ứng dụng hoặc gỡ cài đặt ứng dụng |
| SQLcơ sở dữ liệu nhỏ | Các hoạt động lấy lại thời gian, suy ngẫm, tiến trình thử thách, mục danh sách kiểm tra | Hiển thị hồ sơ và quản lý tiến độ | Tính năng xóa trong ứng dụng, xóa dữ liệu ứng dụng hoặc gỡ cài đặt ứng dụng |
| Tùy chọn chia sẻ | Trạng thái hoàn tất quá trình triển khai, cài đặt lời nhắc, cài đặt cảnh báo giới hạn cố định, cài đặt hiển thị thanh trạng thái, danh sách ứng dụng ngoại lệ lớp phủ, trạng thái đồng ý với quảng cáo cục bộ | Giữ cài đặt ứng dụng | Xóa dữ liệu ứng dụng hoặc gỡ cài đặt ứng dụng |
| Tệp/bộ đệm tạm thời | Hình ảnh thống kê sử dụng được chia sẻ và các tệp tạm thời tương tự | Thực hiện chia sẻ theo yêu cầu của người dùng | Đã xóa sau khi chia sẻ nếu có thể hoặc theo OS/chính sách dọn dẹp ứng dụng |

Khi người dùng xóa dữ liệu ứng dụng hoặc gỡ cài đặt ứng dụng, dữ liệu được lưu trữ trong bộ nhớ trong của ứng dụng thường bị xóa. Tuy nhiên, bản sao lưu của Android, bản sao lưu của nhà sản xuất, bản sao lưu đám mây hoặc các tệp được người dùng chia sẻ trực tiếp có thể được giữ lại riêng biệt theo chính sách của các dịch vụ đó.

Hồ sơ sử dụng và văn bản phản ánh có thể tiết lộ thói quen hoặc sở thích cá nhân. Trên các thiết bị dùng chung, người dùng nên sử dụng các biện pháp bảo vệ thích hợp như khóa thiết bị hoặc tách các tài khoản OS.

### 4-2. Tải lên máy chủ

Dựa trên dự án hiện tại, TimeBack không tự động tải hồ sơ sử dụng, phản ánh hoặc hồ sơ thử thách lên máy chủ frog-im. Nếu người dùng sử dụng tính năng chia sẻ, hình ảnh thống kê được tạo có thể được chuyển sang ứng dụng hoặc dịch vụ bên ngoài do người dùng chọn.

### 4-3. Xử lý quảng cáo

Google AdMob và UMP được sử dụng để quản lý sự đồng ý và quản lý sự đồng ý trong ứng dụng. Thông tin liên quan đến quảng cáo có thể được xử lý trên cơ sở hạ tầng của Google.

## 5. Dịch vụ và bộ xử lý của bên thứ ba

### 5-1. Google AdMob / UMP

Mục đích:

- Phân phối quảng cáo biểu ngữ
- Sự đồng ý của quảng cáo và xử lý tùy chọn quyền riêng tư
- Đo lường hiệu suất quảng cáo và ngăn chặn gian lận

Thông tin có thể được xử lý:

- Mã nhận dạng quảng cáo
- Thông tin thiết bị và mạng
- Thông tin tương tác quảng cáo
- Trạng thái đồng ý và tùy chọn quyền riêng tư

### 5-2. Chia sẻ ứng dụng hoặc dịch vụ mục tiêu

Nếu người dùng trực tiếp sử dụng tính năng chia sẻ hình ảnh theo chỉ số sử dụng thì ứng dụng hoặc dịch vụ bên ngoài đã chọn có thể xử lý hình ảnh được chia sẻ. Quá trình xử lý đó được điều chỉnh bởi chính sách quyền riêng tư của dịch vụ đã chọn.

## 6. Thông báo chuyển tiền xuyên biên giới

Thông tin có thể được xử lý bên ngoài quốc gia của người dùng trong các trường hợp sau.

| Mục | Chi tiết |
|---|---|
| Người nhận | Google LLC và các chi nhánh của nó |
| Điểm đến | Hoa Kỳ và các quốc gia/khu vực khác nơi đặt cơ sở hạ tầng của Google |
| Thời gian | Khi ứng dụng chạy, yêu cầu quảng cáo, hiển thị hoặc đo lường quảng cáo, xử lý lượt nhấp hoặc xử lý sự đồng ý |
| Phương pháp | Giao tiếp mạng được mã hóa (HTTPS/TLS) |
| Mục đích | Phân phối quảng cáo, xử lý trạng thái cá nhân hóa, đo lường, phân tích, cải thiện độ ổn định của dịch vụ, tuân thủ pháp luật |
| dữ liệu | Giá trị nhận dạng quảng cáo, thông tin về thiết bị/ứng dụng/mạng, thông tin tương tác với quảng cáo, trạng thái đồng ý, vị trí gần đúng, v.v. |
| giữ lại | Phù hợp với chính sách của Google và luật hiện hành |

Để biết chi tiết, vui lòng xem [Cross-Border Transfer Notice](./policy/).

## 7. Danh sách ứng dụng đã cài đặt và ngoại lệ lớp phủ

Trên Android, nếu người dùng định cấu hình các ứng dụng ngoại lệ lớp phủ, ứng dụng có thể đọc tên gói và tên ứng dụng của các ứng dụng có thể khởi chạy trên thiết bị để hiển thị danh sách lựa chọn. Tên gói do người dùng chọn làm ngoại lệ sẽ được lưu trữ trong SharedPreferences trên thiết bị và chỉ được sử dụng để tránh hiển thị lớp phủ cảnh báo giới hạn cứng trên đầu các ứng dụng đó.

## 8. Giữ lại

Ứng dụng lưu giữ thông tin theo các tiêu chuẩn sau:

- Thông tin sử dụng cục bộ, mục tiêu, phản ánh và thách thức: cho đến khi người dùng xóa nó, xóa dữ liệu ứng dụng hoặc gỡ cài đặt ứng dụng
- Cài đặt SharedPreferences: cho đến khi người dùng xóa dữ liệu ứng dụng hoặc gỡ cài đặt ứng dụng
- Tệp tạm thời cho hình ảnh được chia sẻ: khi cần để chia sẻ hoặc theo chính sách dọn dẹp OS
- Dữ liệu liên quan đến quảng cáo và sự đồng ý: theo chính sách của Google và các bên thứ ba có liên quan khác

## 9. Quyền

Ứng dụng có thể sử dụng các quyền sau:

- `PACKAGE_USAGE_STATS`: đọc thời gian sử dụng ứng dụng
- `POST_NOTIFICATIONS`: hiển thị lời nhắc sử dụng và thông báo trên thanh trạng thái
- `SYSTEM_ALERT_WINDOW`: hiển thị lớp phủ cảnh báo giới hạn cứng
- `INTERNET`: liên lạc với quảng cáo SDKs và hiển thị các trang thông báo pháp lý
- `ACCESS_NETWORK_STATE`: kiểm tra trạng thái mạng
- `com.google.android.gms.permission.AD_ID`: sử dụng số nhận dạng quảng cáo

Quyền chỉ được sử dụng khi cần thiết cho các tính năng của ứng dụng. Người dùng có thể thu hồi quyền trong cài đặt thiết bị nhưng các tính năng liên quan có thể bị hạn chế.

## 10. Quyền và lựa chọn của người dùng

Người dùng có thể:

- Xem, chỉnh sửa hoặc xóa bản ghi bên trong ứng dụng
- Xóa thông tin cục bộ bằng cách xóa dữ liệu ứng dụng hoặc gỡ cài đặt ứng dụng
- Thay đổi cài đặt quyền truy cập sử dụng, thông báo và mã nhận dạng quảng cáo trong cài đặt thiết bị
- Thu hồi quyền lớp phủ và thay đổi cài đặt ứng dụng ngoại lệ lớp phủ
- Thay đổi tùy chọn bảo mật quảng cáo
- Liên hệ với chúng tôi nếu có câu hỏi về quyền riêng tư hoặc yêu cầu xóa

Email liên hệ: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 11. Các biện pháp an ninh

Ứng dụng áp dụng hoặc có thể áp dụng các biện pháp bảo vệ sau:

- Giao tiếp bên ngoài dựa trên HTTPS/TLS
- Xử lý dữ liệu cục bộ đầu tiên
- Yêu cầu quyền tối thiểu cần thiết cho các tính năng của ứng dụng
- Áp dụng trạng thái đồng ý quảng cáo

Các điều kiện bảo mật thiết bị như root, bẻ khóa, phần mềm độc hại hoặc sử dụng thiết bị dùng chung có thể tạo thêm rủi ro.

## 12. Quyền riêng tư của trẻ em

TimeBack không được thiết kế chủ yếu cho trẻ em. Các cài đặt liên quan đến độ tuổi hoặc chính sách nền tảng của Quảng cáo trên thiết bị di động của Google SDK và UMP có thể áp dụng trong quá trình xử lý quảng cáo và lấy sự đồng ý.

## 13. Thay đổi

Chính sách này có thể được cập nhật do những thay đổi về luật, cấu hình dịch vụ của bên thứ ba hoặc tính năng ứng dụng. Những thay đổi quan trọng sẽ được thông báo qua thông báo trong ứng dụng hoặc bằng cách cập nhật trang này.

## 14. Liên hệ

- Nhà phát triển: frog-im
- Email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
