---
title: Chính sách quyền riêng tư | QDiary
description: Chính sách quyền riêng tư của QDiary
---

# Chính sách quyền riêng tư (QDiary)

- Tên ứng dụng: QDiary
- Nhà phát triển: frog-im
- Liên hệ: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Ngày có hiệu lực: 2026-04-19
- Cập nhật lần cuối: 2026-04-19

Chính sách quyền riêng tư này được xây dựng dựa trên cách triển khai hiện tại của ứng dụng QDiary. QDiary cung cấp các tính năng viết nhật ký, tạo và phản hồi nhiệm vụ (quest), đăng nhập, lưu trữ đám mây thủ công, quảng cáo và thông báo. Trong quá trình đó, ứng dụng có thể xử lý dữ liệu cá nhân hoặc thông tin có thể được coi là dữ liệu cá nhân trong phạm vi cần thiết.

## 1. Các tính năng được cung cấp

QDiary cung cấp các tính năng sau:

- Viết, chỉnh sửa và xem nhật ký
- Phân loại theo danh mục và xem lịch
- Tạo nhiệm vụ, phản hồi nhiệm vụ và xử lý hoàn thành nhiệm vụ
- Khóa ứng dụng nhật ký cục bộ và mã hóa cục bộ
- Đăng nhập bằng email, xác minh email, đăng nhập ẩn danh (khách) và đặt lại mật khẩu
- Lưu và tải dữ liệu đám mây do người dùng chủ động thực hiện
- Hiển thị quảng cáo và xử lý các tùy chọn quyền riêng tư liên quan đến quảng cáo
- Thông báo nhắc nhở nhiệm vụ

## 2. Các loại thông tin được xử lý

### 2-1. Thông tin do người dùng trực tiếp nhập

- Địa chỉ email
- Mật khẩu
- Tiêu đề nhật ký, nội dung, ngày, danh mục và mức độ khó
- Phản hồi nhiệm vụ, nội dung suy ngẫm và thông tin về nhiệm vụ đã chọn
- Các giá trị lựa chọn liên quan đến hồ sơ nhiệm vụ và văn bản tóm tắt
- Cụm mật khẩu dùng để khóa ứng dụng nhật ký

### 2-2. Thông tin được ứng dụng lưu trữ trên thiết bị

- Cơ sở dữ liệu nhật ký cục bộ (SQLite)
- Thông tin trạng thái nhiệm vụ của nhật ký cục bộ
- Các giá trị trạng thái liên quan đến điểm danh, cài đặt, ngôn ngữ, thông báo và quảng cáo
- Giá trị xác minh khóa ứng dụng, salt và siêu dữ liệu mã hóa
- Thông tin lập lịch thông báo nhiệm vụ

### 2-3. Thông tin tài khoản và nhận dạng

Thông qua Firebase Authentication, các thông tin sau có thể được xử lý:

- Firebase UID
- Địa chỉ email
- Tình trạng xác minh email
- Việc có đang sử dụng đăng nhập ẩn danh hay không

### 2-4. Thông tin quảng cáo và xử lý đồng ý

Khi sử dụng Google AdMob và SDK UMP, các thông tin sau có thể được xử lý:

- Mã nhận dạng quảng cáo (như Android AD_ID)
- Địa chỉ IP và thông tin mạng
- Thông tin thiết bị, phiên bản hệ điều hành và thông tin ứng dụng
- Thông tin về lượt hiển thị quảng cáo, lượt nhấp và xử lý phần thưởng
- Trạng thái đồng ý quảng cáo và trạng thái tùy chọn quyền riêng tư

### 2-5. Thông tin liên quan đến thông báo

- Việc người dùng có cấp quyền thông báo hay không
- Giá trị định danh của các nhật ký có nhiệm vụ đang diễn ra
- Nội dung thông báo nhiệm vụ
- Thời gian thông báo đã được lên lịch

## 3. Mục đích xử lý

Ứng dụng xử lý thông tin cho các mục đích sau:

- Đăng ký, đăng nhập, xác minh email và đặt lại mật khẩu
- Viết, lưu và xem nhật ký
- Tạo nhiệm vụ, phản hồi và xác định hoàn thành
- Mã hóa và giải mã cục bộ liên quan đến khóa ứng dụng
- Lưu và tải dữ liệu đám mây theo yêu cầu của người dùng
- Cung cấp thông báo nhiệm vụ
- Cung cấp quảng cáo, xử lý phần thưởng quảng cáo và phản ánh trạng thái đồng ý quảng cáo
- Bảo mật, xử lý lỗi và vận hành dịch vụ

## 4. Lưu trữ cục bộ, lưu trữ đám mây và xử lý bên ngoài

### 4-1. Lưu trữ cục bộ

Thông tin nhật ký và nhiệm vụ chủ yếu được lưu trong cơ sở dữ liệu cục bộ của thiết bị.

