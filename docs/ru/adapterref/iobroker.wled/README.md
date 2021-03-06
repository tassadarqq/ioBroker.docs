---
translatedFrom: en
translatedWarning: Если вы хотите отредактировать этот документ, удалите поле «translationFrom», в противном случае этот документ будет снова автоматически переведен
editLink: https://github.com/ioBroker/ioBroker.docs/edit/master/docs/ru/adapterref/iobroker.wled/README.md
title: ioBroker.wled
hash: kCIU567p3HLKqgoQcJfrWYd3+DYVVDUQpFAtfqomBRI=
---
![логотип](../../../en/adapterref/iobroker.wled/admin/wled_large.png)

![Версия NPM](http://img.shields.io/npm/v/iobroker.wled.svg)
![Загрузки](https://img.shields.io/npm/dm/iobroker.wled.svg)
![Количество установок (последняя)](http://iobroker.live/badges/wled-installed.svg)
![Количество установок (стабильно)](http://iobroker.live/badges/wled-stable.svg)
![Статус зависимости](https://img.shields.io/david/iobroker-community-adapters/iobroker.wled.svg)
![Известные уязвимости](https://snyk.io/test/github/iobroker-community-adapters/ioBroker.wled/badge.svg)
![NPM](https://nodei.co/npm/iobroker.wled.png?downloads=true)

# IoBroker.wled
## Сетевой адаптер для ioBroker
Быстрая и многофункциональная реализация веб-сервера ESP8266 / ESP32 для управления светодиодами NeoPixel (WS2812B, WS2811, SK6812, APA102)!

[WLED - Github Project](https://github.com/Aircoookie/WLED) @Aircoookie

## Инструкции
Адаптер автоматически пытается найти устройства WLED в вашей сети, используя службы Bonjour.
Известные проблемы: сети с разделением VLAN в основном не маршрутизируют широковещательный трафик, что означает сбой автоматического определения.

Не волнуйтесь, в этом случае вы можете добавить устройство вручную по IP-адресу.

1) Убедитесь, что ваше устройство WLED работает и доступно по сети. 2) Установите адаптер. 3) Настройте время интервала для опроса данных и автоматического определения cyclus. 4 - A) Запустите адаптер, устройства должны быть обнаружены автоматически. 4 - B) Если отказывает A используйте кнопку «Добавить устройство» и укажите IP-адрес устройства. 5) Адаптер немедленно отправляет изменения и опрашивает данные каждые x секунд (настраивается).

## Сделать
* [] Переключение опроса на сокетные соединения, ожидающие реализации на прошивке WLED

## Поддержите меня
Если вам нравится моя работа, пожалуйста, не стесняйтесь предоставить личное пожертвование (это личная ссылка на пожертвования для DutchmanNL, никакого отношения к проекту ioBroker!) [![Пожертвовать] (https://raw.githubusercontent.com/iobroker-community-adapters/ioBroker.wled/master/admin/button.png)](http://paypal.me/DutchmanNL)

## Changelog

### 0.5.0 Stable release
* (DutchmanNL) Added translations
* (DutchmanNL) Release to stable repository, beta testing finished

### 0.3.0 Bugfix : Correct handling of polling timer
* (DutchmanNL  & Jey-Cee) Bugfix : Polling timer not saved
* (DutchmanNL) Bugfix : Correct handling of "online" state
* (DutchmanNL) Bugfix : Polling timer (offline devices did not reconnect)

### 0.2.6 Bugfix : Hex state value change
* (DutchmanNL) Bugfix : Hex state value change

### 0.2.5 Stable release candidate
* (DutchmanNL) Code cleanup
* (DutchmanNL) Improved logging information
* (DutchmanNL) Make polling timer configurable
* (DutchmanNL) Correct handling of device online state
* (DutchmanNL) Show online state in instance configuration

### 0.2.0 Possibility to add devices by IP-adress
* (DutchmanNL) Bugfix io-package
* (DutchmanNL) Improved logging at adapter start
* (DutchmanNL) Possibility to add devices by IP-adress implemented. (Needed for situations were autoscan fails)
* (DutchmanNL) Ensure known devices get connected immediatly after adapter start instead of waiting for network scan

### 0.1.9 Code improvements
* (DutchmanNL) Code cleanup and optimalisation
* (DutchmanNL) FIX memory leak by proper handling of bonjour service

### 0.1.8 Bugfix
* (DutchmanNL) Solved incorrect formated API call at state changes causing warning message

### 0.1.7 Bugfix
* (DutchmanNL) Fixed error when API call fails (write warning to log and retry at intervall time)

### 0.1.6 HEX color states implemented
* (DutchmanNL) HEX color states implemented

### 0.1.5 Stable Beta release

### 0.1.2
* (DutchmanNL) Implement drop down menu for effects

### 0.1.1
* (DutchmanNL) Implemented states hidden from JSON-API : tt / psave / nn / time
* (DutchmanNL) Improve logging issue

### 0.1.0
* (DutchmanNL) initial release

## License
MIT License

Copyright (c) 2020 DutchmanNL <rdrozda86@gmail.com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.