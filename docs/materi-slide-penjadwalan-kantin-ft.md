# Materi slide penjadwalan proyek aplikasi mobile kantin FT

Mata kuliah: Rekayasa Perangkat Lunak  
Tanggal: 24 November 2026  
Bentuk dokumen: bahan isi slide dan catatan penyaji

Materi ini mengikuti [rancangan proyek versi 1.2](/home/nathanaelss/.codex/.chatgpt-projects/g-p-6afa873136388191a08a0319179f9f7c/output/rancangan-proyek-kantin-ft.md) dan [panduan isi minimal–maksimal](/home/nathanaelss/.codex/.chatgpt-projects/g-p-6afa873136388191a08a0319179f9f7c/output/panduan-isi-minimal-maksimal-tugas-kantin-ft.md). Susunannya menggunakan tingkat penyajian yang disarankan: kebutuhan aplikasi secara ringkas, penjadwalan sebagai pembahasan utama, serta pemeriksaan keberhasilan dan risiko sebagai pendukung.

Terdapat 14 slide utama. Slide 5 sampai 13 membahas dasar dan pengelolaan jadwal. Alokasi penyampaian yang disarankan adalah sekitar 12–15 menit, menyesuaikan waktu yang diberikan dosen. Angka ini merupakan saran penyampaian.

Bagian **Isi slide** dapat langsung menjadi bahan teks presentasi. Bagian **Catatan penyaji** digunakan untuk penjelasan lisan. Arahan tampilan membantu menyusun tabel atau bagan tanpa memasukkan seluruh catatan ke layar.

Seluruh jadwal menggambarkan skenario pengembangan aplikasi jika proyek dilaksanakan. Luaran tugas saat ini adalah dokumen perencanaan dan penjadwalan. Tidak ada klaim bahwa aplikasi telah dibuat atau diuji.

## Slide 1. Penjadwalan proyek aplikasi mobile kantin FT

### Isi slide

**Penjadwalan proyek aplikasi mobile pemesanan makanan kantin FT**

Rekayasa Perangkat Lunak

Perencanaan kebutuhan, pekerjaan, dan jadwal pengembangan

[Nama anggota kelompok dan NIM]

### Catatan penyaji

Presentasi ini membahas rencana pengembangan aplikasi pemesanan makanan untuk lingkungan Fakultas Teknik. Fokusnya adalah menjelaskan pekerjaan yang diperlukan, perkiraan effort, pembagian tanggung jawab, urutan pengerjaan, dan target pencapaian. Aplikasi mobile merupakan objek yang direncanakan. Tugas yang dikumpulkan berupa perencanaan dan penjadwalannya.

Arahan tampilan: judul dan identitas kelompok. Lengkapi identitas sebelum membuat slide akhir.

Acuan: rancangan bagian 1 dan 16.

## Slide 2. Kebutuhan dan batas proyek

### Isi slide

- Mahasiswa, dosen, dan tendik memesan makanan dari tenant kantin di lingkungan FT.
- Pembeli membayar melalui QRIS atau transfer bank dengan verifikasi otomatis.
- Tenant melihat laporan omzet harian melalui aplikasi.

**Asumsi lingkup:** aplikasi mobile untuk satu platform, satu tenant per pesanan, dan pengambilan makanan di tenant.

**Luaran tugas:** dokumen perencanaan dan penjadwalan.

### Catatan penyaji

Tiga kebutuhan utama berasal dari brief tugas. Bentuk mobile dan aturan pembayaran diperjelas dalam penyusunan rancangan. Pengambilan di tenant dan satu tenant per pesanan menjadi asumsi untuk membatasi pekerjaan. Pilihan sistem operasi belum ditetapkan. Pengelola berperan sebagai pendukung untuk data tenant dan penanganan transaksi yang memerlukan tindak lanjut.

Arahan tampilan: kebutuhan utama di bagian atas, satu baris asumsi dan satu baris luaran tugas di bawahnya.

Acuan: rancangan bagian 1, 3, 4, dan 16.

## Slide 3. Kelompok fitur yang menjadi dasar jadwal

### Isi slide

| Pengguna | Fitur yang direncanakan |
|---|---|
| Pembeli | Akun, katalog kantin dan menu, keranjang, pemesanan, serta riwayat pesanan |
| Pembeli dan sistem | Pembayaran QRIS atau transfer, verifikasi otomatis, pembatalan, dan pengembalian dana |
| Tenant | Pengelolaan menu, harga, ketersediaan porsi, antrean, status pesanan, dan penyerahan |
| Tenant | Laporan omzet harian dan rincian penjualan |
| Pengelola | Pengelolaan akun tenant serta tindak lanjut pengembalian dana |

