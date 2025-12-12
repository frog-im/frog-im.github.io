---
title: Chính sách Quyền riêng tư | Subtitle Tool
description: Chính sách quyền riêng tư cho Subtitle Player & Editor (Subtitle Tool)
lang: vi
last_updated: 2025-12-12
---

# Chính sách Quyền riêng tư (Subtitle Player & Editor / “Subtitle Tool”)

- **Tên ứng dụng:** Subtitle Player & Editor (sau đây gọi là “Subtitle Tool”)  
- **Nhà phát triển:** frog-im  
- **Liên hệ:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Ngày có hiệu lực:** 2025-12-12  

> Chính sách này được xây dựng dựa trên các quy định pháp luật liên quan, bao gồm Luật Bảo vệ Thông tin Cá nhân của Hàn Quốc (PIPA), GDPR/UK GDPR, luật bảo vệ dữ liệu của Thụy Sĩ (FADP) và một số luật về quyền riêng tư tại các bang của Hoa Kỳ.  
> Khi pháp luật tại từng quốc gia/khu vực có quy định bắt buộc riêng, các quy định đó sẽ được ưu tiên áp dụng so với nội dung chung trong Chính sách này.

---

## 1. Mục đích và Phạm vi Áp dụng

Ứng dụng này cung cấp chức năng **chỉnh sửa siêu dữ liệu của tệp âm thanh** (tiêu đề, nghệ sĩ, v.v.) được lưu trữ trên thiết bị, cùng với chức năng **hiển thị lời bài hát/phụ đề dưới dạng lớp phủ (overlay)**.  
Ứng dụng **không tạo tài khoản người dùng** và **không tải nội dung của bạn lên máy chủ** của chúng tôi. Mặc định, việc xử lý được thực hiện **cục bộ trên thiết bị của bạn**.

Tuy nhiên, nhằm phục vụ **quảng cáo** và **tuân thủ quy định pháp luật**, các đối tác bên thứ ba (ví dụ: Google Mobile Ads SDK (AdMob), UMP) có thể thu thập và xử lý thông tin như **định danh quảng cáo**.  
Việc thu thập sự đồng ý và quản lý tùy chọn quyền riêng tư được thực hiện theo đặc tả của **Google UMP (User Messaging Platform)**.

---

## 2. Các Loại Thông tin Chúng tôi Xử lý

### 2-1) Tệp do Người dùng Chủ động Chọn

- **Đường dẫn và nội dung tệp âm thanh/hình ảnh bìa:** được xử lý **cục bộ trên thiết bị**, chỉ nhằm mục đích chỉnh sửa và lưu.  
- **FFmpegKit** được sử dụng cục bộ để mã hóa, chỉnh sửa siêu dữ liệu và trích xuất hình thu nhỏ.  
- Ứng dụng **không tải lên máy chủ** của chúng tôi các tệp mà bạn đã chọn này.

### 2-2) Thiết lập Cục bộ và Giá trị Được Lưu trữ

Để bảo đảm chức năng cốt lõi và sự tiện lợi, ứng dụng lưu trữ một số giá trị sau đây **cục bộ trên thiết bị**.  
Những giá trị này không được gửi đến máy chủ của chúng tôi và sẽ **bị xóa khi dữ liệu ứng dụng hoặc ứng dụng bị xóa**.

#### (1) Tùy chọn (`shared_preferences`)

| Loại | Khóa/Nội dung | Mục đích | Nơi lưu trữ | Cách xóa |
|---|---|---|---|---|
| Vị trí/kích cỡ chữ của overlay | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Khôi phục vị trí overlay và kích thước phông chữ | SharedPreferences trên thiết bị | Bị xóa khi xóa dữ liệu ứng dụng hoặc gỡ cài đặt ứng dụng |
| Thiết lập quảng cáo/quyền riêng tư | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Quảng cáo không cá nhân hóa, tín hiệu U.S. RDP, gắn nhãn COPPA (dành cho trẻ em), gắn nhãn độ tuổi, giới hạn mức xếp hạng nội dung quảng cáo | SharedPreferences trên thiết bị | Như cột bên trái |

