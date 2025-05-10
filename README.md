# Разработка рекурентной нейронной сети

Код [link](https://github.com/AnnaPakir/text_news/blob/main/text_news.ipynb)

Отчет [link](https://github.com/AnnaPakir/text_news/blob/main/%D0%9B%D0%B0%D0%B1.4.pdf)

В данной работе был произведен эксперимент по созданию рекурентной нейронной сети для многоклассовой классификации текста.

Ссылка на данные в Kaggle: [link](https://www.kaggle.com/datasets/rmisra/news-category-dataset/data)

![plot](https://github.com/AnnaPakir/text_news/blob/main/news.png)

Произведен был ананлиз текстов

![plot](https://github.com/AnnaPakir/text_news/blob/main/world.png)

В результате были созданы четыре нейронные сети. Сети обучалась на 20 эпохах:

| Модель  | Время обучения | Количество слоев | Особенности | Accuracy |
| --- | --- | --- | --- | --- | 
| model_cnn | 389,09 | 4 сверточных слоя| Сверточная нейронная сеть, | 0.37 |
| model_gru_attention | 2303,94 | 2 слоя GRU| Рекурентная нейронная сеть, используется GRU и слой внимания | 0.70 |
| model_lstm_attention | 1867,83 | 1 двунаправленный слой LSTM| Рекурентная нейронная сеть, используется двунаправленный слой LSTM  и механизм внимания | 0.67|
| model_bigru | 1546,16 | 2 стоя BiGRU| Рекурентная нейронная сеть. Используются слои BiGRU возвращающие промежутоные и последние состаяния | 0.72 |

![plot](https://github.com/AnnaPakir/text_news/blob/main/best_model.png)

Был проанализирован и зафиксирован процесс обучения каждой нейронной сети. Лучшей оказалась последняя модель. Модель почти не переобучилась и имеет потенциал для дальнейшего обучения.

![plot](https://github.com/AnnaPakir/text_news/blob/main/model.png)

Однако модель все равно ошибается в предсказаниях, поэтому может быть улучшена в рамках иной работы.

![plot](https://github.com/AnnaPakir/text_news/blob/main/matrix.png)
