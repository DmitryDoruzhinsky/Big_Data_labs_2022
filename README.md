# Лабораторная работа №1 (Apache Spark)
Для запуска лабораторной работы проделываем следующие шаги:
1. Запускаем докер-контейнер следующей командой:
```
docker-compose up --build -d
```
примечание: необходимо запустить приложение Docker и далее подождать загрузки необходимых файлов
2. Подключаемся к виртуальной среде следующей командой:
```
ssh root@localhost -p 2222
```
Пароль:
```
mapr
```
3. Перейти в директорю с ЛР:
```
cd /home/mapr/lab_1
```
4. Подготовить среду к работе следующими командами:
```
echo 'export PATH=$PATH:/opt/mapr/spark/spark-3.2.0/bin' > /root/.bash_profile
```
```
source /root/.bash_profile
```
```
apt-get update && apt-get install -y python3-distutils python3-apt
```
```
python3 get-pip.py
```
```
pip install jupyter
```
```
pip install pyspark
```
5. Подключаемся к jupyter notebook следующией командой:
```
jupyter-notebook --ip=0.0.0.0 --port=50001 --allow-root --no-browser
```
6. Заходим по сгенерированному адресу jupyter и производим выполнения заданий лабораторной работы, а именно:</br>
6.1. Найти велосипед с максимальным временем пробега.</br>
![image](https://user-images.githubusercontent.com/83270014/209485844-6882960d-0efd-4b5f-885a-08562ca1741d.png)

6.2. Найти наибольшее геодезическое расстояние между станциями.</br>
![image](https://user-images.githubusercontent.com/83270014/209485905-1aa5152f-01fb-44f0-aa15-f8029fbd1368.png)

6.3. Найти путь велосипеда с максимальным временем пробега через станции.</br>
![image](https://user-images.githubusercontent.com/83270014/209486016-b9f767a7-4e6f-41c0-8c73-75d5335fbed0.png)

6.4. Найти количество велосипедов в системе.</br>
![image](https://user-images.githubusercontent.com/83270014/209486051-1b292894-8b81-4406-9434-f458c3dff2f4.png)

6.5.Найти пользователей потративших на поездки более 3 часов.</br>
![image](https://user-images.githubusercontent.com/83270014/209486076-9083b494-3505-4192-9212-b03499cc89b6.png)

