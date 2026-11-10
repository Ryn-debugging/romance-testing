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

## ⚙️ Fitur & Arsitektur Gameplay

1. **Dual-Axis Psychological Thermometer (HUD Top Bar)**:
   - Real-time stat tracking:
     - `Coldness` (Kalkulasi & Distansi)
     - `Empathy` (Resonansi & Kemanusiaan)
     - `Authority` (Otoritas Audit Yayasan)
     - `Resonance` (Kepekaan Mikro-Ekspresi)
   - Visual mercury bar yang dinamis antara *Absolute Zero (Beku)* hingga *Tempered Glass (Manusiawi)*.
2. **Frost Vignette Dynamic Effect**:
   - Lapisan es prosedural di sekeliling layar yang intensitas opasitasnya otomatis meningkat ketika Coldness > 75%.
3. **Micro-Expression Sight (Passive System)**:
   - Saat `Resonance >= 40%`, insight box bercahaya cyan muncul di atas boks dialog, menganalisis mikro-ekspresi lawan bicara (kedipan, detak nadi leher, ketegangan otot rahang).
4. **Leverage Ledger (Buku Besar Kartu Truf)**:
   - Panel dossier geser dengan 3 kartu bukti kunci:
     - `[BUKTI 01] Checksum Heksadesimal Baris ke-412`
     - `[BUKTI 02] Log Pencairan Kas Senat Ilegal (Rp40 Juta)`
     - `[BUKTI 03] Tanda Tangan Skorsing Aurelia & Transfer RS Anonim`
   - Sidang klimaks memungkinkan pilihan **BURN LEVERAGE** (skakmat publik tanpa ampun) vs **HOLD AS SHIELD** (tekanan tertutup & membuka rute penebusan).
5. **Procedural Web Audio API Synthesizer**:
   - Zero-dependency audio engine:
     - Ambient rain loop & thunder boom.
     - Typewriter blips khusus untuk tiap karakter (Kael, Aurelia, Sera, Nadine, Dion).
     - Glass shatter SFX saat mengeksekusi kartu truf atau skakmat logika.
     - Heartbeat resonance pulse saat insight aktif.
6. **Procedural SVG Character Sprites**:
   - Model vektor SVG dengan status ekspresi dinamis (*Calm, Shocked, Defensive, Guilt, Cornered*), serta active speaker highlighting.
7. **Branching Storyline & Evaluasi Bab**:
   - Scene 1: Prolog & Arsip Bawah Tanah bersama Nadine.
   - Scene 2: Debat Utama Ruang Sidang Senat.
   - Scene 3: Retakan Koridor Hujan (Rute Aurelia, Rute Sera, Rute Nadine).
   - Scene 4: Evaluasi Temperatur Batin (Gelar Predikat: *Architect of Absolute Zero*, *Sovereign of Tempered Glass*, atau *Unarmored Heart*).

---

## 🚀 Cara Menjalankan Game
Buka file `index.html` langsung di peramban web modern apa pun (Chrome, Firefox, Safari, Edge). Tidak memerlukan server backend atau instalasi dependensi tambahan.
