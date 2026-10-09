# 🖐️ Game Kuis Gerakan Tangan (Camera Touch Game)

Game kuis interaktif berbasis browser yang dimainkan menggunakan gestur tangan secara *touchless* melalui webcam. Dibangun menggunakan **MediaPipe Hands** dan **HTML5 Canvas**, pemain dapat memilih jawaban hanya dengan mengarahkan jari telunjuk ke kotak opsi jawaban di layar dan menahannya selama 1,5 detik.

---

## ✨ Fitur Unggulan

- **🖐️ Real-time Hand & Finger Tracking**: Menggunakan model AI MediaPipe Hands berbasis web berlatensi rendah untuk mendeteksi posisi ujung jari telunjuk secara akurat.
- **🎯 Touchless Interaction**: Memilih jawaban dan menekan tombol tanpa menyentuh keyboard atau mouse. Tahan jari selama 1,5 detik dengan animasi indikator progres melingkar.
- **🎨 4 Pilihan Tema Tampilan**:
  - 🌌 *Navy Gelap (Midnight)*
  - ⬛ *Hitam Pekat (OLED)*
  - 🔮 *Violet Mistis (Deep Purple)*
  - 🌲 *Hijau Hutan (Emerald)*
- **🦴 Visualisasi Interaktif**:
  - Tombol toggle untuk menampilkan/menyembunyikan rangka sendi tangan (*Skeleton*).
  - Mode *Mini Camera* (Picture-in-Picture) untuk memantau tampilan asli webcam di sudut layar.
- **🔄 Mulai Ulang / Refresh Seketika**: Mulai ulang kuis kapan saja melalui toolbar kontrol atau tombol Reset di dalam canvas tanpa harus memuat ulang halaman.
- **⚡ Ringan & Mandiri**: Murni menggunakan HTML5, CSS3, dan Vanilla JavaScript tanpa perlu dependensi rumit atau bundler.

---

## 🚀 Cara Menjalankan

### Cara 1: Menggunakan Local Web Server (Direkomendasikan)
Karena fitur webcam dan integrasi MediaPipe membutuhkan konteks aman (*Secure Context* seperti `localhost` atau HTTPS):

```bash
# Opsi A: Menggunakan Python
python3 -m http.server 8000

# Opsi B: Menggunakan npx serve
npx serve .
```

Buka peramban dan akses: `http://localhost:8000` (atau port yang ditampilkan).

### Cara 2: GitHub Pages
Anda dapat mengaktifkan **GitHub Pages** di repositori ini untuk memainkannya secara langsung secara daring:
1. Masuk ke tab **Settings** di repositori GitHub Anda.
2. Pilih menu **Pages** di sisi kiri.
3. Pada bagian **Build and deployment > Branch**, pilih branch `main` dan folder `/ (root)`.
4. Klik **Save**. Game Anda akan langsung aktif di URL GitHub Pages Anda!

---

## 🎮 Cara Bermain

1. **Izinkan Akses Kamera**: Saat browser meminta izin akses webcam, klik **Allow / Izinkan**.
2. **Posisikan Tangan**: Pastikan tangan Anda terlihat jelas di dalam bidang pandang kamera.
3. **Pilih Jawaban**: Arahkan ujung jari telunjuk ke kotak pilihan jawaban (A, B, C, atau D).
4. **Tahan Gestur**: Pertahankan posisi jari pada pilihan tersebut selama **1,5 detik** hingga lingkaran pengisi terisi penuh.
5. **Kumpulkan Skor**: Selesaikan seluruh pertanyaan dan lihat skor akhir Anda!

---

## 🛠️ Teknologi yang Digunakan

- [MediaPipe Hands](https://developers.google.com/mediapipe/solutions/vision/hand_landmarker) via CDN
- HTML5 Canvas 2D Rendering
- CSS3 Modern UI (Dark Theme & Glassmorphism)
- Plus Jakarta Sans Google Fonts

---

## 📄 Lisensi

Dibuat dengan ❤️ oleh [chusni-moklet](https://github.com/chusni-moklet). Bebas digunakan dan dikembangkan untuk keperluan edukasi dan eksplorasi interaksi komputer-manusia (HCI).
