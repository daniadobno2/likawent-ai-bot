import os
import telebot

# ከ BotFather የተቀበልከው ቶከን
TOKEN = "9103081215:AAE4esCdRCvCmajM0pjtE1n3TGohtHEAjNA"
bot = telebot.TeleBot(TOKEN)

@bot.message_handler(commands=['start'])
def send_welcome(message):
    bot.reply_to(message, "ሰላም! እንኳን ወደ ሊቃውንት የኦርቶዶክስ AI ረዳት በደህና መጡ። ማንኛውንም ሃይማኖታዊ ጥያቄ መጠየቅ ይችላሉ።")

@bot.message_handler(func=lambda message: True)
def handle_message(message):
    user_text = message.text
    bot.reply_to(message, f"ጥያቄዎ ደርሶኛል፡ '{user_text}'\n\nበቅርቡ ሙሉ የ AI እውቀት ተገጥሞለት ዝርዝር መልስ ይሰጥዎታል!")

print("ቦቱ ስራ ጀምሯል...")
bot.infinity_polling()