### Catatan penyaji

Fitur pendukung ikut masuk jadwal karena alur utama memerlukannya. Tenant perlu mengatur menu agar pembeli dapat memilih makanan. Status penyerahan diperlukan untuk menentukan kapan penjualan masuk omzet. Akun dan hak akses membatasi pesanan serta laporan yang dapat dilihat setiap pengguna. Tabel ini merangkum kelompok fitur, sementara rincian 29 kebutuhan tersedia pada dokumen rancangan.

Arahan tampilan: tabel sederhana dengan penekanan pada pemesanan, pembayaran, dan laporan sebagai kebutuhan utama.

Acuan: rancangan bagian 5 dan panduan bagian 4.

## Slide 4. Alur pesanan dan aturan utama

### Isi slide

1. Pembeli memilih tenant dan menu, lalu membuat pesanan.
2. Sistem mengonfirmasi pembayaran secara otomatis.
3. Tenant menyiapkan dan menyerahkan makanan.
4. Sistem memasukkan penjualan ke omzet harian.

**Pembatalan:** boleh sebelum tenant mulai menyiapkan. Jika sudah dibayar, dana dikembalikan penuh.

**Omzet:** hanya pesanan yang sudah dibayar dan diserahkan, berdasarkan tanggal penyerahan.

### Catatan penyaji

Tenant hanya mulai menyiapkan setelah pembayaran berhasil. Tindakan Mulai siapkan menjadi batas pembatalan pembeli. Pesanan batal tidak masuk omzet, tetapi riwayat pembayaran dan pengembalian tetap tersimpan. Aturan ini menjelaskan mengapa pekerjaan pengembalian dana dan pencatatan status harus ada dalam rencana. Verifikasi pembayaran otomatis juga tidak berarti seluruh proses pengembalian pasti otomatis. Prosedurnya perlu diperiksa saat memilih penyedia pembayaran.

Arahan tampilan: alur empat langkah dan satu cabang pembatalan sebelum persiapan. Gunakan dua catatan pendek untuk batas pembatalan dan syarat omzet.

Acuan: rancangan bagian 6 dan 7.

## Slide 5. Dasar penyusunan jadwal

### Isi slide

| Tahap perencanaan | Pertanyaan yang dijawab |
|---|---|
| Kebutuhan dan lingkup | Apa yang akan dibuat? |
| WBS dan aktivitas | Pekerjaan apa yang diperlukan? |
| Effort dan kapasitas | Berapa beban kerja dan siapa yang tersedia? |
| Ketergantungan | Pekerjaan mana yang harus mendahului? |
| Gantt chart dan milestone | Kapan dikerjakan dan apa target hasilnya? |

Pendekatan skenario: pengembangan bertahap dengan tinjauan mingguan.

### Catatan penyaji

Jadwal disusun dari pekerjaan yang dibutuhkan untuk memenuhi fitur. WBS adalah penguraian hasil proyek menjadi paket pekerjaan yang lebih kecil. Dari paket itu, tim menetapkan aktivitas, estimasi, dan penanggung jawab. Urutan aktivitas kemudian mengikuti ketergantungan dan kapasitas anggota. Pengembangan bertahap memungkinkan pengujian dilakukan selama pengerjaan, dengan pengujian penerimaan terpadu menjelang akhir skenario proyek.

Arahan tampilan: lima baris tahap perencanaan. Ini menjadi pengantar bagian utama presentasi.

Acuan: rancangan bagian 9 dan panduan bagian 2–3.

## Slide 6. Asumsi tim dan kapasitas kerja

### Isi slide

**Asumsi skenario: 4 anggota, 8 minggu, 10 jam per anggota per minggu.**

| Anggota contoh | Fokus tanggung jawab |
|---|---|
| A | Analisis, koordinasi, pengujian, dan dokumentasi |
| B | Rancangan layar dan pengembangan aplikasi mobile |
| C | Backend, autentikasi, aturan pesanan, dan laporan |
| D | Basis data, pembayaran, pengembalian, dan paket aplikasi uji |

Kapasitas total: **4 × 10 × 8 = 320 jam-orang**.

### Catatan penyaji

