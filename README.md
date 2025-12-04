<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

## Инструкция развёртывния проекта


- Создать пустую папку для клонирования проекта
- Прописать в терминале в той же папке `git clone https://github.com/Zuev-Yaroslav/effective_mobile_test_work.git` (убедитесь, что на вашем ПК установлен GIT)
- Создать дубликат файла .env.example и переименовать на .env
- В .env можете поменять в DB_CONNECTION название субд (sqlite, mysql).
- Прописать в терминале:
```` bash
composer update
php artisan key:generate
php artisan migrate
````
- Запуск сервера:
```` bash
php artisan serv
````
Список роутов
````
  GET             api/v1/tasks 
  POST            api/v1/tasks      {title, description, status}   
  GET             api/v1/tasks/{task} 
  PUT|PATCH       api/v1/tasks/{task}       {title, description, status}
  DELETE          api/v1/tasks/{task}  
````
