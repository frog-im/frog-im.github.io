---
title: Chính sách quyền riêng tư | Subtitle Tool
description: Chính sách quyền riêng tư của Subtitle Tool (Subtitle Player & Editor) - Tiếng Việt
lang: vi
last_updated: 2026-03-11
---

# Chính sách quyền riêng tư (Subtitle Tool / Subtitle Player & Editor)

- **Tên ứng dụng:** Subtitle Player & Editor (trong Chính sách này cũng được gọi là **Subtitle Tool**)
- **Nhà phát triển:** frog-im
- **Liên hệ:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Ngày có hiệu lực:** 2026-03-11

> Chính sách này được xây dựng có tham chiếu đến các luật hiện hành, bao gồm Luật Bảo vệ Thông tin Cá nhân của Hàn Quốc (PIPA), GDPR / UK GDPR, Swiss FADP và các luật về quyền riêng tư liên quan của các bang tại Hoa Kỳ. Nếu có quy định địa phương bắt buộc được áp dụng, các quy định đó sẽ được ưu tiên.

---

## 1. Mục đích và phạm vi

Ứng dụng này cung cấp:

- Phát và chỉnh sửa phụ đề
- Phát video + phụ đề từ các tệp do người dùng chọn
- Lớp phủ phụ đề / lời bài hát nổi hiển thị trên các ứng dụng khác trên Android

Các định dạng phụ đề được hỗ trợ có thể bao gồm:

- `srt`
- `vtt`
- `ass`
- `ssa`
- `lrc`
- `txt`

Ứng dụng **không** tạo tài khoản người dùng và **không** tải tệp phụ đề hoặc tệp phương tiện của người dùng lên máy chủ riêng của nhà phát triển. Việc phân tích, chỉnh sửa, xem trước phụ đề và phần lớn xử lý liên quan đến phát lại được thực hiện **cục bộ trên thiết bị**.

Tuy nhiên, vì mục đích quảng cáo, quản lý sự đồng ý và tuân thủ pháp luật, các SDK của bên thứ ba như **Google Mobile Ads SDK (AdMob)** và **Google UMP** có thể xử lý một số thông tin nhất định như mã định danh quảng cáo, tín hiệu thiết bị và lựa chọn đồng ý.

---

## 2. Các loại thông tin chúng tôi xử lý

### 2-1) Các tệp do người dùng chủ động chọn

Ứng dụng tương tác với các tệp mà người dùng chủ động chọn, bao gồm:

- **Tệp phụ đề**
  - Ví dụ: `.srt`, `.vtt`, `.ass`, `.ssa`, `.lrc`, `.txt`
  - Mục đích sử dụng:
    - Phát phụ đề trong ứng dụng
    - Chỉnh sửa phụ đề
    - Hiển thị phụ đề dạng lớp phủ
    - Chuyển đổi và xuất phụ đề

- **Tệp phương tiện**
  - Ví dụ: tệp video hoặc âm thanh cục bộ do người dùng chọn
  - Mục đích sử dụng:
    - Phát video + phụ đề
    - Căn chỉnh thời gian lớp phủ theo phương tiện đang phát

Các điểm quan trọng:

- Các tệp do người dùng chọn được xử lý cục bộ trên thiết bị.
- Ứng dụng không tải các tệp đó lên máy chủ riêng của nhà phát triển.
- Đường dẫn tệp và nội dung tệp chỉ được sử dụng cho việc phát lại, hiển thị lớp phủ, chỉnh sửa, lưu và các thao tác do người dùng yêu cầu.

### 2-2) Cài đặt cục bộ và các giá trị được lưu trữ

Để cung cấp cài đặt lâu dài và khôi phục trạng thái trước đó, ứng dụng lưu một số giá trị cục bộ trên thiết bị bằng `SharedPreferences` hoặc cơ chế lưu trữ cục bộ tương tự do hệ điều hành cung cấp.

Các giá trị này không được gửi đến máy chủ riêng của nhà phát triển và thông thường sẽ bị xóa khi dữ liệu ứng dụng bị xóa hoặc ứng dụng bị gỡ cài đặt.

#### (1) Cài đặt lớp phủ

Ví dụ bao gồm:

- `overlay_box_x`
- `overlay_box_y`
- `overlay_text_font`
- `overlay_text_color`
- `overlay_outline_enabled`
- `overlay_outline_color`
- `overlay_outline_width`
- `overlay_force_landscape`
- `overlay_interstitial_count`

Mục đích:

- Khôi phục vị trí lớp phủ
- Khôi phục kiểu phụ đề cho lớp phủ và phát phụ đề trong ứng dụng
- Duy trì các tùy chọn về viền / phông chữ / hướng màn hình
- Kiểm soát logic tần suất hiển thị quảng cáo trong một số luồng liên quan đến lớp phủ

#### (2) Vị trí phát hoặc lớp phủ gần đây

Ví dụ bao gồm:

- `overlay_recent_positions`
- `video_subtitle_recent_position`

Mục đích:

