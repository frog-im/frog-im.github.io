---
title: Chính sách quyền riêng tư | know_me
description: know_me (PeopleNote, Memory for People) Chính sách quyền riêng tư (Tiếng Việt)
---

# Chính sách quyền riêng tư (know_me / PeopleNote, Memory for People)

- **Tên ứng dụng:** know_me (PeopleNote, Memory for People)
- **Nhà phát triển:** frog-im
- **Người phụ trách bảo vệ thông tin cá nhân / Người liên hệ:** frog-im
- **Liên hệ:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Ngày có hiệu lực:** 2026-03-04
- **Cập nhật lần cuối:** 2026-03-04

> Chính sách này được xây dựng dựa trên các thông tin mà ứng dụng xử lý và các tính năng liên quan của ứng dụng.  
> Nếu có bất kỳ luật hoặc quy định bắt buộc nào áp dụng tại một quốc gia hoặc khu vực cụ thể, các luật hoặc quy định đó có thể được ưu tiên áp dụng.

---

## 1. Mục đích và phạm vi áp dụng

`know_me` là một ứng dụng được thiết kế để giúp người dùng ghi lại và quản lý thông tin về mọi người, đồng thời khi cần có thể sao lưu, khôi phục và chia sẻ các thông tin đó dưới dạng tệp PDF.

Các tính năng chính của ứng dụng bao gồm:

- Lưu trữ thông tin riêng của từng người (chẳng hạn như tên, văn bản nhận dạng, ghi chú, đặc điểm tính cách, quốc gia, giới tính, thông tin liên hệ, v.v.)
- Phân loại thư mục, tìm kiếm và chức năng hợp nhất
- Đính kèm ảnh và quản lý mô tả
- Xuất và nhập bản sao lưu (`.knm`)
- Xuất tệp PDF
- Khóa ứng dụng (mật khẩu / hình mở khóa)
- Quản lý quảng cáo và sự đồng ý (AdMob / UMP)

Ứng dụng này không yêu cầu đăng ký tài khoản riêng, và dữ liệu cốt lõi của người dùng nhìn chung được lưu trữ cục bộ trên thiết bị của người dùng.  
Tuy nhiên, một số SDK của bên thứ ba được tích hợp cho mục đích quản lý quảng cáo và sự đồng ý có thể xử lý một số thông tin.

---

## 2. Các loại thông tin cá nhân được xử lý

### 2-1) Thông tin do người dùng trực tiếp nhập

Các thông tin sau chỉ được lưu khi người dùng trực tiếp nhập vào:

- Tên
- Văn bản nhận dạng (ví dụ: ngoại hình / đặc điểm được dùng làm nội dung ghi chú)
- Ghi chú
- Đặc điểm tính cách, quốc gia, giới tính
- Số điện thoại
- Văn bản liên quan đến thời điểm xuất hiện / thời điểm gặp gỡ
- Thông tin nền tảng / trang web
- Tên / màu thư mục
- Mô tả hình ảnh (caption)

### 2-2) Tệp được chọn trên thiết bị

- Tệp hình ảnh do người dùng chọn khi đính kèm ảnh
- Tệp sao lưu `.knm` do người dùng chọn khi nhập bản sao lưu
- Đường dẫn lưu và tệp đã lưu do người dùng chọn khi xuất PDF / sao lưu

### 2-3) Dữ liệu được lưu cục bộ trong ứng dụng

Các dữ liệu sau có thể được lưu trên thiết bị của người dùng để cung cấp các tính năng của ứng dụng:

- Cơ sở dữ liệu SQLite (`people_note.db`): siêu dữ liệu liên quan đến người / thư mục / nền tảng / trang web / hình ảnh
- Tệp hình ảnh: được mã hóa và lưu trong thư mục tài liệu của ứng dụng (`.enc`)
- Cài đặt ứng dụng (`SharedPreferences`): giao diện, sắp xếp, tùy chọn quyền riêng tư / quảng cáo, tùy chọn che dữ liệu trong PDF, chính sách khóa ứng dụng, v.v.
- Thông tin khóa ứng dụng: giá trị băm và salt của mật khẩu / hình mở khóa (`SharedPreferences`)
- Khóa mã hóa cục bộ: được lưu trong `flutter_secure_storage`
- Tệp tạm: bản xem trước giải mã hình ảnh, tệp bộ nhớ đệm cho nhập / xuất, v.v. (thư mục tạm)

### 2-4) Thông tin có thể được xử lý tự động trong quá trình quản lý quảng cáo và sự đồng ý

Khi các tính năng quảng cáo hoặc quản lý sự đồng ý được bật, các SDK của Google LLC và các đối tác liên quan (chẳng hạn như AdMob và UMP) có thể tự động xử lý các thông tin sau:

- Mã nhận dạng quảng cáo (AAID / IDFA, v.v.)
- Địa chỉ IP và thông tin mạng
- Thông tin thiết bị (phiên bản hệ điều hành, mẫu thiết bị, phiên bản ứng dụng, v.v.)
- Thông tin tương tác với quảng cáo (lượt hiển thị, lượt nhấp, v.v.)
- Trạng thái đồng ý và thông tin lựa chọn quyền riêng tư
- Thông tin liên quan đến chẩn đoán, hiệu năng và bảo mật

Dữ liệu cốt lõi của người dùng trong ứng dụng nhìn chung không được tải lên máy chủ của nhà phát triển, nhưng một phần các thông tin nêu trên có thể được truyền đến các dịch vụ của bên thứ ba trong khi các tính năng quảng cáo / sự đồng ý đang được sử dụng.

---

## 3. Mục đích xử lý thông tin cá nhân

Ứng dụng xử lý thông tin cá nhân hoặc thông tin liên quan cho các mục đích sau:

- Ghi lại và xem thông tin về người, tập trung vào danh bạ / ghi chú
- Cung cấp các tính năng sắp xếp như phân loại thư mục, tìm kiếm và hợp nhất
- Đính kèm và hiển thị ảnh
- Thực hiện các tính năng do người dùng yêu cầu, chẳng hạn như sao lưu / khôi phục và xuất PDF
- Cung cấp các tính năng bảo mật khóa ứng dụng
- Cung cấp quảng cáo, quản lý sự đồng ý, ngăn chặn hành vi gian lận và tuân thủ các nghĩa vụ pháp lý

---

## 4. Thời gian lưu giữ và lưu trữ thông tin cá nhân

- Dữ liệu nội bộ của ứng dụng (SQLite, cài đặt cục bộ, hình ảnh được mã hóa): được lưu trên thiết bị của người dùng cho đến khi ứng dụng bị xóa, dữ liệu ứng dụng bị xóa hoặc người dùng trực tiếp xóa dữ liệu
- Tệp tạm: được xóa sau khi tác vụ liên quan hoàn tất hoặc được dọn dẹp theo chính sách bộ nhớ đệm của hệ điều hành
- Tệp do người dùng xuất ra (PDF, tệp sao lưu): có thể vẫn còn tại vị trí lưu trữ mà người dùng đã chọn và phải do người dùng trực tiếp xóa
- Dữ liệu liên quan đến quảng cáo / sự đồng ý (được xử lý bởi bên thứ ba): tuân theo chính sách của từng nhà cung cấp dịch vụ và pháp luật hiện hành

Về nguyên tắc, ứng dụng không lưu trữ dữ liệu cốt lõi của người dùng trên máy chủ của nhà phát triển.  
Tuy nhiên, các tệp mà người dùng trực tiếp lưu vào bộ nhớ ngoài sẽ được quản lý trong chính môi trường của người dùng.

---

## 5. Quy trình và phương thức xóa thông tin cá nhân

Khi mục đích xử lý đã đạt được hoặc khi người dùng yêu cầu xóa, ứng dụng sẽ xóa các thông tin liên quan hoặc xử lý chúng theo cách để chúng không còn được tham chiếu nữa, như sau.

### 5-1) Quy trình xóa

- Khi người dùng trực tiếp xóa từng hồ sơ cá nhân, thư mục, hình ảnh, dữ liệu sao lưu, v.v., các dữ liệu đó sẽ được coi là đối tượng cần xóa ngay lập tức.
- Khi người dùng xóa ứng dụng hoặc xóa dữ liệu ứng dụng trong cài đặt thiết bị, dữ liệu được lưu trong vùng lưu trữ nội bộ của ứng dụng sẽ bị xóa theo quy trình xóa của hệ điều hành.
- Các tệp tạm sẽ được đưa vào diện dọn dẹp sau khi tác vụ liên quan kết thúc, và một số dữ liệu bộ nhớ đệm có thể còn tồn tại trong một khoảng thời gian nhất định tùy theo chính sách của hệ điều hành.

### 5-2) Phương thức xóa

- Dữ liệu SQLite: xóa các bản ghi liên quan
- Cài đặt ứng dụng (`SharedPreferences`): xóa khóa liên quan hoặc toàn bộ cài đặt
- Giá trị trong `flutter_secure_storage`: xóa các mục lưu trữ bảo mật liên quan
- Tệp nội bộ của ứng dụng (hình ảnh được mã hóa, tệp tạm, v.v.): xóa các tệp liên quan
- Các tệp PDF / sao lưu do người dùng trực tiếp lưu vào bộ nhớ ngoài: không được ứng dụng tự động xóa và phải do người dùng trực tiếp xóa

