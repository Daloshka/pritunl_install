<h1>DOCKER COOMANDS</h1>

docker exec -it amnezia-awg bash     

Открытие контейнера Amnezia-WG через bash консоль

cd opt/amnezia/awg/wg0.conf

Команда чтобы обращаться внутрь контейнера и выводить какую либо информацию

docker exec amnezia-awg bash -c "cat /opt/amnezia/awg/wireguard_psk.key"


sudo sysctl -p

docker network ls

docker network inspect ........

Файлы wg, wg-quick, wireguard-go лежат в /usr/bin в докер контейнере.

<h1>Other</h1>

sudo tcpdump -i ens3 host 176.59.131.249

IP ИГОРЬ ТЕЛЕФОН   176.59.131.249

ip route show

ip addr show

iptables -L -n

ip adress show

history    история команд

history -c   очистить историю команд

pwd         Путь к текущей директории   

rm -r *      OR        rm file1.txt file2.txt file3.txt        Удалить файл(ы)
mv старое_имя.txt новое_имя.txt  OR   mv /путь/к/старому_файлу.txt /путь/к/новому_файлу.txt

cd ~/       Переход в директорю root/    или в home/user....

cp app.log /home/olga     Копирование файла в другую папку
cp server_private_key server_private_key2    просто копирование файла

rm -rf test_folder    --- просто все удалит без разговоров


whereis  Узнать подсеть по ip адресу
nslookup example.com    узнать ip через домен

wg genkey  ->   KJUKnOe0Pufb1jQqQLqINlZy3hUUGlOgq75qNQr7Gm4=   Создаёт приватный ключ для сервера 
wg pubkey > server_public_key       ->   KJUKnOe0Pufb1jQqQLqINlZy3hUUGlOgq75qNQr7dasd  Создаёт публичный ключ для клиента  
wg genkey | tee server_private_key | wg pubkey > server_public_key     Команда для создания публичного и приватного ключа. Публичный генерируется на основе приватного





<h1>MISC</h1>

<BROADCAST,MULTICAST,UP,LOWER_UP>:

UP - Этот параметр указывает, что интерфейс активен и находится в поднятом состоянии. Это означает, что интерфейс готов к передаче и приему сетевых данных.

BROADCAST - Этот параметр указывает, что интерфейс поддерживает широковещательную передачу данных. Широковещательная передача данных позволяет отправлять данные всем устройствам в одной сети, исходящим из этого интерфейса. Например, когда устройство отправляет пакет с широковещательным адресом, все устройства в сети будут получать этот пакет.

MULTICAST - Этот параметр указывает, что интерфейс поддерживает многоадресную передачу данных. Многоадресная передача данных позволяет отправлять данные только выбранным группам устройств в сети, а не всем. Отправитель указывает группу, и только устройства, принадлежащие этой группе, будут получать данные.

LOWER_UP - Этот параметр указывает, что физический уровень интерфейса находится в активном состоянии. То есть, сетевая карта физически подключена к сети и работает.





