- Khôi phục hoặc gợi ý vị trí bắt đầu gần đây của phụ đề/lớp phủ
- Tiếp tục phát video + phụ đề thuận tiện hơn

#### (3) Các giá trị tùy chọn quảng cáo và quyền riêng tư

Ví dụ có thể bao gồm:

- `pref_npa_always`
- `pref_us_rdp`
- `pref_child_directed`
- `pref_under_age`
- `pref_max_ad_rating`

Mục đích:

- Lưu lựa chọn quyền riêng tư liên quan đến quảng cáo
- Áp dụng cài đặt quyền riêng tư và cấu hình quảng cáo của UMP / AdMob

#### (4) Tệp phụ đề do người dùng tạo

Khi người dùng lưu hoặc xuất tệp phụ đề, ứng dụng có thể ghi các tệp phụ đề mới vào vị trí do người dùng chọn, chẳng hạn như:

- Tải xuống
- Thư mục khác được chọn thông qua trình chọn tệp của hệ thống
- Vị trí lưu trữ do người dùng quản lý

Các tệp do người dùng lưu này có thể vẫn còn trên thiết bị sau khi xóa ứng dụng, trừ khi người dùng xóa thủ công.

#### (5) Tệp tạm thời và bộ nhớ đệm

Ứng dụng và các thư viện bên thứ ba có thể tạo tệp tạm thời hoặc tệp bộ nhớ đệm để vận hành bình thường, chẳng hạn như:

- dữ liệu bộ nhớ đệm của trình chọn tệp
- dữ liệu chuyển đổi phụ đề tạm thời
- dữ liệu bộ nhớ đệm liên quan đến phát lại

Những dữ liệu này chỉ phục vụ cho hoạt động cục bộ và không được tải lên máy chủ riêng của nhà phát triển.

#### (6) Bộ nhớ đệm trạng thái đồng ý UMP

Tại các khu vực nơi Google UMP được áp dụng, SDK có thể lưu trạng thái đồng ý cục bộ trên thiết bị.

Thông thường, trạng thái này có thể được đặt lại bằng cách:

- xóa dữ liệu ứng dụng, hoặc
- thay đổi lựa chọn đồng ý trong ứng dụng khi có mục tùy chọn quyền riêng tư

### 2-3) Xử lý liên quan đến lớp phủ Android và quyền

Trên Android, lớp phủ phụ đề nổi có thể sử dụng:

- quyền `SYSTEM_ALERT_WINDOW` / hiển thị trên các ứng dụng khác
- quyền `POST_NOTIFICATIONS`
- thông báo dịch vụ nền trước cần thiết cho dịch vụ lớp phủ

Mục đích:

- hiển thị lớp phủ phụ đề trên các ứng dụng khác
- duy trì hoạt động của dịch vụ lớp phủ
- cho phép Android hiển thị các thông báo lớp phủ / dịch vụ cần thiết
- đọc thông tin từ thông báo phương tiện khi cần để hỗ trợ tiến trình phụ đề

Các quyền này chỉ được sử dụng cho những tính năng của ứng dụng mà người dùng chủ động chọn sử dụng.

### 2-4) Quảng cáo, sự đồng ý và dữ liệu liên quan (SDK bên thứ ba)

Ứng dụng sử dụng các SDK quảng cáo / đồng ý của Google, bao gồm:

- **Google Mobile Ads SDK (AdMob)**
- **Google UMP**

Ứng dụng có thể hiển thị:

- quảng cáo biểu ngữ
- quảng cáo xen kẽ
- quảng cáo có thưởng hoặc quảng cáo xen kẽ có thưởng

Các SDK này có thể xử lý các dữ liệu như:

- mã định danh quảng cáo (ví dụ: AAID / IDFA nếu áp dụng)
- thông tin dựa trên IP và thông tin liên quan đến mạng
- siêu dữ liệu của thiết bị và ứng dụng
- tín hiệu tương tác với quảng cáo
- lựa chọn đồng ý

Mục đích có thể bao gồm:

- phân phối quảng cáo
- đo lường và báo cáo quảng cáo
- giới hạn tần suất
- phòng chống gian lận
- tuân thủ pháp luật

Nhà phát triển cố gắng cấu hình các SDK này theo cách phù hợp với lựa chọn đồng ý của người dùng và pháp luật hiện hành.

---

## 3. Cách chúng tôi xử lý và lưu giữ dữ liệu

- **Cài đặt cục bộ và dữ liệu vị trí gần đây**
  - được lưu trên thiết bị cho đến khi dữ liệu ứng dụng bị xóa hoặc ứng dụng bị gỡ bỏ

- **Tệp tạm thời / bộ nhớ đệm**
  - chỉ được lưu trong thời gian cần thiết để vận hành, sau đó được ứng dụng xóa khi có thể hoặc được hệ điều hành dọn dẹp sau đó

- **Tệp phụ đề do người dùng lưu**
  - vẫn nằm tại vị trí lưu do người dùng chọn cho đến khi người dùng xóa

