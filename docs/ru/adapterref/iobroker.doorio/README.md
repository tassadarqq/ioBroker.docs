---
translatedFrom: en
translatedWarning: Если вы хотите отредактировать этот документ, удалите поле «translationFrom», в противном случае этот документ будет снова автоматически переведен
editLink: https://github.com/ioBroker/ioBroker.docs/edit/master/docs/ru/adapterref/iobroker.doorio/README.md
title: ioBroker.doorio
hash: LuhsI/3MpnIV58jHpZ51CghSPDkFkf8W27HZ6T6haso=
---
![логотип](../../../en/adapterref/iobroker.doorio/admin/doorio.png)

![Статус сборки](https://travis-ci.org/Bettman66/ioBroker.doorio.svg?branch=master)
![Версия NPM](http://img.shields.io/npm/v/iobroker.doorio.svg)
![Загрузки](https://img.shields.io/npm/dm/iobroker.doorio.svg)
![NPM](https://nodei.co/npm/iobroker.doorio.png?downloads=true)

# IoBroker.doorio
Самодельный адаптер DoorStation для ioBroker

## Ссылки
* https://forum.iobroker.net/topic/23413/ich-baue-eine-t%C3%BCrsprechstelle-ohne-cloud
* https://forum.iobroker.net/topic/22746/test-adapter-doorio-v0-0-x

## Changelog

### 1.0.7
* (bettman66) check states

### 1.0.6
* (bettman66) clearTimeouts

### 1.0.5
* (bettman66) update stable

### 1.0.4
* (bettman66) new config

### 1.0.3
* (bettman66) update adapter-core

### 1.0.2
* (bettman66) add selectID.js

This adapter connects to the Baresip Sip client via tcp.socket to communicate
with a doorphone. As a bell trigger every input from ioBroker can be used.
The adapter also recognizes DTMF tones to switch outputs.
For the self-made door station, any hardware on which Baresip can install
can be used.

Dieser Adapter verbindet sich über tcp.socket mit dem Baresip Sip-Client,
um mit einer Türsprechstelle zu kommunizieren. Als Klingelauslöser kann jeder
Eingang von ioBroker genutzt werden. Der Adapter erkennt auch DTMF-Töne um
Ausgänge zu schalten.
Für die Selbstgemachte Türsprechstelle, kann jede Hardware auf der sich Baresip
installieren lässt genutzt werden.

## License
The MIT License (MIT)

Copyright (c) 2020 Walter Zengel <w.zengel@gmx.de>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.