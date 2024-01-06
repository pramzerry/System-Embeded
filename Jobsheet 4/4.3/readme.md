# C. Transmisi Data Menggunakan Protokol MQTT

## 1. Keterangan Singkat (Abstrak)
<p align="justify">Dalam percobaan ini, program ESP32 memanfaatkan protokol MQTT untuk mentransmisikan data dummy, seperti level, rainfall, dan flow. Server broker MQTT yang digunakan adalah layanan EMQ X, yang merupakan platform perangkat lunak open-source untuk implementasi MQTT. Setelah program diupload, dilakukan pemantauan melalui serial monitor untuk memastikan koneksi dan debug pada Node-Red. Hasil output dari percobaan ini meliputi data yang dipublikasikan ke topik "flood/node1", serta visualisasi data pada dashboard Node-Red.
   
## 2. Alat dan Bahan
1. Node-RED
2. ESP32
3. XAMPP

## 3. Source Code

  ![alt text](https://github.com/rayabima/Embedded-System/blob/main/Jobsheet%204/C.%20Transmisi%20Data%20Menggunakan%20Protokol%20MQTT/Media/Penjelasan%20Kode.jpeg?raw=true)

## 5. Hasil Percobaan

1. Flow chart program ESP32
   
   ![alt text](https://github.com/rayabima/Embedded-System/blob/main/Jobsheet%204/C.%20Transmisi%20Data%20Menggunakan%20Protokol%20MQTT/Media/Flow%20Chart.png?raw=true)
   
2. Output serial monitor
   
   ![alt text](https://github.com/rayabima/Embedded-System/blob/main/Jobsheet%204/C.%20Transmisi%20Data%20Menggunakan%20Protokol%20MQTT/Media/2.%20Output%20serial%20monitor.jpeg?raw=true)
   
3. Debug Node-RED
   
   ![alt text](https://github.com/rayabima/Embedded-System/blob/main/Jobsheet%204/C.%20Transmisi%20Data%20Menggunakan%20Protokol%20MQTT/Media/3.%20Debug%20Node-RED.jpeg?raw=true)
   
4. Dashboard Node-RED
   
   ![alt text](https://github.com/rayabima/Embedded-System/blob/main/Jobsheet%204/C.%20Transmisi%20Data%20Menggunakan%20Protokol%20MQTT/Media/4.%20Dashboard%20Node-RED.jpeg?raw=true)

<p align="justify">
