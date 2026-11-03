# CuddlyNest Research

Trang báo cáo nghiên cứu TikTok, Instagram và workflow AI UGC.

## Deploy lên Vercel

1. Trong Vercel, chọn **Add New → Project**, import repo `Tamnguyen270305/Research`.
2. **Framework Preset:** Other. **Root Directory:** để mặc định (gốc repo).
3. Không cần Build Command hay Install Command. **Output Directory:** `public` (đã có trong `vercel.json`).
4. Chọn **Deploy**.

Không cần biến môi trường hoặc cài dependency. Các lần push lên `main` sẽ tự triển khai lại sau khi repo được kết nối với Vercel.

## Cấu trúc

- `public/index.html`: báo cáo chính, CSS và JavaScript tích hợp.
- `public/assets/ai-ugc/`: 6 ảnh và 2 video demo được báo cáo sử dụng.
- `vercel.json`: cấu hình triển khai trang tĩnh.

## Xem trên máy

```sh
python3 -m http.server 8000 --directory public
```

Mở http://localhost:8000. Sửa `public/index.html` và cập nhật asset tương ứng khi cần thay đổi nội dung.

Tài liệu Vercel: https://vercel.com/docs/builds/configure-a-build
