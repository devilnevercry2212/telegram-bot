# 🚀 ПРОСТОЙ способ загрузки на GitHub

## Что вы видите на странице GitHub?

### Если видите кнопку "uploading an existing file":
1. Нажмите на неё
2. Перетащите файлы из папки `C:\Users\titan\Desktop`
3. Напишите: "Initial commit: Telegram bot"
4. Нажмите "Commit changes"

### Если НЕ видите эту кнопку:

#### Вариант 1: Создайте новый файл
1. Нажмите кнопку **"Create new file"** (или иконку "+")
2. В поле имени файла введите: `bot.py`
3. Скопируйте содержимое файла `bot.py` из папки Desktop
4. Внизу нажмите **"Commit new file"**

#### Вариант 2: Используйте GitHub Desktop
1. Скачайте: https://desktop.github.com/
2. Установите и войдите в аккаунт
3. Нажмите "Clone a repository from the Internet"
4. Введите: `https://github.com/devilnevercry2212/telegram-bot.git`
5. Скопируйте файлы из Desktop в папку репозитория
6. В GitHub Desktop нажмите "Commit to main"

#### Вариант 3: Через терминал (если установлен Git)
```bash
git clone https://github.com/devilnevercry2212/telegram-bot.git
cd telegram-bot
# Скопируйте файлы из Desktop сюда
git add .
git commit -m "Initial commit"
git push
```

## 📁 Файлы для загрузки (по одному):
1. `bot.py` - основной файл
2. `requirements.txt` - зависимости  
3. `README.md` - документация
4. `.gitignore` - исключения
5. `Procfile` - для Heroku
6. `runtime.txt` - версия Python

## ❓ Что именно вы видите на странице?
Опишите, какие кнопки/элементы вы видите на https://github.com/devilnevercry2212/telegram-bot
