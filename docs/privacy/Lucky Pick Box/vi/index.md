---
title: Chính sách quyền riêng tư | Lucky Pick Box
description: Lucky Pick Box Chính sách quyền riêng tư
lang: vi
last_updated: 2026-06-15
---

# Chính sách quyền riêng tư (Lucky Pick Box / 뽑기박스)

- **Tên ứng dụng:** Lucky Pick Box / 뽑기박스
- **Nhà phát triển:** frog-im
- **Người phụ trách bảo vệ thông tin cá nhân / Người liên hệ:** frog-im
- **Liên hệ:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Ngày có hiệu lực:** 2026-06-12
- **Cập nhật lần cuối:** 2026-06-15

> Chính sách này được xây dựng dựa trên các thông tin mà ứng dụng xử lý và các tính năng liên quan của ứng dụng.  
> Nếu có bất kỳ luật hoặc quy định bắt buộc nào áp dụng tại một quốc gia hoặc khu vực cụ thể, các luật hoặc quy định đó có thể được ưu tiên áp dụng.

---

## 1. Mục đích và phạm vi áp dụng

Lucky Pick Box là công cụ giải trí cho lựa chọn ngẫu nhiên, bốc thăm, chọn thứ tự, chia đội, xúc xắc, tung đồng xu, thang, vòng quay và các trò quyết định hằng ngày hoặc theo nhóm tương tự. Ứng dụng không cung cấp cờ bạc tiền thật, cá cược, giao dịch tài chính, giải thưởng tiền mặt hoặc phần thưởng tương đương tiền.

### A. Tính năng chính

- Nhập nhanh mục: văn bản do người dùng nhập hoặc đọc từ hình ảnh đã chọn.
- Trò chơi chọn ngẫu nhiên: thang, vòng quay, plinko, bốc thăm đơn giản, xúc xắc, đồng xu, số ngẫu nhiên, chia đội, chọn thứ tự, thẻ, bom và có/không.
- Lịch sử kết quả: có thể lưu loại trò chơi, tiêu đề, người tham gia/mục, tóm tắt kết quả và thời gian tạo.
- Ô lưu cài đặt: một số trò chơi có thể lưu người tham gia, danh sách, phạm vi, số lượng, đội, trọng số và cài đặt tương tự vào tối đa 3 ô cục bộ.

Ứng dụng không yêu cầu đăng ký hoặc đăng nhập. Chúng tôi không vận hành máy chủ nhận tên, số điện thoại, địa chỉ email, danh bạ, mục nhập trò chơi, hình ảnh đã chọn hoặc kết quả trò chơi từ ứng dụng.

Để cung cấp tính năng, ứng dụng có thể lưu mục nhập trò chơi, nhãn người tham gia, kết quả gần đây, cài đặt trò chơi đã lưu, cài đặt hoạt ảnh, lựa chọn quyền riêng tư quảng cáo và trạng thái liên quan đến đồng ý trong bộ nhớ cục bộ của thiết bị. Lịch sử kết quả gần đây được ứng dụng giới hạn và không gửi đến máy chủ do nhà phát triển vận hành.

---

## 2. Các loại thông tin cá nhân được xử lý

### 2-1) Thông tin do người dùng trực tiếp nhập

Ứng dụng không yêu cầu đăng ký hoặc đăng nhập. Chúng tôi không vận hành máy chủ nhận tên, số điện thoại, địa chỉ email, danh bạ, mục nhập trò chơi, hình ảnh đã chọn hoặc kết quả trò chơi từ ứng dụng.

### 2-2) Tệp được chọn trên thiết bị

Nếu bạn chọn đọc văn bản từ hình ảnh, ứng dụng yêu cầu bạn chọn một hình từ thư viện ảnh. Hình ảnh đã chọn được dùng để nhận dạng văn bản trên thiết bị thông qua trình chọn hình ảnh của nền tảng và các thành phần Google ML Kit. Nhà phát triển không tải hình ảnh lên máy chủ do nhà phát triển vận hành và không lưu trong tài khoản từ xa.

### 2-3) Dữ liệu được lưu cục bộ trong ứng dụng

