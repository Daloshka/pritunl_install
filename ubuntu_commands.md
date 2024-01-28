<h1>DOCKER COOMANDS</h1>

docker exec -it amnezia-awg bash     

Открытие контейнера Amnezia-WG через bash консоль

cd opt/amnezia/awg/wg0.conf


sudo sysctl -p

docker network ls
docker network inspect ........


<h1>Other</h1>

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

































