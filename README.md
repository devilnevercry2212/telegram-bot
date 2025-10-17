# Telegram Bot для сбора заявок

Telegram бот для сбора заявок с поддержкой webhook и polling режимов.

## Возможности

- ✅ Сбор данных пользователя (имя, город, телефон)
- ✅ Отправка заявок в Telegram канал
- ✅ Редактирование сообщений в канале при получении дополнительных сообщений
- ✅ Поддержка webhook и polling режимов
- ✅ Логирование всех действий
- ✅ Обработка ошибок

## Установка

1. Клонируйте репозиторий:
```bash
git clone https://github.com/your-username/telegram-bot.git
cd telegram-bot
```

2. Установите зависимости:
```bash
pip install -r requirements.txt
```

## Настройка

1. Получите токен бота от [@BotFather](https://t.me/BotFather)
2. Создайте Telegram канал и получите его ID
3. Обновите конфигурацию в `bot.py`:
   - `TOKEN` - токен вашего бота
   - `CHAT_ID` - ID канала для заявок

## Запуск

### Локальное тестирование (polling)
```bash
python bot.py
```

### Продакшен (webhook)
```bash
export USE_WEBHOOK=true
export WEBHOOK_URL=https://your-domain.com/webhook
export PORT=8443
python bot.py
```

## Деплой

### Heroku
1. Создайте приложение на Heroku
2. Установите переменные окружения:
   - `USE_WEBHOOK=true`
   - `WEBHOOK_URL=https://your-app.herokuapp.com/webhook`
   - `PORT=8443`
3. Загрузите код и запустите

### Railway
1. Подключите GitHub репозиторий
2. Установите переменные окружения
3. Деплой автоматически

## Структура проекта

```
telegram-bot/
├── bot.py              # Основной файл бота
├── requirements.txt    # Зависимости Python
└── README.md          # Документация
```

## Логика работы

1. Пользователь отправляет `/start`
2. Бот собирает: имя → город → телефон
3. Заявка отправляется в канал
4. При дополнительных сообщениях заявка редактируется в канале
5. Пользователь получает финальное сообщение с приглашением писать дальше

## Требования

- Python 3.7+
- python-telegram-bot 20.7+
- Для webhook: HTTPS сервер с SSL сертификатом

## Лицензия

MIT License
