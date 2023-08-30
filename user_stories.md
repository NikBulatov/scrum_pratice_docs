# Role: Unregistered user
## Theme: Registration and Auth

### Epic: User registration
#### Story: Ввести реквизиты для регистрации
Незарегистрированный пользователь может использовать форму регистрации для создания собственного аккаунта в приложении, чтобы в дальнейшем использовать функционал, предоставляемый приложением. 
##### Positive scenario
- Ввести валидный e-mail -> green sign / yellow sign о том, что нужно подтвердить почту
- Ввести незанятый username -> green sign
- Ввести пароль удовлетворяющий условиям: от 8 символов, содержащий заглавные, строчные буквы, цифры, спец. символы) -> green sign -> Submit button -> modal block about successful registration
##### Negative scenario
- Ввести не валидный e-mail -> red sign or border around input field
- Ввести e-mail, который уже используется в приложении -> такой пользователь существует
- Ввести незанятый username -> modal message about invalid password (короткий или не хватает символов)
- Ввести пароль не удовлетворяющий условиям -> modal message about inputted username is used by other user
### User Authentication and Authorization
#### Ввести реквизиты для аутентификации
Незарегистрированный пользователь не может использовать данные для регистрации в целях аутентификации в системе с дальнейшей авторизацией. Его действия можно рассматривать как негативный сценарий
##### Positive
- input valid e-mail/username -> green sign
- input password -> Login button -> redirect at main/account page?
##### Negative
- incorrect password -> message near input field + red border
- input unknown e-mail/username -> message near input field + red border

### Password recovery
#### Восстановить пароль
Незарегистрированный пользователь не может восстановить пароль к своему аккаунту, так как аккаунта у него нет.
##### Positive
- input valid e-mail -> Submit button -> send link to the passed e-mail to reset password
##### Negative
- input invalid e-mail -> red border
- input unknown e-mail -> Submit button -> Model message about unregistered e-mail

## Theme: Просмотр страниц сайта
### Просмотр страницы
Любой негативный сценарий должен привести ЛЮБОГО пользователя к странице, сообщающая о том, что запрашиваемой страницы нет. В случае попытки входа на страницу с дневником или иным функционалом, который требует авторизации, необходимо перенаправлять на страницу входа в аккаунт.
#### Главная страница
##### Positive
- Может нажать на кнопку "Регистрация/Войти" -> форма регистрации/входа
- Может открыть статью -> открывается страница статьи
- Может прочитать список статей
- Может ознакомиться с функционалом приложения, чтобы в дальнейшем зарегистрироваться 

#### Страница статьи
##### Positive
Может прочитать содержимое статьи
Ознакомиться с автором/источником
Датой публикации

# Role: Registered user
## Theme: Personal account
### Account info
Общая информация о зарегистрированном пользователе
### Positive
- read info
- create/update info
- delete chosen info
### Negative
- input invalid age -> users' age could be from 14 to 1k00 -> message near input field + red border
- input invalid weight -> users' weight could be from 30 to 150 -> message near input field + red border
- input invalid height -> users' height could be from 130 to 250 -> message near input field + red border
- input invalid first_name/last_name -> only string type -> message near input field + red border

## Workout program

