# CB_lists
Мониторинг операций в точках из черного списка ЦБ

CB.ipynb: 
  считывает файл с сайта ЦБ: https://cbr.ru/inside/warning-list/;
  получает нужные данные (имя мерчанта, индекс, город, ИНН) при помощи регулярных выражений;
  приводит их к нужному виду (разбивает по запятым, получает значения из кавычек, транслитерирует);
  формирует списки в формате .xlsx для ручной корректировки

loader.ipynb:
  подготавливает списки для автозагрузчика;
  ставит маски;
  заменяет недопустимые символы %;
  формирует файл формата .csv в кодировке UTF-8 согласно спецификации
