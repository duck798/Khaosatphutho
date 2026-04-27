# 📊 Tra Cứu Kết Quả Khảo Sát – Sở GD&ĐT Phú Thọ

Website tĩnh tra cứu và phân tích kết quả khảo sát chất lượng học sinh lớp 12 của **THPT Hưng Hóa** và **THPT Tam Nông**, năm học 2025–2026.

## 🌐 Truy cập website

> Sau khi deploy lên GitHub Pages:  
> `https://<username>.github.io/<repo-name>/`

---

## 📁 Cấu trúc thư mục

```
/
├── index.html          ← Giao diện chính
└── data/
    ├── hunghoa.js      ← Dữ liệu THPT Hưng Hóa (Sở đợt 1 + Trường + Sở đợt 2)
    └── tamnong.js      ← Dữ liệu THPT Tam Nông (cần cập nhật)
```

---

## 🚀 Hướng dẫn đưa lên GitHub Pages

### Bước 1 – Tạo repository
1. Đăng nhập [github.com](https://github.com)
2. Nhấn **New repository** → đặt tên, ví dụ: `khaosat-phu-tho`
3. Chọn **Public** → **Create repository**

### Bước 2 – Upload toàn bộ file
1. Trong repository vừa tạo, nhấn **Add file → Upload files**
2. Kéo thả toàn bộ thư mục `website/` (gồm `index.html` và folder `data/`)
3. Nhấn **Commit changes**

### Bước 3 – Bật GitHub Pages
1. Vào **Settings** → **Pages** (cột trái)
2. Phần **Source**: chọn `Deploy from a branch`
3. **Branch**: chọn `main` · **Folder**: `/ (root)`
4. Nhấn **Save**
5. Sau 1–2 phút, website sẽ sống tại địa chỉ hiển thị trên trang đó

---

## ➕ Thêm dữ liệu THPT Tam Nông

Mở file `data/tamnong.js` và thêm dữ liệu theo mẫu:

```javascript
var TAMNONG_DATA = [
  {
    "name": "Nguyễn Văn A",
    "dob": "15/06/2008",
    "class": "12A1",
    "so1": {},        // để trống nếu không có
    "truong": {},     // để trống nếu không có
    "so2": {
      "Toán": 7.5,
      "Ngữ văn": 6.25,
      "Lịch sử": 8.0,
      "GD KT&PL": 7.75
    }
  },
  // ... thêm học sinh tiếp theo
];
```

**Tên các môn hợp lệ:**  
`Toán`, `Ngữ văn`, `Vật lí`, `Hóa học`, `Sinh học`, `Lịch sử`, `Địa lí`, `GD KT&PL`, `Tiếng Anh`, `Tin học`

---

## ✨ Tính năng

| Tính năng | Mô tả |
|---|---|
| 🔍 Tra cứu thông minh | Tìm kiếm theo tên + ngày sinh để tránh nhầm lẫn |
| 🏫 Chọn trường | Tách biệt dữ liệu HH và Tam Nông |
| 📋 Điểm theo đợt | Hiển thị đúng môn học sinh đã thi từng kỳ |
| 📊 Bảng so sánh | Xem tăng/giảm điểm giữa các đợt khảo sát |
| 📈 Biểu đồ radar | Trực quan hóa điểm số 3 kỳ |
| 🧮 Tổ hợp môn | Tính và xếp hạng tổ hợp phù hợp |
| 🏛️ Gợi ý ĐH | 10–12 trường đại học phù hợp với mức điểm |
| 📝 Nhận xét AI | Phân tích xu hướng học tập tự động |

---

## 📞 Liên hệ

Sở Giáo dục và Đào tạo Phú Thọ · Năm học 2025–2026
