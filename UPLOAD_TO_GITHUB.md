# 🚀 Загрузка на GitHub через веб-интерфейс

## Способ 1: Через GitHub веб-интерфейс (САМЫЙ ПРОСТОЙ)

### Шаг 1: Откройте ваш репозиторий
Перейдите на: https://github.com/devilnevercry2212/telegram-bot

### Шаг 2: Нажмите "uploading an existing file"
1. Нажмите зеленую кнопку **"Add file"** → **"Upload files"**
2. Перетащите ВСЕ файлы из папки `C:\Users\titan\Desktop`:
   - `bot.py`
   - `requirements.txt`
   - `README.md`
   - `.gitignore`
   - `Procfile`
   - `runtime.txt`
   - `GITHUB_SETUP.md`

### Шаг 3: Добавьте описание коммита
В поле "Commit changes" напишите:
```
Initial commit: Telegram bot with webhook support
```

### Шаг 4: Нажмите "Commit changes"
Готово! Все файлы загружены.

---

## Способ 2: Установка Git и загрузка через терминал

### Шаг 1: Установите Git
1. Скачайте: https://git-scm.com/download/win
2. Установите с настройками по умолчанию
3. Перезапустите терминал

### Шаг 2: Выполните команды
```bash
# Инициализация
git init

# Добавление файлов
git add .

# Коммит
git commit -m "Initial commit: Telegram bot with webhook support"

# Подключение к GitHub
git remote add origin https://github.com/devilnevercry2212/telegram-bot.git

# Загрузка
git branch -M main
git push -u origin main
```

---

## Способ 3: GitHub Desktop (РЕКОМЕНДУЕТСЯ)

### Шаг 1: Скачайте GitHub Desktop
https://desktop.github.com/

### Шаг 2: Установите и войдите в аккаунт

### Шаг 3: Клонируйте репозиторий
1. Нажмите "Clone a repository from the Internet"
2. Введите URL: `https://github.com/devilnevercry2212/telegram-bot.git`
3. Выберите папку для клонирования

### Шаг 4: Скопируйте файлы
Скопируйте все файлы из `C:\Users\titan\Desktop` в папку клонированного репозитория

### Шаг 5: Загрузите
1. В GitHub Desktop нажмите "Commit to main"
2. Напишите: "Initial commit: Telegram bot with webhook support"
3. Нажмите "Publish branch"

---

## 📁 Файлы для загрузки:
- ✅ `bot.py` - основной файл бота
- ✅ `requirements.txt` - зависимости
- ✅ `README.md` - документация
- ✅ `.gitignore` - исключения для Git
- ✅ `Procfile` - для Heroku
- ✅ `runtime.txt` - версия Python
- ✅ `GITHUB_SETUP.md` - инструкции
- ✅ `UPLOAD_TO_GITHUB.md` - этот файл

## 🎯 После загрузки:
Ваш репозиторий будет готов для:
- Деплоя на Heroku/Railway
- Просмотра кода онлайн
- Сотрудничества с другими разработчиками
