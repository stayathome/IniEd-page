IniEd
-----

Lister-плагин для Total Commander для просмотра и редактирования
файлов настроек. (.ini, .inf, .reg). По сравнению с текстовыми
редакторами с подсветкой синтакса отличается удобством редактирования
и высокой скоростью работы с большими файлами.

Минимальные требования
----------------------
- Total Commander 5.51

Ручная инсталляция
------------------
1. Раcпакуйте IniEd.wlx в каталог с плагинами (например c:\wincmd\plugins).
2. В Total Commander выберите пункт меню "Конфигурация -> Настройка"
   ("Configuration -> Options").
3. Откройте страницу "Правка/просмотр" ("View/Edit").
4. Нажмите кнопку "Настройка внутрен. программы" ("Configure internal viewer")
   потом -- кнопку "LS-плагины".
5. Нажмите кнопку "Добавить" ("Add") и выберите IniEd.wlx. Нажмите 'OK'.
6. Пользуйтесь. ;-)

Примечание. Для использования плагина с файлами других типов (.url, .log)
            отредактируйте соответствующую строку '''\_detect''' в файле wincmd.ini,
            добавив туда нужное расширение.

Комбинации клавиш
-----------------
  Tab или Ctrl+Tab   - Переключение между списком секций и списком строк
  Ctrl+Tab           - В режиме редактирования строки: переключение выделения ключ/значение
  Enter              - Редактировать
  F1                 - О плагине... 
  F2 или Shift+Enter - Переименовать
  F7 или Ctrl+F      - Поиск
  F3 или F5          - Повторный поиск
  F9                 - Сортировка
  Ctrl+Del           - Удалить строку
  Shift+Del          - Удалить всю секцию
  Ctrl+Insert        - Вставить строку ниже текущей
  Ctrl+Shift+Insert  - Вставить строку выше текущей
  Ctrl+Up            - Передвинуть строку вниз
  Ctrl+Down          - Передвинуть строку вверх
  Ctrl+PgUp          - Перейти в предыдущую секцию
  Ctrl+PgDown        - Перейти в следующую секцию
  Ctrl+X             - Вырезать
  Ctlr+C             - Копировать
  Ctrl+V             - Вставить
  Сtrl+A             - Выделить все
  Ctrl+D             - Дублировать строку
  Ctrl+N             - Добавить новую секцию ниже текущей
  Ctrl+Shift+N       - Добавить новую секцию в конец
  Ctrl+` или
  Ctrl+BackSpace     - Закомментировать (раскомментировать) строку
  Ctrl+S             - Сохранить изменения
  Ctrl+Shift+S       - Сохранить как...
  Ctrl+Z             - Отменить последнее действие
  Ctrl+Shift+Z или 
  Alt+BackSpace      - Вернуть последнее действие
  Ctrl+P             - Настройки
  Alt+A              - Кодировка ANSI       
  Alt+U              - Кодировка Unicode
  Alt+T              - Кодировка UTF-8
  Alt+S              - Кoдировка ASCII (DOS)

  
Лицензия (у всех есть, а чем я хуже? ;-)
----------------------------------------
Данный плагин является бесплатным (Freeware) и предоставляется "как есть"(As is.)
Вы можете использовать его по собственному усмотрению, при условии соблюдения
целостности дистрибутива. Автор не дает гарантий, что плагин будет отвечать
всем ожидаемым требованиям. Автор не несет никакой ответственности за
возможные последствия работы с плагином. Тем не менее, постараюсь отреагировать
на каждое полученное письмо о наступивших последствиях. :-)
Буду благодарен за посильную помощь в развитии плагина. 
Подробности см. на http://www.stayathome.ho.ua/donate.html


Благодарности
-------------
Плагин был создан с использованием справки и исходных кодов
примера по написанию LS-плагинов от Christian Ghisler.
Автор выражает свою благодарность:
- Ajax'у -- за ценные советы, бета-тестирование и перевод этого файла на английский.
- Tchanturia Irakly -- за интересное бета-тестирование. ;-) 
- Е. Савичу -- за интересные идеи в его "Учебном плагине для просмотра RTF файлов".
- всем форумчанам wincmd.ru и лично Avada и Flasher -- за новые идеи, 
терпение и бета-тестирование.

Автора! :-)
-----------
StayAtHome
Web:    www.stayathome.ho.ua
E-Mail: stayathome@email.ua


История изменений
-----------------
[v. 2.0 - 14.04.2020](files/wlx_inied_2.0.7z)

🗲 Добавлена поддержка 64bit (Total Commander 8.X).  
🗲 Существенно увеличена скорость работы с большими файлами.  
🗲 Добавлена возможность отмены последнего действия  
✓ Настройки плагина (IniEd.ini) могут храниться либо в одном каталоге с wincmd.ini (по умолчанию)  
  либо в каталоге плагина (как в предыдущей версии).  
✓ Улучшена поддержка Unicode в т.ч. для длинных путей файлов (больше 259 символов).  
✓ Улучшено автоопределение кодировок.  
＋ Горизонтальное положение списка секций относительно списка строк (с автоподбором высоты).  
＋ Автоматическое сокращение названий ульев реестра (HKEY_CURRENT_USER <-> HKCU).  
✓ Расширены настройки подсветки (рекомендуется удалить старый файл настроек IniEd.ini).  
＋ Снято ограничение на наличие двух секций с одним именем.  
＋ Настройки символов для заголовка секции, комментария, разделителя ключ/значение.  
＋ Возможность выделения нескольких строк и выполнения с ними стандартных действий.  
＋ Комбинация клавиш Shift+Del - удалить всю секцию из списка строк.  
－ Устранена ошибка при выходе из плагина если IniEd.ini недоступен для записи  
＋ Возможность удалять секции без подтверждения (опционально).  
＋ Горизонтальная полоса прокрутки в списке секций (опционально).  
✓ Предупреждение о длительности сортировки больших файлов.  
－ Некорректный фильтр в диалоговом окне и двойное расширение при выборе "Сохранить как..."  
＋ Подтверждение перезаписи существующего файла при выборе "Сохранить как..."  
＋ Обновление содержимого активной файловой панели TC при сохранении файла в режиме быстрого просмотра (опционально).  
✓ Отключено сообщение о превышении длины строки. Макс. длина строки 65536 символов.  
－ Исправлено отображение символов табуляции.  
＋ Возможность фокуса по умолчанию на списке с строками.  
＋ Комбинация клавиш Ctrl+Tab в режиме редактирования строки для переключения переключает выделение 
   ключа/значения (опционально).  

[v. 1.2 - 20.04.2009](files/wlx_inied_1.2.rar)

✓ Теперь плагин может сохранять файлы с атрибутами "Скрытый", "Системный" или "Только для чтения"  
＋ Добавлено сочетание клавиш Ctrl+Shift+S -- "Сохранить как..."  
＋ Добавлено отображение подсказок в левой панели.  
✓ Снято ограничение на длину строки в 1024 символа. Теперь ограничение задается в настройках.  
＋ При редактировании длинные строки переносятся по словам.  
＋ Добавлен выбор цвета фона для левой и правой панелей.  
＋ Добавлен выбор цвета и стиля шрифта для левой панели а также для символа "=".

v. 1.1 - 13.07.2004

－ Исправлена ошибка возникающая при вызове окна настроек.  
✓ Шрифт списка сеций по умолчанию изменен на "MS Sans Serif".  
－ В некоторых случаях не всплывало контекстное меню.  
＋ Теперь можно отменить выход из плагина при нажатии "Esc".  
－ После нажатия кнопки "Отмена" в окне "Сохранить как..." плагин терял фокус.  
＋ Двойной щелчок по разделителю автоматически устанавливает ширину списка секций.  
✓ Изменен порядок пунктов контекстного меню.  
－ Выдавалось сообщение "Section already exists", если во время редактирования названия секции   
   щелкнуть мышью по другой секции.  
－ Двойной щелчок на пункте "< All sections >" влючал редактирование строки.  
＋ Добавлена возможность сортировать в алфавитном порядке строки и секции.  
＋ Поддержка Unicode.  
＋ Отображение текущей кодировки в строке состояния и возможность ее переключения.  
＋ Можно копировать/вырезать/вставлять секции вместе с их содержимым.  
✓ Теперь плагин открывает файлы с расширениями .ini, .inf, .reg.  
－ При большом размере шрифта некорректно отображались символы.  
✓ Теперь плагин открывает файлы нулевого размера.  
＋ Поддержка UTF-8.  
✓ Добавлена обработка ошибки, возникавшей, если в файле присутствует строка длиннее 1024 символов.  
＋ В строку состояния добавлена информация о секциях и строках.  
＋ Добавлено альтернативное сочетание клавиш для операции закомментирования/раскомментирования (Ctrl+BackSpace).

v. 1.0 - 5.07.2004

✓ Улучшена прорисовка шрифтов в диалоге настроек.  
－ Не действовали некоторые пункты контекстного меню.  
✓ Небольшие изменения в контекстном меню.  
－ При работе в пустой секции возникала ошибка.  
－ Список секций не получал фокус при "принудительном" вызове плагина (клавишей "4").  

v. 0.4 Beta - 27.06.2004

🗲 Плагин полностью переписан.  
＋ Добавлено много комбинаций клавиш (см. выше).  
＋ Добавлена поддержка буфера обмена.  
✓ Улучшена обработка ошибок (в т. ч. пользовательских).  
＋ Добавлено процентное отображение текущей позиции курсора.  
＋ Добавлена строка состояния.  
＋ Добавлен поиск.  
－ Убрана ошибка при попытке открытия файла нулевого размера.  
＋ Добавлен диалог настроек.  
＋ Добавлена горизонтальная полоса прокрутки.  
＋ Добавлена команда меню "Save As..."  
＋ Теперь сохраняется ширина списка секций.  

v. 0.3 Beta - не вышла в свет из-за низкого быстродействия.  

🗲 Подсветка синтаксиса переписана заново на WinAPI и вынесена в отдельный поток.  
✓ Шрифт списка секций, для удобства чтения, изменен с моноширинного  
      на пропорциональный.  
＋ Добавлена панель, отображающая название текущей секции.  
＋ Добавлен шорткат Ctrl+S.  

v. 0.2 Alpha - 31.01.2004

🗲 Первая рабочая версия. Немного медленная, но, как ни странно, почти безглючная.

v. 0.1 Alpha Так и не увидела свет.

Обозначения:
🗲 - Важно
＋ - Добавлено
✓ - Изменено
－ - Исправлена ошибка