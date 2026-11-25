Saya masih membaca bagian tengah materi slide (slide 7-10) sebelum memberi rekomendasi.

Setelah membaca kedua dokumen, arah materi slide Anda sudah tepat. Slide 5-13 sudah mengambil bagian rancangan yang berorientasi penjadwalan (bagian 9, 10, 10.1, 11, 11.1, 14, dan 15). Angka-angkanya juga konsisten dengan rancangan: 256 jam-orang, 7 paket WBS, 8 minggu, dan M5 sebagai minggu terpadat. Dependensi T01-T32 juga sudah saya periksa. Semuanya berpola selesai-lalu-mulai pada tingkat mingguan, dan tidak ada pendahulu yang jatuh di minggu yang sama kecuali T32 setelah T31.

## Yang sebaiknya ditambahkan

1. **Beban per anggota (slide 11).** Tabel 10.1 di rancangan memuat kolom A, B, C, D per minggu, tetapi slide hanya menampilkan total. Kolom per anggota menunjukkan alokasi sumber daya, dan alasan M5 berisiko (B, C, D penuh 10 jam) jadi terlihat langsung.
2. **Penanda milestone ◆ pada Gantt (slide 10).** Gantt di rancangan bagian 11 sudah memuat milestone, sedangkan slide 10 dan 12 terpisah. Menggabungkannya membuat Gantt dan milestone terbaca sebagai satu rencana.
3. **Diagram rantai ketergantungan utama (menggantikan tabel lima baris di slide 9).** Rantai ini ada di bagian 11.2: T03 dan T12 → T16 → T19 dan T20 (paralel) → T21 → T25 → T31 → T32. Diagram lebih meyakinkan daripada tabel, asalkan diberi label "rantai yang dipantau", bukan "jalur kritis". Rancangan memang belum menghitung CPM.
4. **Kolom "aktivitas terkait" pada slide 3.** Bagian 12 rancangan memetakan kelompok fitur ke aktivitas, misalnya pembayaran ke T16, T18, dan T19. Dengan kolom ini slide fitur langsung terhubung ke jadwal.
5. **Tabel lengkap T01-T32 dan pemetaan FR→T sebagai lampiran.** Cukup disiapkan untuk tanya jawab, tidak perlu masuk slide utama.

## Yang sebaiknya dikurangi atau tidak ditampilkan

- **Slide 2-4 (fitur dan aturan):** Padatkan jadi dua slide. Pada slide 4, cukup dua aturan yang berdampak ke jadwal, yaitu pembatalan yang memicu pengembalian dana dan syarat omzet.
- **Slide 14:** Boleh digabung ke slide 13 atau dipersingkat. Cukup pertahankan baris luaran tugas.
- **Bagian rancangan yang tidak perlu tampil:** bagian 2 (pemeriksaan konsistensi), 3.3, 6 (rincian status), 7, 8 (NFR), 13 (U-01 sampai U-17), dan 18 (referensi). Simpan untuk tanya jawab.

## Usulan struktur akhir (12 slide)

1. Judul
2. Kebutuhan, batas proyek, dan dua aturan utama
3. Kelompok fitur beserta aktivitas terkait
4. Dasar penyusunan jadwal
5. Tim, kapasitas, dan estimasi effort (gabungan slide 6 dan 7)
6. WBS dan alokasi effort
7. Ketergantungan (diagram rantai utama)
8. Gantt dengan milestone ◆
9. Beban kerja per anggota per minggu
10. Milestone dan kriteria pencapaian
11. Risiko dan pemantauan jadwal
12. Kriteria keberhasilan dan luaran tugas

Lampiran: tabel T01-T32 dan pemetaan kebutuhan ke aktivitas.

## Perbaikan kecil

- Bagian "Sumber materi" dan paragraf pembuka di materi slide menautkan ke path lokal (`/home/nathanaelss/...`) dan ke file "panduan isi minimal-maksimal" yang tidak ada di unggahan. Hapus tautan itu dari slide akhir.
- Karena tugas ini berfokus pada penjadwalan, tanyakan ke dosen apakah CPM/PERT atau network diagram diwajibkan. Rancangan sendiri mencatat bahwa metode khusus belum diketahui. Jika wajib, aktivitas perlu dipecah dan dihitung ulang, dan saya bisa membantu.

Mau saya susun ulang materi slide sesuai struktur 12 slide ini, atau mulai dari salah satu tambahan dulu, misalnya diagram ketergantungan atau tabel beban per anggota?