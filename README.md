# Nutt Theme

เรียบง่าย อ่านง่าย เน้น typography เป็นหลัก

## การติดตั้ง

```bash
# ติดตั้ง dependencies
bundle install

# รัน dev server
bundle exec jekyll serve
```

## โครงสร้างไฟล์

```
.
├── _config.yml          # ตั้งค่าหลัก (แก้ชื่อบล็อก, author ที่นี่)
├── _layouts/
│   ├── default.html     # Layout หลัก (header, footer)
│   ├── post.html        # สำหรับ blog posts
│   └── page.html        # สำหรับ static pages (About ฯลฯ)
├── _posts/              # ← วาง posts ของคุณที่นี่
├── assets/css/
│   └── main.css         # ทุก style อยู่ที่นี่
├── index.html           # หน้าแรก (รายการ posts จัดกลุ่มตามปี)
└── about.md             # หน้า About (แก้ข้อมูลได้เลย)
```

## ตั้งค่า

แก้ `_config.yml`:

```yaml
title: "ชื่อบล็อกของคุณ"
description: "คำอธิบาย"
author: "ชื่อคุณ"
```

## รูปแบบ Front Matter ของ Post

```yaml
---
layout: post
title: "ชื่อบทความ"
date: 2024-01-15
---
```

## Features

- หน้าแรกจัดกลุ่ม posts ตามปี
- ไม่มี JavaScript
- Syntax highlighting ด้วย Rouge
- RSS feed อัตโนมัติ
- Responsive บน mobile
- Next/Prev navigation ใน post
- Tags support
