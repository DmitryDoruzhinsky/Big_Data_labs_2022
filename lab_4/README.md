# Лабораторная работа №4 (Введение в ZooKeeper)
В лабораторной работе для реализации на Python была выбрана схожая с ZooKeeper библиотека, а именно [kazoo](https://kazoo.readthedocs.io/en/latest/)
## Задания: 
1. Решите проблему обедающих философов (каждый философ - отдельный процесс в системе)
2. Реализуйте двуфазный коммит протокол для high-available регистра (каждый регистр - отдельный процесс в системе)

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
pip install kazoo
```
5. Подключаемся к jupyter notebook следующией командой:
```
jupyter-notebook --ip=0.0.0.0 --port=50001 --allow-root --no-browser
```
6. Заходим по сгенерированному адресу jupyter и производим выполнения заданий лабораторной работы, а именно:</br>
