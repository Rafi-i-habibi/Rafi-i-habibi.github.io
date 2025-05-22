---
layout: post
title: "Belajar Mengenal dan Menggunakan Plugins di jekyll"
date: 2025-04-24
---

Berikut adalah **materi pembelajaran SCSS dan SASS** dalam format **Markdown**, cocok untuk dokumentasi atau bahan belajar.

---

# 🎨 Belajar SCSS dan SASS

## 🧾 Apa itu SASS & SCSS?

SASS (Syntactically Awesome Stylesheets) adalah **preprocessor CSS** yang menambahkan fitur seperti **variabel**, **nesting**, **mixin**, dan lainnya agar penulisan CSS lebih efisien.

SASS memiliki dua sintaks:

| Sintaks  | Ekstensi | Gaya Penulisan                                  |
| -------- | -------- | ----------------------------------------------- |
| **SASS** | `.sass`  | Tanpa kurung kurawal `{}`, tanpa titik koma `;` |
| **SCSS** | `.scss`  | Mirip CSS biasa, menggunakan `{}` dan `;`       |

> 💡 SCSS lebih populer karena kompatibel penuh dengan CSS.

---

## 🚀 Keunggulan SASS/SCSS

* Variabel
* Nesting (penulisan bertingkat)
* Mixin (fungsi reusable)
* Inheritance (`@extend`)
* Modularisasi (`@import` / `@use`)
* Fungsi dan operasi

---

## 🔧 Instalasi SASS

### 1. Instal via npm (Node.js)

```bash
npm install -g sass
```

### 2. Compile SCSS ke CSS

```bash
sass style.scss style.css
```

---

## 🧪 Fitur-Fitur Utama

### 1. 🎯 Variabel

```scss
$primary-color: #3498db;
$padding: 10px;

.button {
  background-color: $primary-color;
  padding: $padding;
}
```

---

### 2. 📚 Nesting (Penulisan Bertingkat)

```scss
nav {
  ul {
    li {
      a {
        color: blue;
      }
    }
  }
}
```

---

### 3. 📦 Mixin

```scss
@mixin flex-center {
  display: flex;
  justify-content: center;
  align-items: center;
}

.box {
  @include flex-center;
}
```

---

### 4. 📜 Extend (Inheritance)

```scss
%btn-base {
  padding: 10px 20px;
  border-radius: 5px;
}

.button {
  @extend %btn-base;
  background: blue;
}
```

---

### 5. 🧩 Import & Modularisasi

#### SCSS Lama:

```scss
@import 'variables';
@import 'header';
```

#### SCSS Modern (`@use` dan `@forward`):

```scss
// _variables.scss
$font-stack: Helvetica, sans-serif;
$primary-color: #333;

// style.scss
@use 'variables';

body {
  font-family: variables.$font-stack;
}
```

---

## 📐 Fungsi & Operasi

```scss
$base: 10px;

.box {
  margin: $base * 2;
  width: percentage(0.5); // 50%
}
```

---

## 🔄 Auto-Compile SCSS

```bash
sass --watch scss:css
```

Akan memantau folder `scss/` dan meng-compile ke `css/`.

---

## 📚 Referensi

* [SASS Resmi](https://sass-lang.com/)
* [SCSS Cheat Sheet](https://devhints.io/sass)
* [Playground Online](https://sassmeister.com/)

---

## 🧠 Tips

* Gunakan **SCSS** jika ingin transisi mulus dari CSS
* Organisasikan file dengan struktur modular (`_variables.scss`, `_mixins.scss`, dsb)
* Gunakan tools seperti **Dart Sass**, **Webpack**, atau **Vite** untuk integrasi dengan proyek besar

---

Jika kamu butuh **template struktur SCSS proyek** atau contoh penggunaan dengan **framework** seperti Bootstrap atau Tailwind, saya bisa bantu juga.