Để cung cấp tính năng, ứng dụng có thể lưu mục nhập trò chơi, nhãn người tham gia, kết quả gần đây, cài đặt trò chơi đã lưu, cài đặt hoạt ảnh, lựa chọn quyền riêng tư quảng cáo và trạng thái liên quan đến đồng ý trong bộ nhớ cục bộ của thiết bị. Lịch sử kết quả gần đây được ứng dụng giới hạn và không gửi đến máy chủ do nhà phát triển vận hành.

### B. Dữ liệu cục bộ trên thiết bị

| Vị trí hoặc khóa | Dữ liệu | Mục đích | Xóa |
|---|---|---|---|
| `SharedPreferences` / `draw_results` | ID, loại trò chơi, tiêu đề, người tham gia/mục, tóm tắt, thời gian; tối đa 50 kết quả gần đây. | Hiển thị kết quả gần đây và lịch sử. | Xóa trong app, xóa dữ liệu app hoặc gỡ cài đặt |
| `game_settings.<gameId>.slot_<n>` | Cài đặt trò chơi, thời gian lưu, danh sách, phạm vi, số lượng, đội, trọng số; tối đa 3 ô. | Tải lại cài đặt trò chơi. | Xóa ô, xóa dữ liệu hoặc gỡ cài đặt |
| `cinematic_motion_enabled`, `fullscreen_game_mode_enabled` | Cài đặt hoạt ảnh và toàn màn hình. | Giữ tùy chọn hiển thị. | Đổi cài đặt, xóa dữ liệu hoặc gỡ cài đặt |
| `ad_non_personalized`, `ad_restricted_data_processing`, `ad_completed_game_count` | Lựa chọn quyền riêng tư quảng cáo và bộ đếm tần suất quảng cáo. | Áp dụng lựa chọn theo khu vực và kiểm soát tần suất. | Đổi cài đặt, xóa dữ liệu hoặc gỡ cài đặt |
| Bộ chọn hình ảnh và OCR | Đường dẫn hình ảnh đã chọn và văn bản nhận dạng có thể được xử lý tạm thời. | Thêm chữ từ ảnh vào nhập nhanh. | Bộ nhớ đệm app/OS hoặc xóa dữ liệu |

Văn bản nhập nhanh không được gửi đến máy chủ của nhà phát triển. Nó chỉ có thể trở thành dữ liệu cục bộ khi được dùng trong kết quả hoặc cài đặt đã lưu.

### 2-4) Thông tin có thể được xử lý tự động trong quá trình quản lý quảng cáo và sự đồng ý

Trên các nền tảng được hỗ trợ, hiện là Android, ứng dụng sử dụng Google AdMob và Google User Messaging Platform (UMP). Google và đối tác quảng cáo có thể xử lý mã định danh quảng cáo, mã định danh phiên bản ứng dụng, địa chỉ IP, vị trí gần đúng, thông tin thiết bị và mạng, phiên bản ứng dụng, hệ điều hành, ngôn ngữ, lượt hiển thị, nhấp và tương tác quảng cáo, chẩn đoán, trạng thái đồng ý và cài đặt quyền riêng tư quảng cáo theo khu vực để phân phối quảng cáo, giới hạn tần suất, chống gian lận, quản lý đồng ý, đo lường, phân tích, bảo mật và tuân thủ pháp luật.

Thực tiễn quyền riêng tư của Google được mô tả tại https://policies.google.com/privacy và https://policies.google.com/technologies/ads.

---

## 3. Mục đích xử lý thông tin cá nhân

Lucky Pick Box là công cụ giải trí cho lựa chọn ngẫu nhiên, bốc thăm, chọn thứ tự, chia đội, xúc xắc, tung đồng xu, thang, vòng quay và các trò quyết định hằng ngày hoặc theo nhóm tương tự. Ứng dụng không cung cấp cờ bạc tiền thật, cá cược, giao dịch tài chính, giải thưởng tiền mặt hoặc phần thưởng tương đương tiền.

### A. Tính năng chính

