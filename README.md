## Установка
#### 1. Composer
`Перейти на ветку main`

`` composer install ``

#### 2. Npm

`` npm install ``

`` npm run dev ``

#### 3. Прописать в конфиге .env логин и пароль от базы данных

`` php artisan storage:link  ``

`` php artisan migrate --seed ``
`` php artisan db:seed ``

`` php artisan serve ``

####  4.  Сгенерировать токен по адресу http://127.0.0.1:8001/sanctum/csrf-cookie, после чего взять получившийся токен из **cookie**)
5. Пройти аутентификацию по следующему адресу `http://127.0.0.1:8000/login` передать в заголовки `X-XSRF-TOKEN` с значением из предыдущего шага, в качестве параметров передать email и password которые созданые в seeder

Функционал приложения: 

Вывод данных с выбором группировки `http://127.0.0.1:8000/sorted` в параметры передать groupBy со значением utm_source, utm_medium по умолчанию группировка по дате

Отправка данных с выбором группировки `http://127.0.0.1:8000/peoples_applications` в параметры передать  значения полез из ТЗ, примерно как [здесь](https://imgur.com/50u4nAL "здесь")