Trừ khi pháp luật hiện hành yêu cầu khác, nhà phát triển không lưu riêng dữ liệu cốt lõi của người dùng trên máy chủ của nhà phát triển.

---

## 6. Cung cấp cho bên thứ ba, thuê xử lý và chuyển dữ liệu xuyên biên giới

Ứng dụng có thể sử dụng các dịch vụ của Google để quản lý quảng cáo và sự đồng ý.

| Mục | Chi tiết |
|---|---|
| **Bên nhận / Bên được ủy thác** | Google LLC và các công ty liên kết của Google (đơn vị vận hành AdMob / UMP) |
| **Quốc gia chuyển dữ liệu** | Hoa Kỳ và các khu vực nơi hạ tầng của Google được vận hành |
| **Thời điểm chuyển dữ liệu** | Diễn ra liên tục trong quá trình yêu cầu quảng cáo, kiểm tra trạng thái đồng ý, khởi tạo SDK và vận hành |
| **Phương thức chuyển dữ liệu** | Truyền qua kết nối mạng giữa ứng dụng và máy chủ của bên thứ ba |
| **Cơ sở pháp lý cho việc chuyển dữ liệu xuyên biên giới** | Được xử lý trong phạm vi cần thiết để cung cấp dịch vụ theo các căn cứ pháp lý hiện hành, hoặc khi cần thiết, dựa trên sự đồng ý của chủ thể dữ liệu |
| **Mục đích** | Phân phối quảng cáo, đo lường quảng cáo, quản lý sự đồng ý, ngăn ngừa gian lận và tuân thủ chính sách / pháp luật |
| **Loại dữ liệu (ví dụ)** | Mã nhận dạng quảng cáo (AAID / IDFA), thông tin IP / mạng, thông tin thiết bị / ứng dụng, thông tin tương tác quảng cáo, trạng thái đồng ý |
| **Thời gian lưu giữ** | Tuân theo chính sách của Google và pháp luật hiện hành |
| **Ảnh hưởng nếu từ chối** | Quảng cáo được cá nhân hóa có thể bị hạn chế, quảng cáo không cá nhân hóa có thể được hiển thị hoặc một số tính năng liên quan đến quảng cáo có thể bị hạn chế |

Nhà phát triển không thu thập hoặc bán dữ liệu cốt lõi về hồ sơ người của ứng dụng thông qua máy chủ riêng của mình.

---

## 7. Thông tin về các quyền được sử dụng

Ứng dụng có thể sử dụng các quyền sau:

- `INTERNET`: dùng cho giao tiếp mạng của SDK quảng cáo và các tính năng mạng liên quan
- `com.google.android.gms.permission.AD_ID`: dùng cho mã nhận dạng quảng cáo (AdMob)
- `READ_MEDIA_IMAGES` (Android 13 trở lên), `READ_EXTERNAL_STORAGE` (Android 12 trở xuống): dùng để đính kèm / chọn ảnh

Các quyền chỉ được sử dụng trong phạm vi cần thiết để cung cấp các tính năng liên quan.

---

## 8. Thiết lập, vận hành và từ chối các cơ chế thu thập tự động

Ứng dụng này không trực tiếp sử dụng cookie của các trang web thông thường.  
Tuy nhiên, liên quan đến các tính năng quảng cáo và quản lý sự đồng ý, SDK của bên thứ ba có thể tự động xử lý mã nhận dạng quảng cáo, thông tin mạng, thông tin thiết bị và các dữ liệu tương tự.

Người dùng có thể điều chỉnh các cài đặt liên quan theo các cách sau:

- Thay đổi lựa chọn trong các tùy chọn quyền riêng tư của ứng dụng hoặc màn hình quản lý sự đồng ý (nếu có)
- Đặt lại hoặc xóa mã nhận dạng quảng cáo trong cài đặt hệ điều hành của thiết bị
- Giới hạn quảng cáo được cá nhân hóa hoặc điều chỉnh các tùy chọn quyền riêng tư liên quan trong cài đặt hệ điều hành của thiết bị

Nếu người dùng giới hạn quảng cáo được cá nhân hóa, quảng cáo không cá nhân hóa có thể được hiển thị hoặc một số tính năng liên quan đến quảng cáo có thể bị hạn chế.

---

## 9. Quyền của người dùng và cách thực hiện

Tùy theo pháp luật hiện hành, người dùng có thể có các quyền sau:

- Yêu cầu truy cập, chỉnh sửa hoặc xóa thông tin cá nhân
- Yêu cầu tạm dừng hoặc hạn chế việc xử lý
- Rút lại sự đồng ý đối với việc xử lý dựa trên sự đồng ý
- Thay đổi lựa chọn về quảng cáo / sự đồng ý

