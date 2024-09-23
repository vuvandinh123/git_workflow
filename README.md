# git_workflow

- 1 Tạo repo với nhánh mặc định là main
- 2 Tạo nhánh develop để quản lý và phát triển ứng dụng trên nhánh này
- 3 Tạo các nhánh feature vd đătj tên feature/1-add-product-model trong đó 1 là id của issues cho từng chức năng phải tạo issues để tạo và quản lý các công việc cần làm 
- 4 khi hoàn thành một chức năng commit với id của issues vd: #1 -`<nội dung>`  lên nhánh develop
- 5 Vô nhánh develop tạo nhánh release-1.0.0 `git checkout -b release-1.0.0 develop`
- 6 Tạo tag `git tag v1.0.0` và `git push --tags`
- 7 Từ release đẩy lên production tức nhánh main
- 8 Xóa các nhánh đã xong như featuer và release 
---
# Các lệnh git cơ bản
## 1 Khởi tạo một dự án 
`git init`
chức năng tạo một thư mục .git để lưu trữ và quản lý các dữ liệu đến repo
## 2 Sao chép một repo từ xa
`git clone <link-ssh> hoặc https`
chức năng sẽ sao chép một repo từ xa và được tải lưu về máy cục bộ và tạo một tên thư mục cùng với tên repo nếu không đổi tên
## 3 Thêm các file cần đổi lên repo cục bôj để chuẩn bị
`git add <file>` hoặc `git add .` nêú đẩy tất cả file đã thay đổi hoặc mới tạo
## 4 Tạo log ghi chú
`git commit -m"add feauter ..."`
giúp gửi các tập tin lên kho repo với ghi chú là add feauter để biết file thay đổi gì và chức năng gì
## 5 đẩy các file chỉ định hay các tệp thay đổi lên nhánh chỉ định 
`git push <remote_repo> <branch>`
## 6 Cập nhật code mới nhất từ repo về nếu có nhiều người làm 
`git pull <remote_repo> <branch>`
## 7 xem các file đã sửa đổi
`git status`
## 8 Xem lịch sử các lệnh git
`git log` 
sẽ hiển thị toàn bộ các lịch sử commit và thời gian
## 9 Tạo nhánh xóa nhánh và xem nhánh
`git branch <ten nhanh muon tạo>` các kí tự đi kèm `-b` để tạo và truy cập `-d` để xóa nhánh 
## 10 Chuyển nhánh
`git checkout <branch_name>` 

