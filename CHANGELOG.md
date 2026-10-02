# Changelog Proyek Terjemahan Umineko no Naku Koro ni — Bahasa Indonesia
Dokumentasi pembaruan naskah, lokalisasi, perbaikan sintaks, dan stabilisasi teknis untuk visual novel *Umineko When They Cry* oleh **LARUS Team**.

---

## [Milestone 2.0.0] - 2026-10-02

### 🌟 Ringkasan Pembaruan Utama
- **Stabilisasi & Audit Mutu Menyeluruh Episode 1 s.d. Episode 5**: Sebanyak **97 file naskah script (76.837 baris dialog/narasi)** telah tuntas diaudit, di-QA/QC, dan divalidasi dengan pencapaian **100% PASS (0 Fatal Syntax Error, 0 Tag Mismatch)**.
- **Penerjemahan Penuh Segmen Kritis**:
  - **Episode 2 Bab 15**: Penerjemahan tuntas segmen klimaks konfrontasi Rosa dan Beatrice (82 baris naskah penting).
  - **Episode 5 Bab 3**: Penerjemahan tuntas pembantaian ruang tamu dan pembuka misteri (578 baris naskah sastrawi berstandar tinggi).
- **Rekonsiliasi Bug Teknis Tingkat Engine**:
  - Memperbaiki *line split drift* pada `umi4_2.txt` yang sebelumnya menggeser 874 baris dialog.
  - Memperbaiki kurung kurawal Blue Truth yang tidak tertutup pada naskah komersial MangaGamer (`umi5_17.txt`) berdasarkan naskah asli Jepang.
  - Mengembalikan karakter kanji dan furigana asli teka-teki emas pada `umi5_5.txt`.
- **Konsistensi Glosarium Kanon**:
  - Penyeragaman istilah dunia cerita: *Furnitur* (bukan *perabot*), *Tanah Emas* (*Golden Land*), *Elang Bersayap Satu*, *Penyihir Emas*, *Penyihir Tak Berujung*, *teater*, *epitaf*, dan catchphrase Battler (*"sama sekali tidak berguna"* / *"it's no good, it's no use at all"*).

---

### 📘 Episode 1: Legenda Penyihir Emas (*Legend of the Golden Witch*)
- **Status Validasi**: ✅ **100% PASS (20 File / 14.108 Baris Script)**.
- **Perbaikan Sintaks & Markup**:
  - Menghilangkan spasi berlebih dan trailing whitespace di luar pembungkus backtick (`` `...` ``) di seluruh chapter.
  - Memverifikasi arsitektur engine pada `umi1_17.txt` (0 byte yang valid sebagai penanda rotasi grafis internal ONScripter).
  - Menyelaraskan seluruh tag warna (`{c:...}`), tag font (`{f:...}`), dan kurung kurawal dialog Kinzo, Beatrice, Battler, Shannon, dan Kanon.
- **Penyelarasan Glosarium**: Menyeragamkan panggilan kehormatan kepala keluarga menjadi *Tuan Besar* (*Lord Kinzo*).

---

### 📘 Episode 2: Kembalinya Penyihir Emas (*Turn of the Golden Witch*)
- **Status Validasi**: ✅ **100% PASS (21 File / 13.893 Baris Script)**.
- **Penerjemahan Segmen Selesai**:
  - Menyelesaikan penerjemahan 82 baris dialog yang tertinggal dalam bahasa Inggris pada Chapter 15 (`umi2_15.txt` baris 775–856), melengkapi momen klimaks pertarungan kehendak antara Rosa dan Beatrice.
- **Perbaikan Sintaks & Markup**:
  - Menyeimbangkan kurung kurawal kutipan dialog Beatrice pada `umi2_10.txt`.
  - Merestorasi tag warna nama panggilan Kanon `{c:86EF9C:Onii-chan}` pada `umi2_12.txt`.
  - Merestorasi tag visual teka-teki `{ruby:...}` dan `{c:...}`.

---

### 📘 Episode 3: Perjamuan Penyihir Emas (*Banquet of the Golden Witch*)
- **Status Validasi**: ✅ **100% PASS (16 Bab Selesai / 12.616 Baris Script)**.
  *(Bab 12–16 berstatus draf kerja komunitas)*.
- **Perbaikan Paritas & Line Drift**:
  - Menghapus baris kosong berlebih di akhir file pada `umi3_4.txt`, `umi3_5.txt`, dan `umi3_7.txt`, memulihkan paritas baris 1:1 sempurna terhadap naskah rujukan Inggris dan Jepang.
