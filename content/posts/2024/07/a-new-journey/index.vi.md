---
title: "Bài Viết Đầu Tiên: Hướng Dẫn Xây Dựng 'Kẻ Lãng Du Bắt Sóng Triều'"
date: 2024-07-25T11:00:00+08:00
categories: ["hugo"]
tags: ["hugo"]
summary: "Đây không chỉ là bài viết đầu tiên trên trang này, mà còn là một tài liệu sống về cách thêm bài viết và hình ảnh mới—một kế hoạch chi tiết cho quy trình sáng tạo của chúng ta trong tương lai."
draft: false
---

Chào tôi của tương lai, và những người bạn có thể ghé thăm nơi đây.

Chào mừng đến với sự khởi đầu của "Kẻ Lãng Du Bắt Sóng Triều". Không gian này được hình dung như một chiếc giỏ để chứa những "vỏ sò" và "vì sao" mà tôi nhặt được dọc theo bờ biển của tri thức và thông tin. Hôm nay, tôi sẽ đặt vào chiếc vỏ sò đầu tiên được lựa chọn cẩn thận—một hướng dẫn về cách tạo nội dung ở đây.

Bài đăng này vừa là một kỷ niệm, vừa là một sổ tay hướng dẫn, đảm bảo rằng mọi hoạt động sáng tạo trong tương lai đều rõ ràng và hiệu quả.

## I. Điểm Khởi Đầu: Một Lệnh Duy Nhất

Chúng ta không tạo tệp theo cách thủ công. Thay vào đó, chúng ta sử dụng công cụ dòng lệnh thanh lịch của HUGO. Nó giống như một cây đũa thần, chuẩn bị mọi thứ cho chúng ta.

Mở terminal của bạn, điều hướng đến thư mục gốc của blog, và đọc thần chú:

```bash
# Định dạng: hugo new loại-nội-dung/YYYY/MM/slug-bài-viết-của-bạn/index.ngôn-ngữ.md
hugo new posts/2024/07/a-new-journey/index.vi.md
```

Lệnh này thực hiện một chút phép thuật:

1.  Nó tạo một thư mục tên là `a-new-journey` trong thư mục `content/posts/2024/07/`.
2.  Bên trong thư mục đó, nó tạo một tệp `index.vi.md`.
3.  Nó tự động điền vào tệp này "thông tin nhận dạng" (Front Matter), bao gồm tiêu đề, ngày tháng và một cờ quan trọng: `draft: true`. Cờ này đánh dấu nó là một bản nháp, có thể xem được ở bản xem trước cục bộ nhưng sẽ bị bỏ qua khi triển khai cuối cùng, điều này rất an toàn.

Khi chúng ta viết xong và sẵn sàng cho thế giới thấy, chúng ta chỉ cần thay đổi `draft: true` thành `draft: false`.

## II. Thổi Hồn: Chữ Viết và Hình Ảnh

Một bài viết hoàn chỉnh bao gồm cả văn bản và hình ảnh. Trong cấu trúc được thiết kế tốt của chúng ta, việc quản lý chúng trở nên vô cùng đơn giản.

### 1. Chữ Viết

Bên dưới "thông tin nhận dạng" của tệp là nơi chúng ta tuôn trào con chữ. Nó tuân theo cú pháp Markdown tiêu chuẩn—ngắn gọn và mạnh mẽ.

### 2. Hình Ảnh: Tạm Biệt Sự Hỗn Loạn

Đây là phần tuyệt vời nhất trong quy trình làm việc của chúng ta. **Mỗi bài viết đều có thư mục riêng**, điều đó có nghĩa là tất cả hình ảnh được sử dụng trong bài viết có thể được lưu trữ ngay bên cạnh chính bài viết đó!

Giả sử chúng ta đang viết bài `a-new-journey` này. Cấu trúc thư mục của nó trông như sau:

```
content/
└── posts/
    └── 2024/
        └── 07/
            └── a-new-journey/          <-- Thư mục riêng của bài viết
                ├── index.vi.md         <-- Tệp bài viết
                └── journey-start.jpg   <-- Hình ảnh đi kèm của nó!
```

**Làm thế nào để tham chiếu đến hình ảnh này?**

Trong tệp `index.vi.md` của bạn, bạn chỉ cần viết như sau, không cần bất kỳ đường dẫn phức tạp nào:

```markdown
![Hành Trình Bắt Đầu](journey-start.jpg)
```

![Hành Trình Bắt Đầu](journey-start.jpg)

Chỉ đơn giản vậy thôi! Hình ảnh và văn bản được "gói" lại với nhau một cách thanh lịch, giúp việc di chuyển, sao lưu và quản lý trở thành một trải nghiệm không còn lo lắng.

## III. "Thẻ Căn Cước" của Bài Viết: Front Matter

Khu vực ở đầu mỗi bài viết, được bao bọc bởi `---`, là siêu dữ liệu của nó. Nó quyết định cách bài viết được phân loại và hiển thị.

-   **`title`**: Tiêu đề của bài viết.
-   **`date`**: Ngày xuất bản, quyết định vị trí của nó trong kho lưu trữ.
-   **`categories`**: Chuyên mục, thường là một phân loại rộng duy nhất như `["Ghi Chú Kỹ Thuật"]` hoặc `["Suy Ngẫm Cuộc Sống"]`.
-   **`tags`**: Thẻ, có thể có nhiều và được sử dụng để lập chỉ mục chi tiết hơn, như `["Go", "Web", "Tối Ưu Hóa Hiệu Năng"]`.
-   **`summary`**: Một bản tóm tắt ngắn sẽ được hiển thị trên trang danh sách bài viết.
-   **`draft`**: `false` có nghĩa là bài viết đã được xuất bản; `true` có nghĩa là nó là một bản nháp.

Việc điền cẩn thận những thông tin này sẽ giữ cho cơ sở kiến thức của chúng ta gọn gàng và có tổ chức.

## Kết Luận

Quá trình sáng tạo nên là một niềm vui, không phải là một gánh nặng.

Bắt đầu hành trình với `hugo new`, đặt chữ viết và hình ảnh vào thư mục riêng của chúng, và cuối cùng, phủi đi lớp bụi `draft`. Đó là toàn bộ bí quyết để ghi lại mọi khám phá ở đây, tại "Kẻ Lãng Du Bắt Sóng Triều".

Mong rằng chiếc giỏ nhỏ này sẽ ngày càng đầy hơn.