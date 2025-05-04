# Sensebox
SenseBox adalah sistem monitoring ruangan berbasis IoT dengan ESP32 yang mengukur suhu, kelembaban, intensitas cahaya/LDR, mendeteksi api, menampilkan hasil monitoring di layar OLED, serta secara otomatis menyalakan LED saat gelap dan buzzer untuk peringatan jika sensor mendeteksi adanya api.

SenseBox akan menampilkan 3 data pada display OLED, yaitu Suhu, kelembaban, dan juga LDR/sensitivitas cahaya. Ketiga data tersebut akan ditampilkan satu persatu secara bergantian dan terus menerus.

Sistem ini memiliki fitur otomatisasi pencahayaan dengan LED WS2812B yang dikendalikan ESP32, dimana LED akan menyala ketika keadaan gelap yang informasinya di dapat dari sensor cahaya/LDR.

Sistem ini juga memiliki sensor api yang akan mengakitkan alarm dengan menyalakan buzzer dan menampilkan icon api jika mendeteksi api. Selain itu jika suhu di atas 39 derajat Celsius, maka buzzer akan menyala juga. 2 push button juga ditambahkan pada sistem ini agar bisa mengatur apakah led dan buzzer mau di nonaktifkan atau tidak. Jika push button tersebut ditekan maka akan menampilkan sebuah icon mute (untuk buzzer) dan icon off light (untuk led).

Komponen Hardwarenya seperti berikut : 
1. ESP32
2. DHT11 (Sebagai Sensor Suhu dan Kelembaban)
3. LED WS281B
4. OLED Display 0.96” (I2C, SSD1306)
5. Sensor LDR + Resistor 10k
6. IR Flame Sensor
7. Active Buzzer 5V
8. 2 x push button (Sebagai menonaktifkan buzzer dan juga menonaktifkan LED)
9. Breadboard
10. Kabel jumper secukupnya
