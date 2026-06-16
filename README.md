# Dashboard Polarisasi Opini Publik

Dashboard interaktif untuk memvisualisasikan polarisasi opini publik di media sosial X menggunakan **Signed Directed Graph** dan **Dual-Vector Signed PageRank**.

Proyek ini adalah bagian dari tugas akhir mata kuliah Teori Graf.

## Cara Penggunaan

Buka website dan klik salah satu tombol skenario di bagian atas:

- **Skenario 1 — Judi Online / Komdigi**
- **Skenario 2 — RUU TNI / RUU Polri**
- **Skenario 3 — IKN (Ibu Kota Nusantara)** *(Fokus Utama)*

Anda juga dapat mengunggah file JSON graf kustom menggunakan tombol **"Unggah JSON Kustom"**.

## Fitur Utama

- Visualisasi jaringan interaktif berbasis *Force Atlas 2*
- Kalkulasi *Dual-Vector Signed PageRank* (G+ dan G-)
- Peringkat aktor: *Opinion Leaders*, *Controversy Hubs*, *Polarizing Influencers*
- Metrik *Balance Index* (Teori Keseimbangan Heider)
- Pencarian aktor berdasarkan username
- Panel detail per node (degree, PageRank, daftar interaksi)

## Struktur Folder

```
.
├── index.html        ← Dashboard utama
└── data/
    ├── graf_ikn.json       ← Skenario 3: IKN
    ├── graf_kontra.json    ← Skenario 1: Judi Online / Komdigi
    └── graf_pro.json       ← Skenario 2: RUU TNI / RUU Polri
```

## Deploy ke GitHub Pages

1. Buat repository baru di GitHub.
2. Push semua isi folder ini ke branch `main`.
3. Pergi ke **Settings > Pages > Branch: main > Save**.
4. Akses dashboard di: `https://username.github.io/nama-repo`

## Teknologi

- [vis-network](https://visjs.github.io/vis-network/docs/network/) — Rendering graf interaktif
- [TailwindCSS](https://tailwindcss.com/) — Styling
- Semua kalkulasi algoritma berjalan sepenuhnya di sisi klien (*client-side JavaScript*)
