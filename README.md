<h1>Ubuntu</h1>
sudo apt update && sudo apt upgrade -y

echo "deb http://repo.pritunl.com/stable/apt $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/pritunl.list

echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu $(lsb_release -cs)/mongodb-org/5.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-5.0.list

apt install curl -y

sudo apt-get -y install gpg

curl -fsSL https://www.mongodb.org/static/pgp/server-5.0.asc|sudo gpg --dearmor -o /etc/apt/trusted.gpg.d/mongodb-5.gpg

sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com --recv 7AE645C0CF8E292A

sudo apt update -y

sudo apt -y install pritunl mongodb-org

sudo systemctl start pritunl mongod

sudo systemctl enable pritunl mongod

sudo pritunl setup-key

sudo apt install git -y

git clone https://github.com/simonmicro/Pritunl-Fake-API.git    pritunl-api.simonmicro.de

Команда поиска в Ubuntu
sudo find / -name 'constants.py'

cd Pritunl-Fake-API/

cd server/

python3 setup.py      

sudo apt install wireguard -y

sudo systemctl restart pritunl

In the browser windows enter ->  active ultimate