Nama A sampai D adalah pengganti nama anggota. Pembagian ini menunjukkan fokus utama, dan penanggung jawab tiap aktivitas tercantum dalam jadwal rinci. Sepuluh jam per minggu mencerminkan pengerjaan paruh waktu dalam skenario. Delapan minggu merupakan rentang pengembangan aplikasi hipotetis, bukan waktu yang dibutuhkan untuk menulis laporan tugas. Platform serta teknologi masih menjadi keputusan awal dalam rencana.

Arahan tampilan: tabel anggota dan satu angka kapasitas total. Jangan menampilkan angka asumsi seolah-olah ketentuan dosen.

Acuan: rancangan bagian 9.1.

## Slide 7. Estimasi effort dan durasi

### Isi slide

| Komponen | Estimasi |
|---|---:|
| Pekerjaan terencana | 256 jam-orang |
| Kapasitas cadangan | 64 jam-orang |
| Kapasitas total | 320 jam-orang |

- Effort adalah jumlah kerja orang. Durasi adalah rentang waktu pengerjaan.
- Contoh: 8 jam-orang dapat dialokasikan dalam satu minggu.
- Cadangan sebesar 20% kapasitas untuk kendala yang belum terduga.

### Catatan penyaji

Total 256 jam-orang berasal dari penjumlahan 32 aktivitas pada dokumen rancangan. Angka ini merupakan estimasi awal berdasarkan penguraian pekerjaan, belum berasal dari pengukuran produktivitas tim. Tim diasumsikan sudah mengenal teknologi mobile dan backend yang akan dipakai. Cadangan 64 jam-orang tersebar sepanjang delapan minggu, sehingga tidak otomatis berarti tersedia tambahan waktu kalender di akhir proyek. Jadwal perlu ditinjau jika platform atau kompleksitas integrasi berubah.

Arahan tampilan: tabel angka dan satu contoh effort dibanding durasi. Bila memakai diagram batang, bagian pekerjaan adalah 256 dan cadangan 64 dari total 320.

Acuan: rancangan bagian 9.1 dan panduan bagian 8.

## Slide 8. WBS dan alokasi effort

### Isi slide

| Paket pekerjaan | Effort (jam-orang) |
|---|---:|
| 1. Kebutuhan, aturan bisnis, dan kelayakan pembayaran | 38 |
| 2. Rancangan rinci dan fondasi mobile serta backend | 24 |
| 3. Akun, katalog, stok, dan pemesanan | 56 |
| 4. Pembayaran, pembatalan, dan pengembalian | 56 |
| 5. Laporan, penyerahan, dan riwayat transaksi | 26 |
| 6. Integrasi, pengujian penerimaan, dan perbaikan | 34 |
| 7. Rilis demonstrasi dan dokumen yang direncanakan | 22 |
| **Total** | **256** |

### Catatan penyaji

Tujuh paket ini merupakan ringkasan WBS pada dokumen rancangan. Setiap paket terdiri dari beberapa aktivitas. Paket pertama juga mencakup kriteria penerimaan, sedangkan paket pembayaran mencakup pengujiannya. Jadi pengujian tidak seluruhnya menunggu paket keenam. Nama paket diringkas untuk slide, tetapi cakupan dan effort tetap mengikuti rancangan. Rilis demonstrasi adalah target dalam skenario proyek yang dijadwalkan, bukan berkas yang harus diwujudkan untuk tugas sekarang.

Arahan tampilan: tabel tujuh paket. Hindari memasukkan semua 32 aktivitas ke slide ini.

Acuan: rancangan bagian 9.2.

## Slide 9. Contoh aktivitas dan ketergantungan

### Isi slide

| ID | Aktivitas ringkas | PIC | Effort | Waktu | Pendahulu |
|---|---|---|---:|---|---|
| T12 | Pesanan dan penahanan stok | D | 8 | M3 | T05, T08 |
| T16 | Integrasi pembayaran | D | 10 | M4 | T03, T07, T12 |
| T19 | Status pembayaran dan batas pembatalan | C | 10 | M5 | T15, T16 |
| T20 | Pengembalian dana | D | 10 | M5 | T03, T15, T16 |
| T21 | Uji pembayaran dan pembatalan | A | 8 | M6 | T17, T18, T19, T20 |

Effort dalam jam-orang. M berarti minggu. Tabel merupakan cuplikan jadwal.

### Catatan penyaji

T16 memerlukan hasil T12 karena pembayaran harus terhubung dengan pesanan dan nilainya. T19 dan T20 direncanakan pada minggu yang sama dengan PIC berbeda setelah pekerjaan pendahulu tersedia. T21 menunggu hasil keduanya serta alur dan layar pendukung. Inilah alasan beberapa pekerjaan berjalan berurutan dan sebagian dapat berjalan bersamaan. Seluruh aktivitas pada cuplikan ini memiliki jendela durasi satu minggu, dengan jam kerja sebagaimana kolom effort.

