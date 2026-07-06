# Greenhouse ESP32

This project is an ESP32 greenhouse / smart farming sketch prepared for GitHub sharing.

## Features / Purpose

- ESP32 WiFi connection
- Firebase Realtime Database integration
- DHT temperature and humidity sensor support
- I2C LCD support
- NTP time support

> Note: Do not upload your real WiFi password, Firebase API key, or account password to GitHub.

## Required Arduino Libraries

Install these libraries in Arduino IDE:

- Firebase ESP Client by Mobizt
- DHT sensor library
- LiquidCrystal I2C
- NTPClient

## Setup

1. Download or clone this repository.
2. Copy `secret.example.h` and rename the copy to `secret.h`.
3. Fill in your own WiFi and Firebase information in `secret.h`:

```cpp
#define WIFI_SSID "YOUR_WIFI_NAME"
#define WIFI_PASSWORD "YOUR_WIFI_PASSWORD"
#define API_KEY "YOUR_FIREBASE_API_KEY"
#define DATABASE_URL "YOUR_FIREBASE_DATABASE_URL"
#define USER_EMAIL "YOUR_FIREBASE_EMAIL"
#define USER_PASSWORD "YOUR_FIREBASE_PASSWORD"
```

4. Open `Greenhouse-ESP32.ino` in Arduino IDE.
5. Select your ESP32 board and upload the code.

## Security

`secret.h` is ignored by Git using `.gitignore`, so your private credentials should stay on your own computer.
Only `secret.example.h` should be uploaded to GitHub.

## License

MIT License
