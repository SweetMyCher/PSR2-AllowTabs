# PSR2-AllowTabs

Стандарт PSR2, который поддерживает TABS в виде обычного отступа.
Данный стандарт создан для  [PHP_CodeSniffer](https://github.com/squizlabs/PHP_CodeSniffer/ "PHP CodeSniffer на GitHub"). Инструкция по установке находится по ссылке.

## Установка стандарта

После установки [phpcs](https://github.com/squizlabs/PHP_CodeSniffer/ "PHP CodeSniffer на GitHub") необходимо пройти по пути: "PHP_CodeSniffer\src\Standards" и вставить папку PSR2-AllowTabs. Готово. Теперь можно использовать данный формат из командой строки. Пример: 
![Проверка с помощью формата](/images/cmd.jpg "Проверка с помощью формата")

## Настройка SublimeText 3

Для того, чтобы пользоваться phpcs в [SublimeText 3](https://www.sublimetext.com/3 "SublimeLinter на GitHub"), необходимо установить [SublimeLinter](https://github.com/SublimeLinter/SublimeLinter/ "SublimeLinter на GitHub"). После установки данного пакета, необходимо прописать настройки. Для этого нужно зайти в Preference -> Package Settings -> SublimeLinter -> Settngs. Октроется файл, в котором необходимо прописать:

```json
{
   "delay": 0.5,
      "linters": {
          "phpcs": {
              "standard": "PSR2_AllowTabs"
          }
      }
}
```
Перезагружаем Sublime Text 3. Все, стандарт подключен!

