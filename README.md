# Sesi 2 — Enkapsulasi dan Penjagaan Invariant

Proyek ini merupakan latihan Pemrograman Berorientasi Objek (OOP) yang berfokus pada enkapsulasi dan penjagaan invariant (kondisi yang harus selalu bernilai benar) pada sebuah kelas domain `Mahasiswa`.

---

## 📌 Deskripsi Masalah

Sistem akademik mencatat data mahasiswa yang terdiri dari:
* **NIM** (Nomor Induk Mahasiswa)
* **Nama** Mahasiswa
* **Tiga Komponen Nilai:** Tugas, UTS, dan UAS

### Aturan & Invariant:
1. **NIM Tidak Boleh Berubah (Immutable):** NIM tidak pernah diubah setelah objek mahasiswa terbuat.
2. **Identitas Wajib Valid:** NIM dan Nama tidak boleh bernilai `null`, kosong, atau hanya berisi spasi.
3. **Komponen Nilai Valid:** Setiap komponen nilai (Tugas, UTS, UAS) berada dalam rentang inklusif **0 hingga 100**.
4. **Bobot Penilaian Tetap:** 
   * **Tugas:** 30% (`0.30`)
   * **UTS:** 30% (`0.30`)
   * **UAS:** 40% (`0.40`)
5. **Aturan Huruf Mutu:**
   * $\ge 80 \rightarrow$ **A**
   * $\ge 70 \rightarrow$ **B**
   * $\ge 60 \rightarrow$ **C**
   * $\ge 50 \rightarrow$ **D**
   * $< 50 \rightarrow$ **E**

---

## 📁 Struktur Berkas

```text
.
├── Mahasiswa.java    # Implementasi kelas Mahasiswa (Java)
├── Mahasiswa.php     # Implementasi kelas Mahasiswa (PHP 8+)
├── Main.java         # Program uji / Main driver (Java)
├── analisis.md       # Analisis detail invariant
└── README.md         # Dokumentasi petunjuk proyek