- Nhập nhanh mục: văn bản do người dùng nhập hoặc đọc từ hình ảnh đã chọn.
- Trò chơi chọn ngẫu nhiên: thang, vòng quay, plinko, bốc thăm đơn giản, xúc xắc, đồng xu, số ngẫu nhiên, chia đội, chọn thứ tự, thẻ, bom và có/không.
- Lịch sử kết quả: có thể lưu loại trò chơi, tiêu đề, người tham gia/mục, tóm tắt kết quả và thời gian tạo.
- Ô lưu cài đặt: một số trò chơi có thể lưu người tham gia, danh sách, phạm vi, số lượng, đội, trọng số và cài đặt tương tự vào tối đa 3 ô cục bộ.

Trên các nền tảng được hỗ trợ, hiện là Android, ứng dụng sử dụng Google AdMob và Google User Messaging Platform (UMP). Google và đối tác quảng cáo có thể xử lý mã định danh quảng cáo, mã định danh phiên bản ứng dụng, địa chỉ IP, vị trí gần đúng, thông tin thiết bị và mạng, phiên bản ứng dụng, hệ điều hành, ngôn ngữ, lượt hiển thị, nhấp và tương tác quảng cáo, chẩn đoán, trạng thái đồng ý và cài đặt quyền riêng tư quảng cáo theo khu vực để phân phối quảng cáo, giới hạn tần suất, chống gian lận, quản lý đồng ý, đo lường, phân tích, bảo mật và tuân thủ pháp luật.

Thực tiễn quyền riêng tư của Google được mô tả tại https://policies.google.com/privacy và https://policies.google.com/technologies/ads.

---

## 4. Thời gian lưu giữ và lưu trữ thông tin cá nhân

Lịch sử cục bộ và cài đặt có thể ở lại trên thiết bị cho đến khi bạn xóa lịch sử, xóa dữ liệu ứng dụng hoặc gỡ cài đặt ứng dụng. Bạn có thể thay đổi lựa chọn quyền riêng tư quảng cáo có sẵn trong cài đặt ứng dụng, mở tùy chọn quyền riêng tư của Google khi cần và quản lý hoặc đặt lại mã định danh quảng cáo trong cài đặt quyền riêng tư thiết bị. Việc lưu giữ thông tin do Google xử lý tuân theo chính sách và nghĩa vụ pháp lý của Google.

### B. Dữ liệu cục bộ trên thiết bị

| Vị trí hoặc khóa | Dữ liệu | Mục đích | Xóa |
|---|---|---|---|
| `SharedPreferences` / `draw_results` | ID, loại trò chơi, tiêu đề, người tham gia/mục, tóm tắt, thời gian; tối đa 50 kết quả gần đây. | Hiển thị kết quả gần đây và lịch sử. | Xóa trong app, xóa dữ liệu app hoặc gỡ cài đặt |
| `game_settings.<gameId>.slot_<n>` | Cài đặt trò chơi, thời gian lưu, danh sách, phạm vi, số lượng, đội, trọng số; tối đa 3 ô. | Tải lại cài đặt trò chơi. | Xóa ô, xóa dữ liệu hoặc gỡ cài đặt |
| `cinematic_motion_enabled`, `fullscreen_game_mode_enabled` | Cài đặt hoạt ảnh và toàn màn hình. | Giữ tùy chọn hiển thị. | Đổi cài đặt, xóa dữ liệu hoặc gỡ cài đặt |
| `ad_non_personalized`, `ad_restricted_data_processing`, `ad_completed_game_count` | Lựa chọn quyền riêng tư quảng cáo và bộ đếm tần suất quảng cáo. | Áp dụng lựa chọn theo khu vực và kiểm soát tần suất. | Đổi cài đặt, xóa dữ liệu hoặc gỡ cài đặt |
| Bộ chọn hình ảnh và OCR | Đường dẫn hình ảnh đã chọn và văn bản nhận dạng có thể được xử lý tạm thời. | Thêm chữ từ ảnh vào nhập nhanh. | Bộ nhớ đệm app/OS hoặc xóa dữ liệu |

Văn bản nhập nhanh không được gửi đến máy chủ của nhà phát triển. Nó chỉ có thể trở thành dữ liệu cục bộ khi được dùng trong kết quả hoặc cài đặt đã lưu.

---

