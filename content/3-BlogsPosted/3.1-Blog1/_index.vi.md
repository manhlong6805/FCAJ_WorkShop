---
title: "Blog 1"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 3.1. </b> "
---


# Blog 1 - XÂY DỰNG HỆ THỐNG AI ĐA NGƯỜI DÙNG AN TOÀN VỚI AMAZON BEDROCK

Bài blog từ AWS giới thiệu cách PAR Technology xây dựng hệ thống AI đa người dùng (Multi-tenant AI) sử dụng Amazon Bedrock để phân tích dữ liệu bằng ngôn ngữ tự nhiên. Thách thức chính là đảm bảo nhiều người dùng có thể sử dụng chung một hệ thống AI nhưng vẫn duy trì tính bảo mật và phân quyền truy cập dữ liệu chính xác. Để giải quyết vấn đề này, PAR Technology đã xây dựng kiến trúc bảo mật ba lớp nhằm ngăn chặn truy cập trái phép và hạn chế nguy cơ rò rỉ dữ liệu giữa các tổ chức.

 **Các điểm chính cần nắm:** 

* Multi-tenant AI cho phép nhiều tổ chức sử dụng chung một hệ thống AI nhưng dữ liệu của từng tổ chức phải được bảo vệ độc lập.
* Amazon Bedrock cung cấp mô hình AI giúp hiểu câu hỏi bằng ngôn ngữ tự nhiên và tạo truy vấn SQL phục vụ phân tích dữ liệu.
* AWS Signature Version 4 (SigV4) xác thực danh tính và bảo vệ tính toàn vẹn của yêu cầu truy cập.
* Semantic Validation kiểm tra nội dung câu hỏi, đảm bảo yêu cầu hợp lệ trước khi truy xuất dữ liệu.
* Row-Level Security giới hạn quyền truy cập đến từng hàng dữ liệu theo vai trò và danh tính người dùng.
* Split-Plane SQL tách biệt quá trình kiểm soát quyền dữ liệu với quá trình tạo truy vấn bằng AI, ngăn mô hình truy cập dữ liệu ngoài phạm vi cho phép.
* Hệ thống sử dụng kiến trúc bảo mật nhiều lớp để giảm nguy cơ rò rỉ dữ liệu ngay cả khi mô hình AI tạo truy vấn không chính xác.

Giải pháp đặc biệt hữu ích đối với các doanh nghiệp cung cấp ứng dụng AI cho nhiều khách hàng, nơi việc phân quyền và bảo vệ dữ liệu là yêu cầu quan trọng. Qua đó cho thấy Amazon Bedrock có thể kết hợp với các cơ chế bảo mật AWS để xây dựng hệ thống AI linh hoạt, an toàn và có khả năng mở rộng.

**Cấu trúc phân cấp**
![Cấu trúc phân cấp](/FCAJ_WorkShop/images/structured.png)

**Kiến trúc hệ thống**
![Kiến trúc AI đa người dùng](/FCAJ_WorkShop/images/blog1.png)

**Link bài gốc:**  https://aws.amazon.com/vi/blogs/machine-learning/multi-tenant-llm-analytics-with-row-level-security-how-we-built-a-secure-agent-on-aws/

