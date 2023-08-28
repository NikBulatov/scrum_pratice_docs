# Needed functional
- User registration
- Authentication and Authorization

# Scenarios

# Registration and Auth
## User registration
### Positive
- input valid e-mail -> green sign / yellow sign о том, что нужно подтвердить почту
- unused username -> green sign
- input valid password (от 8 символов пароль, содержащий заглавные, строчные буквы, цифры, спец. символы) -> green sign -> Submit button -> modal block about successful registration
### Negative
- input invalid e-mail -> red sign or border around input field
- input invalid password -> modal message about invalid password (короткий или не хватает символов)
- used username -> modal message about inputted username is used by other user
## User Authentication and Authorization
### Positive
- input valid e-mail/username -> green sign
- input password -> Login button -> redirect at main/account page?
### Negative
- incorrect password -> message near input field + red border
- input unknown e-mail/username -> message near input field + red border

## Password recovery
### Positive
- input valid e-mail -> green sign
- input known e-mail -> Submit button -> send link to the passed e-mail to reset password

### Negative
- input invalid e-mail -> red border
- input unknown e-mail -> Model message about unregistered e-mail
# Personal account
- Создать программу тренировок
- Записать результат тренировки (выполнено/не выполнено)

## Account info
Common information about registered user.
### Positive
- read info
- create/update info
- delete chosen info
### Negative
- input invalid age -> users' age could be from 14 to 100 -> message near input field + red border
- input invalid weight -> users' weight could be from 30 to 150 -> message near input field + red border
- input invalid height -> users' height could be from 130 to 250 -> message near input field + red border
- input invalid first_name/last_name -> only string type -> message near input field + red border

## Workout program

