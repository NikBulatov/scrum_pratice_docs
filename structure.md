# Structure
## Project entities
### User
- id (int)
- e-mail\* (str)
- password\* (str)
- username\* (str)
- type (enum)
#### User types
- Admin
- Registered user (default)
- Unregistered user

### Account
- id (int)
- user_id (int)
- first_name (str)
- last_name (str)
- gender (enum)
- age (int)
- weight (float)
- height (float)
- lifestyle/level (enum)

#### Level
- Newer
- Hobbyist
- Pro

### Program
- id (int)
- title (str)
- target (str)
- location (enum)
- level (enum)
- frequency (int)
- prefer_time (time)
- start_date (date)
- description (str)
#### Location
- Home
- Street
- Gym

### Workout
- id (int)
- title (str)
- description/instruction (str)
- exercises
- status (enum)

#### Status
- New
- WIP (work in process)
- Done

### ~~Exercise~~
- id (int)
- title (str)
- description/instruction (str)
- picture(s)/video (path to file)

## Pages

### Main page
- Title and description (сайт персональных тренировок, благодаря нам ты сможешь достичь..., для этого необходимо войти или зарегистрироваться)
- Sign up/Sign in
- Last news/articles

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
- target
- user characteristics
- frequency and quantity of workout
### Workout dairy
- Список тренировок, которые входят в программу
- Можно отмечать выполнено/не выполнено, затраченное время 
### Admin UI
Site' entities management by Django
CRUD:
- users
- articles
- exercises
- workouts
- programs

### Article
- title
- author/sourse
- public data
- body