Kode pendahulu lain mengacu ke tabel lengkap: T03 adalah pemeriksaan penyedia pembayaran, T05 kriteria penerimaan, T07 fondasi backend, T08 basis data, T15 aturan proses tenant, T17 pengujian alur awal pembayaran, dan T18 layar pembayaran serta status. Keterangan ini cukup disampaikan jika ditanyakan.

Arahan tampilan: tabel lima aktivitas, dengan penekanan pada T19 dan T20 yang sejajar. Bila membuat bagan, beri label sebagai contoh ketergantungan. Dokumen belum menghitung jalur kritis dengan CPM.

Acuan: rancangan bagian 10 dan 11.2.

## Slide 10. Gantt chart skenario delapan minggu

### Isi slide

| Paket WBS | M1 | M2 | M3 | M4 | M5 | M6 | M7 | M8 |
|---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1. Kebutuhan dan kelayakan | ■ | ■ | | | | | | |
| 2. Desain dan fondasi aplikasi | | ■ | | | | | | |
| 3. Akun, katalog, dan pemesanan | | | ■ | ■ | | | | |
| 4. Pembayaran dan pengembalian | | | | ■ | ■ | ■ | | |
| 5. Laporan dan penyerahan | | | | | | ■ | | |
| 6. Integrasi dan penerimaan | | | | | | | ■ | |
| 7. Rilis dan dokumen | | | | | | | | ■ |

■ = minggu pelaksanaan aktivitas dalam paket. Pengujian modul sudah termasuk pada paket terkait.

### Catatan penyaji

Gantt chart ini merangkum aktivitas T01 sampai T32 berdasarkan tujuh paket WBS pada slide 8. Pada minggu kedua, pekerjaan kriteria penerimaan dan fondasi aplikasi dapat berlangsung bersamaan karena hasil analisis awal tersedia. Pembayaran berlangsung sampai minggu keenam karena mencakup pengujian. Laporan dan penyerahan juga dijadwalkan pada minggu keenam setelah aturan transaksi tersedia.

Rentang paket menunjukkan kapan aktivitas di dalamnya berlangsung. Rentang ini tidak berarti setiap aktivitas bekerja penuh sepanjang rentang tersebut, dan ketergantungan tetap mengikuti aktivitas rinci. Pengelompokan ini berbeda dari label kegiatan pada Gantt dokumen awal, tetapi menggunakan minggu dan aktivitas sumber yang sama.

Arahan tampilan: gunakan Gantt sebagai visual utama dengan lebar slide penuh. Pertahankan nama atau nomor paket yang sama dengan slide WBS.

Acuan: rancangan bagian 9.2 dan 10. Gantt ini merupakan pengelompokan ulang dari aktivitas sumber.

## Slide 11. Pemeriksaan beban kerja mingguan

### Isi slide

| Minggu | Effort terencana | Kapasitas | Cadangan |
|---|---:|---:|---:|
| M1 | 30 | 40 | 10 |
| M2 | 32 | 40 | 8 |
| M3 | 32 | 40 | 8 |
| M4 | 34 | 40 | 6 |
| M5 | 38 | 40 | 2 |
| M6 | 34 | 40 | 6 |
| M7 | 34 | 40 | 6 |
| M8 | 22 | 40 | 18 |

Satuan: jam-orang. M5 paling padat. Beban tiap anggota maksimal 10 jam per minggu.

### Catatan penyaji

Jumlah kerja tim setiap minggu tidak melebihi kapasitas 40 jam-orang. Pemeriksaan per anggota pada dokumen rinci juga menunjukkan tidak ada yang melebihi 10 jam dalam satu minggu. Namun, total kapasitas yang cukup belum menjamin semua keterlambatan mudah ditangani. Pada M5, hanya tersisa dua jam-orang dan anggota B, C, serta D sudah mendapat alokasi penuh. Kapasitas anggota lain belum tentu dapat menggantikan pekerjaan yang membutuhkan kemampuan khusus.

Arahan tampilan: tabel atau diagram batang effort dengan garis kapasitas 40. Tandai M5 agar alasan pemantauan pembayaran terlihat.

Acuan: rancangan bagian 10.1.

## Slide 12. Milestone dan kriteria pencapaian

### Isi slide

