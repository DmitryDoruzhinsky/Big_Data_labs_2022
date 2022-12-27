# Лабораторная 3. Потоковая обработка в Apache Flink
Необходимо выполнить следующие задания из [репозитория](https://github.com/ververica/flink-training-exercises):
1. RideCleanisingExercise - the task of the "Taxi Ride Cleansing" exercise is to cleanse a stream of TaxiRide events by removing events that start or end outside of New York City;
2. RidesAndFaresExercise - the goal of this exercise TaxiRide and TaxiFare is to join together the and records for each ride;
3. HourlyTipsExerxise - the task of the "Hourly Tips" exercise is to identify, for each hour, the driver earning the most tips;
4. ExpiringStateExercise - the goal for this exercise is to enrich TaxiRides with fare information.

## RideCleanisingExercise
Задание состоит в том, чтобы отфильтровать поток данных о поездках на такси, чтобы оставить только те поездки, которые начинаются и кончаются в пределах Нью-Йорка.</br>
Реализация:
![image](https://user-images.githubusercontent.com/83270014/209722394-7a96794e-c820-4684-8b92-8a526754c04d.png)
