# nginx_vts_template_5.4_javascript
# zabbix_nginx_vts

**Требования**

[nginx](https://nginx.org/ru/) и установленный модуль [nginx-module-vts](https://github.com/vozlt/nginx-module-vts)

**Установка**

 1. Импортировать шаблон Zabbix
 2. Добавить в host или шаблон макрос указывающий путь к url status  в формате json (!!!)
 {$URL_VTS_STATUS} например https://site.com/status/format/json
 3. Присоединить шаблон Nginx VTS к узлу сети
 4. Проверить наличие свежих данных

Шаблон подходит для тех, кто не хочет/не может устанавливать самописные скрипты для вытаскивания данных из nginx-vts.
Данные получаются элементом данных script, который доступен "из коробки".
