# A. Setting SSID dan Password Wi-Fi ESP32 melalui Web Server

## 1. Alat dan Bahan
1) ESP32
2) Arduino IDE

## 2. Source Code

![alt text](https://github.com/rayabima/Embedded-System/blob/main/Media/Penjelasan%20Kode.jpeg?raw=true)

## 3. Flowchart
![alt text](https://github.com/rayabima/Embedded-System/blob/main/Media/Flow%20Chart.png?raw=true)


## 4. Hasil dan Pembahasan
## Jika gagal terhubung
![alt text](https://github.com/rayabima/Embedded-System/blob/main/Media/3.%20serial%20monitor%20setelah%20memasukan%20ssid%20dan%20pass.jpeg?raw=true)

## Jika berhasil terhubung
![alt text](https://github.com/rayabima/Embedded-System/blob/main/Media/4.%20Serial%20Monitor%20Setelah%20Berhasil%20Terhubung.jpeg?raw=true)

### Pembahasan Kode
#### **Fungsi Utama Kode:**

  * Menghubungkan perangkat ke jaringan WiFi.
  * Memberikan opsi untuk mengubah kredensial WiFi melalui halaman web jika koneksi gagal.

#### **Penjelasan Alur Kode:**
  1. Setup Awal:
  * Memulai komunikasi serial untuk monitoring.
  * Menginisialisasi EEPROM untuk penyimpanan data.
  * Membaca kredensial WiFi yang tersimpan di EEPROM.
  * Mencoba menghubungkan ke WiFi menggunakan kredensial tersebut.

  2. Loop Utama:
  * Jika terkoneksi ke WiFi:
    * Mencetak pesan konfirmasi koneksi.
  * Jika tidak terkoneksi ke WiFi:
    * Mengecek status tombol untuk memaksa mode AP (Access Point).
    * Jika tombol tidak ditekan dan koneksi gagal, memulai mode AP dan membuat halaman web untuk konfigurasi WiFi.
    * Menunggu hingga terkoneksi ke WiFi.

  3. Fungsi testWifi:
  * Mencoba menghubungkan ke WiFi selama 10 detik.
  * Mengembalikan nilai 'true' jika terkoneksi, 'false' jika tidak.

  4. Fungsi launchWeb:
  * Mencetak informasi IP address perangkat (local dan softAP jika ada).
  * Menjalankan fungsi createWebServer untuk membuat halaman web konfigurasi WiFi.

  5. Fungsi setupAP:
  * Mengatur perangkat sebagai Access Point (AP) dengan nama "MiSREd IoT".
  * Mencari jaringan WiFi di sekitar dan menyimpan daftarnya dalam variabel st.
  * Menjalankan fungsi launchWeb untuk menampilkan halaman konfigurasi WiFi.

  6. Fungsi createWebServer:
  * Menangani permintaan ke halaman web:
    * '/' : Menampilkan halaman utama dengan daftar jaringan WiFi yang ditemukan dan formulir untuk memasukkan kredensial WiFi baru.
    * '/scan' : Memindai ulang jaringan WiFi dan menampilkan hasilnya.
    * '/setting' : Menerima kredensial WiFi baru, menyimpannya ke EEPROM, dan me-restart perangkat.
  
### Kesimpulan:
Kode ini dirancang untuk memudahkan konfigurasi WiFi pada perangkat dengan menyediakan antarmuka web yang dapat diakses dari perangkat lain. Pengguna dapat mengubah kredensial WiFi tanpa perlu mengubah kode secara langsung.

