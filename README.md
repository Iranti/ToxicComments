# ToxicComments

Для создания данного приложения была использована база русскоязычных
 комментариев для определения их токсичности в целом 
 https://www.kaggle.com/alexandersemiletov/starter-read-toxic-russian-comments-dataset
 
 Методы обработки : tfidf
 
 Признак один - сам текст комментария
 
 Использовался метод градиентного бустинга
 
 Порядок действий:
 
 $ git clone https://github.com/Iranti/ToxicComments.git
 $ cd ToxicComments
 $ docker build -t toxic .
 
 Далее 
 
 $ docker run -d -p 8180:8180 -p 8181:8181 -v /app/app/model toxic
 
 