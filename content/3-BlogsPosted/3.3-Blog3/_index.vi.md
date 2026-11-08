---
title: "Blog 3"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 3.3. </b> "
---

# BLOG 3: Ứng dụng AI để tự động kiểm thử website với Amazon Nova Act

Bài blog từ AWS giới thiệu cách công ty Epsilon ứng dụng Amazon Nova Act và Amazon Bedrock AgentCore Browser để xây dựng hệ thống tự động kiểm thử giao diện website bằng trí tuệ nhân tạo. Phương pháp kiểm thử truyền thống thường yêu cầu lập trình viên viết mã và xác định các thành phần giao diện, gây tốn thời gian khi website thay đổi. Giải pháp của Epsilon cho phép mô tả các bước kiểm thử bằng ngôn ngữ tự nhiên, giúp đơn giản hóa quy trình kiểm thử và giảm công việc bảo trì mã lệnh.

**Các điểm chính cần nắm:**

* Amazon Nova Act là dịch vụ hỗ trợ xây dựng AI Agent có khả năng tương tác với giao diện website dựa trên chỉ dẫn bằng ngôn ngữ tự nhiên.

* Intent-driven UI Testing cho phép mô tả mục tiêu kiểm thử thay vì phải viết mã điều khiển từng thao tác trên giao diện.

* Amazon Bedrock AgentCore Browser cung cấp môi trường trình duyệt được quản lý để thực hiện các tác vụ kiểm thử tự động.

* Natural Language Instructions giúp AI hiểu và thực hiện các hành động như nhập dữ liệu, nhấn nút, cuộn trang và kiểm tra kết quả.

* Amazon S3 lưu trữ ảnh chụp màn hình, báo cáo và kết quả của quá trình kiểm thử.

* AWS IAM hỗ trợ quản lý quyền truy cập và cách ly môi trường kiểm thử giữa các nhóm phát triển.

* Automated Test Reporting ghi nhận trạng thái thành công hoặc thất bại của từng bước kiểm thử, hỗ trợ phân tích lỗi.

* Hệ thống có thể kết hợp AI Testing với Playwright để tận dụng khả năng hiểu giao diện của AI và tính ổn định của các bài kiểm thử truyền thống.

Theo kết quả thử nghiệm nội bộ của Epsilon, Amazon Nova Act giúp giảm công sức xây dựng kịch bản kiểm thử khoảng 4–6 lần so với phương pháp Playwright tương đương. Giải pháp cho thấy tiềm năng của Agentic AI trong việc tự động hóa kiểm thử phần mềm, giảm thời gian xây dựng kịch bản và nâng cao hiệu quả quản lý chất lượng ứng dụng web.

**Kiến trúc dịch vụ kiểm thử**
![Kiến trúc dịch vụ kiểm thử](/FCAJ_WorkShop/images/blog3.png)

**Link bài gốc:**https://aws.amazon.com/vi/blogs/machine-learning/building-intent-driven-ui-testing-with-amazon-nova-act/

