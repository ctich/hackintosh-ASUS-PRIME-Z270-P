# hackintosh ASUS PRIME Z270-P

    * установка проверена на всех версиях bios от 0325 до 1205/2001 Beta Version

=== Актуализация EFI по состоянию на 05.02.2023 ===

**"EFI"** актуальна для систем: 10.14.6 | 10.15.3  **Clover v2.5k LastVers**

**"EFI on OpenCore"** актуальна для систем: macOS 12.4 | 13.2 **OpenCore v.0.8.8**

 - *В SMbios необходимо заменить "default" значения на свои .*

## Конфигурация PC:

- **Процессор Intel® Core™ i5-7400**
 - Intel® HD Graphics 630 for Intel Quick Sync Video via 0x59120003
- **Материнская плата ASUS PRIME Z270-P**
 - LAN: Realtek® RTL8111H, ок.
 - AUDIO: Realtek® ALC887, ok
 - USB:  Intel® Z270 Chipset, ok.
- **Видеокарта Sapphire PULSE Radeon RX 550 4G G5 640SP (11268-15)**
- **Жесткий диск SSD NVMe Samsung 970 EVO 250Gb (MZ-V7E250)**
- **Оперативная память DDR4 Samsung M378A1G43EB1-CPB 8 Gb * 2шт.** 

### Установка:

**Настройте биос согласно скриншотам из папки "Bios Settings".**

- Создайте установочную флешку через BootDisk Utility (BDU) воспользовавшись мануалом:
 - https://www.applelife.ru/threads/bdu-macos-i-clover-iz-windows-izgotovlenie-zagruzochnoj-flehshki.37189/
  - http://cvad-mac.narod.ru/index/bootdiskutility_exe/0-5

**Скачайте установочный образ для  BDU:**

 - https://nnmclub.to/forum/viewtopic.php?t=1285341
 - http://mac-ru.net/login.php?redirect=/viewtopic.php?t=1402

**Разверните образ на ранее подготовленную флешку утилитой BDU.**

- Замените папку EFI подготовленную утилитой BDU на флешку, из этого репозитория.
- Подключите флешку в порт USB2.0 на материнской плате (это важно!)
- Установите macOs следуя инструкциям.

### После установки:

- Запустите утилиту - "EFI Agent" - https://www.insanelymac.com/forum/topic/337807-efi-agent-v123-menu-bar-utility/

- Смонтируйте скрытый раздел EFI;

- Скопируйте в него подготовленную "EFI"(из этого репозитория);

- В биосе выставьте приорит загрузки с UEFI "Название вашего диска";

**Все, система должна загружаться с EFI.**
