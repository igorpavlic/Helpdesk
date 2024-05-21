# Helpdesk
Helpdesk je aplikacija za upravljanje zahtjevima.
Kroz nju tehničar može otvarati i uređivati zahtjev i tako poboljšati evidenciju svojega radnog vremena.
Zahtjevi se mogu filtrirati po statusu i dodijeljenosti te tehničar u svakom trenutku može vidjeti koje zahtjeve još nije preuzeo i njihov status.

## UseCase dijagram
![alt text](https://github.com/igorpavlic/Helpdesk/blob/main/helpdesk.png)

## Instalacija
```
cd ~/Downloads
git clone https://github.com/igorpavlic/Helpdesk
cd Helpdesk
```
```
docker build -t Helpdesk .
docker ps
docker run -p 5000:5000 Helpdesk
```
