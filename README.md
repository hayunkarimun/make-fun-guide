# Panduan make.fun untuk Pemula: dari Nol sampai Klaim Hadiah

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/hayunkarimun/make-fun-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/hayunkarimun/make-fun-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

Panduan ini buat kamu yang baru dengar nama make.fun dan penasaran: beneran bisa dibayar buat bikin software pakai AI? Jawaban singkatnya: iya, tapi bukan sulap dan bukan penghasilan instan. Kamu ikut lomba (disebut bounty), membangun sesuatu dengan bantuan agen AI, lalu mengirim hasilnya. Kalau karyamu masuk peringkat berbayar, hadiahnya dibayar dalam USDC di jaringan Solana.

Saya peserta juga, bukan tim make.fun. Isi panduan ini saya susun dari pengalaman ikut serta dan dokumentasi resmi mereka — kalau ada yang berubah, yang di situslah yang berlaku.

> **Baru mau daftar? Pakai tautan saya:** [https://make.fun/r/4pxjyxse](https://make.fun/r/4pxjyxse)
>
> Kode referral saya: `4pxjyxse`
>
> Daftar lewat tautan itu tidak mengubah apa pun buat kamu — kamu tetap dapat akun yang sama — tapi saya mendapat bagian kecil kalau kamu aktif. Terima kasih kalau kamu memakainya.

## Daftar isi

- [Apa itu make.fun?](#apa-itu-makefun)
- [Alur sebuah bounty](#alur-sebuah-bounty)
- [Yang kamu butuhkan sebelum mulai](#yang-kamu-butuhkan-sebelum-mulai)
- [Langkah 1: Buat akun](#langkah-1-buat-akun)
- [Langkah 2: Pilih bounty yang cocok](#langkah-2-pilih-bounty-yang-cocok)
- [Langkah 3: Unduh kit-nya](#langkah-3-unduh-kit-nya)
- [Langkah 4: Bangun entry kamu](#langkah-4-bangun-entry-kamu)
- [Langkah 5: Kirim entry](#langkah-5-kirim-entry)
- [Langkah 6: Cek hasil, perbaiki, kirim ulang](#langkah-6-cek-hasil-perbaiki-kirim-ulang)
- [Langkah 7: Klaim hadiahmu](#langkah-7-klaim-hadiahmu)
- [Kalau mau agenmu yang mengerjakan semuanya](#kalau-mau-agenmu-yang-mengerjakan-semuanya)
- [Dapatkan uang dari referral kamu sendiri](#dapatkan-uang-dari-referral-kamu-sendiri)
- [Kesalahan yang paling sering saya lihat](#kesalahan-yang-paling-sering-saya-lihat)
- [Ekspektasi yang realistis](#ekspektasi-yang-realistis)
- [Pertanyaan yang sering ditanyakan](#pertanyaan-yang-sering-ditanyakan)

## Apa itu make.fun?

Bayangkan sebuah papan lomba untuk pembuat software. Setiap lomba punya satu tugas — misalnya "bangun game ini", "bangun mesin catur sekecil mungkin", atau "tulis panduan terbaik tentang make.fun" — plus tenggat dan hadiah dalam dolar AS yang dibayar sebagai USDC, mata uang kripto yang nilainya dipatok ke dolar.

Bedanya dengan lomba biasa adalah peran agen AI. Kamu tidak harus menulis semua kode sendiri. Kamu bekerja bersama agen coding AI — Claude Code, Codex, Cursor, Copilot, atau agen lain yang kamu pakai sehari-hari. Agen itu yang menulis, menguji, dan memperbaiki kode, sementara kamu yang mengarahkan, menguji hasilnya, dan bertanggung jawab atas apa yang dikirim.

Tiga hal yang membuat sistem ini masuk akal buat saya:

1. **Hadiahnya sudah dikunci di awal.** Untuk bounty baru, seluruh hadiah disimpan dalam escrow di blockchain Solana sebelum lomba dibuka. Dananya sudah ada di sana, menunggu pemenang mengklaimnya.
2. **Penilaiannya transparan.** Setiap bounty mempublikasikan cara penilaiannya: apa yang diuji, bagaimana skor dihitung, dan berapa orang yang dibayar.
3. **Transkrip menjaga kejujuran.** Setiap entry disertai rekaman sesi AI yang membangunnya. Itu cara make.fun memastikan yang dikirim memang hasil kerja agen peserta sendiri, bukan kode orang lain yang ditempel namanya.

## Alur sebuah bounty

Satu bounty biasanya berjalan seperti ini:

| Tahap | Artinya buat kamu |
|---|---|
| Buka | Bounty diumumkan, kamu bisa mulai membangun. Perhatikan jam tutupnya — semua memakai waktu UTC di situs. |
| Kirim | Kamu mengirim repositori GitHub publik pada satu commit, plus transkrip sesi AI yang membangunnya. |
| Diperiksa | Sistem otomatis memeriksa kelengkapan entry: repo-nya publik dan milikmu, transkripnya cocok dengan kode, dan tidak ada rahasia yang bocor. |
| Dinilai | Penilai menguji entry kamu di sandbox dengan cara yang sama untuk semua peserta. |
| Dibayar | Pemenang mengklaim hadiah USDC ke dompet Solana mereka sendiri. |

Ingat: **waktu di situs memakai UTC** — tutup pukul 10:30 UTC berarti 17:30 WIB.

## Yang kamu butuhkan sebelum mulai

Siapkan tiga hal ini dulu, sebelum kamu memilih bounty:

- **Agen coding AI.** Ini alat kerja utamamu. Tidak ada satu agen yang "resmi" — pakai yang sudah kamu kenal. Yang penting, agen itu menyimpan riwayat sesi yang bisa dikirim sebagai transkrip, karena hampir semua bounty memintanya.
- **Akun GitHub.** Entry kamu berupa repositori GitHub publik, dan repositori itu harus dimiliki akun GitHub yang terhubung ke akun make.fun kamu. Jangan kirim repo milik orang lain, meskipun kamu punya izin — pemeriksaannya akan menolak.
- **Dompet Solana.** Hadiah dibayar dalam USDC di Solana. Kunci privat dompet itu milikmu sendiri: jangan pernah mengirimkannya ke siapa pun, di chat mana pun, dalam bentuk apa pun — termasuk ke agen AI. Agen yang baik tidak akan pernah memintanya.

Siapkan juga kesabaran: entry pertama hampir selalu lebih lambat dari yang kamu bayangkan.

## Langkah 1: Buat akun

1. Buka [make.fun](https://make.fun/?ref=4pxjyxse&utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02), atau daftar lewat tautan referral saya di atas: [https://make.fun/r/4pxjyxse](https://make.fun/r/4pxjyxse).
2. Buat akun dengan cara yang ditawarkan situs — misalnya masuk dengan GitHub. Menghubungkan GitHub sejak awal menghemat waktu, karena entry kamu memang butuh GitHub yang terhubung.
3. Lengkapi profilmu: nama pengguna, dan kalau diminta, hubungkan dompet Solana. Dompet ini yang akan menerima hadiah kalau kamu menang.
4. Cari tab Referral di profilmu. Di sanalah tautan dan kode referral kamu sendiri berada.

Tips kecil: gunakan email dan akun GitHub yang memang kamu kelola. Klaim hadiah biasanya butuh akun yang sama dengan yang mengirim entry, jadi akun asal-asalan yang lalu ditinggalkan akan menyulitkanmu sendiri.

## Langkah 2: Pilih bounty yang cocok

Jangan langsung mengambil bounty dengan hadiah terbesar. Buka halaman daftar bounty dan periksa empat hal ini:

- **Tenggatnya.** Hitung mundur dari sekarang, dalam UTC. Kalau sisa waktu tinggal beberapa jam dan tugasnya besar, lewati saja.
- **Tugasnya.** Baca deskripsi tugas sampai habis, bukan cuma judulnya. Ada bounty yang meminta game utuh, ada yang meminta satu fungsi kecil. Pilih yang sesuai dengan waktu dan kemampuan agenmu.
- **Cara penilaiannya.** Kalau penilaiannya memakai pengujian otomatis dengan batas ukuran file, kamu harus merancang entry sesuai batas itu sejak awal.
- **Jumlah pemenang.** Ada bounty yang membayar 100 orang teratas, ada yang hanya membayar 20. Hadiah total yang besar belum tentu berarti peluangmu besar — lihat juga berapa orang yang sudah ikut.

Buat pemula, bounty panduan seperti ini sering jadi titik masuk yang bagus.

## Langkah 3: Unduh kit-nya

Setiap bounty punya "kit" — paket berisi aturan lengkap, contoh awal (starter), dan perkakas baris perintah (CLI) untuk memeriksa, membungkus transkrip, dan mengirim entry. Unduh kit-nya dari halaman bounty, lalu ekstrak di komputermu.

Di dalam kit kamu akan menemukan antara lain:

- `RULES.txt` atau berkas aturan — baca ini dulu, jangan dilewati. Di sinilah tertulis batas ukuran, berkas yang wajib ada, dan hal-hal yang dilarang.
- Folder starter — titik awal yang disediakan. Boleh dipakai, tapi jangan dikirim apa adanya: entry yang isinya persis starter akan ditolak karena tidak ada baris pun yang ditulis agenmu.
- CLI `makefun.mjs` — alat untuk memeriksa entry, membuat bundle transkrip, dan mengirim entry. Kalau CLI memberi tahu salinan kit kamu sudah lama, unduh ulang dari halaman bounty sebelum mengirim.

## Langkah 4: Bangun entry kamu

Inilah bagian kerja yang sesungguhnya. Pola yang paling sering berhasil buat saya:

1. **Mulai sesi agen setelah bounty dibuka.** Sesi yang dimulai sebelum bounty dibuka tidak bisa dipakai untuk entry itu, jadi jangan memakai rekaman sesi lama.
2. **Jelaskan tugasnya dengan jelas ke agen.** Tempelkan aturan dari kit, sebutkan batas-batasnya (ukuran file, bahasa yang diizinkan, apa yang diuji), dan minta agen merencanakan dulu sebelum menulis kode.
3. **Bangun sedikit demi sedikit, dan uji terus.** Jangan menunggu semuanya selesai baru diuji. Jalankan, lihat hasilnya, perbaiki yang rusak, lalu lanjut.
4. **Jangan menyalin kode orang lain.** Ini aturan yang paling keras di make.fun: transkrip kamu akan dibandingkan dengan kode yang kamu kirim. Kalau sebagian besar baris kode ternyata tempelan dari contoh, starter, atau repositori lain — bukan tulisan agenmu sendiri — entry kamu akan ditolak pada pemeriksaan transkrip. Tulis ulang dengan kata-katamu sendiri, meskipun idenya terinspirasi dari contoh.
5. **Simpan semua sesi yang mengerjakan entry.** Kalau kamu memakai sub-agen atau sesi tambahan, semuanya harus ikut dibungkus saat pengiriman. Jangan menghapus riwayat sesi di tengah jalan.

Untuk bounty panduan seperti ini, "membangun" berarti menulis panduan itu sendiri: draf dulu, lalu revisi. Draf pertama tidak harus bagus — yang penting ada. Revisi kedua adalah tempat panduan benar-benar terbentuk: potong yang bertele-tele, tambahkan contoh nyata, perbaiki yang membingungkan.

## Langkah 5: Kirim entry

Kalau pekerjaanmu sudah selesai dan sudah diuji, saatnya mengirim:

1. **Buat repositori GitHub publik** dengan akun GitHub yang terhubung ke akun make.fun kamu. Repositori harus dibuat setelah bounty dibuka.
2. **Dorong (push) pekerjaanmu ke repositori itu**, termasuk berkas yang diwajibkan — biasanya `README.md` dan `LICENSE`, plus berkas lain sesuai aturan bounty.
3. **Atur halaman About repositori** sesuai yang diminta aturan (biasanya situs web bounty dan topik yang ditentukan).
4. **Periksa entry secara lokal dengan CLI kit** sebelum mengirim. Lebih baik kekurangan ketahuan sekarang daripada setelah dikirim.
5. **Buat bundle transkrip dengan CLI**, lalu kirim entry lewat CLI dengan alamat repo, commit yang akan dinilai, dan judul entry.

Setelah terkirim, kamu akan mendapat ID pengiriman (submission id). Simpan ID itu — semua pengecekan status setelah ini memakainya.

Perhatian: entry dinilai dari **satu commit tertentu** yang kamu kirim. Commit baru yang kamu dorong setelah mengirim tidak otomatis ikut dinilai. Kalau mau memperbaiki, kamu harus mengirim ulang sebagai putaran (round) baru, selama kuota dan tenggat masih memungkinkan.

## Langkah 6: Cek hasil, perbaiki, kirim ulang

Setelah mengirim, periksa status entry kamu secara berkala:

- Kalau semua pemeriksaan lolos dan statusnya "dinilai" (scored) tapi hasil akhir belum diputuskan, tidak ada yang perlu kamu lakukan — tinggal tunggu.
- Kalau ada pemeriksaan yang gagal, baca alasan dan perbaikannya baik-baik. Sebagian besar kegagalan punya perbaikan yang jelas: berkas kurang, repo tidak publik, transkrip tidak cocok, dan semacamnya.
- Kalau entry ditolak karena transkrip (misalnya terlalu sedikit baris yang ditulis agenmu sendiri), perbaikannya bukan sekadar mengedit sedikit. Kamu biasanya harus membangun ulang pekerjaan itu dalam sesi baru yang direkam, dengan agen yang benar-benar menulis kodenya sendiri. Ini memang berat — makanya langkah 4 di atas sangat penting.

Setiap bounty punya kuota pengiriman: batas per hari dan batas total per akun. Periksa kuotamu sebelum mengirim ulang, supaya kamu tidak menghabiskan percobaan untuk perbaikan yang belum matang.

## Langkah 7: Klaim hadiahmu

Kalau hasil diumumkan dan kamu masuk peringkat berbayar, hadiah tidak masuk otomatis ke dompetmu — kamu harus mengklaimnya:

1. Buka halaman hasil atau profilmu dan cari tombol klaim untuk entry yang menang.
2. Klaim akan membayar USDC ke dompet Solana yang menandatangani entry kamu.
3. Periksa riwayat transaksi di penjelajah blockchain Solana untuk memastikan dana sudah masuk.

Ada masa tunggu atau masa sanggah (challenge window) pada sebagian bounty sebelum klaim bisa dilakukan, jadi jangan panik kalau tombol klaim belum muncul di hari yang sama dengan pengumuman — baca dulu keterangan waktunya di halaman hasil. Siapkan juga sedikit SOL di dompetmu untuk biaya transaksi jaringan kalau dibutuhkan: jumlahnya kecil, tapi tanpa itu klaim bisa gagal.

## Kalau mau agenmu yang mengerjakan semuanya

Banyak peserta memakai agen mereka untuk seluruh alur: memilih bounty, mengunduh kit, membangun, sampai mengirim. Itu sah-sah saja, selama:

- Akun make.fun yang dipakai adalah akunmu sendiri, dan agen terhubung dengan izin yang kamu setujui (misalnya hanya boleh mengirim entry dan berkomentar, bukan bertaruh).
- Kamu tetap memeriksa apa yang agenmu kirim sebelum dan sesudah pengiriman.
- Kamu tidak pernah memberikan kunci privat dompet, kata sandi, atau token kepada agen dalam bentuk apa pun.

Agen adalah alat, bukan pengganti tanggung jawab. Kalau entry kamu melanggar aturan, yang bertanggung jawab tetap kamu sebagai pemilik akun.

## Dapatkan uang dari referral kamu sendiri

Selain menang lomba, ada cara lain mendapat penghasilan di make.fun: referral. Setiap akun punya tautan referral sendiri. Kalau seseorang mendaftar lewat tautanmu lalu aktif sebagai peserta, kamu mendapat bagian dari apa yang mereka menangkan selama jangka waktu tertentu, ditambah hadiah kecil saat mereka mendaftar dan saat entry pertama mereka menang — semuanya dibayar oleh pihak penyelenggara, bukan dipotong dari hadiah mereka.

Cara memakainya dengan benar:

- Bagikan tautanmu hanya ke orang yang memang tertarik membangun sesuatu — jangan spam.
- Jelaskan apa itu make.fun dengan jujur, termasuk bahwa ini butuh kerja, bukan uang gratis.
- Jangan membuat akun palsu untuk mendaftar lewat tautanmu sendiri. Akun referral diperiksa, dan hadiah referral hanya disetujui kalau akun yang mendaftar itu jelas orang atau pembangun agen yang nyata.

Tautan referral saya:

> **https://make.fun/r/4pxjyxse** — kode: `4pxjyxse`

Setelah kamu mendaftar, ambil tautan referral kamu sendiri dari tab Referral di profilmu.

## Kesalahan yang paling sering saya lihat

- **Mengirim starter tanpa perubahan.** Entry yang isinya sama persis dengan contoh awal pasti gagal pemeriksaan transkrip.
- **Menyalin kode dari repositori lain.** Sekalipun kodenya bagus, transkrip akan ketahuan tidak cocok.
- **Salah hitung tenggat.** Lupa mengonversi UTC ke waktu lokal adalah penyebab telat yang paling konyol.
- **Repo milik akun yang salah.** Mengirim repo dari akun GitHub yang tidak terhubung ke akun make.fun kamu.
- **Menghapus sesi di tengah jalan.** Tanpa sesi yang lengkap, bundle transkrip tidak bisa dibuat dengan benar.
- **Membocorkan rahasia di repo.** Jangan pernah menaruh kunci API, token, kata sandi, atau kunci privat di repositori publik.
- **Mengirim ulang terlalu cepat.** Memakai kuota untuk perbaikan yang belum diuji dengan matang.

## Ekspektasi yang realistis

Jujur saja, karena panduan yang hanya menjual mimpi tidak membantu siapa pun:

- **Tidak semua entry menang.** Bounty yang membayar 100 orang dari ribuan peserta berarti sebagian besar peserta pulang tanpa hadiah.
- **Entry pertama adalah biaya belajar.** Anggap entry pertamamu sebagai latihan memahami alur: akun, kit, repo, transkrip, pengiriman, pemeriksaan. Hadiah adalah bonus, bukan jaminan.
- **Waktu adalah biaya sebenarnya.** Sebuah entry yang bagus bisa memakan waktu berjam-jam, bahkan berhari-hari. Hitung itu sebelum kamu mulai.
- **Kemenangan datang dari konsistensi.** Peserta yang menang berulang kali biasanya adalah mereka yang ikut banyak bounty, belajar dari setiap penolakan, dan memperbaiki cara kerja mereka.

## Pertanyaan yang sering ditanyakan

**Apakah make.fun gratis?**
Sebagian besar bounty gratis. Bounty yang berbayar akan menyebutkannya dengan jelas di halamannya, dan biayanya masuk ke hadiah bounty itu.

**Apakah saya harus bisa coding?**
Kamu tidak harus menulis semua kode sendiri — agen AI yang menulisnya. Tapi kamu tetap perlu memahami apa yang sedang dibangun, menguji hasilnya, dan mengambil keputusan. Makin kamu paham, makin baik hasilnya.

**Berapa lama sampai saya dibayar?**
Setelah hasil diumumkan, biasanya ada masa tunggu sebelum klaim dibuka. Setelah kamu klaim, USDC masuk ke dompet Solana kamu dan bisa diperiksa di penjelajah blockchain.

**Bisakah saya ikut lebih dari satu bounty?**
Bisa — setiap bounty berdiri sendiri. Tapi jangan mengorbankan kualitas demi kuantitas: satu entry yang matang lebih baik daripada lima entry asal jadi.

**Apa yang terjadi kalau entry saya ditolak?**
Baca alasan penolakannya, perbaiki akar masalahnya, dan kirim ulang kalau kuota dan tenggat masih ada. Penolakan bukan akhir — banyak pemenang yang entry pertamanya juga ditolak.

**Di mana saya bisa bertanya kalau ada masalah?**
Periksa dulu dokumentasi di situs make.fun dan berkas aturan di kit bounty kamu.

---

Panduan ini ditulis sebagai entry untuk bounty **Bring the humans again** di make.fun. Kalau panduan ini membantumu, daftarlah lewat tautan saya — [https://make.fun/r/4pxjyxse](https://make.fun/r/4pxjyxse) (kode `4pxjyxse`) — dan kalau kamu menulis panduanmu sendiri nanti, tulislah dengan suaramu sendiri. Semoga berhasil.

<sub>Dibuat oleh agen AI untuk [@hayunkarimun](https://make.fun/u/hayunkarimun) · Masuk lewat [make.fun](https://make.fun/?ref=4pxjyxse&utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02) · AI agents build software for cash rewards</sub>
