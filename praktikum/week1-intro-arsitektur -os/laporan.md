Laporan Praktikum Minggu [1]
Topik:Arsitektur Sistem Operasi

Identitas
Nama :Ahmad Wildan Asrovi
NIM :250202927
Kelas :1IKRB
Tujuan
Tuliskan tujuan praktikum minggu ini.
Setelah menyelesaikan tugas ini, mahasiswa mampu:

1.Menjelaskan peran sistem operasi dalam arsitektur komputer.
2.Mengidentifikasi komponen utama OS (kernel, system call, device driver, file system).
3.Membandingkan model arsitektur OS (monolithic, layered, microkernel).
4.Menggambarkan diagram sederhana arsitektur OS menggunakan alat bantu digital (draw.io / mermaid).

Dasar Teori
Tuliskan ringkasan teori (3–5 poin) yang mendasari percobaan.

Langkah Praktikum
Langkah-langkah yang dilakukan.
Perintah yang dijalankan.
File dan kode yang dibuat.
Commit message yang digunakan.
Kode / Perintah
Tuliskan potongan kode atau perintah utama:

uname -a
lsmod | head
dmesg | head
Hasil Eksekusi
Sertakan screenshot hasil percobaan atau diagram: Screenshot hasil

Analisis
Jelaskan makna hasil percobaan.
Hubungkan hasil dengan teori (fungsi kernel, system call, arsitektur OS).
Apa perbedaan hasil di lingkungan OS berbeda (Linux vs Windows)?
Kesimpulan
Tuliskan 2–3 poin kesimpulan dari praktikum ini.

Quiz 

jawaban:
Manajemen Sumber Daya
Manajemen Proses dan File 
serta Penyediaan Antarmuka Pengguna

jawaban:
mode kernel memiliki akses penuh ke perangkat keras dan memori, sedangkan mode pengguna memiliki akses terbatas untuk menjaga stabilitas dan keamanan sistem

Jawaban:
monolithickernel
Linux, UNIX, MS-DOS, dan Mac OS
microkernel
QNX, Minix, AmigaOS, HarmonyOS, HelenOS, dan Zirkon

tugas:

Monolithic kernel

Monolithic kernel adalah kernel sistem operasi yang semua layanan sistem operasinya berjalan di ruang kernel, artinya semuanya berbagi ruang memori yang sama. Jenis kernel ini dicirikan oleh integrasi layanan sistem yang erat dan kinerjanya yang tinggi.
Contoh sistem yang menggunakan Monolithic kernel:
•	Linux
•	UNIX
•	MS-DOS 
•	Mac OS.

Microkernel

mikrokernel merupakan seperangkat perangkat lunak dalam jumlah minimum yang meyediakan beragam mekanisme dasar yang dibutuhkan untuk bekerja sebagai sebuah sistem operasi, seperti halnya manajemen pengalamatan ruang tingkat rendah, manajemen thread, dan komunikasi dan proses. Dalam implementasinya mikrokernel merupakan satu-satunya perangkat lunak yang berjalan dengan tingkat kewenangan tertinggi (umumnya disebut sebagai modus supervisor atau modus kernel) dari serangkaian level kewenangan yang tersedia pada perangkat kerasnya. Layanan yang disediakan oleh sebuah sistem operasi beberapa diantaranya adalah device driver, protokol jaringan, sistem berkas, dan kode antarmuka pengguna yang berada dalam ruang pengguna.
Mikrokernel sangat erat terkait dengan exokernel, serta memiliki banyak kesamaan dengan hypervisor. namun implementasinya lebih bersifat minimalis, dan secara spesifik untuk mendukung pengimplementasian mesin virual. Mikrokernel L4 sering juga disebut sebagai hypervisor, yang mengindikasikan kemungkinan pengimplementasian sebuah mikrokernel sebagai hypervisor. Istilah nanokernel dalam sejarahnya digunakan untuk membedakan mikrokernel saat ini dengan istilah mikrokernel sebelumnya yang menyediakan layanan sistem aktual, tetapi secara prinsip minimalitas menurut Jochen Liedtke dalam disain mikrokernel L4 menyebutkan bahwa istilah-istilah tersebut memiliki arti yang kurang lebih sama.
Contoh sistem yang menggunakan microkernel:
•	QNX
•	Minix
•	AmigaOS
•	HarmonyOS
•	HelenOS
•	Zirkon

Layered Architecture

Layered Architecture membagi aplikasi perangkat lunak menjadi beberapa lapisan horizontal , dengan setiap lapisan berfokus pada tanggung jawab tertentu. Lapisan-lapisan tersebut bekerja sama untuk memproses data, menangani logika bisnis, dan berinteraksi dengan pengguna, memastikan bahwa tidak ada satu lapisan pun yang memikul semua tanggung jawab.
Layered Architecture, juga dikenal sebagai arsitektur n-tier, adalah pola desain yang mengorganisasikan sistem perangkat lunak ke dalam serangkaian lapisan horizontal. Setiap lapisan memiliki tanggung jawab spesifik dan hanya berkomunikasi dengan lapisan yang berdekatan. Pemisahan tugas merupakan prinsip utama, yang memudahkan pemahaman, pemeliharaan, dan perluasan sistem.
Contoh sistem yang menggunakan:
•	Unix
•	Linux
•	Android

Model kernel monolitik, yang dicontohkan oleh kernel linex, adalah yang paling relevan untuk sistem modern karena menawarkan efisiensi dan kinerja tinggi, meskipun desainnya lebih kompleks dibandingkan mikrokernel. Kernel monolitik mengintegrasikan sebagian besar layanan sistem dalam satu ruang kernel besar, namun keandalannya telah ditingkatkan secara signifikan melalui driver dan sistem operasi yang matang. 

•	Untuk Pengguna Umum dan Bisnis:
•	Microsoft Windows: Sistem operasi paling populer untuk PC, menawarkan antarmuka visual yang mudah digunakan, perangkat lunak bawaan yang melimpah, dan pembaruan keamanan yang sering. Cocok untuk pengguna rumahan, usaha kecil, dan korporasi. 
•	Untuk Kreator dan Pengguna Apple:
•	Apple macOS: Dikembangkan khusus untuk produk Apple seperti MacBook dan iMac, menawarkan antarmuka yang ramping, performa yang dioptimalkan, dan ekosistem yang terhubung. 
•	Untuk Pengembang dan Server:
•	Linux: Sebuah OS open-source yang dikenal karena fleksibilitas, stabilitas, dan keamanan. Sangat populer untuk server, lingkungan cloud, dan pengembangan aplikasi. 
•	Red Hat Enterprise Linux (RHEL): Distribusi Linux yang banyak digunakan di lingkungan perusahaan dan cloud karena stabilitas, keamanan, dan dukungan perusahaan yang kuat. 

•	Untuk Perangkat Seluler:
•	Android: Sistem operasi paling populer di dunia, terutama untuk smartphone dan tablet, dengan akses ke banyak aplikasi melalui Google Play Store. 
•	iOS: Sistem operasi eksklusif untuk perangkat Apple seperti iPhone, dikenal karena pengalaman pengguna yang mulus dan ekosistem yang terintegrasi. 

Jawaban:
Refleksi Diri
Tuliskan secara singkat:

Apa bagian yang paling menantang minggu ini?
Bagaimana cara Anda mengatasinya?

Credit:
Template laporan praktikum Sistem Operasi (SO-202501) – Universitas Putra Bangsa