#### (2) Tệp Tạm thời (thư mục tạm của hệ thống)

- **Ví dụ:** `cover_*.jpg`, `tmp_*.flac`  
- **Mục đích:** trích xuất ảnh bìa, gán nhãn FLAC, mã hóa tạm thời  
- **Vị trí:** thư mục tạm của hệ điều hành (`systemTemp`)  
- **Thời gian lưu giữ:** ứng dụng sẽ cố gắng xóa sau khi xử lý hoàn tất; ngoài ra chúng có thể bị xóa bởi cơ chế dọn dẹp của hệ thống.

#### (3) Đường dẫn Lưu trữ do Người dùng Chọn (SAF)

- Khi người dùng chọn “Lưu dưới tên khác”, tệp âm thanh cuối cùng có thể được lưu vào vị trí do bạn xác định (ví dụ: thư mục Tải xuống, lưu trữ đám mây).  
- Những tệp này nằm trên **bộ nhớ ngoài** và **có thể vẫn tồn tại sau khi ứng dụng bị gỡ cài đặt**. Người dùng có thể tự xóa thủ công.

#### (4) Trạng thái Đồng ý (bộ nhớ đệm UMP)

- Tại khu vực EEA/UK/Thụy Sĩ, SDK UMP **lưu trữ trạng thái đồng ý quảng cáo của người dùng trong bộ nhớ đệm cục bộ**.  
- Trạng thái này có thể được đặt lại bằng cách xóa dữ liệu ứng dụng hoặc thông qua màn hình **Tùy chọn quyền riêng tư** trong ứng dụng (nếu có).

---

### 2-3) Dữ liệu Liên quan đến Quảng cáo và Đồng ý (SDK Bên thứ Ba)

- **Google Mobile Ads SDK (AdMob) và UMP** có thể thu thập và xử lý, ví dụ: **định danh quảng cáo (AAID/IDFA)**, **dải địa chỉ IP**, **thông tin thiết bị/ứng dụng**, **tín hiệu tương tác với quảng cáo**, **trạng thái đồng ý**, v.v.  
- **Mục đích:** hiển thị quảng cáo, giới hạn tần suất, phòng chống gian lận, đo lường hiệu suất, tuân thủ pháp luật.  
- **Khu vực yêu cầu phải có đồng ý (EEA/UK/Thụy Sĩ):** đồng ý được thu thập thông qua giao diện UMP và màn hình **Tùy chọn quyền riêng tư** sẽ được cung cấp khi pháp luật yêu cầu.  
  Ở những khu vực không có yêu cầu như vậy (ví dụ Hàn Quốc), tùy chọn này **có thể không được hiển thị**.

---

## 3. Xử lý và Thời gian Lưu trữ

- **Thiết lập cục bộ:** được lưu trên thiết bị cho đến khi người dùng xóa dữ liệu ứng dụng hoặc gỡ ứng dụng.  
- **Tệp tạm thời:** được tạo trong quá trình mã hóa/trích xuất, bị xóa sau khi xử lý hoặc có thể tồn tại tạm thời trong bộ nhớ đệm hệ thống.  
- **Dữ liệu quảng cáo/đồng ý (bên thứ ba):** được lưu giữ và xóa theo **chính sách của Google**.

---

## 4. Chuyển giao cho Bên thứ Ba và Dòng chảy Dữ liệu Xuyên biên giới

Để phục vụ quảng cáo và quản lý đồng ý, một phần thông tin của người dùng có thể được truyền đến và xử lý trên hệ thống hạ tầng của Google.

| Mục | Chi tiết |
|---|---|
| **Bên nhận** | Google LLC và các công ty liên kết/các bên xử lý phụ |
| **Đích đến** | Hoa Kỳ (và các khu vực khác nơi hạ tầng của Google đặt trụ sở) |
| **Mục đích sử dụng** | Hiển thị quảng cáo, đo lường và hiệu suất, tuân thủ pháp luật, quản lý đồng ý |
| **Dữ liệu** | Định danh quảng cáo, dải IP, thông tin thiết bị/ứng dụng, tương tác quảng cáo, trạng thái đồng ý, v.v. |
| **Thời gian lưu trữ** | Theo chính sách của Google |
| **Ảnh hưởng khi từ chối** | Quảng cáo cá nhân hóa có thể bị hạn chế; quảng cáo không cá nhân hóa vẫn có thể được hiển thị |