Các quyền này có thể được thực hiện theo các cách sau:

- Trực tiếp chỉnh sửa hoặc xóa dữ liệu trong ứng dụng
- Khởi tạo lại dữ liệu cục bộ bằng cách xóa dữ liệu ứng dụng hoặc gỡ cài đặt ứng dụng
- Thay đổi sự đồng ý đối với quảng cáo thông qua các tùy chọn quyền riêng tư / màn hình đồng ý của ứng dụng (tại các khu vực có cung cấp tính năng này)
- Đặt lại / xóa mã nhận dạng quảng cáo hoặc giới hạn quảng cáo được cá nhân hóa thông qua cài đặt hệ điều hành của thiết bị
- Liên hệ: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 10. Biện pháp bảo mật

Nhà phát triển áp dụng hoặc nỗ lực áp dụng các biện pháp sau:

- Dữ liệu người dùng nhìn chung được lưu trữ cục bộ trên thiết bị
- Các tệp hình ảnh đính kèm được lưu cục bộ ở dạng mã hóa (dựa trên AES-GCM)
- Thông tin khóa ứng dụng được lưu ở dạng băm thay vì văn bản thuần
- Tệp sao lưu được lưu sau khi đã được mã hóa dựa trên mật khẩu của người dùng
- Giao tiếp với các SDK của bên thứ ba được mã hóa (HTTPS / TLS)
- Các quyền được sử dụng với phạm vi truy cập tối thiểu cần thiết

Tuy nhiên, các rủi ro phát sinh từ tình trạng bảo mật của thiết bị người dùng (như root / jailbreak, ứng dụng độc hại hoặc lộ dữ liệu lưu trữ dùng chung) không thể được loại bỏ hoàn toàn.

---

## 11. Thông tin liên quan đến dữ liệu nhạy cảm

Ứng dụng này không yêu cầu nhập dữ liệu nhạy cảm.  
Người dùng được khuyến nghị không nhập các nội dung nhạy cảm như thông tin sức khỏe, quan điểm chính trị, tôn giáo, thông tin sinh trắc học hoặc thông tin liên quan đến đời sống tình dục vào ghi chú hoặc các trường nhập tự do.

Nếu người dùng tự nguyện nhập nội dung nhạy cảm, các thông tin đó có thể được lưu dưới dạng dữ liệu cục bộ trên thiết bị do chính người dùng trực tiếp quản lý.

---

## 12. Bảo vệ thông tin cá nhân của trẻ em

Ứng dụng này không được thiết kế chủ yếu dành cho trẻ em.  
Người giám hộ có thể quản lý việc sử dụng thông qua các tính năng kiểm soát của phụ huynh do thiết bị hoặc cửa hàng ứng dụng cung cấp.

---

## 13. Ra quyết định tự động

Ứng dụng này không thực hiện việc ra quyết định tự động dựa trên thông tin cá nhân mà tạo ra hiệu lực pháp lý hoặc ảnh hưởng quan trọng tương tự.

---

## 14. Thông báo về an toàn dữ liệu (Google Play, v.v.)

Nhà phát triển nỗ lực duy trì và cập nhật các nội dung công bố về an toàn dữ liệu trên các cửa hàng ứng dụng (chẳng hạn như Google Play) phù hợp với thực tiễn xử lý thực tế của ứng dụng và thực tiễn xử lý thực tế của các SDK bên thứ ba.

Tuy nhiên, thông tin được hiển thị trên các cửa hàng ứng dụng có thể khác nhau tùy theo phiên bản ứng dụng, quốc gia phân phối, cấu hình SDK của bên thứ ba và các thay đổi về chính sách.

---

## 15. Thông báo về mã nguồn mở

Ứng dụng sử dụng một số thư viện mã nguồn mở.  
Thông tin về các giấy phép liên quan có thể được tìm thấy trong màn hình tương ứng trong ứng dụng hoặc trong các thông báo được cung cấp thông qua kênh phân phối.

---

## 16. Liên hệ

Nếu có thắc mắc liên quan đến Chính sách quyền riêng tư này, vui lòng liên hệ:

- **Người phụ trách bảo vệ thông tin cá nhân / Người liên hệ:** frog-im
- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 17. Thay đổi đối với Chính sách quyền riêng tư này

Chính sách này có thể được sửa đổi do có thay đổi về pháp luật / chính sách, tính năng của ứng dụng hoặc SDK của bên thứ ba.  
Nếu có những thay đổi quan trọng, thông báo có thể được cung cấp thông qua thông báo trong ứng dụng, trang phân phối hoặc các bản cập nhật trên trang chính sách.

Cập nhật lần cuối: **2026-03-04**