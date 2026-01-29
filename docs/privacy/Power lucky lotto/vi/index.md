---
title: Chính sách Quyền riêng tư | Power lucky lotto
description: Chính sách Quyền riêng tư của Power lucky lotto (Tiếng Việt)
lang: vi
last_updated: 2026-01-29
---

# Chính sách Quyền riêng tư (Power lucky lotto)

- **Tên ứng dụng:** Power lucky lotto  
- **Nhà phát triển:** frog-im  
- **Liên hệ:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Ngày có hiệu lực:** 2026-01-29  

> Chính sách này được soạn thảo tham chiếu các luật về quyền riêng tư có liên quan như PIPA (Hàn Quốc), GDPR/UK GDPR, FADP (Thụy Sĩ) và các luật quyền riêng tư cấp bang của Hoa Kỳ.  
> Nếu khu vực của bạn có yêu cầu bắt buộc riêng, các yêu cầu đó sẽ được ưu tiên áp dụng.

---

## 1. Mục đích và phạm vi

Power lucky lotto là ứng dụng quản lý trò chơi xổ số và xem bản ghi. Các tính năng chính gồm:

- Chọn quốc gia/trò chơi và thiết lập (ví dụ: KR 6/45, US Powerball)  
- Tạo/lưu số và xem log (lịch sử)  
- Xem và xóa bảng log (danh sách bảng/chi tiết)  
- Chỉnh sửa/quản lý dữ liệu kết quả theo JSON (phục vụ thống kê/hiển thị)  
- Quảng cáo (bao gồm quảng cáo thưởng) và quản lý đồng ý (khi cần)

Ứng dụng **không yêu cầu tạo tài khoản** và theo mặc định **không tải dữ liệu của bạn lên máy chủ của nhà phát triển.**  
Phần lớn xử lý diễn ra **trên thiết bị của bạn**.

Tuy nhiên, để phục vụ **quảng cáo**, **quản lý đồng ý**, và **tuân thủ pháp lý**, các SDK bên thứ ba như  
**Google Mobile Ads SDK (AdMob)** và **Google UMP (User Messaging Platform)** có thể thu thập và xử lý một số dữ liệu (ví dụ: mã định danh quảng cáo).

---

## 2. Loại dữ liệu được xử lý

### 2-1) Dữ liệu lưu trên thiết bị của bạn (lưu trữ cục bộ)

Ứng dụng lưu một số dữ liệu **cục bộ trên thiết bị** để cung cấp tính năng và tăng tiện ích sử dụng.  
Dữ liệu này thường **không được truyền tới máy chủ của nhà phát triển** và sẽ bị xóa khi bạn xóa dữ liệu ứng dụng hoặc gỡ cài đặt (trừ các tệp bạn xuất ra nơi khác).

#### (1) Cài đặt (SharedPreferences)

| Danh mục | Khóa (ví dụ) | Mục đích | Lưu trữ | Xóa |
|---|---|---|---|---|
| Hoàn tất thiết lập | `setup_done` | Lưu trạng thái thiết lập ban đầu | SharedPreferences | Xóa khi xóa dữ liệu/gỡ cài đặt |
| Lịch sử quốc gia | `selected_countries` | Lưu các quốc gia đã chọn gần đây | Tương tự | Tương tự |
| Quốc gia đang chọn | `active_country` | Lưu quốc gia hiện tại | Tương tự | Tương tự |
| Trò chơi đã chọn | `selected_lotto_ids` | Lưu các ID trò chơi được tick | Tương tự | Tương tự |
| Trò chơi đang dùng | `active_lotto_id` | Lưu ID trò chơi đang hoạt động | Tương tự | Tương tự |
| **Chọn thời gian seed (tùy chọn)** | `birth_datetime_iso` | Lưu thời điểm tham chiếu seed do người dùng chọn (có thể dùng cho seeding/cá nhân hóa) | Tương tự | Tương tự |

> **Lưu ý:** “Chọn thời gian seed (tùy chọn)” chỉ được xử lý khi người dùng chủ động thiết lập và có thể không cần cho việc sử dụng cốt lõi.

#### (2) Dữ liệu log (SQLite)

Ứng dụng có thể lưu các bản ghi đã tạo/đã lưu trong cơ sở dữ liệu SQLite cục bộ.

- Ví dụ bảng: `log_...`  
- Ví dụ trường:  
  - `id`, `date_id` hoặc `date_text` (mốc thời gian), `choice1..choiceN` (các số đã chọn), `isFinger` (cờ liên quan vân tay, v.v.)

Bạn có thể xem log trong màn hình danh sách/chi tiết bảng và xóa (theo bảng hoặc theo dòng) nếu muốn.

#### (3) Tệp dữ liệu JSON (theo trò chơi)

Ứng dụng có thể lưu dữ liệu JSON theo từng trò chơi trong thư mục tài liệu của ứng dụng.

- Ví dụ: `game_json/<gameId>.json`  
- Mục đích: dữ liệu kỳ quay/kết quả do người dùng quản lý/chỉnh sửa (phục vụ thống kê/hiển thị)

Các tệp này được lưu trên thiết bị và thường bị xóa khi gỡ cài đặt, tùy thuộc hành vi OS/sao lưu.

---

### 2-2) Quảng cáo, đồng ý và dữ liệu liên quan (SDK bên thứ ba)

