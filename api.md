# base URL - http://aras.rossonero.kz/profile/site/

# SignUp - регистрация пользователя
## ``` sign-up/ ```
```
fields:{
    email
    first_name
    last_name
    password
    birth_year
}
response:{
    state
    user
}
```

# login для пользователя и компании
## ``` sign-in/ ```
```
fields:{
    email
    password
}
response:{
    state
    user или company
}
```


# получение всех компаний
## ``` get-companies/ ```
```
fields:{
}
response:{
    state
    [companies]
}
```


# регистрация компании (хз надо или нет, мб они будут добавляться с админки)
## ``` company-sign-up/ ```
```
fields:{
    email,
    password,
    name,
    description,
    contacts,
    avatar - file
    
}
response:{
    state
    [companies]
}
```



# получение ленты новости + компании
## ``` get-feed/ ```
```
fields:{
}
response:{
    [news]
    [companies]
}
```


# отправление брифа какой-нибудь компании
## ``` make-order/ ```
```
fields:{
    token,
    company_id,
    name,
    problem,
    budget,
    gender,
    age,
    phone,
    comment
}
response:{
    state
}
```



# получение моих заказов (компания)
## ``` get-my-orders/ ```
```
fields:{
    token
}
response:{
    [orders]
}
```



# при открытии заказа вы должны кинуть запрос 
## ``` watch-order/ ```
```
fields:{
    token,
    order_id
}
response:{
    ОТСУТСТВУЕТ (не надо теребить Таира с криками: СЕРВЕР УПАЛ, МНЕ РЕСПОНС НЕ ПРИХОДИТ И ТД)
}
```





# при открытии заказа вы должны кинуть запрос 
## ``` get-my-orders/ ```
```
fields:{
    token,
    order_id
}
response:{
    ОТСУТСТВУЕТ (не надо теребить Таира с криками: СЕРВЕР УПАЛ, МНЕ РЕСПОНС НЕ ПРИХОДИТ И ТД)
}
```




# Запрос на отправку монет со своего счета, клиенту
## ``` send-money/ ```
```
fields:{
    token,
    order_id
}
response:{  
    state  
}
```






# Запрос на получение своих бонусов
## ``` get-my-bonuses/ ```
```
fields:{
    token
}
response:{  
    state,
    [bonuses]  
}
```