- Nếu không bật khóa ứng dụng: được lưu cục bộ theo dạng thông thường
- Nếu bật khóa ứng dụng: một số thông tin như tiêu đề nhật ký, nội dung và trạng thái nhiệm vụ có thể được mã hóa và lưu cục bộ

### 4-2. Lưu trữ đám mây

Ứng dụng chỉ lưu dữ liệu vào Firebase Firestore khi người dùng trực tiếp thực hiện tính năng `Save`.

Theo cấu hình hiện tại của dự án:

- Không sử dụng đồng bộ hóa toàn bộ tự động
- Dữ liệu chỉ được lưu vào Firestore `savedDiaries` khi người dùng tự lưu thủ công
- Khi lưu, tiêu đề nhật ký, nội dung và trạng thái nhiệm vụ có thể được lưu dưới dạng mã hóa tùy theo trạng thái khóa ứng dụng tại thời điểm đó
- Dữ liệu chỉ được tải trở lại bộ nhớ cục bộ khi người dùng thực hiện `Load`

### 4-3. Xử lý bên ngoài cho việc tạo và phản hồi nhiệm vụ

Khi người dùng yêu cầu tạo nhiệm vụ hoặc phản hồi, các thông tin sau có thể được dùng cho xử lý bên ngoài thông qua Firebase Functions:

- Tiêu đề nhật ký
- Nội dung nhật ký hoặc nội dung phản hồi
- Danh mục
- Mức độ khó
- Nhiệm vụ đã chọn
- Thông tin tóm tắt hồ sơ nhiệm vụ

Những thông tin này được sử dụng để tạo và đánh giá nhiệm vụ thông qua OpenAI API.

Lưu ý quan trọng:

- Nội dung nhật ký liên quan chỉ được dùng cho xử lý bên ngoài khi tính năng nhiệm vụ được sử dụng.
- Theo cấu hình hiện tại của dự án, không sử dụng mã lưu nhật ký nhiệm vụ vào một bộ sưu tập riêng có tên `questLogs`.

## 5. Dịch vụ của bên thứ ba và xử lý ủy thác

### 5-1. Google Firebase

Mục đích:

- Xác thực (Firebase Authentication)
- Lưu trữ trên Firestore
- Thực thi Cloud Functions

Thông tin có thể được xử lý:

- UID, địa chỉ email và trạng thái xác thực
- Dữ liệu nhật ký do người dùng lưu thủ công
- Dữ liệu yêu cầu nhiệm vụ

### 5-2. OpenAI

Mục đích:

- Tạo nhiệm vụ
- Phản hồi nhiệm vụ và đánh giá hoàn thành

Thông tin có thể được xử lý:

- Tiêu đề/nội dung nhật ký
- Văn bản nhiệm vụ
- Mức độ khó và danh mục
- Nội dung phản hồi do người dùng nhập
- Thông tin tóm tắt hồ sơ nhiệm vụ

### 5-3. Google AdMob / UMP

Mục đích:

- Cung cấp quảng cáo biểu ngữ, quảng cáo xen kẽ và quảng cáo có thưởng
- Xử lý đồng ý quảng cáo và các tùy chọn quyền riêng tư

Thông tin có thể được xử lý:

- Mã nhận dạng quảng cáo
- Thông tin thiết bị và mạng
- Thông tin tương tác với quảng cáo
- Trạng thái đồng ý

## 6. Thông báo về chuyển dữ liệu ra nước ngoài

Ứng dụng có thể xử lý dữ liệu cá nhân hoặc thông tin liên quan bên ngoài quốc gia của người dùng trong các trường hợp sau:

| Mục | Chi tiết |
|---|---|
| Bên nhận | Google LLC, OpenAI và các đơn vị vận hành hạ tầng liên quan |
| Quốc gia nhận dữ liệu | Hoa Kỳ, v.v. |
| Thời điểm chuyển | Trong quá trình đăng nhập, tạo/phản hồi nhiệm vụ, yêu cầu quảng cáo và xử lý đồng ý |
| Phương thức chuyển | Giao tiếp mạng được mã hóa |
| Mục đích chuyển | Xác thực, lưu trữ dữ liệu, xử lý serverless, tạo/đánh giá nhiệm vụ bằng AI và cung cấp quảng cáo |

## 7. Thời gian lưu giữ và sử dụng

Ứng dụng lưu giữ thông tin theo các tiêu chí sau:

- Thông tin nhật ký/cài đặt cục bộ: cho đến khi người dùng xóa hoặc gỡ cài đặt ứng dụng
- Thông tin tài khoản Firebase: trong thời gian người dùng duy trì tài khoản
- Dữ liệu lưu trên Firestore: trong thời gian người dùng giữ lại các mục đã lưu
- Dữ liệu xử lý yêu cầu nhiệm vụ: trong phạm vi cần thiết cho xử lý serverless
- Dữ liệu liên quan đến quảng cáo/đồng ý: theo chính sách của từng nhà cung cấp bên ngoài

Ngoài ra, dự án hiện tại còn bao gồm logic dọn dẹp tự động như sau:

