<h1 align="center">Lottery</h1>
 <h2>Описание:</h2>
  <p>  Это лотерейна игра. 
  Можно создавать матчи, записываться на них, победитель определяется случайным образом. 
  За победу начисляются очки.
  Есть распределение ролей пользователей.
  </p>

<h2> Чтобы запустить проект, выполните следующие шаги:</h2>

1. Создайте контейнеры:

```make start```

2. Зайдите в контейнер

```make bash```

3. Нстановите нужные библиотеки и создайте таблицы в базе данных, заполните их данными

``` composer install && make migrate && make seed```

4. Далее можно пользоваться роутами.

<h2>API:</h2>
<ul>

- POST /api/users/register - Регистрация пользователя 

- POST /api/login - Авторизация пользователя, выдается JWT токен  

- PUT /api/users/{id} - Редактирование пользователя  

- DELETE /api/users/{id}- Удаление пользователя

- GET /api/lottery_games - Получение списка всех лотерейных игр

- POST /api/lottery_game_matches - Создание матча лотерейной игры

- PUT /api/lottery_game_matches - Завершение матча лотерейной игры

- POST /api/lottery_game_match_users - Запись игрока на лотерейную игру

- GET /api/lottery_game_matches?lottery_game_id=1 - Получение списка всех матчей по id лотерейной игры

- GET /api/users - Получение списка всех пользователей

</ul>