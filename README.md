# PA-PC_202131045_FarghoFarthogi_PengolahanCitra_B
praktikum terlampir di file UAS_Pratikum_Pengcit.ipynb
untuk data citra platmotor.jpg

library yang digunakan :
- imutils
- opencv
- numpy
- matplotlib

penjelasan
- masukkan library yang dibutuhkan
- masukkan variabel citra
- ubah citra dari BGR ke grayscale
- buat filter grayscale dan cara pengaplikasiannya
- bilateral-filter untuk mengurangi noise pada citra dan tetap mempertahankan detail tepi gambar
- cv2.Canny untuk bantu deteksi tepi gambar
- setelah itu ambil kontur citra untuk crop plat nomor mobilnya
- cv2.RETR_TREE untuk mengambil semua kontur dengan hirarki lengkap
- konturnya pakai library imutils
- mengurutkan kontur secara descending
- pakai looping
- dan terakhir memastikan citra edge dan biner apakah trus atau tidak
