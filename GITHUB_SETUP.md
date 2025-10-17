# Инструкции по созданию GitHub репозитория

## Шаг 1: Установите Git
1. Скачайте Git с https://git-scm.com/download/win
2. Установите Git с настройками по умолчанию
3. Перезапустите терминал

## Шаг 2: Создайте репозиторий на GitHub
1. Перейдите на https://github.com
2. Нажмите "New repository"
3. Название: `telegram-bot`
4. Описание: `Telegram Bot для сбора заявок с поддержкой webhook`
5. Выберите "Public" или "Private"
6. НЕ добавляйте README, .gitignore или лицензию (они уже созданы)
7. Нажмите "Create repository"

## Шаг 3: Загрузите код
После установки Git выполните команды:

```bash
# Инициализация репозитория
git init

# Добавление файлов
git add .

# Первый коммит
git commit -m "Initial commit: Telegram bot with webhook support"

# Подключение к GitHub (замените YOUR_USERNAME на ваш GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/telegram-bot.git

# Загрузка на GitHub
git branch -M main
git push -u origin main
```

## Шаг 4: Настройка для деплоя

### Для Heroku:
1. Создайте приложение на https://heroku.com
2. Подключите GitHub репозиторий
3. Установите переменные окружения:
   - `USE_WEBHOOK=true`
   - `WEBHOOK_URL=https://your-app.herokuapp.com/webhook`
   - `PORT=8443`

### Для Railway:
1. Перейдите на https://railway.app
2. Подключите GitHub репозиторий
3. Установите переменные окружения
4. Деплой автоматически

## Файлы в репозитории:
- `bot.py` - основной файл бота
- `requirements.txt` - зависимости Python
- `README.md` - документация
- `.gitignore` - исключения для Git
- `GITHUB_SETUP.md` - эти инструкции
