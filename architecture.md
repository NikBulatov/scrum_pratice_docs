# Project entities
### User
- id (int)
- e-mail\* (str)
- password\* (str)
- username\* (str)
- type (enum)
#### User types
- Admin
- Registered user (default)
- Unregistered user (not used)

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
- telegram_chat_id (int)

#### Level
- Newer
- Hobbyist
- ~~Pro~~

### Program
- id (int)
- title (str)
- target (enum)
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

#### Target
- slim
- relief
- mass
- keep fit 

### Dairy
- id
- account_id
### Workout
- id (int)
- title (str)
- description/instruction (text)
- exercises (???)
- status (enum)
- result (???)

#### Status
- New
- WIP (work in process)
- Done

### ~~Exercise~~
> [!attention]
>OpenAi не будет давать людям одинаковые упражнения и программы. Отсюда мы в базу не можем сохранить такие сущности как Упражнение.
- id (int)
- title (str)
- description/instruction (str)
- picture(s)/video (path to file)

### Article
- id (int)
- title (str)
- author/source (str)
- public data (date)
- body (text)