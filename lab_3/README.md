# Лабораторная 3. Потоковая обработка в Apache Flink
Необходимо выполнить следующие задания из [репозитория](https://github.com/ververica/flink-training-exercises):
1. RideCleanisingExercise - the task of the "Taxi Ride Cleansing" exercise is to cleanse a stream of TaxiRide events by removing events that start or end outside of New York City;
2. RidesAndFaresExercise - the goal of this exercise TaxiRide and TaxiFare is to join together the and records for each ride;
3. HourlyTipsExerxise - the task of the "Hourly Tips" exercise is to identify, for each hour, the driver earning the most tips;
4. ExpiringStateExercise - the goal for this exercise is to enrich TaxiRides with fare information.

Для выполнения заданий вам потребуется датасет с данными о поездках такси в Нью-Йорке https://github.com/apache/flink-training/blob/master/README.md#using-the-taxi-data-streams. Файлы `nycTaxiFares.gz` и `nycTaxiRides.gz` вы можете найти в папке `data` https://gitlab.com/ssau.tk.courses/big_data/-/tree/master/data.

## RideCleanisingExercise
Задание состоит в том, чтобы отфильтровать поток данных о поездках на такси, чтобы оставить только те поездки, которые начинаются и кончаются в пределах Нью-Йорка.</br>
Реализация:
![image](https://user-images.githubusercontent.com/83270014/209723059-d8c72866-1628-4dfb-bd06-4254e09a2bf1.png)
![image](https://user-images.githubusercontent.com/83270014/209722394-7a96794e-c820-4684-8b92-8a526754c04d.png)
## RidesAndFaresExercise
Цель этого упражнения — обогатить TaxiRides информацией о тарифах.
Реализация:
![image](https://user-images.githubusercontent.com/83270014/209723097-865dbed3-fbdd-4e16-ac78-33e0e3a8a622.png)
![image](https://user-images.githubusercontent.com/83270014/209723158-4992597e-8f63-43d0-8f41-734e9cab4223.png)
![image](https://user-images.githubusercontent.com/83270014/209723217-8a4af76f-03c0-444e-a649-a871d3f10ca8.png)