| Target | Pencapaian yang direncanakan |
|---|---|
| Akhir M1 | Kebutuhan, platform, dan kelayakan pembayaran telah ditinjau. |
| Akhir M2 | Rancangan mobile, basis data, dan fondasi akun tersedia. |
| Akhir M4 | Alur pemesanan dasar terhubung. |
| Akhir M5 | Pembayaran dan pengembalian dapat diuji. |
| Akhir M6 | Penyerahan dan laporan terintegrasi, total dapat ditelusuri. |
| Akhir M7 | Kriteria penerimaan terpenuhi. |
| Akhir M8 | Paket aplikasi uji dan dokumen siap pada skenario proyek. |

### Catatan penyaji

Milestone menunjukkan hasil yang dapat diperiksa. Contohnya, target akhir M5 berarti QRIS dan transfer dapat dikonfirmasi dalam sandbox, dan alur pengembalian tersedia untuk diuji. Ini berbeda dari sekadar menyatakan minggu pembayaran telah berakhir. Untuk laporan pada M6, angka omzet harus dapat dicocokkan dengan rincian pesanan. Semua pencapaian ini merupakan target rencana, sehingga tidak ditandai sebagai hasil yang sudah tercapai.

Arahan tampilan: garis waktu tujuh titik atau tabel. Gunakan kriteria hasil yang singkat, bukan hanya nama fase.

Acuan: rancangan bagian 11.1, MS-01 sampai MS-07.

## Slide 13. Risiko dan penyesuaian jadwal

### Isi slide

| Risiko | Dampak | Penanganan yang direncanakan |
|---|---|---|
| Pembayaran atau pengembalian tidak sesuai asumsi | Integrasi dan pengujian tertunda | Periksa dukungan sejak M1 dan alur dasar pada M4. |
| Kapasitas atau kemampuan anggota berbeda | Aktivitas meleset dari estimasi | Tinjau beban mingguan dan sesuaikan penugasan. |
| Kebutuhan bertambah | Effort meningkat dan milestone bergeser | Periksa dampak sebelum mengubah lingkup dan jadwal. |

Tinjauan mingguan memeriksa hasil, pekerjaan tersisa, ketergantungan, dan penggunaan cadangan.

### Catatan penyaji

Risiko pembayaran mendapat perhatian karena M5 sudah padat dan hasilnya diperlukan untuk pengujian serta pelaporan. Jika aktivitas terlambat, tim meninjau pekerjaan yang bergantung padanya, lalu menghitung ulang sisa effort. Cadangan dipakai untuk kendala yang belum terduga. Jika kapasitas tetap tidak cukup, jadwal perlu direvisi. Langkah ini adalah mekanisme pemantauan yang diusulkan apabila proyek dilaksanakan.

Arahan tampilan: tabel tiga risiko dan satu kalimat mekanisme tinjauan.

Acuan: rancangan bagian 14–15 dan panduan bagian 7.

## Slide 14. Kriteria keberhasilan dan luaran tugas

### Isi slide

**Pemeriksaan yang direncanakan**

- Pesanan sesuai tenant, menu, dan ketersediaan porsi.
- Kedua metode pembayaran menghasilkan konfirmasi yang benar.
- Pembatalan sebelum persiapan mengikuti aturan pengembalian penuh.
- Omzet hanya memuat pesanan yang dibayar dan diserahkan.
- Hak akses dan alur utama bekerja pada ponsel sasaran.

**Luaran tugas:** dokumen kebutuhan ringkas, WBS, estimasi, jadwal, Gantt chart, milestone, serta rencana pemeriksaan dan risiko.

### Catatan penyaji

Kriteria ini menjelaskan bagaimana tim akan menilai hasil jika aplikasi dikembangkan. Pengujian tetap membutuhkan alokasi waktu dalam jadwal meskipun tugas sekarang hanya berupa rencana. Dokumen tugas menunjukkan hubungan kebutuhan dengan pekerjaan, kapasitas, urutan, dan pencapaian yang ditargetkan. Pertanyaan mengenai platform atau kebutuhan tambahan dapat dijawab melalui asumsi dan dampaknya pada estimasi.

Arahan tampilan: daftar pemeriksaan dan satu baris luaran. Tidak perlu menampilkan tanda lulus karena pengujian belum dilaksanakan.

Acuan: rancangan bagian 13 dan 16 serta panduan bagian 7.

## Bahan pendukung untuk tanya jawab

Bagian ini merupakan catatan tambahan bagi penyaji. Tidak perlu memasukkannya ke slide utama kecuali dosen meminta penjelasan lebih rinci.

