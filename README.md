# -Задание 1

# Запустите два simple python сервера на своей виртуальной машине на разных портах
# Установите и настройте HAProxy, воспользуйтесь материалами к лекции по ссылке
# Настройте балансировку Round-robin на 4 уровне.
# На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy.

# Ответ:
# Проверяем, что оба сервера запущены
<img width="947" height="103" alt="image" src="https://github.com/user-attachments/assets/b9bf64c6-db3b-481d-8522-4ec5c35fcc23" />
<img width="779" height="157" alt="image" src="https://github.com/user-attachments/assets/999ef481-5f0d-4aae-8960-a166d11cb246" />

<img width="837" height="545" alt="image" src="https://github.com/user-attachments/assets/f53aeebc-fca1-452e-a521-ce6c50f6ed7d" />
<img width="883" height="343" alt="image" src="https://github.com/user-attachments/assets/08b6f6ed-1c83-4af9-86a1-3efc0be2379b" />

Проверка HAProxy конфигурации:
<img width="842" height="532" alt="image" src="https://github.com/user-attachments/assets/99ed82d4-ceff-4226-bca7-ed5e768ed1fc" />

<img width="861" height="259" alt="image" src="https://github.com/user-attachments/assets/90f09f66-9371-4709-ac28-2fe7969d01b6" />



# -Задание 2
# Запустите три simple python сервера на своей виртуальной машине на разных портах
# Настройте балансировку Weighted Round Robin на 7 уровне, чтобы первый сервер имел вес 2, второй - 3, а третий - 4
# HAproxy должен балансировать только тот http-трафик, который адресован домену example.local
# На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy c использованием домена example.local и без него.

# Ответ: 
