# 📜 Team Manifesto — Tim Vortex
### Proyek: Aplikasi Mobile Kantin Pintar Kampus (Vortex Store)

> Dokumen ini adalah kesepakatan resmi tim dalam hal cara berkomunikasi dan memberi masukan terhadap kode satu sama lain. Dibuat agar konflik yang dialami tim sebelumnya — saling menyalahkan karena format data JSON yang berubah tanpa komunikasi — **tidak terulang** di tim ini.

---

## 👥 Anggota Tim

| Nama | Peran |
|---|---|
| Adit | Developer |
| Dafa | Developer |
| Brigga | Developer |

*(Sesuaikan kolom Peran di atas, misalnya jika ada yang merangkap sebagai Scrum Master atau Product Owner.)*

---

## 1. SOP Code Review

### Tujuan
Code review dilakukan untuk menjaga kualitas kode dan saling belajar — **bukan** untuk menyalahkan atau menjatuhkan anggota lain. Kritik diarahkan ke kode, bukan ke orangnya.

### Aturan Umum
1. Setiap *pull request* (PR) wajib di-review oleh minimal **1 anggota lain** sebelum di-*merge* ke branch utama (`main`).
2. Review diberikan dalam waktu maksimal **24 jam** setelah PR dibuka, agar tidak menghambat progres tim.
3. Gunakan kolom *comment* di GitHub untuk diskusi teknis — hindari membahas kesalahan kode lewat chat pribadi atau grup, supaya ada jejak diskusi yang bisa dilihat semua orang.
4. Jika menemukan kesalahan, **jelaskan alasannya** dan beri **saran solusi**, jangan hanya menyalahkan.
5. Penulis kode berhak menjelaskan alasan keputusan teknisnya; jika reviewer tetap tidak sepakat, diskusikan singkat di stand-up, bukan berlarut-larut di kolom komentar.

### Contoh Kalimat: Dilarang vs Dianjurkan

| ❌ Dilarang | ✅ Dianjurkan |
|---|---|
| "Kode ini berantakan banget, siapa yang nulis ini?" | "Menurutku bagian ini bisa disederhanakan, gimana kalau pakai fungsi terpisah? Ini juga akan memudahkan testing." |
| "Lo lagi yang bikin error, ganggu kerjaan gue." | "Sepertinya ada konflik antara perubahanmu dan punyaku di bagian ini, yuk kita samakan dulu sebelum lanjut." |
| "Format JSON-nya salah, jadi gak nyambung ke frontend." | "Aku lihat struktur JSON di endpoint ini berbeda dari yang kita sepakati di dokumentasi API. Boleh disesuaikan, atau ada alasan khusus kenapa diubah?" |
| "Ini gampang, harusnya gak usah lama-lama." | "Aku lihat task ini makin kompleks dari perkiraan awal, mungkin perlu kita re-estimasi story point-nya." |
| "Pokoknya punyaku udah bener, punya kamu yang error." | "Boleh kita debug bareng? Aku belum yakin masalahnya di endpoint atau di sisi frontend." |

### Proses Review Singkat
1. Buat PR dengan deskripsi singkat: apa yang diubah & kenapa.
2. Tag minimal 1 anggota lain untuk review.
3. Reviewer beri komentar (jika ada perbaikan) atau approve.
4. Penulis kode merespons/memperbaiki sesuai komentar.
5. Setelah disetujui, PR boleh di-*merge*.

---

## 2. Protokol Komunikasi

### Jam Kerja & Batas Komunikasi
- **Tidak ada chat koordinasi tugas di atas jam 21.00 WIB**, kecuali ada **sistem yang down / error kritis** yang mengganggu deployment.
- Jam kerja efektif yang disepakati tim: **09.00 – 21.00 WIB**. Di luar jam ini, anggota tidak wajib merespons chat non-darurat.
- Tujuannya: menghindari *burnout* dan menjaga kesehatan mental tim selama sprint yang padat (2 minggu).

### Kanal Komunikasi
| Kebutuhan | Kanal |
|---|---|
| Diskusi teknis terkait kode | Komentar di GitHub PR/Issue |
| Koordinasi harian & info cepat | Grup chat tim (WhatsApp/Discord) |
| Laporan progres ke Product Owner | Ringkasan tertulis di akhir setiap stand-up |
| Darurat (sistem down) | Chat langsung + tag semua anggota, boleh di luar jam kerja |

### Update Harian (Daily Stand-up)
- Dilakukan setiap hari, maksimal 15 menit (boleh lewat chat singkat jika tidak bisa video call).
- Setiap anggota menjawab 3 hal:
  1. Apa yang dikerjakan kemarin?
  2. Apa yang akan dikerjakan hari ini?
  3. Ada kendala/blocker?

### Eskalasi Darurat
Jika terjadi error kritis yang menghentikan progres (misalnya server down, build gagal total):
1. Laporkan segera ke grup chat tim dengan tag semua anggota, kapan pun waktunya.
2. Jangan menunggu jam kerja berikutnya untuk melaporkan masalah kritis.
3. Anggota yang menerima laporan wajib merespons secepatnya meski di luar jam kerja normal, khusus untuk kategori darurat ini.

---

## 3. Kesepakatan Khusus: Kontrak Data (Anti Konflik JSON)

Karena konflik utama tim sebelumnya adalah format data JSON yang berubah-ubah tanpa komunikasi, tim ini sepakat:

1. Format JSON setiap endpoint **didokumentasikan tertulis** sebelum endpoint dikerjakan (lihat dokumentasi API di Deliverable A).
2. Jika ada perubahan format data di tengah jalan, **wajib diinfokan ke grup tim** dan didiskusikan dulu — tidak boleh diubah sepihak.
3. Perubahan kontrak API yang sudah disepakati harus diperbarui juga di dokumentasinya, bukan hanya di kode.

---

## ✅ Komitmen Tim

Dengan menandatangani (mencantumkan nama) di bawah, setiap anggota sepakat untuk mengikuti SOP Code Review dan Protokol Komunikasi di atas selama proyek berlangsung.

| Nama | Tanda Tangan / Konfirmasi |
|---|---|
| Adit | [ ] Setuju |
| Dafa | [ ] Setuju |
| Brigga | [ ] Setuju |
