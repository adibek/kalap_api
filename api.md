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