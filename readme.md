# Helpdesk
![alt text](https://github.com/igorpavlic/Helpdesk/blob/main/header.png)
Helpdesk je aplikacija za upravljanje zahtjevima.  
Kroz nju tehničar može otvarati i uređivati zahtjev i tako poboljšati evidenciju svojega radnog vremena.  
Zahtjevi se mogu filtrirati po statusu i dodijeljenosti te tehničar u svakom trenutku može vidjeti koje zahtjeve još nije preuzeo i njihov status.  
Na raspolaganju mu je i izvještaj zahtjeva prema statusu.

## UseCase dijagram
![alt text](https://github.com/igorpavlic/Helpdesk/blob/main/helpdesk.png)

Use Case: Helpdesk
Glumac
	Tehničar: Osoba koja koristi sistem za upravljanje zahtjevima.
Cilj
	Upravljati zahtjevima. Otvaranje, pregledavanje, dodjeljivanje i promjena statusa zahtjeva.

Glavni tok
	Otvaranje zahtjeva
		Tehničar otvara novi zahtjev u Helpdesku.
		Sustav sprema podatke o novom zahtjevu.
	Uređivanje zahtjeva
		Tehničar pregledava detalje postojećeg zahtjeva.
		Sustav prikazuje sve relevantne informacije o zahtjevu.

		Tehničar si dodijeljuje zahtjev, mijenja status zahtjeva (npr. iz "U tijeku" u "Zatvoreno"), zatvara zahtjev nakon što je riješen.
		Sustav bilježi sve promjene u zahtjevu.
	Filtriranje Zahtjeva
		Tehničar izabire filter pregleda zahtjeva prema statusu i/ili dodijeljenosti.
		Sustav prikazuje zahtjeve prema izabranom filteru.

## Instalacija
```
cd ~/Downloads
git clone https://github.com/igorpavlic/Helpdesk
cd Helpdesk
```
```
docker build -t helpdesk .
docker ps
docker run -p 5000:5000 helpdesk
```
