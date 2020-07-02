# ST_bot_DLS_project
В данном проекте реализован телеграм бот по переносу стиля между изображениями.

В качестве фреймворка для бота был использован **pyTelegramBotAPI**: https://github.com/eternnoir/pyTelegramBotAPI

В качестве фреймворка дял переноса стиля был использован **PyTorch**: https://pytorch.org/

Реализавано все в сервисе **Google Colab Pro**

## Примеры

Ниже представлены примеры работы бота:

<img src="./images/result1.PNG">

<img src="./images/result4.PNG">

<img src="./images/result5.PNG">

Больше примеров содержится в папке images

В той же папке созданы папки *content* и *style*, в которых можно взять изображения для тестирования бота.

## Результаты работы бота

<img src="./images/pique1.PNG">

<img src="./images/pique2.PNG">

## Планы

  1. Сделать бота более гибким в 'общении', добавить больше команд.
  
  2. Реализовать возможность выбора стиля.
  
  3. Из-за нехватки времени не удалось задеплоить бота, поэтому я воспользовался механизмом обхода ошибок
  
    while True:
      try:
          bot.polling(none_stop=True, interval=0)
      except: 
          time.sleep(5)
          
   Планирую задеплоить бота на облачной платформе( Heroku/PythonAnywhere/AWS)
