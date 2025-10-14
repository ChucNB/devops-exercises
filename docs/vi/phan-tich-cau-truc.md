# Phân tích cấu trúc repository `devops-exercises`

Tài liệu này cung cấp cái nhìn tổng thể về các thư mục và tệp quan trọng trong repo, giúp bạn định hướng nhanh khi lần đầu tìm hiểu.

## Tài liệu và tệp gốc ở thư mục root

- **`README.md`**: Trang giới thiệu chính bằng tiếng Anh, liệt kê danh sách chủ đề và cách sử dụng bộ câu hỏi.
- **`README-vi.md`**: Phiên bản giới thiệu nhanh bằng tiếng Việt.
- **`README-zh_CN.md`**: Bản dịch tiếng Trung giản thể.
- **`CONTRIBUTING.md`**: Quy tắc đóng góp và chuẩn định dạng khi mở pull request.
- **`faq.md`** và **`prepare_for_interview.md`**: Giải đáp thắc mắc thường gặp và hướng dẫn chuẩn bị phỏng vấn.
- **`credits.md`**: Ghi nhận đóng góp của cộng đồng.
- **`LICENSE`**: Thông tin giấy phép MIT.

## Thư mục nội dung chính

- **`topics/`**: Trái tim của repo với hơn 50 thư mục con (ví dụ: `aws`, `linux`, `kubernetes`, `terraform`, `security`...). Mỗi thư mục thường có `README.md` chứa bộ câu hỏi theo chủ đề. Một số chủ đề còn có cấu trúc con như `topics/aws/README.md`, `topics/linux/README.md`, `topics/devops/README.md`...
- **`exercises/`**: Bài tập tình huống chuyên sâu. Hiện có các phần như `docker/docker-debugging.md` và bài giải shell trong `shell/solutions/`.
- **`coding/`**: Bài tập coding ngắn gọn hỗ trợ tư duy thuật toán (ví dụ: `python/binary_search.py`, `python/merge_sort.py`).
- **`certificates/`**: Tài liệu định hướng chứng chỉ (AWS, Azure, Kubernetes). Mỗi file mô tả lộ trình hoặc mẹo thi cụ thể.
- **`docs/`**: Tài liệu bổ trợ. Nhánh `docs/vi/` chứa các hướng dẫn bằng tiếng Việt như `huong-dan-bat-dau.md` và tài liệu phân tích này.
- **`images/`**: Tài sản hình ảnh dùng trong README (logo, sơ đồ thiết kế, minh hoạ cloud, v.v.). Các thư mục con phân loại theo chủ đề (`aws`, `design`, `distributed`, ...).

## Tự động hoá, kiểm thử và tiện ích

- **`.github/workflows/ci_workflow.yml`**: Thiết lập GitHub Actions để lint Markdown và chạy kiểm tra tự động khi có PR.
- **`scripts/`**: Công cụ dòng lệnh phục vụ bảo trì repo, như `count_questions.sh` (đếm số câu hỏi), `random_question.py` (chọn ngẫu nhiên), `update_question_number.py` (cập nhật tổng câu hỏi) và thư mục con `'aws s3 event triggering'` chứa mẫu cấu hình sự kiện S3.
- **`tests/`**: Bộ kiểm thử Python bảo đảm chất lượng câu hỏi (`scripts_question_utils_unittest.py`, `syntax_checker_unittest.py`) và thư mục `testcases/` với các ví dụ kiểm tra.

## Những file hỗ trợ khác

- **`coding/`**, `scripts/` và `tests/` thường sử dụng chung tiện ích trong `scripts/question_utils.py`.
- Các ảnh minh hoạ trong `images/` được tham chiếu xuyên suốt README và các chủ đề.

## Gợi ý điều hướng khi học

1. Bắt đầu bằng việc đọc `README.md` (hoặc `README-vi.md`) để nắm phạm vi chủ đề.
2. Chọn chủ đề trong `topics/` phù hợp mục tiêu của bạn.
3. Dùng `exercises/` khi muốn thử thách sâu hơn sau khi hoàn thành câu hỏi lý thuyết.
4. Tham khảo `certificates/` nếu bạn lên kế hoạch thi chứng chỉ.
5. Khai thác `scripts/` và `tests/` nếu muốn đóng góp câu hỏi mới, bảo đảm tuân thủ tiêu chuẩn repo.

Tài liệu này sẽ được cập nhật khi cấu trúc repo thay đổi hoặc khi bổ sung tài liệu tiếng Việt mới.