Chúng tôi tuân thủ yêu cầu công bố trong mục **Data safety** của Google Play và duy trì thông tin ở đó phù hợp với hoạt động xử lý thực tế.

---

## 5. Quyền của Bạn và Cách Thực hiện

- **Từ chối quảng cáo cá nhân hóa / thay đổi đồng ý**  
  - Ở các khu vực được hỗ trợ (EEA/UK/Thụy Sĩ): bạn có thể thay đổi tùy chọn tại **Cài đặt → Tùy chọn quyền riêng tư**.  
  - Ở các khu vực khác: hãy sử dụng cài đặt hệ điều hành để **đặt lại ID quảng cáo / giới hạn theo dõi quảng cáo**.
- **Đặt lại thông tin cục bộ:** khi xóa dữ liệu ứng dụng hoặc gỡ cài đặt, các tọa độ overlay, kích thước phông chữ và các thiết lập cục bộ khác sẽ được đặt lại.  
- Theo **GDPR/UK GDPR/FADP của Thụy Sĩ/các luật về quyền riêng tư của từng bang ở Hoa Kỳ**, bạn có thể có quyền truy cập, chỉnh sửa, xóa, di chuyển dữ liệu, hạn chế xử lý, rút lại sự đồng ý, v.v. (trong giới hạn luật định).  
  Đối với dữ liệu quảng cáo do Google xử lý, vui lòng sử dụng **các cơ chế do Google cung cấp**.

---

## 6. Quyền riêng tư của Trẻ em

Ứng dụng này **không được thiết kế dành riêng cho trẻ em**.  
Nếu trẻ dưới độ tuổi tối thiểu theo luật định sử dụng ứng dụng, trẻ nên dừng sử dụng và cùng với người giám hộ cấu hình các tính năng hạn chế quảng cáo ở cấp hệ điều hành.  
Khi phù hợp, chúng tôi có thể áp dụng nhãn như **TFUA (child-directed tag)** hoặc các lựa chọn bảo vệ trẻ em tương tự.

---

## 7. Biện pháp An ninh

- **Giảm thiểu dữ liệu** trong quá trình thu thập và lưu trữ  
- Chỉ sử dụng tệp tạm thời khi cần và xóa chúng sau khi xử lý nếu có thể  
- Chỉ xử lý trong **phạm vi quyền hạn của hệ điều hành**  
- Sử dụng mã hóa **TLS hoặc tương đương** khi truyền dữ liệu cho bên thứ ba (theo chuẩn bảo mật của SDK liên quan)

---

## 8. An toàn Dữ liệu (Google Play)

Chúng tôi chuẩn bị và duy trì mục **Data safety** trên Google Play Console một cách chính xác, đồng thời cập nhật kịp thời khi có thay đổi trong hoạt động xử lý dữ liệu.

---

## 9. Thông báo về Phần mềm Mã nguồn Mở

Ứng dụng sử dụng phần mềm mã nguồn mở như **FFmpeg**.  
Bên trong ứng dụng có tệp thông tin (ví dụ: `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) giải thích cách lấy mã nguồn.  
Khi có yêu cầu, chúng tôi sẽ cung cấp mã nguồn theo hướng dẫn được nêu trong tệp đó.

---

## 10. Liên hệ

- Email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Thay đổi đối với Chính sách này

Chúng tôi có thể sửa đổi Chính sách này khi có thay đổi về pháp luật hoặc dịch vụ.  
Các cập nhật sẽ được đăng **trong ứng dụng** và trên **trang chính sách** này.  
Đối với các thay đổi quan trọng, chúng tôi sẽ thông báo **ít nhất 7 ngày trước** ngày có hiệu lực.
