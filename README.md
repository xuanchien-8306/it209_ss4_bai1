# Bài 1: Khởi tạo Local Repository và Cấu hình danh tính

## 1. Khởi tạo Git Repository

Lệnh đã sử dụng:

```bash
git init
```

## 2. Cấu hình danh tính Local

Cấu hình tên:

```bash
git config --local user.name "Ta Xuan Chien"
```

Cấu hình email:

```bash
git config --local user.email "xuanchien319@gmail.com"
```

Kiểm tra:

```bash
git config --local user.name
git config --local user.email
```

## 3. Tạo file

```bash
echo "# IT209 - Session 04 - Exercise 1" > README.md
```

## 4. Đưa file vào Staging Area

```bash
git add README.md
```

## 5. Commit đầu tiên

```bash
git commit -m "Initial commit"
```

## 6. Kiểm tra lịch sử commit

```bash
git log --oneline
```

Kết quả:

```text
Initial commit
```

## 7. Kiểm tra cấu hình Local

```bash
git config --local --list
```

Kết quả cho thấy repository đã được cấu hình `user.name` và `user.email` ở cấp độ local.

## 8. Trạng thái Repository

```bash
git status
```

Sau khi commit thành công, working tree không còn file chưa commit.
