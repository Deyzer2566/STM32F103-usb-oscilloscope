# STM32-blue-pill-usb-oscilloscope
Осциллограф на stm32f103c8t6, передающий данные через usb

# Используемое ПО
- STM32CubeMX
- Keil uVision5
- Python и пакеты pyGame и pySerial

# Сборка
1. Скачать репозиторий
2. Запустить файл oscilloscope.ioc в STM32CubeMX
3. Собрать проект
4. Закинуть в папку проекта папку Core
5. Открыть файл MDK-ARM\oscilloscope.uvprojx в Keil uVision
6. Скомпилировать проект
7. Прошить МК

# Использование
Осциллограф снимает напряжение с пина A0 (0 .. 3,3 вольта!)

Для получения осциллограммы необходимо:
1. подключить плату МК в USB порт
2. определить номер её COM-порта
3. в файле display.py во 2 строке поменять название порта на ваше
4. запустить файл display.py с помощью Python'а

![alt text](https://github.com/Deyzer2566/STM32-blue-pill-usb-oscilloscope/blob/main/example.jpg)
