# (Bài tập tổng hợp) Dựng README.md cho Dự Án CLB SmartCampus

## Phần 1 – Khung sườn README

````markdown
#  SmartCampus

**SmartCampus** là ứng dụng di động giúp sinh viên PTIT tra cứu *lịch học*, phòng trống và nhận thông báo mới nhất từ nhà trường.

## Tính năng đã hoàn thành

- Tra cứu lịch học theo mã sinh viên
  - Nhập mã sinh viên để xem lịch học
- Xem danh sách phòng trống theo tòa nhà

Trang chủ CLB: [CLB Lập trình](https://clblaptrinh.ptit.edu.vn)

![Logo SmartCampus](https://clblaptrinh.ptit.edu.vn/logo.png)

>  **Cảnh báo:** Dự án đang trong giai đoạn phát triển, chưa dùng cho mục đích chính thức.

---
````

## Phần 2 – Phần kỹ thuật của README

````markdown
## :rocket: Cài đặt

```bash
git clone https://github.com/clb-lap-trinh/smartcampus.git
npm install
npm start
```

## Tiến độ

- [x] Tra cứu lịch học theo mã sinh viên
- [x] Xem danh sách phòng trống theo tòa nhà
- [ ] Thông báo đẩy (push notification)
- [ ] Đăng nhập bằng tài khoản trường

## Thư viện sử dụng

| Thư viện | Phiên bản | Mục đích |
| :--- | :---: | :--- |
| React Native | 0.74 | Xây giao diện đa nền tảng iOS/Android |
| Axios | 1.6 | Gọi API lấy dữ liệu lịch học |

## Lưu ý

Trong Markdown, dấu \* dùng để in nghiêng và dấu \# dùng để tạo tiêu đề.
````

## Phần 3 – Hỏi AI đúng cách và lưu tài liệu

### Prompt theo Công thức 3 Phần

```markdown
## Tôi là ai / Bối cảnh
Tôi là sinh viên năm nhất, mới vào nhóm dự án SmartCampus của CLB Lập trình.

## Chủ đề / Nội dung cần xử lý
Giải thích thuật ngữ API.

## Yêu cầu
- Giải thích bằng ngôn ngữ đơn giản, dễ hiểu
- Có một ví dụ đời thường để so sánh
- Có một ví dụ gắn với ứng dụng tra cứu lịch học

## Không cần
- Không cần đi sâu vào code hay các loại API nâng cao
```

### Tóm tắt câu trả lời của AI (tối đa 3 câu)

> API là cầu nối giúp hai phần mềm trao đổi dữ liệu. Nó giống người phục vụ nhận yêu cầu rồi mang kết quả về. Trong SmartCampus, API giúp ứng dụng lấy lịch học từ hệ thống của trường.

### Lưu file

Dán nguyên câu trả lời của AI vào StackEdit và lưu thành `api_giai_thich.md`.

## Phần 4 – Bẫy cú pháp

### Hai lỗi

1. Bảng thiếu **dòng phân cách** `| --- | --- |` ngay dưới dòng tiêu đề, nên bảng không render.
2. Task list thiếu **dấu cách** sau `-` (`-[x]`, `-[ ]`), nên không thành checkbox.

### Đoạn đã sửa

```markdown
| Tính năng | Trạng thái |
| --- | --- |
| Tra cứu lịch học | Xong |
| Push notification | Đang làm |

- [x] Tra cứu lịch học
- [ ] Push notification
```
