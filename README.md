# CAN Sniffer
Код для Arduino и ESP8266.

Тестировалось на Arduino UNO, Arduino Nano, ESP8266 (ESP-12F совместимый с NodeMCU 1.0). Для Arduino работает передача через последовательный порт. Для ESP8266 работает передача данных черех последовательный интерфейс и Wi-Fi.

В ESP8266 крайне медленно работает передача данных через Wi-Fi малыми порциями (пакет данных, который необходимо передать занимает от 10 до 17 байт и таких пакетов от 700 до 1000 в секунду), происходит потеря данных. Поэтому данные собираются в пакет до 1000 байт и потом отправляются через интерфейс.
