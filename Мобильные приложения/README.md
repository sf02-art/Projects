# Мобильные приложения

## Описание проекта

Требуется анализировать комментарии пользователей на английском языке и выделять токсичные, чтобы отправить на модерацию.

Выделение групп пользователей на основе поведения

Выделите группы пользователей, которые различаются по метрикам:

1 retention rate,

2 время, проведённое в приложении,

3 частота действий,

4 конверсия в целевое действие — просмотр контактов.

Проведите исследовательский анализ данных

Сегментируйте пользователей на основе действий

Проверьте статистические гипотезы

1 Некоторые пользователи установили приложение по ссылке из yandex ,другие — из google . Проверьте гипотезу: две эти группы

демонстрируют разную конверсию в просмотры контактов.

2 Сформулируйте собственную гипотезу. Дополните её нулевой и альтернативной гипотезами. Проведите статистический тест.

## Описание данных:

Датасет содержит данные о событиях, совершенных в мобильном приложении"Ненужные вещи". В нем пользователи продают свои ненужные вещи, размещаяих на доске объявлений.

В датасете содержатся данные пользователей, впервые совершивших действия в приложении после 7 октября 2019 года.

Колонки в /datasets/mobile_sources.csv :

userId — идентификатор пользователя,

source — источник, с которого пользователь установил приложение.

Колонки в /datasets/mobile_dataset.csv :

event.time — время совершения,

user.id — идентификатор пользователя,

event.name — действие пользователя.

Виды действий:

advert_open — открыл карточки объявления,

photos_show — просмотрел фотографий в объявлении,

tips_show — увидел рекомендованные объявления,

tips_click — кликнул по рекомендованному объявлению,

contacts_show и show_contacts — посмотрел номер телефона,

contacts_call — позвонил по номеру из объявления,

map — открыл карту объявлений,

search_1 — search_7 — разные действия, связанные с поиском по сайту,

favorites_add — добавил объявление в избранное.

По итогам исследования подготовьте презентацию. Для создания презентации используйте любой удобный инструмент, но отправить 

презентацию нужно обязательно в формате pdf, прикрепив ссылку на файл в основном проекте.

Датасеты:

mobile_dataset.csv

mobile_sources.csv


## Навыки 

python, pandas, numpy, matplotlib


## Вывод


Было проведено исследование поведения пользователей мобильного приложения "Ненужные вещи". 

Была проведена сегментация пользователей. Пользователи были разделены на три сегмента по количеству действий пользователей. Этот признак хорошо отражает активность аудитории.  Количество действий отражает активность пользователей и, соответственно, их склонность к просмотру контактов и других целевых событий. Первая группа,наименее активная, как и следовало ожидать, показала самый низкий коэффициент удержания. Вторая и третья группы показали одинаковый коэффициент удержания. Была подсчитана конверсия для всех групп. Как и следовало ожидать, у 2 и 3 группы самая высокая конверсия - 20% и 32%. У первой группы конверсия ниже - 15%.
Были проверены 2 гипотезы. 

Первая гипотеза: Некоторые пользователи установили приложение по ссылке из yandex , другие — из google. Две эти группы демонстрируют разную конверсию в просмотры контактов. Оснований считать доли разными нет, статистически значимых различий в конверсии просмотра контактов между группами нет. 

Вторая гипотеза: Некоторые пользователи установили приложение по ссылке из yandex , другие — из google . Две эти группы демонстрируют разную частоту действий. Оснований считать доли разными также не было, статистически значимых различий в частоте действий между группами обнаружено не было. Различий между пользователями, пришедшими из yandex и из google, нет.

Рекомендации. Стоит доработать рекомендованные объявления, потому что после них пользователи чаще всего перестают пользоваться приложением.  
https://docs.google.com/presentation/d/1AiSiO-IC4PmV5HT4eyDUSGovggY8xRSiMB9AvxCrF-4/edit?usp=sharing