## 5. Quy trình và phương thức xóa thông tin cá nhân

Lịch sử cục bộ và cài đặt có thể ở lại trên thiết bị cho đến khi bạn xóa lịch sử, xóa dữ liệu ứng dụng hoặc gỡ cài đặt ứng dụng. Bạn có thể thay đổi lựa chọn quyền riêng tư quảng cáo có sẵn trong cài đặt ứng dụng, mở tùy chọn quyền riêng tư của Google khi cần và quản lý hoặc đặt lại mã định danh quảng cáo trong cài đặt quyền riêng tư thiết bị. Việc lưu giữ thông tin do Google xử lý tuân theo chính sách và nghĩa vụ pháp lý của Google.

### C. Quyền, SDK, sao lưu và bảo mật

Ứng dụng có thể dùng `INTERNET`, `ACCESS_NETWORK_STATE` và `com.google.android.gms.permission.AD_ID` cho quảng cáo và thông báo pháp lý. Quyền truy cập ảnh hoặc bộ chọn ảnh chỉ dùng khi người dùng chọn đọc chữ từ ảnh.

Google Mobile Ads SDK có thể xử lý địa chỉ IP, tương tác quảng cáo, chẩn đoán và mã định danh thiết bị/tài khoản cho quảng cáo, phân tích và chống gian lận. UMP có thể xử lý trạng thái đồng ý và lựa chọn quyền riêng tư.

Dữ liệu cục bộ có thể xóa bằng tính năng trong app, xóa dữ liệu app của hệ điều hành hoặc gỡ cài đặt. Bản sao lưu hệ thống, ảnh chụp màn hình hoặc tệp người dùng chia sẻ có thể còn lại theo chính sách của nhà cung cấp. Không nên nhập dữ liệu nhạy cảm vào trường văn bản tự do.

---

## 6. Cung cấp cho bên thứ ba, thuê xử lý và chuyển dữ liệu xuyên biên giới

Chúng tôi không bán mục nhập trò chơi, nhãn người tham gia, kết quả trò chơi hoặc hình ảnh đã chọn của bạn. Khi các tính năng quảng cáo hoặc đồng ý được yêu cầu, Google LLC, các công ty liên kết của Google và nhà cung cấp dịch vụ của họ có thể xử lý thông tin quảng cáo và đồng ý ở các quốc gia ngoài quốc gia hoặc khu vực của bạn. Xem "Thông báo chuyển dữ liệu quốc tế" trong ứng dụng để biết thêm chi tiết.

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

---

## 7. Thông tin về các quyền được sử dụng

### C. Quyền, SDK, sao lưu và bảo mật

Ứng dụng có thể dùng `INTERNET`, `ACCESS_NETWORK_STATE` và `com.google.android.gms.permission.AD_ID` cho quảng cáo và thông báo pháp lý. Quyền truy cập ảnh hoặc bộ chọn ảnh chỉ dùng khi người dùng chọn đọc chữ từ ảnh.

Google Mobile Ads SDK có thể xử lý địa chỉ IP, tương tác quảng cáo, chẩn đoán và mã định danh thiết bị/tài khoản cho quảng cáo, phân tích và chống gian lận. UMP có thể xử lý trạng thái đồng ý và lựa chọn quyền riêng tư.

Dữ liệu cục bộ có thể xóa bằng tính năng trong app, xóa dữ liệu app của hệ điều hành hoặc gỡ cài đặt. Bản sao lưu hệ thống, ảnh chụp màn hình hoặc tệp người dùng chia sẻ có thể còn lại theo chính sách của nhà cung cấp. Không nên nhập dữ liệu nhạy cảm vào trường văn bản tự do.

---

## 8. Thiết lập, vận hành và từ chối các cơ chế thu thập tự động

Trên các nền tảng được hỗ trợ, hiện là Android, ứng dụng sử dụng Google AdMob và Google User Messaging Platform (UMP). Google và đối tác quảng cáo có thể xử lý mã định danh quảng cáo, mã định danh phiên bản ứng dụng, địa chỉ IP, vị trí gần đúng, thông tin thiết bị và mạng, phiên bản ứng dụng, hệ điều hành, ngôn ngữ, lượt hiển thị, nhấp và tương tác quảng cáo, chẩn đoán, trạng thái đồng ý và cài đặt quyền riêng tư quảng cáo theo khu vực để phân phối quảng cáo, giới hạn tần suất, chống gian lận, quản lý đồng ý, đo lường, phân tích, bảo mật và tuân thủ pháp luật.

