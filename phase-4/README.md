# Phase 4 — Remote Control (Bluetooth)

Bu aşamada ESP32 drift car, telefon üzerinden Bluetooth ile kontrol edilecektir.

## Bu aşamada yapılacaklar:

### 1. ESP32 Bluetooth Başlangıcı
- BluetoothDeviceName tanımlama
- BluetoothSerial kütüphanesi ile bağlantı kurma

### 2. Komut Sistemi
Telefon üzerinden aşağıdaki karakterler gönderilecek:
- **F** = Forward (İleri)
- **B** = Backward (Geri)
- **L** = Left
- **R** = Right
- **S** = Stop
- **D** = Drift mode (özel kontrol)

### 3. switch-case Kontrol Blokları
Bluetooth'tan gelen karaktere göre ilgili motor fonksiyonları çalıştırılacak.

### 4. Simülasyon (Wokwi)
- Gerçek Bluetooth Wokwi’de çalışmaz.
- Bu nedenle **Bluetooth yerine Serial Input simülasyonu** yapılacak.
- ESP32, Serial Monitor’den gelen komutları Bluetooth yerine okuyacak.

## Notlar:
- Bu faz, gerçek donanım eline ulaştığında gerçek Bluetooth ile test edilecektir.
- Drift mode yalnızca Phase 3 motor algoritmaları tamamlandıktan sonra gerçek anlamda çalışacaktır.
