# hackintosh ASUS PRIME Z270-P
    * установка проверена на всех версия bios от 0325 до 1205.

EFI папка актуальна для систем:
    10.12.6
    10.13.6
    10.14.4

Настройте биос согласно скриншотам из папки "Bios Settings".
Создайте установочную флешку через BootDisk Utility (BDU) воспользовавшись мануалом:
    https://www.applelife.ru/threads/bdu-macos-i-clover-iz-windows-izgotovlenie-zagruzochnoj-flehshki.37189/
    http://cvad-mac.narod.ru/index/bootdiskutility_exe/0-5

Скачайте установочный образ для  BDU:
        https://nnmclub.to/forum/viewtopic.php?t=1285341
        http://mac-ru.net/login.php?redirect=/viewtopic.php?t=1402

Разверните образ на ранее подготовленную флешку утилитой BDU.

Замените папку EFI подготовленную утилитой BDU на флешку, из этого репозитория.

Подключите флешку в порт USB2.0 на материнской плате (это важно!)

Установите macOs следуя инструкциям.

После установки.

Запустите утилиту - "EFI Agent" - https://www.insanelymac.com/forum/topic/337807-efi-agent-v123-menu-bar-utility/
Смонтируйте скрытый раздел EFI;
Скопируйте в него подготовленную мной "EFI"(из этого репозитория);
В биосе выставьте приорит загрузки с UEFI "Название вашего диска";
Все, система должна загружаться с EFI.
