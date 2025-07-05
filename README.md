# 🔐 ỨNG DỤNG BẢO MẬT TIN NHẮN VĂN BẢN

## 📌 Mô tả
Đây là một ứng dụng bảo mật cho phép người dùng **gửi và nhận tin nhắn văn bản đã mã hoá**. Hệ thống sử dụng:
- **Thuật toán mã hoá DES** để mã hoá nội dung tin nhắn.
- **Thuật toán RSA** để xác thực người gửi và đảm bảo tính toàn vẹn dữ liệu.

Ứng dụng được xây dựng với mục tiêu học tập và nghiên cứu về **an toàn thông tin** và **mật mã học**.

---

## 🔒 Tính năng chính
- ✅ Mã hoá tin nhắn bằng thuật toán **DES**.
- ✅ Xác thực người gửi bằng chữ ký số **RSA**.
- ✅ Giải mã và kiểm tra tính toàn vẹn của tin nhắn nhận được.
- ✅ Giao diện thân thiện, dễ sử dụng (nếu có GUI).
- ✅ Mô phỏng quá trình mã hoá và xác thực để dễ học tập.

---

## 🛠️ Công nghệ sử dụng
- Ngôn ngữ: `Python` hoặc `Java` (tuỳ vào code bạn đang dùng)
- Mã hoá đối xứng: `DES`
- Mã hoá bất đối xứng & xác thực: `RSA`
- Thư viện hỗ trợ (ví dụ): `PyCryptodome`, `tkinter` (nếu có giao diện)

---

## 🚀 Cách sử dụng

```bash
# Bước 1: Clone repo
git clone https://github.com/vuhoan1312312343/Antoanbaomat.git
cd Antoanbaomat

# Bước 2: Cài đặt thư viện (nếu dùng Python)
pip install -r requirements.txt

# Bước 3: Chạy ứng dụng
python app.py
