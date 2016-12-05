# overlayfs
leo thanng đặc quyền

Các hệ thống tập tin overlayfs không kiểm tra một cách chính xác cho phép tập tin khi
tạo file mới trên vùng upper của thư mục hệ thống tập tin. Điều này có thể được khai thác
bởi một quá trình không có đặc quyền trong hạt nhân với CONFIG_USER_NS = y và nơi
overlayfs có cờ FS_USERNS_MOUNT, cho phép gắn kết của overlayfs
bên trong không có đặc quyền gắn kết không gian tên. Đây là cấu hình mặc định của
Ubuntu 12.04, 14.04, 14.10, 15.04

