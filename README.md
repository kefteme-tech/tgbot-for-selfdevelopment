# Telegram-бот для мотивации и саморазвития
Telegram-бот для мотивации и саморазвития. Основные функции: трекер ежедневого и/или еженедельного прогресса (пользователь выбирает в каких направлениях он хочет "работать", например, ежедневное чтение или физ активность, и бот ежедневно спрашивает у пользователя оценку насколько хорошо он выполнил ежедневную задачу. Данные сохраняются в эксель табличку), генерирование мотивационных речей (по запросу пользователя, так и без его запроса), генерирование советов по продуктивности и борьбе с прокрастинацией (по запросу пользователя), возможно также напоминания по заданным пользователем дедлайнам.

Студентов в команде 2: *Ермолинский Олег Викторович, Климкин Максим Николаевич.*

Выполнено в качестве проектного задания по дисциплине "Исскуственный интеллект в инженерном образовании"



# Код Telegram-бота размещен в Google Colab
Ссылка для просмотра: https://colab.research.google.com/drive/1W0wVvkcXcnyzwZUY37hjxk-R26FL6BaI?usp=sharing



# Имеющийся функционал

На данный момент Telegram-бот имеет 3 основные команды: 

/start - команда при запуске бота, запускает регистрацию 

/info - информация о боте и пользователе

/advice - получение уникального ответа от GigaChat по теме саморазвития и дисциплины



**Используемые в боте инструменты:**

✅Машина состояний

Middleware

✅Большая языковая модель



**Требования к интерфейсу:**

✅Русский язык. 
бот полностью на русском языке

✅Наличие командного меню (Меню /). 
командное меню, состоящее из перечисленных выше команд

✅Наличие inline и обычных клавиатур.
inline клавиатура при проверке подписки на канал и при выборе цели. Обычная клавиатура, дублирующая командное меню.

✅Реакция/ответ бота на любое действие пользователя.
если сообщение не является командой, бот напишет об этом.

✅Проверка корректности ввода данных пользователем.
при регистрации в качестве имени нельзя задать команду. Проверка ввода возраста.



**Общий функционал:**

✅Ввод регистрационных данных пользователем.

✅Заполнение пользователем анкеты при регистрации (FSM).

Проверка зарегистрированности пользователя при вызове команд (Middleware).

Запись действий пользователя в БД (Middleware). Вместо БД можно использовать csv-файл с разделителями или Excel-файл с несколькими столбцами.

✅Напоминания или периодические сообщения (библиотека Apsheduler).

Заполнение анкеты пользователем по окончании использования или спустя какое-то время, после начала использования (FSM).

✅Использование LangChain (память, промпты, цепочки).

✅Разграничение использование БЯМ между разными пользователями.

