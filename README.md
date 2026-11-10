# GLASS CORONATION: Titik Beku di Bawah Menara Gading

Sebuah game web **Visual Novel & Social-Strategy RPG** interaktif dengan estetika **Dark Academia x Frosted Glassmorphism**, dibangun dengan teknologi web native (HTML5, CSS3, Vanilla JS, Web Audio API, SVG procedural sprites, dan HTML5 Canvas).

---

## ❄️ Ringkasan Naratif & Premis
> *"Kamu merindukan orang yang dulu bisa kamu injak-injak? Sayang sekali, dia sudah mati karena kebaikan hatinya sendiri. Sekarang, bicaralah dengan urusan yang jelas atau silakan pergi."*

Enam bulan lalu, **Kaelen Vance (Kael)** dikorbankan demi menyelamatkan reputasi busuk Senat Mahasiswa. Beasiswanya dicabut, kodenya dicuri, dan ibunya terbaring koma di ruang ICU. Hari ini, ia kembali melangkah ke lantai empat Menara Gading bukan sebagai pemohon, melainkan sebagai **Special Auditor Dewan Pembina Yayasan** dengan mandat audit investigatif dan wewenang mutlak untuk membekukan kekuasaan mereka.

---

## 🏛️ Karakter Utama & Heroine

1. **Kaelen "Kael" Vance** (*Protagonist / Special Auditor*)
   - Menguasai kalkulasi dingin dan kepekaan mikro-ekspresi.
   - Pilihan pemain mengkalibrasi suhu batinnya antara *Titik Beku (Coldness)* dan *Empati (Humanity)*.

2. **Aurelia Vanya Rajasa** (*Ketua Komisi Etik Senat — "The Complicit Bystander"*)
   - Putri aristokrat akademik yang mematuhi sistem demi melindungi keluarganya.
   - Menyimpan rasa bersalah mendalam: diam-diam membayar biaya ICU ibu Kael secara anonim.

3. **Seraphina "Sera" Kirana** (*Bintang Debat Fakultas — "The Defector"*)
   - Retorika tajam dan ambisius. Membelot ke faksi Dion demi medali dan pengakuan, namun terancam hancur ketika kode curiannya terbongkar.

4. **Nadine Larasati** (*Penjaga Arsip Forensik Data — "The Mirror"*)
   - Sahabat setia Kael di rubanah server bawah tanah. Penjaga kunci bukti sekaligus jangkar moral agar Kael tidak berubah menjadi monster sepenuhnya.

5. **Dion Pratama** (*Ketua BEM Fakultas / Antagonis Utama*)
   - Sosok politisi kampus licik yang merancang penyelewengan dana kas senat Rp40 Juta dan penjebakan Kael.

---

## ⚙️ Fitur & Arsitektur Gameplay (Expanded Edition)

1. **Dual-Axis Psychological Thermometer (HUD Top Bar)**:
   - Real-time stat tracking:
     - `Coldness` (Kalkulasi & Distansi)
     - `Empathy` (Resonansi & Kemanusiaan)
     - `Authority` (Otoritas Audit Yayasan)
     - `Resonance` (Kepekaan Mikro-Ekspresi)
   - Visual mercury bar yang dinamis antara *Absolute Zero (Beku)* hingga *Tempered Glass (Manusiawi)*.

2. **Peta Kampus Universitas Mahakarya Pradipta (Day/Night Action Phase)**:
   - Muncul setelah Scene 3 berakhir, menjelang Sidang Hari Jumat.
   - Pemain memiliki **3 Action Points (AP)** per hari untuk mengunjungi 4 lokasi strategis:
     - **Ruang Komisi Etik (Lantai 3)**: Berinteraksi dengan Aurelia Vanya, membuka celah regulasi (+10 Otoritas).
     - **Podium Debat Fakultas**: Berinteraksi dengan Seraphina Kirana, mendapatkan rekaman tekanan Dion (+15 Resonansi).
     - **Ruang Server Arsip Tua (Rubanah B2)**: Menikmati teh chamomile bersama Nadine, memulihkan ketenangan batin (+15 Empati).
     - **Ruang Kantor Dekanat**: Investigasi senyap brankas dokumen rahasia, membuka **`[BUKTI 04] Draft Kontrak Konsorsium Gelap Rektorat & PT Pradipta Digital (Rp1.2 Miliar)`**.

3. **Debate Battle Turn-Based (Sidang Dewan Komisaris Hari Jumat)**:
   - Pertarungan retorika turn-based melawan **Dion Pratama** di hadapan Dewan Komisaris dan Senat.
   - Bar **Kredibilitas Dion (100 HP)** vs **Ketenangan Kaelen (100 HP)**.
   - Patahkan 3 argumen manipulasi Dion:
     - **Ronde 1**: Argumen fitnah dendam personal -> dipatahkan dengan `[BUKTI 02]` Log Kas Rp40 Juta atau Serangan Otoritas.
     - **Ronde 2**: Argumen kambing hitam terhadap Seraphina -> dipatahkan dengan `[BUKTI 01]` Checksum Baris 412 atau Bedah Resonansi (Stun).
     - **Ronde 3**: Ancaman patronase dinasti yayasan -> dipatahkan dengan `[BUKTI 04]` Kontrak Konsorsium Gelap.
   - Pilihan aksi:
     - `[OTORITAS]`: Serangan Statuta Audit Yayasan (-25 s/d -35 HP).
     - `[RESONANSI]`: Bedah Mikro-Ekspresi & Stun Turn (-20 HP).
     - `[KARTU TRUF]`: Skakmat mutlak menggunakan bukti spesifik (-50 s/d -60 HP CRITICAL).

4. **Frost Vignette Dynamic Effect**:
   - Lapisan es prosedural di sekeliling layar yang intensitas opasitasnya otomatis meningkat ketika Coldness > 75%.

5. **Micro-Expression Sight (Passive System)**:
   - Saat `Resonance >= 40%`, insight box bercahaya cyan muncul di atas boks dialog dan arena debat, menganalisis bahasa tubuh lawan bicara secara presisi.

6. **Leverage Ledger (Buku Besar Kartu Truf)**:
   - Panel dossier geser dengan 4 bukti kunci:
     - `[BUKTI 01] Checksum Heksadesimal Baris ke-412`
     - `[BUKTI 02] Log Pencairan Kas Senat Ilegal (Rp40 Juta)`
     - `[BUKTI 03] Tanda Tangan Skorsing Aurelia & Transfer RS Anonim`
     - `[BUKTI 04] Draft Kontrak Konsorsium Gelap Rektorat & PT Pradipta Digital`

7. **Procedural Web Audio API Synthesizer**:
   - Zero-dependency audio engine: Ambient rain & thunder, distinct typewriter blips, glass-shatter SFX, heartbeat pulse, and UI chimes.

8. **Scene Jump & Replayability**:
   - Menu *Scene Jump* memungkinkan pengujian instan ke:
     - Scene 1: Bayangan di Balik Kaca (Prolog)
     - Scene 2: Variabel Keempat yang Hilang (Sidang Awal)
     - Scene 3: Retakan di Koridor Hujan (Heroine Hub)
     - Peta Kampus: Day/Night Action Phase (3 AP)
     - Sidang Jumat: Debate Battle Turn-Based (vs Dion)
     - Scene 4: Evaluasi Temperatur Batin (Ending Report)

---

## 🚀 Cara Menjalankan Game
Buka file `index.html` langsung di peramban web modern apa pun (Chrome, Firefox, Safari, Edge). Tidak memerlukan server backend atau instalasi dependensi tambahan.
