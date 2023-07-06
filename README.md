# PA-PC_202131045_FarghoFarthogi_PengolahanCitra_B
praktikum terlampir di file UAS_Pratikum_Pengcit.ipynb
untuk data citra platmotor.jpg

Berikut adalah beberapa konsep yang dapat digunakan:

1. Segmentasi Citra: Segmentasi adalah proses memisahkan objek dari latar belakang dalam citra. Dalam konteks deteksi plat nomor, langkah pertama adalah segmentasi citra untuk memisahkan plat nomor dari latar belakangnya. Teknik segmentasi seperti metode berbasis ambang (thresholding) atau pengolahan morfologi dapat digunakan.

2. Deteksi Tepi: Deteksi tepi adalah proses untuk menemukan perbedaan intensitas piksel yang signifikan di sepanjang kontur objek. Dalam deteksi plat nomor, deteksi tepi dapat membantu dalam mengidentifikasi kontur plat nomor. Algoritma populer untuk deteksi tepi meliputi Operator Sobel, Operator Prewitt, atau Operator Canny.

3. Transformasi Hough: Transformasi Hough adalah metode yang digunakan untuk mendeteksi objek berdasarkan pola atau bentuk geometrisnya. Dalam deteksi plat nomor, Transformasi Hough dapat digunakan untuk mendeteksi garis-garis lurus pada citra yang mungkin mewakili batas plat nomor.

4. Pemrosesan Citra Biner: Setelah plat nomor terdeteksi, dapat dilakukan pemrosesan citra biner untuk meningkatkan kualitas deteksi. Metode pengolahan biner seperti dilatasi, erosi, penghilangan noise, atau operasi morfologi lainnya dapat diterapkan untuk meningkatkan kualitas gambar biner dari plat nomor.

5. Pengenalan Karakter: Setelah plat nomor terdeteksi dan diolah, langkah selanjutnya adalah pengenalan karakter. Metode pengenalan karakter dapat beragam, mulai dari pendekatan berbasis template hingga pendekatan berbasis pembelajaran mesin seperti Jaringan Saraf Tiruan (Neural Network) atau metode berbasis Klasifikasi seperti Support Vector Machine (SVM).

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