Thực tiễn quyền riêng tư của Google được mô tả tại https://policies.google.com/privacy và https://policies.google.com/technologies/ads.

Lịch sử cục bộ và cài đặt có thể ở lại trên thiết bị cho đến khi bạn xóa lịch sử, xóa dữ liệu ứng dụng hoặc gỡ cài đặt ứng dụng. Bạn có thể thay đổi lựa chọn quyền riêng tư quảng cáo có sẵn trong cài đặt ứng dụng, mở tùy chọn quyền riêng tư của Google khi cần và quản lý hoặc đặt lại mã định danh quảng cáo trong cài đặt quyền riêng tư thiết bị. Việc lưu giữ thông tin do Google xử lý tuân theo chính sách và nghĩa vụ pháp lý của Google.

---

## 9. Quyền của người dùng và cách thực hiện

Lịch sử cục bộ và cài đặt có thể ở lại trên thiết bị cho đến khi bạn xóa lịch sử, xóa dữ liệu ứng dụng hoặc gỡ cài đặt ứng dụng. Bạn có thể thay đổi lựa chọn quyền riêng tư quảng cáo có sẵn trong cài đặt ứng dụng, mở tùy chọn quyền riêng tư của Google khi cần và quản lý hoặc đặt lại mã định danh quảng cáo trong cài đặt quyền riêng tư thiết bị. Việc lưu giữ thông tin do Google xử lý tuân theo chính sách và nghĩa vụ pháp lý của Google.

---

## 10. Biện pháp bảo mật

### C. Quyền, SDK, sao lưu và bảo mật

Ứng dụng có thể dùng `INTERNET`, `ACCESS_NETWORK_STATE` và `com.google.android.gms.permission.AD_ID` cho quảng cáo và thông báo pháp lý. Quyền truy cập ảnh hoặc bộ chọn ảnh chỉ dùng khi người dùng chọn đọc chữ từ ảnh.

Google Mobile Ads SDK có thể xử lý địa chỉ IP, tương tác quảng cáo, chẩn đoán và mã định danh thiết bị/tài khoản cho quảng cáo, phân tích và chống gian lận. UMP có thể xử lý trạng thái đồng ý và lựa chọn quyền riêng tư.

Dữ liệu cục bộ có thể xóa bằng tính năng trong app, xóa dữ liệu app của hệ điều hành hoặc gỡ cài đặt. Bản sao lưu hệ thống, ảnh chụp màn hình hoặc tệp người dùng chia sẻ có thể còn lại theo chính sách của nhà cung cấp. Không nên nhập dữ liệu nhạy cảm vào trường văn bản tự do.

### C. Quyền, SDK, sao lưu và bảo mật

Ứng dụng có thể dùng `INTERNET`, `ACCESS_NETWORK_STATE` và `com.google.android.gms.permission.AD_ID` cho quảng cáo và thông báo pháp lý. Quyền truy cập ảnh hoặc bộ chọn ảnh chỉ dùng khi người dùng chọn đọc chữ từ ảnh.

Google Mobile Ads SDK có thể xử lý địa chỉ IP, tương tác quảng cáo, chẩn đoán và mã định danh thiết bị/tài khoản cho quảng cáo, phân tích và chống gian lận. UMP có thể xử lý trạng thái đồng ý và lựa chọn quyền riêng tư.

Dữ liệu cục bộ có thể xóa bằng tính năng trong app, xóa dữ liệu app của hệ điều hành hoặc gỡ cài đặt. Bản sao lưu hệ thống, ảnh chụp màn hình hoặc tệp người dùng chia sẻ có thể còn lại theo chính sách của nhà cung cấp. Không nên nhập dữ liệu nhạy cảm vào trường văn bản tự do.

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

Cập nhật lần cuối: **2026-06-15**
