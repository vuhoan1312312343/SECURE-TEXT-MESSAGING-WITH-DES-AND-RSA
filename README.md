# 🔐 ỨNG DỤNG BẢO MẬT TIN NHẮN VĂN BẢN VỚI DES VÀ RSA

## 📌 Giới thiệu

Đây là một ứng dụng bảo mật tin nhắn thời gian thực, sử dụng sự kết hợp giữa ba kỹ thuật:
- **DES (Data Encryption Standard)**: Mã hoá nội dung tin nhắn.
- **RSA (Rivest–Shamir–Adleman)**: Xác thực danh tính và bảo vệ khóa DES.
- **SHA-256**: Kiểm tra tính toàn vẹn của dữ liệu.

Hệ thống mô phỏng cách thức mã hoá, xác thực và truyền tin an toàn trong môi trường mạng, phù hợp với các tình huống như:
- Nhắn tin nội bộ trong doanh nghiệp
- Giao tiếp cá nhân
- Giao dịch tài chính cần xác thực

---

## 🎯 Mục tiêu và lý do chọn đề tài

- Xây dựng ứng dụng bảo mật tin nhắn đơn giản, trực quan.
- Minh họa rõ cách kết hợp giữa mã hoá đối xứng và bất đối xứng.
- Hướng đến học tập và hiểu sâu về an toàn thông tin.
- Giải quyết vấn đề nghe lén, giả mạo, chỉnh sửa nội dung khi truyền tin.

---

## ⚙️ Công nghệ sử dụng

| Thành phần | Công nghệ |
|------------|-----------|
| Frontend   | Vue.js |
| Backend    | Node.js, Socket.IO |
| Mã hóa     | JSEncrypt (RSA), Crypto-js (DES) |
| Kiểm tra toàn vẹn | SHA-256 |

---

## 🔄 Luồng xử lý chính

1. **Trao đổi khoá RSA** qua kết nối `Socket.IO` (peer-to-peer).
2. **Sinh khoá DES**, mã hoá bằng RSA, gửi kèm IV.
3. **Mã hoá tin nhắn bằng DES**, ký số bằng RSA/SHA-256.
4. Người nhận **giải mã khoá**, xác minh chữ ký và kiểm tra SHA-256.

---

## 🚀 Hướng dẫn chạy dự án

### ✅ Cài đặt

```bash
git clone https://github.com/vuhoan1312312343/Antoanbaomat.git
cd Antoanbaomat

# Cài đặt thư viện backend
cd server
npm install

# Cài đặt thư viện frontend
cd ../client
npm install
