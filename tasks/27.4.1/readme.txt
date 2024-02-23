Задание:
В какой период осуществлялись заказы по предоставленным данным?

SQL запрос:

select 
    to_char(min(order_date), 'YYYY-MM-DD') min_order_date,
    to_char(max(order_date), 'YYYY-MM-DD') max_order_date
from 
    sql.store_delivery