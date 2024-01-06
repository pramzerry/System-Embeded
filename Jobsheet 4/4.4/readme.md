# D. Akuisi Data dan Kendali Perangkat IoT Menggunakan Protokol MQTT

## 1. Keterangan Singkat (Abstrak)
<p align="justify">Dalam percobaan ini program ESP32 menggunakan protokol MQTT untuk mengakuisisi data sensor dan mengendalikan perangkat, seperti LED, melalui topik-topik MQTT. Setelah program diupload, dilakukan pemantauan melalui serial monitor dan dashboard Node-Red untuk mengendalikan nyala LED melalui tombol switch pada dashboard. Program yang kedua merupakan pengendalian LED ESP32 menggunakan layanan Adafruit MQTT, dalam hal ini pengendalian LED melalui dashboard yang ada di laman Adafruit.
   
## 2. Alat dan Bahan
1. Node-RED
2. Laman Adafruit
3. ESP32
4. Kabel jumper
5. LED
6. XAMPP

## 3. Source Code

![alt text](https://github.com/rayabima/Embedded-System/blob/main/Jobsheet%204/D.%20Akuisi%20Data%20dan%20Kendali%20Perangkat%20IoT%20Menggunakan%20Protokol%20MQTT/Media/Penjelasan%20Kode.jpeg?raw=true)

## 4. Flow Program
<img src="https://github.com/brianrahma/system-embedded/blob/master/jobsheet%204/B.%20Transmisi%20Data%20Menggunakan%20Protokol%20HTTP/flow%20program%20.png" width="800">

## 5. Hasil Percobaan Kontrol Nyala LED Melalui Dashboard Node-RED

1. Flow chart program ESP32
   
   <img src="https://github.com/brianrahma/system-embedded/assets/82065700/6d63519d-f4b5-4fc5-b70b-da925b0001ee" width="300">
   
2. Dokumentasi
   
   ![alt text](https://github.com/rayabima/Embedded-System/blob/main/Jobsheet%204/D.%20Akuisi%20Data%20dan%20Kendali%20Perangkat%20IoT%20Menggunakan%20Protokol%20MQTT/Media/2.%20Dokumentasi%201.jpeg?raw=true)

3. Debug Node-RED
   
   ![alt text](https://github.com/rayabima/Embedded-System/blob/main/Jobsheet%204/D.%20Akuisi%20Data%20dan%20Kendali%20Perangkat%20IoT%20Menggunakan%20Protokol%20MQTT/Media/3.%20Debug%20Node-RED.jpeg?raw=true)
   
4. Dashboard Node-RED
   
   <img src="https://github.com/brianrahma/system-embedded/blob/master/jobsheet%204/D.%20Akuisi%20Data%20dan%20Kendali%20Perangkat%20IoT%20Menggunakan%20Protokol%20MQTT/dashboard1.png" width="700">

## 6. Hasil Percobaan Kontrol Nyala LED Melalui Dashboard Adafruit
1. Flow chart program ESP32

   <img src="https://github.com/brianrahma/system-embedded/assets/82065700/9986c798-6e72-4c3d-b454-1c55d0c21d70" width="500">

2. Dokumentasi
   
   ![alt text](https://github.com/rayabima/Embedded-System/blob/main/Jobsheet%204/D.%20Akuisi%20Data%20dan%20Kendali%20Perangkat%20IoT%20Menggunakan%20Protokol%20MQTT/Media/2.%20Dokumentasi%202.jpeg?raw=true)
   
3. Widget On/Off Adafruit
   
   ![alt text](https://github.com/rayabima/Embedded-System/blob/main/Jobsheet%204/D.%20Akuisi%20Data%20dan%20Kendali%20Perangkat%20IoT%20Menggunakan%20Protokol%20MQTT/Media/gif.gif?raw=true)
