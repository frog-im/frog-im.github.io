---
title: Chính sách quyền riêng tư | Lyrics Overlay & Tag Editorr
description: Chính sách quyền riêng tư của Lyrics Overlay & Tag Editorr (Tiếng Việt)
lang: vi
last_updated: 2025-10-30
---

# Chính sách quyền riêng tư (Lyrics Overlay & Tag Editorr)

- **Tên ứng dụng:** Lyrics Overlay & Tag Editorr  
- **Nhà phát triển:** frog-im  
- **Liên hệ:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Ngày hiệu lực:** 2025-10-30

> Chính sách này được soạn thảo tham chiếu các luật hiện hành, gồm Luật Bảo vệ Thông tin Cá nhân của Hàn Quốc (PIPA), GDPR/UK GDPR, FADP của Thụy Sĩ và các luật quyền riêng tư cấp bang của Hoa Kỳ. Nếu có yêu cầu bổ sung theo từng khu vực tài phán, các yêu cầu đó sẽ được ưu tiên áp dụng.

---

## 1. Mục đích và phạm vi xử lý

Ứng dụng cung cấp chức năng **chỉnh sửa siêu dữ liệu (metadata)** (tiêu đề, nghệ sĩ, v.v.) cho các tệp âm thanh **lưu trên thiết bị**, và **lớp phủ lời bài hát (lyrics overlay)**.  
Ứng dụng **không** tạo **tài khoản** và **không** tải nội dung của người dùng lên máy chủ của chúng tôi; mặc định, xử lý được thực hiện **trên thiết bị của người dùng**.

Tuy nhiên, cho mục đích **quảng cáo** và **tuân thủ pháp lý**, đối tác bên thứ ba (ví dụ: Google Mobile Ads SDK (AdMob), UMP) có thể thu thập/xử lý thông tin như **định danh quảng cáo**. Việc thu thập đồng ý và cung cấp tùy chọn quyền riêng tư tuân theo đặc tả của **Google UMP (User Messaging Platform)**.

---

## 2. Các hạng mục thông tin được xử lý

### 2-1) Tệp người dùng chủ động chọn
- **Đường dẫn và nội dung âm thanh/ảnh bìa:** chỉ được xử lý **cục bộ trên thiết bị** nhằm mục đích chỉnh sửa/lưu.  
- **FFmpegKit** được dùng cục bộ cho mã hóa, chỉnh sửa siêu dữ liệu và trích xuất ảnh thu nhỏ.  
- Ứng dụng **không tải lên** máy chủ của chúng tôi các tệp do người dùng chọn.

### 2-2) Thiết lập cục bộ và giá trị được lưu

Để vận hành tính năng và nâng cao tiện ích, ứng dụng lưu các giá trị sau **cục bộ trên thiết bị**.  
Các giá trị này không được gửi đến máy chủ của chúng tôi và **sẽ bị xóa khi xóa dữ liệu ứng dụng hoặc gỡ cài đặt ứng dụng**.

#### (1) Tùy chọn (`shared_preferences`)
| Loại | Khóa/Nội dung | Mục đích | Vị trí lưu | Cách xóa |
|---|---|---|---|---|
| Vị trí/phông chữ lớp phủ | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Khôi phục vị trí lớp phủ và cỡ chữ | SharedPreferences trên thiết bị | Xóa khi xóa dữ liệu ứng dụng hoặc gỡ cài đặt |
| Quảng cáo/Quyền riêng tư | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Quảng cáo không cá nhân hóa (NPA), RDP tại Hoa Kỳ, gắn nhãn COPPA, nhãn độ tuổi, giới hạn xếp hạng nội dung quảng cáo | SharedPreferences trên thiết bị | Tương tự bên trái |

#### (2) Tệp tạm (thư mục tạm của hệ thống)
- **Ví dụ:** `cover_*.jpg`, `tmp_*.flac`  
- **Mục đích:** trích xuất ảnh bìa, gắn thẻ FLAC, mã hóa tạm  
- **Vị trí:** thư mục tạm của hệ điều hành (`systemTemp`)  
- **Thời gian lưu:** cố gắng xóa sau khi xử lý xong; hệ điều hành cũng có thể dọn định kỳ

#### (3) Lưu do người dùng chọn (SAF)
- Với “Lưu thành…”, tệp đầu ra có thể được ghi vào vị trí do người dùng chọn (ví dụ: Tải xuống, đám mây).  
- Các tệp này nằm ở **bộ nhớ ngoài** và **có thể còn lại sau khi gỡ cài đặt ứng dụng**. Người dùng có thể tự xóa.

#### (4) Trạng thái đồng ý (bộ nhớ đệm của SDK UMP)
- Tại EEA/Vương quốc Anh/Thụy Sĩ, SDK UMP **lưu đệm cục bộ** trạng thái đồng ý quảng cáo của người dùng.  
- Có thể đặt lại bằng cách xóa dữ liệu ứng dụng hoặc qua màn hình **Privacy Options (Tùy chọn quyền riêng tư)** trong ứng dụng (nếu khả dụng).

---

### 2-3) Dữ liệu quảng cáo và đồng ý (SDK bên thứ ba)
- **Google Mobile Ads SDK (AdMob) và UMP** có thể thu thập/xử lý, ví dụ: **định danh quảng cáo (AAID/IDFA)**, **dải IP**, **thông tin thiết bị/ứng dụng**, **tín hiệu tương tác quảng cáo**, **trạng thái đồng ý**, v.v.  
- **Mục đích:** phân phối quảng cáo, giới hạn tần suất, chống gian lận, đo lường hiệu suất, tuân thủ pháp luật  
- **Khu vực cần đồng ý (EEA/Vương quốc Anh/Thụy Sĩ):** thu thập đồng ý qua UMP và cung cấp màn hình **Privacy Options** khi cần.  
  Ở khu vực không có yêu cầu này (ví dụ: Hàn Quốc), **tùy chọn có thể không hiển thị**.

