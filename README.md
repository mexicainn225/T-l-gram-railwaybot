import os
from telebot import TeleBot

bot = TeleBot(os.environ["7392348080:AAFZTwZgm4EsAa56kW5wIBuqUeOeQscejww"])

@bot.message_handler(func=lambda msg: True)
def reply_all(message):
    bot.send_message(
        message.chat.id,
        "Bienvenue ! Utilise le code promo MEXICAIN225 pour activer les signaux du bot maintenant."
    )

if __name__ == "__main__":
    bot.infinity_polling()
pyTelegramBotAPI
