# 🚀 Setup Remote Repository - Quick Guide

## ⚡ Langkah Cepat

### **1. Dapatkan Link Repository Teman**
Minta teman kelompok untuk memberikan link repository GitHub mereka, contoh:
```
https://github.com/username-teman/insightmind-project.git
```

### **2. Setup Remote (Pilih salah satu)**

#### **Opsi A: Ganti Remote yang Ada**
```bash
git remote set-url origin https://github.com/username-teman/repo-name.git
```

#### **Opsi B: Tambahkan Remote Baru**
```bash
git remote add origin https://github.com/username-teman/repo-name.git
```

### **3. Verifikasi**
```bash
git remote -v
```

### **4. Pull Perubahan dari Teman (PENTING!)**
```bash
# Pull dulu sebelum push
git pull origin main --allow-unrelated-histories

# Atau jika branch-nya master:
git pull origin master --allow-unrelated-histories
```

### **5. Push Perubahan Anda**
```bash
git push -u origin main
```

---

## 📝 Contoh Lengkap

```bash
# 1. Setup remote
git remote add origin https://github.com/teman-kelompok/insightmind.git

# 2. Cek remote
git remote -v

# 3. Pull dari teman
git pull origin main --allow-unrelated-histories

# 4. Push perubahan Anda
git push -u origin main
```

---

## ⚠️ Jika Ada Error

### Error: "refusing to merge unrelated histories"
**Solusi:** Tambahkan flag `--allow-unrelated-histories`
```bash
git pull origin main --allow-unrelated-histories
```

### Error: "failed to push some refs"
**Solusi:** Pull dulu, lalu push
```bash
git pull origin main --rebase
git push origin main
```

---

## ✅ Checklist

- [ ] Dapatkan link repository teman
- [ ] Setup remote repository
- [ ] Pull perubahan dari teman
- [ ] Push perubahan Anda
- [ ] Verifikasi di GitHub

---

**Selanjutnya:** Lihat `PANDUAN_GIT_COLLABORATION.md` untuk workflow lengkap!