- **Dữ liệu quảng cáo / đồng ý do bên thứ ba xử lý**
  - được lưu giữ theo chính sách của Google và pháp luật hiện hành

---

## 4. Xử lý bởi bên thứ ba và chuyển dữ liệu xuyên biên giới

Vì mục đích quảng cáo và quản lý sự đồng ý, một số thông tin có thể được Google và các đối tác liên quan xử lý.

| Mục | Chi tiết |
|---|---|
| Bên nhận | Google LLC và các công ty liên kết / đơn vị xử lý liên quan |
| Mục đích | Phân phối quảng cáo, đo lường, phòng chống gian lận, quản lý sự đồng ý và tuân thủ pháp luật |
| Dữ liệu có thể được xử lý | Mã định danh quảng cáo, thông tin thiết bị/ứng dụng, thông tin dựa trên IP, dữ liệu tương tác quảng cáo, trạng thái đồng ý |
| Điểm đến | Hoa Kỳ và các khu vực khác nơi hạ tầng của Google hoạt động |
| Lưu giữ | Theo chính sách của Google và pháp luật hiện hành |

Nhà phát triển cố gắng giữ cho các nội dung công bố quyền riêng tư trên cửa hàng ứng dụng phù hợp với hành vi thực tế của SDK.

---

## 5. Quyền và lựa chọn của bạn

Tùy thuộc vào khu vực pháp lý của bạn, bạn có thể có các quyền như:

- truy cập
- chỉnh sửa
- xóa
- hạn chế xử lý
- khả năng di chuyển dữ liệu
- phản đối
- rút lại sự đồng ý khi sự đồng ý là cơ sở pháp lý

Các biện pháp kiểm soát thực tế bao gồm:

- thay đổi lựa chọn quảng cáo / quyền riêng tư trong ứng dụng khi có sẵn
- xóa dữ liệu ứng dụng để loại bỏ cài đặt cục bộ và các tùy chọn đã được lưu vào bộ nhớ đệm
- gỡ cài đặt ứng dụng
- xóa thủ công các tệp phụ đề đã xuất khỏi bộ nhớ của người dùng
- sử dụng các công cụ kiểm soát ở cấp hệ điều hành như cài đặt thông báo, đặt lại ID quảng cáo hoặc cài đặt cá nhân hóa quảng cáo

Đối với dữ liệu do Google xử lý, người dùng cũng nên tham khảo các công cụ về quyền riêng tư và tài khoản của chính Google khi phù hợp.

---

## 6. Quyền riêng tư của trẻ em

Ứng dụng này không chủ yếu dành cho trẻ em.

Mục đích chính của ứng dụng là phát phụ đề, chỉnh sửa, hiển thị lớp phủ và các tính năng tiện ích liên quan. Khi phù hợp, cấu hình SDK quảng cáo có thể áp dụng các cờ liên quan đến độ tuổi hoặc cờ hướng đến trẻ em phù hợp với yêu cầu của nền tảng và cài đặt của nhà phát triển.

---

## 7. Biện pháp bảo mật

Trong giới hạn kiến trúc của ứng dụng, nhà phát triển cố gắng:

- giảm thiểu việc thu thập bằng cách giữ phần lớn quá trình xử lý phụ đề và phương tiện trên thiết bị
- sử dụng trình chọn tệp của hệ thống và quyền truy cập tệp do người dùng chủ động thực hiện
- sử dụng quyền hệ thống một cách minh bạch
- dựa vào truyền tải mạng được mã hóa do các SDK bên thứ ba sử dụng khi phù hợp

Không có phương thức lưu trữ hoặc truyền tải nào an toàn tuyệt đối, nhưng ứng dụng được thiết kế để tránh việc thu thập dữ liệu không cần thiết bởi nhà phát triển.

---

## 8. Phần mềm mã nguồn mở

Ứng dụng sử dụng phần mềm mã nguồn mở, bao gồm các thư viện liên quan đến:

- phân tích và tuần tự hóa phụ đề
- chọn tệp
- tùy chọn cục bộ
- cửa sổ lớp phủ
- phát video
- WebView

Thông báo về mã nguồn mở có sẵn trong ứng dụng. Đối với một số thành phần, ứng dụng có thể sử dụng bản sao đã được chỉnh sửa cục bộ của một gói mã nguồn mở trong khi vẫn giữ nguyên thông báo giấy phép gốc.

---

## 9. Liên hệ

Nếu bạn có câu hỏi hoặc yêu cầu liên quan đến quyền riêng tư:

- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Vui lòng ghi rõ tên ứng dụng **Subtitle Player & Editor** trong thư của bạn.

---

## 10. Thay đổi đối với Chính sách này

Chính sách này có thể được cập nhật nếu:

- các tính năng của ứng dụng thay đổi
- quyền hoặc việc sử dụng SDK thay đổi
- yêu cầu pháp lý hoặc yêu cầu của nền tảng thay đổi

Các thay đổi quan trọng sẽ được phản ánh trên trang chính sách đã cập nhật và, khi phù hợp, trong ứng dụng.
