### Debian 7, AP9630, UPS-RT-3000

## Что нужно:
- скрепка
- кабель COM-USB
- кабель COM-APC
- ноутбук

## Порядок действий:
1. Устанавливаем сетевой адрес AP9630 согласно документации
2. Конфигурируем трапы на хосты через web или telnet
3. Устанавливаем apcupsd
4. Отключаем сервис: `sudo update-rc.d apcupsd disable`
5. `sudo cp apcupsd_down /etc/network/if-up.d/`
6. `sudo cp apcupsd_down /etc/network/if-down.d/`
7. `sudo cp apcupsd.conf /etc/apcupsd/`
8. Конфигурируем по желанию apcupsd.
