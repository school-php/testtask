Исходное положение:
1. Имеем 3 модели двух доменов: Goods и Orders
2. Имеем миграции, создающие соответствующие таблицы моделям
3. Good - товары на сайте, которые можно купить
4. Order - корзина заказа
5. Order Item - товар, лежащий в корзине. Связующая таблица между Order и Good
6. Документация написана на swagger:
   1. Перед началом работы разово необходимо выполнить php artisan vendor:publish --provider "L5Swagger\L5SwaggerServiceProvider"
   2. После добавления правок в swagger необходимо вызвать php artisan l5-swagger:generate
   3. Документация доступна по адресу: http://localhost/api/documentation
