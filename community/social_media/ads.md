# 📖 ads 
## ℹ️ Dataset info 
Description: `Data feed contains information about delivery from 1 company in 1 country aggregated by phone number.` 

Labels:`owner:upgini` `dataset_type:community` `dataset_source:social_media` 

Search keys: `MSISDN`

Row count: `7,056,223`

Created: `2022-10-26 15:38:17` 

Last updated: `Never` 

## ℹ️ Features info:
|feature name|feature type|descrition|
|---|---|---|
|shipping_phone_rows_cnt|INTEGER|Number of rows in data feed linked to phone number|
|shipping_phone_order_cnt|INTEGER|Number of orders|
|shipping_phone_couriers_cnt|INTEGER|Nuber of couriers who delivered the orders for the phone number owner|
|shipping_phone_region_cnt|INTEGER|Number of regions where phone number owner made an order|
|shipping_phone_region_id_max|INTEGER|Maximum region ID where phone number owner made an order|
|shipping_phone_region_id_min|INTEGER|Minimum region ID where phone number owner made an order|
|shipping_phone_location_latitude_min|FLOAT|Minimum latitude where phone number owner made an order|
|shipping_phone_location_latitude_max|FLOAT|Maximum latitude where phone number owner made an order|
|shipping_phone_location_latitude_avg|FLOAT|Average latitude where phone number owner made an order|
|shipping_phone_location_longitude_avg|FLOAT|Average longitude where phone number owner made an order|
|shipping_phone_location_longitude_min|FLOAT|Minimum longitude where phone number owner made an order|
|shipping_phone_location_longitude_max|FLOAT|Maximum longitude where phone number owner made an order|
|shipping_phone_location_latitude_dif|FLOAT|Difference between minimum and maximum latitude where phone number owner made an order|
|shipping_phone_location_longitude_dif|FLOAT|Difference between minimum and maximum longitude where phone number owner made an order|
|shipping_phone_amount_charged|INTEGER|Total charged from phone number owner for delivery products|
|shipping_phone_amount_client_paid|INTEGER|Total paid by phone number owner for delivery products|
|shipping_phone_dif_amount_charged_paid|INTEGER|Difference between charged and paid by phone number owner for delivery products|
|shipping_phone_amount_avg|FLOAT|Average total price of 1 order|
|shipping_phone_is_ios|INTEGER|Boolean is customer make order by iOS application|
|shipping_phone_asap_cnt|INTEGER|Number of orders with label 'asap'|
|shipping_phone_asap_ratio|FLOAT|Ratio (Number of orders with label 'asap')/(Total number of orders)|
|shipping_phone_delayed_cnt|INTEGER|Number of delayed orders|
|shipping_phone_delayed_ratio|FLOAT|Ratio (Number of delayed orders)/(Total number of orders)|
|shipping_phone_adopted_by_courier_cnt|INTEGER|Number of adopted by couriers orders for the phone number owner|
|shipping_phone_adopted_by_courier_ratio|FLOAT|Ratio (Number of adopted by couriers orders for the phone number owner)/(Total number of orders)|
|shipping_phone_fully_payed_cnt|INTEGER|Number of fully paid orders for the phone number owner|
|shipping_phone_fully_payed_ratio|FLOAT|Ratio (Number of fully paid orders for the phone number owner)/(Total number of orders)|
|shipping_phone_place_cnt|INTEGER|The number of places where orders were made by the owner of the phone number|
|shipping_phone_flow_type_shop_cnt|INTEGER|Number of orders with type label = 'shop'|
|shipping_phone_flow_type_native_cnt|INTEGER|Number of orders with type label = 'native'|
|shipping_phone_flow_type_fastfood_1_cnt|INTEGER|Number of orders with type label = 'Fastfood 1'|
|shipping_phone_flow_type_pickup_cnt|INTEGER|Number of orders with type label = 'Pickup'|
|shipping_phone_flow_type_retail_cnt|INTEGER|Number of orders with type label = 'Retail'|
|shipping_phone_flow_type_gas_station_snacks_1_cnt|INTEGER|Number of orders with type label = 'Gas station snacks 1'|
|shipping_phone_flow_type_gas_station_snacks_cnt|INTEGER|Number of orders with type label = 'Gas station snacks'|
|shipping_phone_flow_type_shop_ratio|FLOAT|Ratio (Number of orders with type label = 'shop')/Total number of orders|
|shipping_phone_flow_type_native_ratio|FLOAT|Ratio (Number of orders with type label = 'native')/Total number of orders|
|shipping_phone_flow_type_fastfood_1_ratio|FLOAT|Ratio (Number of orders with type label = 'Fastfood 1')/Total number of orders|
|shipping_phone_flow_type_pickup_ratio|FLOAT|Ratio (Number of orders with type label = 'pickup')/Total number of orders|
|shipping_phone_flow_type_retail_ratio|FLOAT|Ratio (Number of orders with type label = 'retail')/Total number of orders|
|shipping_phone_flow_type_gas_station_snacks_1_ratio|FLOAT|Ratio (Number of orders with type label = 'Gas station snack 1')/Total number of orders|
|shipping_phone_flow_type_gas_station_snacks_ratio|FLOAT|Ratio (Number of orders with type label = 'Gas station snack')/Total number of orders|
|shipping_phone_payment_service_1_payment_cnt|INTEGER|Number of orders with payment service '1'|
|shipping_phone_payment_service_2_cnt|INTEGER|Number of orders with payment service '2'|
|shipping_phone_payment_service_3_cnt|INTEGER|Number of orders with payment service '3'|
|shipping_phone_payment_service_4_cnt|INTEGER|Number of orders with payment service '4'|
|shipping_phone_payment_service_5_cnt|INTEGER|Number of orders with payment service '5'|
|shipping_phone_payment_service_6_cnt|INTEGER|Number of orders with payment service '6'|
|shipping_phone_payment_method_1_cnt|INTEGER|Number of orders with payment method '1'|
|shipping_phone_payment_method_0_cnt|INTEGER|Number of orders with payment method '0'|
|shipping_phone_payment_status_0_cnt|INTEGER|Number of orders with payment status '0'|
|shipping_phone_payment_status_1_cnt|INTEGER|Number of orders with payment status '1'|
|shipping_phone_payment_status_2_cnt|INTEGER|Number of orders with payment status '2'|
|shipping_phone_payment_status_3_cnt|INTEGER|Number of orders with payment status '3'|
|shipping_phone_first_name_len|INTEGER|Length of customer first name|
|shipping_phone_first_name_cnt|INTEGER|Number of unique customer first names used in delivery|
|shipping_phone_floor_max|STRING|Maximum floor where orders were made by the owner of the phone number|
|shipping_phone_floor_min|STRING|Minimum floor where orders were made by the owner of the phone number|
|shipping_phone_comments_cnt|INTEGER|Number of comments to orders from customer|
|shipping_phone_comments_ratio|FLOAT|Ratio (Number of comments to orders from customer )/Total number of orders|
|shipping_phone_delivery_time_avg|FLOAT|Average delivery time for customer|
|shipping_phone_delivery_time_min|INTEGER|Minimum delivery time for customer|
|shipping_phone_delivery_time_max|INTEGER|Maximum delivery time for customer|
|shipping_phone_app_service_1_cnt|INTEGER|Number of orders made from app '1'|
|shipping_phone_app_grocery_1_android_cnt|INTEGER|Number of orders made from grocery app '1' with os='android'|
|shipping_phone_app_service_2_iphone_cnt|INTEGER|Number of orders made from service app '2' with os='iOS'|
|shipping_phone_app_grocery_1_web_cnt|INTEGER|Number of orders made from grocery app '1' from web|
|shipping_phone_app_grocery_2_android_cnt|INTEGER|Number of orders made from grocery app '2' with os='android'|
|shipping_phone_app_grocery_4_iphone_cnt|INTEGER|Number of orders made from grocery app '4' with os='iOS'|
|shipping_phone_app_web_cnt|INTEGER|Number of orders made from web|
|shipping_phone_app_grocery_1_iphone_cnt|INTEGER|Number of orders made from grocery app '1' with os='iOS'|
|shipping_phone_app_service_3_iphone_cnt|INTEGER|Number of orders made from service app '3' with os='iOS'|
|shipping_phone_app_service_2_android_cnt|INTEGER|Number of orders made from service app '2' with os='android'|
|shipping_phone_app_fastfood_1_web_android_cnt|INTEGER|Number of orders made from fastfood app '1' with os='android'|
|shipping_phone_app_fastfood_1_iphone_cnt|INTEGER|Number of orders made from fastfood app '1' with os='iOS'|
|shipping_phone_app_fastfood_1_android_cnt|INTEGER|Number of orders made from fastfood app '1' with os='android'|
|shipping_phone_app_fastfood_1_web_iphone_cnt|INTEGER|Number of orders made from fastfood app '1' from web with os='iOS' |
|shipping_phone_app_service_3_android_cnt|INTEGER|Number of orders made from service app '3' with os='android'|
|shipping_phone_app_service_4_android_cnt|INTEGER|Number of orders made from service app '4' with os='android'|
|shipping_phone_app_grocery_4_android_cnt|INTEGER|Number of orders made from grocery app '4' with os='android'|
|shipping_phone_app_grocery_3_android_cnt|INTEGER|Number of orders made from grocery app '3' with os='android'|
|shipping_phone_app_grocery_3_iphone_cnt|INTEGER|Number of orders made from grocery app '3' with os='iOS'|
|shipping_phone_app_is_iphone_cnt|INTEGER|Number of orders made from iOS application|
|shipping_phone_app_is_iphone_ratio|FLOAT|Ratio (Number of orders made from iOS application)/Total number of orders|
|shipping_phone_app_is_android_cnt|INTEGER|Number of orders made from android application|
|shipping_phone_app_is_android_ratio|FLOAT|Ratio (Number of orders made from android application)/Total number of orders|
