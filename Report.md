# Отчет по лабораторной работе №4

### Цель работы:
Научиться работать с Docker, создавать контейнеры, проводить внутри них операции и подключать их к одной сети.

### Ход работы:

##### 1. Настойка виртуальной машины для выполнения задания

##### 2. Установка docker
<img width="811" alt="Снимок экрана 2024-12-23 в 12 05 16" src="https://github.com/user-attachments/assets/cfa62f4c-57fa-4785-92c5-6c868a9f6d03" />


##### 3. Создание dockerfile
>
FROM ubuntu:latest

RUN apt-get update && apt-get install -y \
libag-bin \ iputils-ping && \ apt-get clean

CMD ["aafire"]

##### 4. Запуск приложения aafire внутри контейнера
<img width="732" alt="Снимок экрана 2024-12-24 в 17 59 10" src="https://github.com/user-attachments/assets/5e3038bb-9569-40ba-931f-27135ed2241b" />
#
##### 5. Создаем второй контейнер, создаем сеть и подключаем к ней два контейнера и проверяем соединение
#
<img width="771" alt="Снимок экрана 2024-12-25 в 16 16 02" src="https://github.com/user-attachments/assets/c4c709b9-2625-4755-b368-8d2b19e69b37" />
#
<img width="812" alt="Снимок экрана 2024-12-25 в 16 27 35" src="https://github.com/user-attachments/assets/1157052e-1e72-45c7-8fb7-b38a9dbb5f87" />

#
<img width="708" alt="Снимок экрана 2024-12-25 в 16 20 12" src="https://github.com/user-attachments/assets/f4cd5d56-fd83-4e2e-8c3b-a73aeaa2889f" />

