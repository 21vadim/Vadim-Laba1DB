1) Выберите из таблицы orders все заказы SELECT * FROM orders;


    [image](https://github.com/user-attachments/assets/3512143c-8da0-477c-8184-793fc43ec073)


3) Выберите из таблицы orders все заказы кроме новых. У новых заказов status равен "new". Использовать in
'''


SELECT * FROM orders WHERE STATUS IN ('in_progress', 'cancelled' , 'delivery');
'''

 ![image](https://github.com/user-attachments/assets/de772b49-2b0b-4702-ba00-c4043795c2cc)


Задание 3

3) Выберите из таблицы orders все новые и отмененные заказы. У отмененных заказов status равен "cancelled". У новых заказов status равен "new".

SELECT * FROM orders WHERE STATUS IN ('new', 'cancelled')


![image](https://github.com/user-attachments/assets/b760b9cb-2c2d-4a6f-b176-8b44ceb7d067)


Задание №4

Выберите из таблицы orders все заказы содержащие более 3 товаров (products_count). Вывести нужно только номер (id) и сумму (sum) заказа

![4](https://github.com/user-attachments/assets/d641e093-7c8e-49a6-87b9-abf642b882f2)


SELECT id,sum FROM orders WHERE products_count > 3
