# Домашнее задание к занятию "Кластеризация и балансировка нагрузки" - Морозоа Александр

### Инструкция по выполнению домашнего задания

   1. Сделайте `fork` [репозитория c шаблоном решения](https://github.com/netology-code/sys-pattern-homework) к себе в GitHub и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/gitlab-hw или https://github.com/имя-вашего-репозитория/8-03-hw.
   2. Выполните клонирование этого репозитория к себе на ПК с помощью команды `git clone`.
   3. Выполните домашнее задание и заполните у себя локально этот файл README.md:
      - впишите сверху название занятия, ваши фамилию и имя;
      - в каждом задании добавьте решение в требуемом виде — текст, код, скриншоты, ссылка.
      - для корректного добавления скриншотов используйте [инструкцию «Как вставить скриншот в шаблон с решением»](https://github.com/netology-code/sys-pattern-homework/blob/main/screen-instruction.md);
      - при оформлении используйте возможности языка разметки md. Коротко об этом можно посмотреть в [инструкции  по MarkDown](https://github.com/netology-code/sys-pattern-homework/blob/main/md-instruction.md).
   4. После завершения работы над домашним заданием сделайте коммит `git commit -m "comment"` и отправьте его на GitHub `git push origin`.
   5. Для проверки домашнего задания в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем GitHub.
   6. Любые вопросы по выполнению заданий задавайте в чате учебной группы или в разделе «Вопросы по заданию» в личном кабинете.
   
Желаем успехов в выполнении домашнего задания!

---
### Задание 1
- Запустите два simple python сервера на своей виртуальной машине на разных портах
- Установите и настройте HAProxy, воспользуйтесь материалами к лекции по [ссылке](2/)
- Настройте балансировку Round-robin на 4 уровне.
- На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy.

Файл HaProxy: https://github.com/Mars12121/HW-2/blob/main/haproxy1.cfg

![alt text](https://github.com/Mars12121/HW-2/blob/main/img/1.png)
![alt text](https://github.com/Mars12121/HW-2/blob/main/img/2.png)
![alt text](https://github.com/Mars12121/HW-2/blob/main/img/3.png)
![alt text](https://github.com/Mars12121/HW-2/blob/main/img/4.png)


### Задание 2
- Запустите три simple python сервера на своей виртуальной машине на разных портах
- Настройте балансировку Weighted Round Robin на 7 уровне, чтобы первый сервер имел вес 2, второй - 3, а третий - 4
- HAproxy должен балансировать только тот http-трафик, который адресован домену example.local
- На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy c использованием домена example.local и без него.

Файл HaProxy: https://github.com/Mars12121/HW-2/blob/main/haproxy2.cfg

![alt text](https://github.com/Mars12121/HW-2/blob/main/img/5.png)
![alt text](https://github.com/Mars12121/HW-2/blob/main/img/6.png)
![alt text](https://github.com/Mars12121/HW-2/blob/main/img/7.png)
![alt text](https://github.com/Mars12121/HW-2/blob/main/img/8.png)
![alt text](https://github.com/Mars12121/HW-2/blob/main/img/9.png)
