---
layout: post
title: "Belajar Config Yml"
date: 2025-04-24
---


Berikut adalah contoh materi mengenai konfigurasi file `.yml` dalam format **Markdown**, cocok untuk dijadikan bahan pembelajaran atau dokumentasi:

---

# 📘 Panduan Konfigurasi File `.yml`

## Apa itu File YAML?

YAML (YAML Ain't Markup Language) adalah format serialisasi data yang mudah dibaca manusia, sering digunakan untuk file konfigurasi.

---

## 🧱 Struktur Dasar YAML

```yaml
key: value
```

* **Key** = nama properti/parameter
* **Value** = nilai dari properti tersebut
* Menggunakan **indentasi** (spasi, bukan tab) untuk menandai level hierarki

Contoh:

```yaml
server:
  port: 8080
  host: localhost
```

---

## 📁 Contoh Struktur Konfigurasi Aplikasi

```yaml
app:
  name: MyApp
  version: 1.0.0

server:
  port: 3000
  host: 127.0.0.1

database:
  type: mysql
  host: localhost
  port: 3306
  username: root
  password: secret
```

---

## 🔁 List / Array dalam YAML

```yaml
fruits:
  - apple
  - banana
  - orange
```

Bisa juga dalam bentuk inline:

```yaml
fruits: [apple, banana, orange]
```

---

## 🔗 Nested Struktur / Hierarki

```yaml
user:
  name: John Doe
  contact:
    email: john@example.com
    phone: "123-456-7890"
```

---

## ✅ Boolean, Null, dan Number

```yaml
isActive: true
isVerified: false
points: 150
data: null
```

---

## 📌 Tips Penting

* Gunakan **2 spasi** untuk indentasi, **bukan tab**
* File biasanya berekstensi `.yml` atau `.yaml`
* Jangan gunakan tanda kutip kecuali diperlukan
* Format ini sangat sensitif terhadap spasi!

---

## 🛠️ Penggunaan YAML dalam Berbagai Tools

### 1. GitHub Actions (`.github/workflows/ci.yml`)

```yaml
name: CI

on: [push]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - name: Install Dependencies
        run: npm install
```

### 2. Docker Compose (`docker-compose.yml`)

```yaml
version: '3'
services:
  web:
    image: nginx
    ports:
      - "80:80"
```

---

## 📚 Referensi

* [YAML Official Spec](https://yaml.org/spec/)
* [Learn YAML in Y Minutes](https://learnxinyminutes.com/docs/yaml/)

---

Jika kamu ingin materi ini dikembangkan ke dalam format presentasi atau ditambahkan studi kasus spesifik (misalnya Spring Boot, Ansible, dsb), beri tahu saja!
