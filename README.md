# RM Quality Dashboard

Dashboard monitoring & retensi debitur untuk RM Quality BRI.

## Fitur
- Upload data Excel LW321 (Laporan Kolektibilitas & Tunggakan Per AO)
- Monitoring debitur SML 1, SML 2, SML 3, dan NPL
- Analisis per wilayah / kantor cabang
- Analisis per RM Pengelola
- Monitoring risiko pergeseran kolektibilitas
- Generate priority list (index gabungan OS + umur tunggakan)
- Input laporan kunjungan (komitmen / restruk / paksa bayar)
- Laporan EOD dengan export Excel & print

## Deploy

### Vercel (Recommended)
1. Push repository ini ke GitHub
2. Buka [vercel.com](https://vercel.com) → Import Project → pilih repo ini
3. Klik Deploy — selesai, tidak perlu konfigurasi tambahan

### Manual
Cukup buka `index.html` di browser — tidak perlu server.

## Penggunaan
1. Buka aplikasi
2. Upload file Excel **LW321** dari sistem BRI (format `.xlsx`)
3. Dashboard otomatis memproses dan menampilkan analisa
4. Navigasi antar tab sesuai kebutuhan

## Struktur File
```
/
├── index.html      # Aplikasi utama (single file)
├── vercel.json     # Konfigurasi deploy Vercel
├── .gitignore
└── README.md
```

## Format Excel yang Didukung
File LW321 — Laporan Kolektibilitas dan Tunggakan Per AO  
Kolom yang digunakan: `NAMA_DEBITUR`, `NOMOR_REKENING`, `NEXT_PMT_DATE`, `BALANCE DALAM IDR`, `PLAFON`, `TUNGGAKAN POKOK/BUNGA/PINALTI`, `PN PENGELOLA`, `KOL_ADK`, `DESCRIPTION`, dll.