- **Restorasi Teka-teki & Parodi**:
  - `umi3_10.txt`: Merestorasi tag kanji anagram epitaf Eva Ushiromiya untuk ikan ayu `{ruby:kougyo:{p:0:香魚}}`, penghapusan huruf `{ruby:nuki:...}`, dan desa `{ruby:sato:{p:0:里}}` agar petunjuk pemecahan misteri dapat dipahami pemain.
  - `umi3_18.txt`: Merestorasi tag debat anime/galge/tsundere/yandere antara Battler dan Beatrice.
  - `umi3_9.txt`: Menyeimbangkan format kurung kurawal surat tantangan Beatrice.

---

### 📘 Episode 4: Aliansi Penyihir Emas (*Alliance of the Golden Witch*)
- **Status Validasi**: ✅ **100% PASS (22 File / 20.312 Baris Script)**.
  *(6 Bab Selesai Penuh: `umi4_op`, `umi4_1`, `umi4_2`, `umi4_10`, `umi4_11`, `umi4_12`)*.
- **Perbaikan Kritis Line Split Drift (`umi4_2.txt`)**:
  - Memperbaiki pemisahan baris tidak sengaja pada baris 68–69 yang sebelumnya mendesak tanda backtick ke baris baru dan menyebabkan **874 baris dialog di bawahnya bergeser 1 baris ke bawah**.
  - Merestorasi tag ruby auman boneka Sakutarou: `` ` Uryu-, {ruby:ngaum:gaooo}." ` `` (L639).
  - Memperbaiki typo dialog Maria & Sakutarou pada L644 (*Maria dan Sakutaro*).
- **Perbaikan Sintaks & Visual**:
  - `umi4_1.txt`: Merestorasi tag warna parodi pelari maraton Glico `{c:86EF9C:kotak karamel tertentu}` (L105).
  - `umi4_11.txt`: Memperbaiki tanda backtick hilang pada monolog obsesi Kinzo (L458) dan merestorasi tag warna distro 666 `{c:86EF9C:666}` (L1161).
  - `umi4_12.txt`: Menyelaraskan relasi karakter pada dialog pacar Rosa (mengubah *"merawat putri kita"* menjadi *"merawat putrimu"*).
  - `umi4_op.txt`: Proofreading komprehensif ejaan bahasa Indonesia sastrawi.
  - Stabilisasi seluruh tag ruby dan warna pada 16 bab draf komunitas lainnya (`umi4_3`–`umi4_9`, `umi4_13`–`umi4_21`).

---

### 📘 Episode 5: Akhir dari Penyihir Emas (*End of the Golden Witch*)
- **Status Validasi**: ✅ **100% PASS (18 File / 15.908 Baris Script)**.
  *(4 Bab Selesai Penuh: `umi5_op`, `umi5_1`, `umi5_2`, `umi5_3`)*.
- **Penerjemahan Penuh Chapter 3 (`umi5_3.txt`)**:
  - Menerjemahkan secara tuntas 578 baris naskah klimaks penemuan korban twilight pertama dengan akurasi sastrawi tinggi (**0 Error, 0 Warning**).
- **Penyelarasan Glosarium Bab 0–2**:
  - Menyeragamkan istilah *Furnitur Elang Bersayap Satu*, tag kuliner gyoza/xiaolongbao, dan catchphrase Battler.
- **Restorasi Teka-teki Kanji Epitaf (`umi5_5.txt`)**:
  - Memulihkan kanji kanon *Ougonkyou* (`黄金郷`) dan *Kampung Halaman / Sato* (`郷`) serta *Malam Pertama* (`第一の晩`).
- **Koreksi Sintaks Blue Truth MangaGamer (`umi5_17.txt`)**:
  - Menutup tanda kurung kurawal Blue Truth pada L1073 yang hilang pada naskah resmi bahasa Inggris berdasarkan rujukan naskah asli Jepang.
- **Penyelarasan Red Truth Jendela Cornelia (`umi5_12.txt`)**:
  - Menyelaraskan klausa kalimat agar tag Red Truth jendela tetap berada di baris 256 sinkron dengan timing suara.
- **Penyeimbangan Kurung Kurawal Red Truth Dlanor**:
  - Menyeimbangkan penutupan multiline Red Truth Dlanor pada `umi5_11.txt` dan `umi5_14.txt`.

---

## 🛠️ Standar Kualitas & Arsitektur
- **Paritas Baris**: 1:1 sempurna terhadap naskah bahasa Inggris dan Jepang.
- **Validasi Parsing**: Seluruh naskah lulus uji parser ONScripter-RU dan validator otomatis tim.
- **Integritas Format**: Pembungkus aksen nonjol (backtick) bersih tanpa spasi luar liar.
- **Manajemen Repositori**: Pemisahan ketat antara ruang kerja eksperimen (`umineko-idn-translation-work`) dan repositori resmi (`umineko-scripting-idn`).
