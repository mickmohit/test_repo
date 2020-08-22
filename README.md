# test_repo
test_repo

## Order Item service

``Post request``
URL:
http://localhost:8082/api/v1/item

Body:
{
        "product_code": "103C",
        "product_name":"Cooler",
        "quantity":2    
}

# Order service

``Post request``
URL:
http://localhost:8081/api/v1/order

Body:
{
        "id":1,
        "customer_name": "Mohit",
        "order_date":"2020-03-29",
        "shipping_address":"abc",
        "order_items":[{
                 "product_code": "105C",
        "product_name":"Cooler",
        "quantity":2
        }]   
}

``Get request`` to call order item service from order service
URL: http://localhost:8081/api/v1/allOrderItem/
