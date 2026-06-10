# 🌸 Evelyn Hartwell — Healing Books Website

Website quảng bá sách KDP chữa lành trên Amazon.

---

## 📁 Cấu trúc file

```
/
├── index.html          ← Trang web chính
├── books.json          ← Danh sách tất cả sách (CẬP NHẬT FILE NÀY)
├── covers/             ← Thư mục ảnh bìa sách
│   ├── book-01.jpg
│   ├── book-02.jpg
│   └── ...
└── README.md
```

---

## 🚀 Cài đặt trên GitHub Pages (miễn phí)

### Bước 1 — Tạo repository GitHub
1. Vào [github.com](https://github.com) → đăng nhập
2. Nhấn **New repository**
3. Đặt tên: `evelyn-hartwell-books` (hoặc tên bạn thích)
4. Chọn **Public**
5. Nhấn **Create repository**

### Bước 2 — Upload files
1. Kéo thả toàn bộ file vào repository
2. Hoặc dùng GitHub Desktop nếu có nhiều ảnh bìa

### Bước 3 — Bật GitHub Pages
1. Vào **Settings** → **Pages**
2. Source: chọn **Deploy from a branch**
3. Branch: `main` → Folder: `/ (root)`
4. Nhấn **Save**
5. Sau 1-2 phút, website live tại: `https://TÊN_BẠN.github.io/evelyn-hartwell-books`

---

## ✏️ Cách cập nhật sách mới

Chỉ cần **chỉnh sửa file `books.json`** — thêm sách mới vào đầu mảng:

```json
{
  "id": 7,
  "title": "Tên cuốn sách mới",
  "description": "Mô tả ngắn về cuốn sách, khoảng 1-2 câu.",
  "category": "Self-Compassion",
  "amazonUrl": "https://www.amazon.com/dp/ASIN_CỦA_BẠN?tag=TAG_AFFILIATE",
  "coverImage": "covers/book-07.jpg",
  "badge": "New",
  "price": "$4.99"
}
```

### Các category có thể dùng:
- `Self-Compassion`
- `Grief & Loss`
- `Inner Child`
- `Anxiety`
- `Mindfulness`
- `Relationships`
- `Boundaries`
- `Trauma Healing`
- Hoặc tự tạo category mới!

### Badge options:
- `"New"` — hiện nhãn New màu vàng
- `"Bestseller"` — hiện nhãn Bestseller
- `""` — không có nhãn

---

## 🖼️ Cách thêm ảnh bìa

1. Đặt ảnh bìa vào thư mục `covers/`
2. Tên file: `book-01.jpg`, `book-02.jpg`, ...
3. Kích thước khuyến nghị: **400 × 600px** (tỉ lệ 2:3)
4. Nếu **không có ảnh**, xóa trường `coverImage` hoặc để `""` — website sẽ tự tạo placeholder đẹp

---

## 🔗 Affiliate Link

Thay `YOUR_AFFILIATE_TAG` trong `books.json` bằng Amazon Associates tag của bạn:

```
https://www.amazon.com/dp/B0XXXXXXXX?tag=yourname-20
```

---

## 🎨 Tùy chỉnh website

Mở `index.html` và tìm phần `<style>` để thay đổi màu sắc:

```css
--rose-deep: #c4878f;    /* Màu chính (hồng đậm) */
--text-dark: #3a3038;    /* Màu chữ tối */
--gold: #c8a96e;         /* Màu vàng gold */
```

---

## 📊 Tích hợp Google Ads

Thêm đoạn code này vào `<head>` của `index.html` (lấy từ Google Ads của bạn):

```html
<script async src="https://www.googletagmanager.com/gtag/js?id=AW-XXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'AW-XXXXXXXXX');
</script>
```

---

## 💡 Mẹo dùng link cho Google Ads

URL landing page nên là:
- Trang chủ: `https://yourname.github.io/evelyn-hartwell-books/`
- Lọc theo category: `https://yourname.github.io/evelyn-hartwell-books/#books`

---

*Made with 💕 for healing journeys everywhere.*
