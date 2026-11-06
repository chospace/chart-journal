# Jurnal Chart

Arsip screenshot chart + catatan terstruktur buat referensi setup dan pola yang berulang.

Live: https://chospace.github.io/chart-journal/

## Cara nambah entri

1. Simpan screenshot dengan nama `YYYY-MM-DD-INSTRUMEN-TF-tradeNN.jpg`.
2. Tambahkan satu objek ke array `DATA` di `index.html` (gambar disematkan sebagai data-URI base64, karena push teks tidak bisa membawa file biner utuh).
3. Field per entri: `date`, `date_label`, `instrument`, `tf`, `trade`, `img`, `konteks`, `bacaan`, `hasil`, `whatif`, `pelajaran`, `tags`.

Format catatan mengikuti format jurnal chart yang disepakati (Konteks · Bacaan · Hasil · What-if · Pelajaran · Tag).
