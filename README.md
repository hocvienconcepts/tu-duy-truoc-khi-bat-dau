# Playbook 00 — Tư duy trước khi bắt đầu

**Học viện Concepts (VCS)**  
Trang tĩnh deploy lên Cloudflare Pages qua GitHub.

## Cấu trúc repo

```
/
├── index.html    ← Playbook 00 (trang chủ Cloudflare Pages)
├── README.md     ← File này
└── .gitignore
```

## Hướng dẫn deploy lên Cloudflare Pages (qua GitHub Web)

### Bước 1 — Tạo repo GitHub
1. Vào [github.com/new](https://github.com/new)
2. Đặt tên repo, ví dụ: `tu-duy-truoc-khi-bat-dau`
3. Để **Public**, chọn **Create repository**

### Bước 2 — Upload file qua giao diện web
1. Trong repo mới, click **"uploading an existing file"** (hoặc **Add file → Upload files**)
2. Kéo thả 3 file: `index.html`, `README.md`, `.gitignore` vào vùng upload
3. Nhập commit message: `Initial deploy — Playbook 00`
4. Click **"Commit changes"**

### Bước 3 — Kết nối Cloudflare Pages
1. Vào [dash.cloudflare.com](https://dash.cloudflare.com) → **Pages** → **Create a project**
2. Chọn **Connect to Git** → Authorize GitHub → Chọn repo vừa tạo
3. Cấu hình build:
   - **Framework preset:** `None`
   - **Build command:** _(để trống)_
   - **Build output directory:** `/` (hoặc để trống)
4. Click **Save and Deploy**

### Bước 4 — Đặt tên miền tùy chỉnh (nếu muốn)
- Cloudflare Pages tự tạo domain dạng: `ten-repo.pages.dev`
- Nếu muốn custom subdomain như `tu-duy-truoc-khi-bat-dau.pages.dev`:  
  Vào **Settings → Custom domains**

---

*Cập nhật lần cuối: 2026-08-01 · VCS info@vcs.edu.vn*