### Mengapa menggunakan delapan minggu?

Delapan minggu adalah asumsi skenario pengembangan yang disusun dari aktivitas pada dokumen rancangan. Waktu tersebut bukan tenggat resmi dosen dan bukan lama pengerjaan laporan. Estimasi perlu ditinjau setelah platform, kemampuan tim, dan cara integrasi pembayaran diketahui.

### Mengapa effort hanya 256 jam-orang dari kapasitas 320?

Selisih 64 jam-orang merupakan kapasitas cadangan. Besarnya 20% berasal dari 64 dibagi 320. Cadangan tersebar per minggu dan anggota. Waktu kosong pada minggu pertama tidak dapat langsung digunakan untuk pekerjaan yang baru siap pada minggu kelima.

### Mengapa pembatalan dan pengembalian masuk jadwal?

Kebutuhan yang disepakati mengizinkan pembatalan setelah pembayaran selama makanan belum disiapkan. Karena uang bisa sudah masuk, sistem membutuhkan pengembalian penuh beserta pencatatannya. Menghilangkan pekerjaan tersebut akan membuat jadwal tidak mencakup aturan yang telah dipilih.

### Apakah seluruh kegiatan berlangsung berurutan?

Sebagian mempunyai ketergantungan dan sebagian dapat sejajar. Contohnya, T19 dan T20 berada di M5 dengan PIC berbeda setelah pendahulunya tersedia. Kegiatan dengan PIC sama tetap perlu memperhatikan pembagian jam. T31 dan T32 pada M8 juga harus dikerjakan berurutan walaupun berada pada minggu yang sama.

### Apakah jadwal ini memakai CPM atau PERT?

Belum. Materi menggunakan WBS, estimasi effort, ketergantungan aktivitas, kapasitas anggota, dan Gantt chart. Jika dosen mewajibkan CPM atau PERT, durasi aktivitas dan perhitungannya perlu dilengkapi. Contoh ketergantungan pada slide 9 tidak boleh disebut sebagai hasil perhitungan jalur kritis.

### Mengapa ada integrasi, pengujian, dan rilis jika aplikasinya tidak dibuat?

Tugas menjadwalkan pekerjaan yang akan dibutuhkan apabila pengembangan berlangsung. Karena itu, jadwal tetap mencakup siklus pekerjaan sampai target akhir. Mahasiswa menyerahkan dokumen perencanaannya, tanpa membuat produk dan bukti uji aktual.

## Penyesuaian jumlah slide

Gunakan 14 slide sebagai susunan utama. Jika waktu presentasi singkat, susunan dapat dipadatkan menjadi 10 slide dengan cara berikut:

1. Gabungkan slide 2 dan 3 menjadi gambaran serta kelompok fitur.
2. Sampaikan materi slide 5 secara lisan saat membuka pembahasan WBS pada slide 8.
3. Gabungkan slide 6 dan 7 menjadi asumsi tim, kapasitas, dan effort.
4. Pindahkan tabel slide 11 ke cadangan, lalu sebutkan M5 sebagai minggu terpadat ketika membahas risiko.

Dalam versi singkat, pertahankan contoh aktivitas beserta PIC dan pendahulunya, Gantt chart, serta milestone. Untuk penjelasan maksimal, gunakan tabel 32 aktivitas, beban per anggota, dan skenario uji pada dokumen rancangan sebagai lampiran terpisah di akhir presentasi. Pilihan jumlah slide ini merupakan rekomendasi penyajian, bukan ketentuan dosen.

## Sumber materi

- [Rancangan proyek kantin FT versi 1.2](/home/nathanaelss/.codex/.chatgpt-projects/g-p-6afa873136388191a08a0319179f9f7c/output/rancangan-proyek-kantin-ft.md). Sumber kebutuhan, aturan bisnis, estimasi, aktivitas, dan milestone.
- [Panduan isi minimal–maksimal tugas kantin FT](/home/nathanaelss/.codex/.chatgpt-projects/g-p-6afa873136388191a08a0319179f9f7c/output/panduan-isi-minimal-maksimal-tugas-kantin-ft.md). Acuan pemilihan tingkat rincian dan struktur presentasi.

Daftar referensi eksternal untuk dasar penjadwalan dan contoh kelayakan pembayaran tersedia pada bagian 18 dokumen rancangan. Materi slide ini merangkum keputusan dan estimasi dari kedua dokumen tersebut. Tidak ada hasil implementasi atau pengujian baru yang ditambahkan.
