Hệ thống phát hiện cryptojacking malware
DEMO nhóm thực hiện gồm 2 module: (mô hình paper gồm 4 modules)
- Wasm module auto-collector: 
	Khi người dung sử dụng trình duyệt 
	-> Thu thập tự động WebAssembly (wasm) module từ các trang web này 
	-> Lưu tất cả module đó thành từng file trong các thư mục đã tạo (tự động). 
- Preprocessor: 
	Chuyển đổi từng tệp nhị phân trong folder thành gray-scale image
	-> Sau đó thực hiện normalizes và reshapes thành 1 dạng mà mạng nơ-ron 
	-> Có thể sử dụng làm đầu vào (hình ảnh 4D).

#############################################################

Đầu tiên phải đảm bảo đã cài đặt Nodejs và npm bằng lệnh: 
	sudo apt-get install nodejs npm
Sau đó thực hiện: sudo npm install

##############################################################

Thực hiện thu thập các Wasm module từ một list các trang web (url)
