# РУС

## Описание

Данный репозиторий предназначен для тех кто как и я столкнулся с проблемами запуска прошивки и игр на картридже SAROO.
Здесь будет собираться вся полезная информация о SAROO.

### SAROO

SAROO — это эмулятор оптического привода Sega Saturn, некоторые называют его HDLoader. SAROO вставляется в слот для картриджа и реализует функцию CDBLOCK оригинальной материнской платы, загружая игры с SD-карты и запуская их. SAROO также обеспечивает функцию карты-ускорителя 1 МБ/4 МБ. Так же вроде бы есть возможность запускать пиратские диски на оригинальной консоли.

## Инструкция

1. Сначало нужно найти подходящий firmware. Их можно посмотреть в [Здесь](https://github.com/tpunix/SAROO/releases).
2. После этого распаковать содержимое в корень вашей SD карты.
3. Добавлять игры в папку ISO, по одной папки на игру. Не важно какого формата игра они все должны лежать в папке ISO.

## Структура

Есть несколько структур папок в зависимости от firmware.
та которая р данном репозитории:

<pre><code class="fenced-code-block language-SAROO">[SD card root folder]
  + [SAROO]
    + [BIN]
    + [ISO]; хранит образы игр. Одна игра на каталог. Имя каталога будет отображаться в меню;
      + [batman forever]; единственная игра которая у меня заработала, поэтому лежит в ISO
  + ramimage.bin; Прошивка
  + saroocfg.txt; файл конфигурации
  + ssmaster.bin; нужен для запуска?
  + SSMaster.rbf; FPGA?
</code></pre>

В файле ramimage.bin (TODO: добавить смещение) содержиться текст который выводиться в меню.

и общепринятая:


## Пример конфиг файла SAROO


## Аппаратное обеспечение и прошивка
Схема и печатная плата созданы с помощью AltiumDesigner 14. Для корректной работы версии V1.1 требуются свободные кабели. Эту версию больше не следует использовать. Для версии V1.2 по-прежнему требуется дополнительный подтягивающий резистор для использования режима конфигурации FPGA AS.

FPGA разработана с помощью Quartus 14.0.

Firm_Saturn скомпилирована с помощью компилятора SH-ELF, который поставляется с SaturnOrbit.

Firm_v11 скомпилирована с помощью MDK4. Firm_V12 скомпилирована с помощью MDK5.

## Ссылки

1. [GitHub - martinx72/SAROO_Firmware: Enhanced firmware for SAROO cartridge for SEGA SATURN](https://github.com/martinx72/SAROO_Firmware)
2. [SAROO is a SEGA Saturn HDloader](https://github.com/tpunix/SAROO)
3. [Запись в группе "Блог [Константин Савенков]" ВК](https://vk.com/wall-212668087_34)
4. [Техническая информация на китайском](https://github.com/xvortex/SAROO/blob/master/doc/SAROO技术点滴.txt)


# ENG
<b>WIP</b>
