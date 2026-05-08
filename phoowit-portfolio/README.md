# Phoowit Yaisog — Portfolio

Personal portfolio website for Phoowit (Ace) Yaisog — 3D modeling, animation, and digital art.

**Live:** _add your GitHub Pages URL here after deploy_

---

## Structure

```
.
├── index.html               # หน้าหลัก (single-page app)
├── .nojekyll                # บอก GitHub Pages ไม่ต้องผ่าน Jekyll
├── images/                  # รูปสำหรับ home gallery + about
├── media/
│   ├── mattepaint/          # 7 ผลงาน Mattepaint Series
│   ├── nymmie/              # ภาพ concept + modeling stages
│   └── sister/              # Sister Blonde — sketches, model, wireframe, animation
└── videos/
    └── skaven/              # 7 วิดีโอ rotating turntable
```

---

## Deploy ขึ้น GitHub Pages

### วิธีที่ 1 — ผ่านเว็บ GitHub (ง่ายที่สุด, แนะนำ)

1. ล็อกอิน [github.com](https://github.com) แล้วกด **New repository**
2. ตั้งชื่อ repo (เช่น `portfolio` หรือ `username.github.io` ถ้าอยากได้ URL หลัก)
3. ตั้งเป็น **Public** (Pages ต้องใช้ public ถ้าใช้บัญชีฟรี)
4. ในหน้า repo คลิก **Add file → Upload files** แล้วลากไฟล์ในโฟลเดอร์นี้ทั้งหมดขึ้นไป (รวม `.nojekyll`)
5. Commit
6. ไปที่ **Settings → Pages**
7. ใต้ "Build and deployment" เลือก:
   - Source: **Deploy from a branch**
   - Branch: **main** / folder: **/ (root)** → กด Save
8. รอ 1–2 นาที จะได้ URL `https://USERNAME.github.io/REPO_NAME/`

### วิธีที่ 2 — ผ่าน Git CLI

```bash
# unzip แล้วเข้าโฟลเดอร์
cd portfolio_deploy

git init
git add .
git commit -m "Initial portfolio commit"
git branch -M main
git remote add origin https://github.com/USERNAME/REPO_NAME.git
git push -u origin main
```

จากนั้นทำตามขั้นตอน 6–8 ของวิธีที่ 1

---

## ข้อควรระวัง

- **ขนาดไฟล์รวม ~125 MB** — GitHub มี soft limit ที่ ~1 GB ต่อ repo และเตือนเมื่อไฟล์เดี่ยวเกิน 50 MB ตอนนี้ไม่มีไฟล์เกิน 50 MB แต่ก็เกือบ ๆ — ถ้าจะเพิ่มผลงานอนาคต อาจต้อง compress วิดีโอก่อน
- **ทุก path ใน HTML เป็น relative path** (เช่น `media/sister/ColF.png`) — ใช้งานได้ทันทีบน Pages และเปิด local ก็ได้ ไม่ต้องแก้
- **วิดีโอ MP4 H.264** — รองรับทุกเบราว์เซอร์โมเดิร์น
- **Email link** — `mailto:phoowit.yaisog@gmail.com` คลิกแล้วเปิดแอปเมลของผู้ใช้ทันที

---

## โครงสร้างหน้า

- **Home** — sidebar + grid gallery 4 ภาพหลัก
- **About me** — แนะนำตัว + Skills + Programs + Email
- **Artworks** — กริด 4 ผลงาน (Nymmie WIP, Skavens, Sister Blonde, Mattepaint Series)
- **Project pages** (เปิดเมื่อคลิกการ์ด):
  - Skavens — 7 วิดีโอ turntable
  - Sister Blonde — sketches → final → wireframe → animation
  - Nymmie (WIP) — concept sheet + modeling + base color
  - Mattepaint Series — 7 ผลงาน digital art (เปิด lightbox ได้)

---

Built with vanilla HTML, CSS, JavaScript — ไม่ใช้ framework ใด ๆ
