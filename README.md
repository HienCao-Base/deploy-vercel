# Deploy project với Vercel — Slide hướng dẫn nội bộ

Bộ slide HTML (zero dependency, tự chạy trong browser) hướng dẫn cách deploy một project lên Vercel qua giao diện web — không dùng CLI.

## Xem thử local

Mở trực tiếp file `index.html` bằng browser, hoặc chạy một server tĩnh:

```
npx serve .
```

## Điều hướng slide

- `→` / `Space` / vuốt sang trái: slide tiếp theo
- `←` / vuốt sang phải: slide trước
- Chấm tròn ở thanh điều khiển dưới màn hình: nhảy tới slide bất kỳ

## Chỉnh sửa nội dung trực tiếp trong browser

- Di chuột vào góc trên-trái màn hình hoặc nhấn `E` để vào chế độ edit
- Click vào bất kỳ đoạn text nào để sửa
- `Ctrl/Cmd + S` để lưu (lưu vào localStorage của browser)

## Deploy lên Vercel (qua UI, không cần CLI)

1. Push repo này lên GitHub (xem hướng dẫn push ở dưới).
2. Vào [vercel.com](https://vercel.com) → đăng nhập bằng GitHub.
3. **Add New...** → **Project** → **Import** repo này.
4. Vercel tự nhận diện đây là static site — giữ nguyên cấu hình mặc định, bấm **Deploy**.
5. Sau khi build xong, bạn sẽ có một URL dạng `https://<ten-project>.vercel.app`.

## Push repo này lên GitHub

```bash
git remote add origin <URL-repo-GitHub-cua-ban>
git branch -M main
git push -u origin main
```

Thay `<URL-repo-GitHub-cua-ban>` bằng URL repo bạn vừa tạo trên GitHub (ví dụ: `https://github.com/<username>/vercel-deploy-slides.git`).
