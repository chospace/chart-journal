# Jurnal Chart

Arsip screenshot chart + catatan terstruktur buat referensi setup dan pola yang berulang.

Live: https://chospace.github.io/chart-journal/

## Cara nambah entri

1. Simpan screenshot dengan nama `YYYY-MM-DD-INSTRUMEN-TF-tradeNN.jpg`.
2. Tambahkan satu objek ke array `DATA` di `index.html` (gambar disematkan sebagai data-URI base64, karena push teks tidak bisa membawa file biner utuh).
3. Field per entri: `date`, `date_label`, `instrument`, `tf`, `trade`, `kind` (`trade` = review trade, `pola` = arsip pola referensi), `img`, `img2` (opsional, chart konteks TF besar), `konteks`, `bigpic` (opsional, gambaran besar dari chart konteks), `bacaan`, `hasil`, `whatif`, `pelajaran`, `tags`.

## UX halaman (v2)

- Menu atas: tautan ke Jurnal Trading, 100 Challenge, Briefspace, Blog.
- Statistik ringkas (total entri / review trade / arsip pola) + filter Jenis, Instrumen, Tag, dan pencarian teks.
- Kartu ringkas (gambar rasio asli tanpa crop, konteks, pelajaran); klik kartu membuka panel detail berisi semua field + kedua chart ukuran penuh, dengan navigasi entri sebelumnya/berikutnya (tombol atau panah keyboard).
- Sumber template halaman: `template-v2.html` (placeholder `/*__DATA__*/` diisi array DATA saat build).

Format catatan mengikuti format jurnal chart yang disepakati (Konteks · Bacaan · Hasil · What-if · Pelajaran · Tag).
