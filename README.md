# Telegram bot by HowdyHo

[video](https://www.youtube.com/watch?v=M8fhrtvedHA)

1. Install this: `pip3 install pyTelegramBotAPI`
2. Create config file, there we will place TOKEN
3. Find BotFather in Telegram and create new bot
4. Then copy TOKEN
5. Create bot.py file with this code:
```python
import telebot
import config

bot = telebot.TeleBot(config.TOKEN)

@bot.message_handler(content_types=['text'])
def lalala(message):
    bot.send_message(message.chat.id, message.text)

#RUN
bot.polling(none_stop=True)
```
