## mp_stats_loader
Выгрузка понедельной статистики из Маркетплейсов (ВБ и ОЗОН)

Ключи доступа к апи аккаунтов содержатся в файле **api-keys/api-keys.json**. Содержимое папки скрыто. При отсутствии файлов в этой папке, скрипт забирает шаблон этих файлов из папки **temlates/** и создает всю необходимую структуру файлов.

### Обязательно наличие файла *templates/settings.json*, т.к. оттуда берутся все дальнейшие настройки для первого запуска ###

- [x] Создать структуру папок (папка со скрытым содержимым **api-keys** и с шаблонами этих ключей - **templates**).
- [x] Проверяем наличие файла **settings.json**. Если он отсутствует - проверяем наличие файла **templates/settings.json**. Если и он отсутстует - выходим с ошибкой.
- [x] Если файл **templates/settings.json** существует - копируем его в корень проекта и дальше работаем с ним.
- [x] Если файл **api-keys/api-keys.json** отсутствует, то берем данные из файла **templates/api-keys.json** и сохраняем в рабочий файл.
- [x] Получить api ключи от ВБ и ОЗОН, внести их в файл **api-keys/api-keys.json** для дальнейшей работы и тестов.
- [x] Вынести загрузку загрузку/выгрузку файлов в отдельный модуль.
- [ ] Загрузить первые пробные данные из статистики OZON (**не удается из-за перманентной ошибки API**).
- [ ] Вынести в отдельную функцию создание файлов и папок при их отсутствии.
- [ ] Сделать запрос в консоль перед сохранением файлов.
- [ ] Открыть в цикле страницу статистики всех необходимых рекламных кампаний. Получить и вывести коды ответа в консоль.
- [ ] Получить данные из заданных элементов сайта.
- [ ] Найти библиотеку, которая может манипулировать содержимым сайта как пользователь.
