# Langkah-langkah Menjalankan Program Input Nilai Mahasiswa

1'Buka VS Code
Jalankan aplikasi Visual Studio Code di komputer kamu.

2'Buka Folder Proyek
Klik File → Open Folder, lalu pilih folder tempat kamu menyimpan tugas, misalnya PRAKTIKUM 4.

3.Buat File Program
4.Klik New File, beri nama praktikum4.py
(hindari spasi pada nama file).

4.Tulis Kode Program
Salin kode berikut ke dalam file:
data_mahasiswa = []

while True:
    print("\n=== Input Data Mahasiswa ===")
    nama = input("Masukkan nama mahasiswa: ")
    tugas = float(input("Masukkan nilai Tugas: "))
    uts = float(input("Masukkan nilai UTS: "))
    uas = float(input("Masukkan nilai UAS: "))

    nilai_akhir = (tugas * 0.30) + (uts * 0.35) + (uas * 0.35)

    data_mahasiswa.append({
        "nama": nama,
        "tugas": tugas,
        "uts": uts,
        "uas": uas,
        "akhir": nilai_akhir
    })

    if len(data_mahasiswa) == 2:
        print("\nData dua mahasiswa telah dimasukkan.")
        break

print("\n=== Daftar Nilai Mahasiswa ===")
print(f"{'Nama':<15}{'Tugas':<10}{'UTS':<10}{'UAS':<10}{'Nilai Akhir':<10}")
print("-" * 55)

for mhs in data_mahasiswa:
    print(f"{mhs['nama']:<15}{mhs['tugas']:<10}{mhs['uts']:<10}{mhs['uas']:<10}{mhs['akhir']:<10.2f}")

print("\nProgram selesai.")

5.Simpan File
Tekan Ctrl + S untuk menyimpan.

6.Buka Terminal di VS Code
Tekan Ctrl + ` (tombol di bawah ESC).

7.Jalankan Program
Ketik perintah:

python praktikum4.py

lalu tekan Enter.

8.Masukkan Data Mahasiswa
Isikan nama dan nilai sesuai instruksi di terminal (contoh: Milan dan Nugroho).

9.Lihat Hasil
Setelah dua data dimasukkan, hasil tabel nilai akan muncul di terminal.

10.Buat README.md

*Klik New File lagi.

*Simpan dengan nama README.md.

*Isi dengan deskripsi singkat, rumus, dan langkah di atas.



