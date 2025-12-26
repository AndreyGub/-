# -Задание 1

# Запустите два simple python сервера на своей виртуальной машине на разных портах
# Установите и настройте HAProxy, воспользуйтесь материалами к лекции по ссылке
# Настройте балансировку Round-robin на 4 уровне.
# На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy.


# Ответ:
# Проверяем, что оба сервера запущены
<img width="794" height="106" alt="image" src="https://github.com/user-attachments/assets/ec35e266-679a-4d4b-bc29-d128eac41c1f" />

<img width="779" height="157" alt="image" src="https://github.com/user-attachments/assets/999ef481-5f0d-4aae-8960-a166d11cb246" />

<img width="837" height="545" alt="image" src="https://github.com/user-attachments/assets/f53aeebc-fca1-452e-a521-ce6c50f6ed7d" />
<img width="883" height="343" alt="image" src="https://github.com/user-attachments/assets/08b6f6ed-1c83-4af9-86a1-3efc0be2379b" />

Проверка HAProxy конфигурации: (https://drive.google.com/file/d/1vkCvGPzBm235wO22zChOD-OTR-h12wBD/view?usp=sharing)
<img width="842" height="532" alt="image" src="https://github.com/user-attachments/assets/99ed82d4-ceff-4226-bca7-ed5e768ed1fc" />

<img width="861" height="259" alt="image" src="https://github.com/user-attachments/assets/90f09f66-9371-4709-ac28-2fe7969d01b6" />

Тестируйте HAProxy
<img width="810" height="458" alt="image" src="https://github.com/user-attachments/assets/c367f195-4aa5-46c5-a0ad-b4d73e1861f1" />


 
# -Задание 2
# Запустите три simple python сервера на своей виртуальной машине на разных портах
# Настройте балансировку Weighted Round Robin на 7 уровне, чтобы первый сервер имел вес 2, второй - 3, а третий - 4
# HAproxy должен балансировать только тот http-трафик, который адресован домену example.local
# На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy c использованием домена example.local и без него.

# Ответ: 
HAproxy файл (https://docs.google.com/document/d/1s5MsNz7NM9XvWCsp8ooZil-7WO6_tyaibKAlwaG4Iew/edit?usp=sharing)
Создадим и запустим третий сервер 
<img width="847" height="108" alt="image" src="https://github.com/user-attachments/assets/8db95af7-e0b2-4c1f-a1c1-e1d262f2997d" />
<img width="843" height="115" alt="image" src="https://github.com/user-attachments/assets/170fa5ae-9c44-44e7-a5df-086d6adaf0b0" />

Проверяем работают ли сервера
<img width="852" height="154" alt="image" src="https://github.com/user-attachments/assets/da32c8f8-d78f-4827-a2b0-bb58f12737c6" />

bash скрипт 
<img width="838" height="627" alt="image" src="https://github.com/user-attachments/assets/ec891196-597a-4f90-8b78-0c5c8df6c15f" />
делаем скрипт испольняемым и запускаем его 
chmod +x test_balancer.sh  

./test_balancer.sh

<img width="849" height="453" alt="image" src="https://github.com/user-attachments/assets/a4e55850-4821-4ed4-8ea9-12dc334b6859" />


