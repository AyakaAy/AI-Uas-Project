# AI-Uas-Project
Project UAS Mata Kuliah Artificial Intelligence


---

## 👥 Team

| Nama | NIM | Role |
| ---- | --- | ---- |
| Ida Bagus Oka Wedhana   | 2501010331   | -    |
| I Komang Mahistha Widia    | -   | -    |
| I Made Ian Sanjaya    | -   | -    |
| Mahardika Wijaya    | -   | -    |

---

## 📌 Project Overview

> Akan diisi setelah topik proyek ditentukan.

---

## 🎯 Problem

> Akan diisi setelah masalah yang ingin diselesaikan ditentukan.

---

## 💡 Proposed Solution

> Akan diisi setelah konsep proyek ditentukan.

---

## 🧠 AI / ML Approach

- Python
- Generative AI (GenAI)
- Machine Learning: TBD
- Approach: TBD

---

## 📊 Dataset

- Source: Kaggle
- Dataset: TBD
- Preprocessing: TBD

---

## 🛠️ Tech Stack

- **Language:** Python
- **AI / ML:** TBD
- **Backend:** TBD
- **Frontend:** TBD
- **Database:** TBD

---

## 📁 Project Structure

> Akan diperbarui setelah struktur proyek ditentukan.

---

## 🚀 Development Status

- [x] Repository dibuat
- [ ] Menentukan ide proyek
- [ ] Menentukan dataset
- [ ] Data preprocessing
- [ ] Model / AI development
- [ ] Backend
- [ ] Frontend
- [ ] Integrasi sistem
- [ ] Testing
- [ ] Final documentation
- [ ] Final release

---

# 🔀 Git Workflow

Repository ini menggunakan **Git dan GitHub** untuk version control dan kolaborasi tim.

## 🌳 Branch Structure

Branch utama yang digunakan:

```text
main
  │
  └── develop
        │
        ├── feature/...
        ├── feature/...
        └── feature/...
```

### `main`

Digunakan untuk versi proyek yang sudah stabil dan siap digunakan/dipresentasikan.

> **Jangan melakukan development langsung di `main`.**

### `develop`

Digunakan sebagai branch utama untuk menggabungkan fitur-fitur yang sedang dikembangkan.

> Anggota tim juga tidak melakukan development langsung di `develop`.

### `feature/*`

Setiap anggota membuat branch sendiri berdasarkan fitur atau pekerjaan yang sedang dikerjakan.

Contoh:

```text
feature/ml
feature/genai
feature/backend
feature/frontend
```

---

## 🔄 Development Workflow

Setiap anggota mengikuti alur berikut:

```text
develop
   ↓
Create Feature Branch
   ↓
Coding
   ↓
Commit
   ↓
Push
   ↓
Pull Request
   ↓
Code Review
   ↓
Merge → develop
   ↓
Testing
   ↓
Merge → main
```

---

## 1. Clone Repository

Jika belum memiliki repository di komputer:

```bash
git clone <repository-url>
cd AI-Uas-Project
```

Contoh:

```bash
git clone https://github.com/AyakaAy/AI-Uas-Project.git
cd AI-Uas-Project
```

---

## 2. Pastikan Branch Terbaru

Sebelum mulai bekerja, pindah ke `develop`:

```bash
git switch develop
```

Kemudian ambil perubahan terbaru:

```bash
git pull origin develop
```

> Biasakan melakukan `git pull` sebelum membuat branch baru agar pekerjaan dimulai dari versi terbaru.

---

## 3. Membuat Feature Branch

Buat branch baru berdasarkan pekerjaan yang akan dilakukan:

```bash
git switch -c feature/nama-fitur
```

Contoh:

```bash
git switch -c feature/ml
```

atau:

```bash
git switch -c feature/backend
```

### Contoh penamaan branch

| Branch             | Kegunaan              |
| ------------------ | --------------------- |
| `feature/ml`       | Machine Learning      |
| `feature/genai`    | Generative AI         |
| `feature/backend`  | Backend               |
| `feature/frontend` | Frontend              |
| `feature/database` | Database              |
| `fix/login-error`  | Memperbaiki bug login |

Gunakan nama branch yang singkat dan menggambarkan pekerjaan.

---

## 4. Mengecek Status

Untuk melihat perubahan yang dilakukan:

```bash
git status
```

Contoh:

```text
On branch feature/ml
Changes not staged for commit:
  modified: model.py
```

---

## 5. Menambahkan Perubahan

Setelah pekerjaan selesai atau mencapai bagian yang layak di-commit:

```bash
git add .
```

Kemudian cek kembali:

```bash
git status
```

---

## 6. Membuat Commit

Simpan perubahan menggunakan commit:

```bash
git commit -m "feat: add data preprocessing"
```

Contoh commit lainnya:

```bash
git commit -m "feat: add ML model"
git commit -m "feat: add GenAI integration"
git commit -m "fix: resolve API error"
git commit -m "docs: update README"
```

### Format commit

Gunakan format sederhana:

```text
type: description
```

Beberapa `type` yang digunakan:

| Type       | Kegunaan                                    |
| ---------- | ------------------------------------------- |
| `feat`     | Menambahkan fitur                           |
| `fix`      | Memperbaiki bug                             |
| `docs`     | Dokumentasi                                 |
| `refactor` | Mengubah struktur kode tanpa menambah fitur |
| `test`     | Menambahkan atau memperbaiki testing        |
| `chore`    | Perubahan konfigurasi atau maintenance      |

Contoh:

```bash
git commit -m "feat: add student productivity prediction"
```

---

## 7. Push ke GitHub

Push branch ke repository:

```bash
git push -u origin feature/nama-fitur
```

Contoh:

```bash
git push -u origin feature/ml
```

Setelah push pertama, biasanya cukup:

```bash
git push
```

---

# 🔀 Pull Request

Setelah pekerjaan pada feature branch selesai, buat **Pull Request (PR)** melalui GitHub.

### Tujuan Pull Request

Pull Request digunakan agar perubahan dapat diperiksa sebelum digabungkan ke branch `develop`.

### Alur Pull Request

1. Push feature branch ke GitHub.
2. Buka repository di GitHub.
3. Pilih **Compare & pull request**.
4. Pastikan:
   - **Base:** `develop`
   - **Compare:** branch yang dikerjakan
5. Tulis judul dan deskripsi perubahan.
6. Minta anggota lain melakukan review.
7. Perbaiki jika terdapat feedback.
8. Setelah disetujui, merge ke `develop`.

Contoh:

```text
base: develop
        ↑
compare: feature/ml
```

> **Jangan langsung membuat Pull Request ke `main` untuk pekerjaan biasa.**

---

# 🔍 Code Review

Sebelum Pull Request di-merge, minimal satu anggota lain melakukan review.

Hal yang perlu diperiksa:

- Apakah kode berjalan?
- Apakah perubahan sesuai dengan tugas?
- Apakah ada bug yang terlihat?
- Apakah ada file yang tidak seharusnya ikut di-commit?
- Apakah kode dapat dipahami oleh anggota lain?
- Apakah perubahan merusak fitur yang sudah ada?

Setelah review selesai dan perubahan dianggap aman, Pull Request dapat di-merge ke `develop`.

---

# 🧪 Testing

Setelah beberapa fitur digabungkan ke `develop`, lakukan testing terhadap sistem.

Jika ditemukan masalah:

```text
develop
   ↓
buat branch fix/...
   ↓
perbaikan
   ↓
Pull Request
   ↓
develop
```

Contoh:

```bash
git switch develop
git pull origin develop
git switch -c fix/api-error
```

---

# 🚀 Release ke Main

Branch `main` digunakan untuk versi proyek yang sudah stabil.

Alur:

```text
feature/*
    ↓
 develop
    ↓
 testing
    ↓
   main
```

Setelah sistem dianggap stabil dan siap digunakan/presentasi, perubahan dari `develop` dapat di-merge ke `main`.

---

# 📖 Git Quick Reference

| Command                       | Fungsi                                     |
| ----------------------------- | ------------------------------------------ |
| `git status`                  | Melihat status perubahan                   |
| `git switch develop`          | Pindah ke branch `develop`                 |
| `git pull origin develop`     | Mengambil perubahan terbaru dari `develop` |
| `git switch -c <branch>`      | Membuat dan berpindah ke branch baru       |
| `git add .`                   | Menyiapkan semua perubahan untuk commit    |
| `git commit -m "..."`         | Membuat commit                             |
| `git push -u origin <branch>` | Push branch pertama kali                   |
| `git push`                    | Mengirim commit ke GitHub                  |
| `git log --oneline`           | Melihat riwayat commit                     |
| `git branch`                  | Melihat branch lokal                       |
| `git switch <branch>`         | Berpindah branch                           |

---

# ⚠️ Important Rules

1. **Jangan melakukan development langsung di `main`.**
2. **Jangan melakukan development langsung di `develop`.**
3. Setiap fitur dikerjakan pada `feature/*`.
4. Selalu lakukan `git pull origin develop` sebelum membuat feature branch baru.
5. Buat commit secara berkala dengan pesan yang jelas.
6. Jangan melakukan `git add .` secara sembarangan tanpa mengecek `git status`.
7. Jangan commit file yang berisi password, API key, token, atau informasi sensitif.
8. Gunakan `.gitignore` untuk file yang tidak perlu masuk repository.
9. Pull Request harus ditujukan ke `develop`, bukan `main`.
10. Lakukan review sebelum merge.
11. Pastikan aplikasi tetap dapat dijalankan setelah perubahan digabungkan.
12. Jika terjadi konflik Git, **jangan langsung menghapus perubahan anggota lain**. Diskusikan dan selesaikan konfliknya terlebih dahulu.

---

# 📄 Documentation

Dokumentasi pengembangan proyek akan ditempatkan di folder `docs/`.

Dokumentasi dapat mencakup:

- Project planning
- Dataset
- Data preprocessing
- Model / AI methodology
- System architecture
- Testing
- Development notes

Dokumentasi akan diperbarui seiring perkembangan proyek.

---

# 📌 Project Status

> 🚧 **Early Development**

Project masih berada pada tahap perencanaan dan pengumpulan ide.
