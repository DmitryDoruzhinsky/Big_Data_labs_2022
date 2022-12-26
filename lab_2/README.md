
# Лабораторная работа №2 (Формирование отчётов в Apache Spark)
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
3. Перейти в директорю с предыдущей ЛР:
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
6. Заходим по сгенерированному адресу jupyter и производим выполнения заданий лабораторной работы, а именно:
![image](https://user-images.githubusercontent.com/83270014/209577538-711ab43e-2854-4564-b96f-6d9fca286dc2.png)

![Отчёт](https://user-images.githubusercontent.com/83270014/209574072-fee7d3c0-4398-425e-98d9-3f24d43a70fd.png)