Ứng dụng sử dụng **Google Mobile Ads SDK (AdMob)** và **Google UMP** để:

- Hiển thị quảng cáo (bao gồm **quảng cáo thưởng**)  
- Quản lý đồng ý quảng cáo theo yêu cầu pháp lý

Các SDK này có thể thu thập/xử lý, ví dụ:

- **ID quảng cáo** (ví dụ AAID, IDFA)  
- Thông tin dựa trên IP, vị trí xấp xỉ, thông tin mạng  
- Thông tin thiết bị/ứng dụng (phiên bản OS, phiên bản ứng dụng, ngôn ngữ, thông tin chẩn đoán)  
- Tương tác quảng cáo (lượt hiển thị, lượt nhấp, hoàn tất thưởng)  
- Lựa chọn đồng ý được ghi bởi UMP

Tại một số khu vực (ví dụ EEA/UK/CH), có thể hiển thị biểu mẫu đồng ý UMP và cung cấp mục **Privacy Options** khi cần.

---

## 3. Thời hạn lưu giữ

- **Cài đặt cục bộ (SharedPreferences):** lưu đến khi bạn xóa dữ liệu ứng dụng hoặc gỡ cài đặt  
- **Dữ liệu log (SQLite):** lưu đến khi bạn xóa hoặc gỡ/xóa dữ liệu ứng dụng  
- **Tệp JSON:** lưu trong thư mục tài liệu; thường bị xóa khi gỡ cài đặt, nhưng bản xuất/sao lưu do người dùng quản lý  
- **Dữ liệu quảng cáo/đồng ý (bên thứ ba):** lưu theo chính sách của Google và luật áp dụng

---

## 4. Chia sẻ bên thứ ba và chuyển dữ liệu quốc tế

Để phục vụ quảng cáo và quản lý đồng ý, một số dữ liệu có thể được xử lý bởi **Google và đối tác**.

| Mục | Chi tiết |
|---|---|
| **Bên nhận** | Google LLC, công ty liên kết và bên xử lý phụ |
| **Nơi chuyển đến** | Hoa Kỳ và các khu vực khác nơi hạ tầng Google đặt tại |
| **Mục đích** | Phân phối quảng cáo, đo lường, chống gian lận, quản lý đồng ý, tuân thủ |
| **Dữ liệu** | ID quảng cáo, thông tin dựa trên IP, thông tin thiết bị/ứng dụng, dữ liệu tương tác quảng cáo, trạng thái đồng ý |
| **Lưu giữ** | Theo chính sách Google và luật áp dụng |
| **Ảnh hưởng khi từ chối** | Quảng cáo cá nhân hóa có thể bị hạn chế; có thể hiển thị quảng cáo không cá nhân hóa hoặc ít quảng cáo hơn |

---

## 5. Quyền của bạn và cách thực hiện

Tùy theo luật áp dụng, bạn có thể có các quyền như truy cập, chỉnh sửa, xóa, hạn chế xử lý, phản đối, chuyển dữ liệu, và rút lại đồng ý (khi đồng ý là cơ sở pháp lý).

Ví dụ:

- **Điều chỉnh lựa chọn quảng cáo/đồng ý:** qua Privacy Options trong ứng dụng (nếu có) hoặc cài đặt quảng cáo của OS (đặt lại ID quảng cáo, hạn chế cá nhân hóa).  
- **Đặt lại dữ liệu cục bộ:** xóa dữ liệu ứng dụng hoặc gỡ cài đặt để xóa cài đặt/log/tệp cục bộ.

---

## 6. Quyền riêng tư của trẻ em

Ứng dụng này **không được thiết kế cho trẻ em**. Nếu trẻ em sử dụng, người giám hộ nên cân nhắc các kiểm soát của phụ huynh ở cấp OS và các tính năng hạn chế quảng cáo.

---

## 7. Biện pháp bảo mật

Trong phạm vi ứng dụng, chúng tôi nỗ lực:

- Chỉ lưu tối thiểu dữ liệu cần thiết trên thiết bị  
- Giữ xử lý trên thiết bị khi có thể  
- Sử dụng TLS/đường truyền an toàn cho liên lạc mạng của SDK (trong giới hạn SDK)

---

## 8. Google Play Data safety

Nếu phát hành trên Google Play, chúng tôi cố gắng đảm bảo khai báo Data safety chính xác và được cập nhật, đặc biệt khi SDK hoặc cách xử lý thay đổi.

---

## 9. Thông báo mã nguồn mở

Ứng dụng có thể dùng thư viện mã nguồn mở cho icon quốc gia, lưu trữ, quảng cáo/đồng ý và UI.  
Thông tin giấy phép có trong màn hình “Open-source licenses” (hoặc tương đương) của ứng dụng.

---

## 10. Liên hệ

Mọi thắc mắc về quyền riêng tư:

- **Email:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Vui lòng nêu rõ **“Power lucky lotto”** trong nội dung liên hệ.

---

## 11. Thay đổi chính sách

Chính sách này có thể thay đổi do cập nhật pháp luật, thay đổi tính năng (ví dụ thêm SDK mới) hoặc điều chỉnh nội bộ.  
Thay đổi nhỏ sẽ được đăng trong ứng dụng hoặc trên trang này; thay đổi quan trọng sẽ được thông báo trước theo yêu cầu.
