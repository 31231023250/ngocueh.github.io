# PYDATA BOOK

**TRẦN THỊ KIM NGỌC - 31231023250**# vào thư mục cha, rồi cd vào đúng folder cần đẩy
cd /path/đến/thư-mục-cha
cd "Lab-midterm"

# khởi tạo repo
git init

# (khuyến nghị) đặt tên nhánh chính là main
git checkout -b main

# cấu hình tên/email (nếu máy chưa cấu hình)
git config user.name "Your Name"
git config user.email "you@example.com"

# bỏ qua file rác & checkpoint của Jupyter
printf ".ipynb_checkpoints/\n.DS_Store\n*.~lock*\n" > .gitignore

# add toàn bộ & commit
git add .
git commit -m "Initial commit: Lab-midterm notebooks & data"

# thêm remote (thay URL bằng repo của bạn trên GitHub/GitLab, HTTPS hoặc SSH đều được)
git remote add origin https://github.com/<user>/<repo>.git
# hoặc: git remote add origin git@github.com:<user>/<repo>.git

# đẩy lên lần đầu
git push -u origin main

