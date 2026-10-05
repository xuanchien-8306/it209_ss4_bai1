# Bài 1: Khởi tạo Local Repository và Cấu hình danh tính

## 1. Khởi tạo Repository

```bash
git init
```

Kết quả:

```text
Initialized empty Git repository in C:/Users/Admin/Documents/it209/SS4/bai1/.git/
```

## 2. Cấu hình danh tính cục bộ

Cấu hình tên:

```bash
git config --local user.name "Xuan Chien"
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

Kết quả:

```text
Xuan Chien
xuanchien319@gmail.com
```

## 3. Đưa file vào Staging Area

```bash
git add README.md
```

Kiểm tra:

```bash
git status
```

Kết quả:

```text
On branch master

No commits yet

Changes to be committed:
        new file:   README.md
```

## 4. Commit đầu tiên

```bash
git commit -m "Initial commit"
```

Kết quả:

```text
[master (root-commit) 1fbbdb7] Initial commit
1 file changed, 76 insertions(+)
create mode 100644 README.md
```

## 5. Kiểm tra lịch sử Commit

```bash
git log --oneline
```

Kết quả:

```text
1fbbdb7 (HEAD -> master) Initial commit
```

## 6. Kiểm tra cấu hình Local

```bash
git config --local --list
```

Kết quả:

```text
core.repositoryformatversion=0
core.filemode=false
core.bare=false
core.logallrefupdates=true
user.name=Xuan Chien
user.email=xuanchien319@gmail.com
```

## 7. Kết luận

Repository Git local đã được khởi tạo thành công. Danh tính tác giả đã được cấu hình ở cấp độ local bằng `--local`. File `README.md` đã được đưa vào Staging Area và commit đầu tiên đã được tạo thành công với thông điệp `Initial commit`.
