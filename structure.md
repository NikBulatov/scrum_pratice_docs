# Structure
## Project entities
### User
- id
- e-mail\*
- password\*
- username\*
- type
#### User types
- Admin
- Registered user (account)
- Unregistered user

### Account
- id
- user_id
- first_name
- last_name
- gender
- age
- weight
- height
- lifestyle

### Program
- id
- title
- description

### Workout
- id
- title
- description (instruction)

### Exercise
- id
- title
- description (instruction)
- picture(s)/video

## Pages

### Main page
- Title and description (сайт персональных тренировок, благодаря нам ты сможешь достичь...)
- Sign up/Sign in
- Last news/articles
- *Shops?*

### Login page
- email/username
- password
- password recovery

### Registration page
- e-mail
- username
- password

### Personal account
- Account info (actual info about user)
- Workout dairy - done, undone exercises
- Food diary

### Create program
- title
- goal
- user characteristics
- frequency and quantity of workout
### Workout dairy
- Список тренировок, которые входят в программу
- Можно отмечать выполнено/не выполнено, затраченное время 
### Admin UI
Site' entities management
CRUD:
- users
- articles
- exercises
- workouts
- programs

