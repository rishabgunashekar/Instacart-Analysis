# Instacart Market Basket Analysis

  

## About Instacart

-   An American based company that delivers grocery items to customers on the same day.
    
-   The Goal of this company is to be an efficient real-time logistics platform of moving goods from the store to the customer place as efficiently and predictably as possible
    
-   Product recommendation plays a crucial role.
    

  

![](https://lh4.googleusercontent.com/-RGWaOYNgzvqxZUklVJD9HLTX9SHQ3xXuhQZPlA9uu8psgIBbv4bxWALa2ORDAqH8ASfHQLEAYYtyLGrOgBxnoGpkrlhv6srvVKQQlO6tmx8Lkdtm8Zt-3Bhq4xvEZCpmc7Qczpm)

  

## Aim of the Project

-   Analyze grocery purchasing data and group customers who have similar buying habits together.
    
-   Provide product suggestions based on keyword searches, as well as additional cart products.
    

## Dataset Description

The dataset is anonymized and contains a sample of over 3 million grocery orders from more than 200,000 Instacart users.

### aisles.csv

```
 aisle_id,aisle  
 1,prepared soups salads  
 2,specialty cheeses  
 3,energy granola bars  
 ...

```

### departments.csv

```
 department_id,department  
 1,frozen  
 2,other  
 3,bakery  
 ...

```

### order_products__*.csv

These files specify which products were purchased in each order. order_products__prior.csv contains previous order contents for all customers. 'reordered' indicates that the customer has a previous order that contains the product. Note that some orders will have no reordered items. You may predict an explicit 'None' value for orders with no reordered items. See the evaluation page for full details.

```
 order_id,product_id,add_to_cart_order,reordered  
 1,49302,1,1  
 1,11109,2,1  
 1,10246,3,0  
 ... 

```

### orders.csv

This file tells to which set (prior, train, test) an order belongs. You are predicting reordered items only for the test set orders. 'order_dow' is the day of week.

```
 order_id,user_id,eval_set,order_number,order_dow,order_hour_of_day,days_since_prior_order  
 2539329,1,prior,1,2,08,  
 2398795,1,prior,2,3,07,15.0  
 473747,1,prior,3,3,12,21.0  
 ...

```

### products.csv

```
 product_id,product_name,aisle_id,department_id
 1,Chocolate Sandwich Cookies,61,19  
 2,All-Seasons Salt,104,13  
 3,Robust Golden Unsweetened Oolong Tea,94,7  
 ...

```

### sample_submission.csv

```
order_id,products
17,39276  
34,39276  
137,39276  
...
```

  
## Streamlit Output
  
![Streamlit](https://user-images.githubusercontent.com/71303032/116770068-ea2cca00-aa0e-11eb-850f-47cd55971ec9.jpeg)
 
 
