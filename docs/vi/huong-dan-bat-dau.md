# Hướng dẫn bắt đầu học với devops-exercises

Tài liệu này giúp bạn thiết lập lộ trình tự học từ repo devops-exercises và chuẩn bị cho việc mở pull request đóng góp bản dịch.

## 1. Chuẩn bị

- **Công cụ đọc Markdown:** VS Code, Obsidian hoặc trình đọc Markdown bất kỳ.
- **Kho riêng để dịch:** Fork repo về tài khoản GitHub của bạn.
- **Ngôn ngữ sử dụng:** Ghi chú và câu trả lời bằng tiếng Việt để dễ hệ thống hóa.

## 2. Lộ trình học theo giai đoạn

### Giai đoạn 1 – Nắm nền tảng DevOps
1. Đọc phần giới thiệu trong [`README-vi.md`](../../README-vi.md) để hiểu cấu trúc repo.
2. Học các chủ đề cốt lõi:
   - [topics/devops](../../topics/devops/README.md)
   - [topics/git](../../topics/git/README.md)
   - [topics/linux](../../topics/linux/README.md)
3. Làm bài tập nhỏ: tự trả lời các câu hỏi rồi kiểm tra chéo với tài liệu chính thức.

### Giai đoạn 2 – Hệ thống & mạng
1. Nghiên cứu mục **Network** trong [`README.md`](../../README.md) để nắm khái niệm giao thức.
2. Tập trung vào các câu hỏi về TCP/IP, OSI, subnet trong thư mục `topics/networking` (nếu có) hoặc phần Network của README.
3. Viết ghi chú bằng tiếng Việt cho từng khái niệm quan trọng.

### Giai đoạn 3 – Tự động hóa & CI/CD
1. Đọc [topics/cicd](../../topics/cicd/README.md) và [topics/containers](../../topics/containers/README.md).
2. Thử tự động hóa đơn giản: viết script bash nhỏ hoặc dùng Docker để thực hành.
3. Ghi lại kinh nghiệm, lỗi gặp phải và cách khắc phục.

### Giai đoạn 4 – Cloud & hạ tầng
1. Chọn một nhà cung cấp cloud (AWS/Azure/GCP) phù hợp mục tiêu nghề nghiệp.
2. Dùng các thư mục tương ứng (`topics/aws`, `topics/azure`, `topics/gcp`).
3. Đối chiếu với tài liệu chính thức của nhà cung cấp để cập nhật kiến thức mới.

## 3. Chiến lược dịch tài liệu

1. **Ưu tiên tệp cốt lõi**: `README.md`, `faq.md`, `prepare_for_interview.md`.
2. **Chia nhỏ công việc**: mỗi commit dịch một phần hoặc một chủ đề để dễ review.
3. **Giữ nguyên liên kết & cấu trúc**: chỉ dịch nội dung văn bản, không đổi đường dẫn.
4. **Kiểm tra chính tả/thuật ngữ**: thống nhất cách dịch các thuật ngữ (ví dụ: *continuous integration* → *tích hợp liên tục*).

## 4. Quy trình tạo Pull Request

1. Tạo nhánh mới: `git checkout -b feature/dich-readme`.
2. Dịch và lưu các tệp cần thiết (`README-vi.md`, ghi chú...).
3. Chạy `git status` để kiểm tra thay đổi, `git add` những tệp mới.
4. Commit với thông điệp rõ ràng, ví dụ: `git commit -m "Add Vietnamese quickstart guide"`.
5. Đẩy nhánh lên fork: `git push origin feature/dich-readme`.
6. Tạo Pull Request trên GitHub, mô tả ngắn gọn nội dung dịch và phạm vi thay đổi.

## 5. Duy trì thói quen học

- Đặt lịch học cố định (ví dụ 30 phút mỗi ngày).
- Mỗi tuần chọn một chủ đề mới trong `topics/` để đào sâu.
- Chia sẻ kiến thức vừa học được bằng blog hoặc ghi chú công khai.

Chúc bạn học hiệu quả và đóng góp được nhiều nội dung tiếng Việt cho cộng đồng!