---

## 3. Xử lý và thời hạn lưu trữ

- **Thiết lập cục bộ:** lưu trên thiết bị cho đến khi người dùng xóa dữ liệu ứng dụng hoặc gỡ cài đặt  
- **Tệp tạm:** tạo trong quá trình mã hóa/trích xuất; xóa sau xử lý hoặc có thể tạm thời còn trong bộ nhớ đệm của hệ điều hành  
- **Dữ liệu quảng cáo/đồng ý (bên thứ ba):** theo **chính sách của Google**

---

## 4. Cung cấp cho bên thứ ba và chuyển dữ liệu xuyên biên giới

Để phục vụ quảng cáo và quản lý đồng ý, thông tin của người dùng có thể được truyền tới và xử lý trên hạ tầng của Google.

| Mục | Nội dung |
|---|---|
| **Bên nhận** | Google LLC và các công ty liên kết/bên xử lý phụ |
| **Quốc gia đích** | Hoa Kỳ (và các khu vực khác nơi đặt hạ tầng của Google) |
| **Mục đích** | Phân phối quảng cáo, hiệu suất/đo lường, tuân thủ pháp lý, quản lý đồng ý |
| **Dữ liệu chuyển** | Định danh quảng cáo, dải IP, thông tin thiết bị/ứng dụng, tương tác quảng cáo, trạng thái đồng ý, v.v. |
| **Thời hạn lưu** | Theo chính sách của Google |
| **Ảnh hưởng khi từ chối** | Hạn chế cá nhân hóa; có thể chỉ hiển thị quảng cáo không cá nhân hóa |

Ứng dụng tuân thủ yêu cầu công bố trong phần **“An toàn dữ liệu (Data safety)” của Google Play** và duy trì tính phù hợp với thực tiễn xử lý.

---

## 5. Quyền của người dùng và cách thực hiện

- **Tắt quảng cáo cá nhân hóa / thay đổi đồng ý**  
  - Ở các khu vực được hỗ trợ (EEA/Vương quốc Anh/Thụy Sĩ): thay đổi trong **Cài đặt → Tùy chọn quyền riêng tư**.  
  - Khu vực khác: dùng cài đặt hệ điều hành để **đặt lại ID quảng cáo / hạn chế theo dõi**.
- **Đặt lại thông tin cục bộ:** xóa dữ liệu ứng dụng hoặc gỡ cài đặt sẽ đặt lại tọa độ lớp phủ, cỡ chữ và các thiết lập cục bộ khác.
- Các quyền theo **GDPR/UK GDPR/FADP của Thụy Sĩ/các luật quyền riêng tư bang của Hoa Kỳ** (truy cập, chỉnh sửa, xóa, di chuyển, hạn chế xử lý, rút lại đồng ý, v.v.) có thể được thực hiện theo thủ tục của luật.  
  Với dữ liệu quảng cáo do Google xử lý, vui lòng sử dụng **quy trình của Google**.

---

## 6. Quyền riêng tư của trẻ em

Ứng dụng **không hướng tới trẻ em**. Trẻ dưới độ tuổi tối thiểu theo luật định nên ngừng sử dụng và cùng người giám hộ dùng chức năng hạn chế quảng cáo ở cấp hệ điều hành. Khi phù hợp, chúng tôi có thể áp dụng **TFUA (thẻ “hướng tới trẻ em”)** hoặc lựa chọn bảo vệ tương đương.

---

## 7. Biện pháp bảo mật

- **Tối thiểu hóa dữ liệu** trong thu thập và lưu trữ  
- **Giới hạn sử dụng** tệp tạm và cố gắng xóa sau khi xử lý  
- Xử lý **trong phạm vi quyền hệ điều hành**  
- **Mã hóa khi truyền** (TLS hoặc tương đương) khi chuyển cho bên thứ ba theo chuẩn của SDK

---

## 8. Công bố dữ liệu (Google Play “Data safety”)

Chúng tôi soạn và duy trì chính xác phần **“Data safety”** trong Play Console và cập nhật kịp thời khi có thay đổi.

---

## 9. Thông báo mã nguồn mở

Ứng dụng sử dụng phần mềm mã nguồn mở như **FFmpeg**. Tệp hướng dẫn (ví dụ: `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) trong ứng dụng nêu cách nhận mã nguồn; theo yêu cầu, chúng tôi sẽ cung cấp theo hướng dẫn trong tệp.

---

## 10. Liên hệ

- Email: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Thông báo thay đổi

Chính sách có thể được sửa đổi do thay đổi pháp luật/dịch vụ; thay đổi sẽ được đăng **trong ứng dụng** và trên **trang chính sách** này.  
Với thay đổi trọng yếu, chúng tôi sẽ thông báo **ít nhất 7 ngày trước** ngày hiệu lực.

---

## Phụ lục: Hướng dẫn cho người dùng

- **Liên kết trong ứng dụng:** mở trang này từ **Cài đặt → Quyền riêng tư (Privacy)**.  
- **Hành vi theo khu vực:** tại EEA/Vương quốc Anh/Thụy Sĩ sẽ hiển thị Privacy Options; **tại Hàn Quốc và một số nơi khác, nút có thể không hiển thị tùy chọn bổ sung** nếu pháp luật không yêu cầu.