- Dọn dẹp tài khoản người dùng ẩn danh và dữ liệu Firestore thuộc các bộ sưu tập con của người dùng sau một khoảng thời gian nhất định
- Dọn dẹp tài khoản người dùng thông thường không hoạt động trong thời gian dài và dữ liệu Firestore thuộc các bộ sưu tập con của người dùng

Tuy nhiên, việc các cơ chế này có thực sự được áp dụng trong môi trường vận hành hay không có thể khác nhau tùy thuộc vào trạng thái triển khai và cấu hình máy chủ.

## 8. Thông báo về khóa ứng dụng và mã hóa cục bộ

Ứng dụng cung cấp một tính năng riêng là `Diary App Lock`.

- Cụm mật khẩu dùng để khóa ứng dụng là độc lập với mật khẩu tài khoản.
- Cụm mật khẩu dùng để khóa ứng dụng được sử dụng để mã hóa và giải mã nhật ký cục bộ.
- Ngay cả khi nhập sai cụm mật khẩu, bản thân ứng dụng có thể không phải lúc nào cũng bị khóa hoàn toàn; thay vào đó, một số nội dung nhật ký có thể không đọc được.
- Một số nhật ký có thể được mã hóa riêng dựa trên cụm mật khẩu được sử dụng tại thời điểm viết hoặc mở khóa tạm thời.

Người dùng cần giữ cụm mật khẩu của mình an toàn; nếu làm mất, việc khôi phục một phần dữ liệu cục bộ có thể gặp khó khăn.

## 9. Thông báo về nhiệm vụ

Nếu người dùng bật thông báo nhiệm vụ, các thông báo cục bộ có thể được lên lịch cho từng nhật ký có nhiệm vụ đang diễn ra.

- Việc lên lịch chủ yếu được xử lý thông qua hệ thống lập lịch nội bộ của thiết bị.
- Theo cấu hình hiện tại của dự án, không có cấu trúc nào được xác nhận là sẽ định kỳ gửi nguyên văn nội dung nhật ký tới máy chủ trung tâm chỉ nhằm mục đích thông báo.

## 10. Thông báo về việc sử dụng quyền

Ứng dụng có thể sử dụng các quyền sau để cung cấp chức năng của mình:

- `INTERNET`: giao tiếp với Firebase, OpenAI và các SDK quảng cáo
- `com.google.android.gms.permission.AD_ID`: sử dụng mã nhận dạng quảng cáo
- `POST_NOTIFICATIONS`: hiển thị thông báo nhiệm vụ
- `RECEIVE_BOOT_COMPLETED`: khôi phục các thông báo đã lên lịch sau khi thiết bị khởi động lại

Các quyền chỉ được sử dụng trong phạm vi cần thiết để thực hiện các chức năng tương ứng.

## 11. Quyền của chủ thể dữ liệu và cách thực hiện

Người dùng có thể thực hiện các quyền sau:

- Truy cập, chỉnh sửa và xóa dữ liệu trong ứng dụng
- Xóa hoặc ghi đè dữ liệu đã lưu trên đám mây
- Yêu cầu đăng xuất và xóa tài khoản
- Thay đổi các tùy chọn quyền riêng tư của quảng cáo
- Tắt quyền thông báo

Cách thực hiện các quyền này:

- Xóa hoặc chỉnh sửa nhật ký trực tiếp trong ứng dụng
- Xóa ứng dụng hoặc đặt lại dữ liệu cục bộ
- Đăng xuất khỏi tài khoản và yêu cầu xóa riêng
- Thay đổi thông báo, mã nhận dạng quảng cáo và quyền trong phần cài đặt thiết bị
- Email liên hệ: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 12. Biện pháp bảo mật

Ứng dụng áp dụng hoặc có thể áp dụng các biện pháp bảo vệ sau:

- Giao tiếp dựa trên HTTPS
- Khóa ứng dụng nhật ký cục bộ và mã hóa
- Lưu trữ tách biệt các giá trị xác minh cụm mật khẩu
- Sử dụng Firebase Authentication
- Yêu cầu quyền ở mức tối thiểu cần thiết

Tuy nhiên, rủi ro vẫn có thể phát sinh tùy thuộc vào trạng thái bảo mật của thiết bị người dùng, chẳng hạn như root, jailbreak, phần mềm độc hại hoặc việc sử dụng thiết bị dùng chung.

## 13. Dữ liệu cá nhân của trẻ em

Ứng dụng này không được thiết kế như một dịch vụ chủ yếu dành cho trẻ em. Tuy nhiên, các tùy chọn liên quan đến độ tuổi trong UMP có thể được áp dụng trong quá trình xử lý quảng cáo/đồng ý.

## 14. Thay đổi đối với chính sách này

Chính sách này có thể được sửa đổi do thay đổi về pháp luật, dịch vụ của bên thứ ba hoặc các tính năng của ứng dụng.

- Cập nhật lần cuối cho phiên bản hiện tại: **2026-04-19**

## 15. Liên hệ

- Nhà phát triển: frog-im
- Email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

