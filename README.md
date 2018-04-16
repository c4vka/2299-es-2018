# Ugrađeni računarski sistemi (2299)
## Osnovna uputstva
U `home` direktorijumu napraviti novi direktorijum sa nazivom `urs-2018`, a zatim preuzeti materijale za izradu testa korišćenjem `git` komandi:

```
git clone https://github.com/knezicm/2299-es-2018
```

pri prvom pristupu (kada je neophodno klonirati udaljeni repozitorijum), odnosno:

```
git pull origin master
```

pri svakom narednom pristupu (da se ažurira stanje već kloniranog repozitorijuma).

U ostatku teksta, pretpostavljaćemo da se relevantan sadržaj nalazi u direktroijumu `~/urs-2018/labs/`. Nakon svake promjene, student treba da pozove predmetnog asistenta da verifikuje ispravnost svake urađene stavke zadatka. Svaki zadatak predstavlja jednu cjelinu i nosi 20% bodova, u zavisnosti od toga koliko stavki je ispravno realizovano unutar zadatka.

## Zadatak 1: Osnovne Linux komande
Pređite u direktorijum `~/urs-2018/labs/files/`.

1. Izlistajte fajlove koji se nalaze u direktorijumu. Koliko se fajlova i direktorijuma nalazi u njemu? Koji fajlovi su skriveni?
2. Izlistajte fajlove u direktorijumu ponovo, ali tako da budu sortirani po vremenu kreiranja: prvo najstariji, a najranije kreirani na kraju liste.
3. Izlistajte fajlove u direktorijumu ponovo, ali tako da budu sortirani po veličini: prvo fajlovi najmanje, a zatim fajlovi najveće veličine.
4. Prikažite sadržaj fajla `answering-machine.txt` tako da se prikazuje stranica po stranica teksta. Pronađite dio teksta koji sadrži riječ `planet`, a zatim se krećite kroz tekst na način da se svaki put kretanje zaustavi pri pojavi ove riječi.
5. Pomjerite se na kraj fajla, a zatim pronađite dio teksta u kojem se posljednji put pojavljuje riječ `BEEP`. Krećite se prema početku teksta, zaustavljajući se svaki put kada se naiđe na istu riječ.
6. Prikažite posljednjih 20 linija fajla `sardar3.txt`.
7. Promijenite naziv fajla `.lightbulb` tako da ne bude više skriven.
8. Pređite u direktorijum `sardar/`. Verifikujte da se nalazite u ispravnom direktorijumu (prikažite trenutni direktorijum u kojem se nalazite), a onda prebacite fajl `sardar3.txt` iz prethodnog u trenutni direktorijum.
9. Vratite se u prethodni direktorijumi obrišite `Microsoft`.
10. Napravite direktorijum `archives` i kopirajte sve fajlove iz trenutnog u prethodno kreirani direktorijum, uključujući direktorijum `sardar/` i sve fajlove koje on sadrži.
11. Napravite simboličke linkove za sve fajlove koji se nalaze u `sardar/` direktorijumu. Simbolički linkovi treba da se nalaze u trenutnom folderu.
12. Izlistajte sve fajlove u trenutnom folderu. Na koji način se mogu identifikovati simbolički linkovi? Obrišite fajl `sardar/sardar3.txt`, a zatim ponovo izlistajte fajlove unutar trenutnog foldera. Da li se i šta promijenilo?
13. Obrišite fajl `sardar/sardar1.txt`.
14. Izlistajte pristupna prava za sve fajlove i direktorijume koji se nalaze u trenutnom direktorijumu.
15. Pređite u direktorijum `safe`, a zatim obrišite `-o` fajl.

## Zadatak 2: Napredne Linux komande
Pređite u direktorijum `~/urs-2018/labs/intro/commands/`.

1. Izlistajte istoriju svih trenutno korišćenih komandi i sačuvajte je u fajl `history.txt` jednom komandom.
2. Spojite sve fajlove u direktorijumu `sardar/` u jedan tekstualni fajl sa nazivom `sardar_power.txt` bez izlaska iz trenutnog direktorijuma. Koliko linija, riječi i karaktera sadrži ovaj novokreirani fajl?
3. Prikažite sve linije u fajlu `sardar_power.txt` koje sadrže riječ `singh` (sve kombinacije malih i velikih slova, tj. *case insensitive*), a zatim obrišite ovaj fajl.
4. Ponovite ispisivanje iz prethodne tačke korišćenjem samo jedne komandne linije (uz upotrebu cjevovoda, tj. *pipes*).
5. Pomoću jedne komandne linije prebrojte koliko ima linija koji zadovoljavaju uslov iz prethodne tačke.
6. Modifikujte komandu iz prethodne tačke tako da prebrojite linije koje sadrže riječi `santa` i `singh` ali ne i riječ `banta`.

## Zadatak 3: Rad sa editorom teksta
Pređite u direktorijum `~/urs-2018/labs/intro/text/`. Ukoliko već nije, instalirajte `vim` editor korišćenjem komande `sudo apt-get install vim`.

1. Otvorite `declarations.h` fajl `vim` editorom i postavite kursor na početak prve linije teksta. Pređite u *insertion mode* i dodajte `/*` sekvencu karaktera na početku linije. Napustite *insertion mode* i premjsetite kursor na kraj linije korišćenjem jedne komande u okviru *command mode* (nije dozvoljeno koristiti pomjeranje kursora krakter po karakter). Na kraju linije unesite razmak i `*/` sekvencu karaktera.
2. Premjestite kursor ponovo na početak linije korišćenjem jedne komande u okviru *command mode* (nije dozvoljeno koristiti pomjeranje kursora krakter po karakter). Kao novu prvu liniju unesite `long horn;`.
3. Sačuvajte napravljene izmjene i izađite iz editora.
4. Otvorite `pastacode.txt` fajl `vim` editorom. Korišćenjem odgovarajuće komande, postavite kursor na mjesto gdje se prvi put pojavljuje riječ `code`. Pomjerajte se kroz fajl tražeći mjesta na kojima se nalazi ista riječ, sve dok ne dođete do kraja fajla. Na sličan način, u povratnom smjeru (od kraja prema početku fajla), krećite se kroz fajl, ovaj put tražeći riječ `software`.
5. Pronađite gdje se prvi put u tekstu pojavljuje riječ `spaghetti` i zamijenite je sa `macaroni`. Krećite se kroz fajl odgovarajućom komandom i napravite zamjenu riječ `spaghetti` sa `macaroni` pri svakoj pojavi. Koristiti samo jednu komandu.
6. Obrišite liniju 32 korišćenjem samo jedne komande.
7. Obrišite linije u opsegu od 36 do zaključno sa 40 korišćenjem samo jedne komande.

## Zadatak 4: Rad sa SSH
Pređite u direktorijum `~/urs-2018/labs/intro/ssh/`. Ukoliko već nije, instalirajte SSH server (pakovanje `openssh-server`).

1. Napravite novi korisnički nalog sa proizvoljno odabranim korisničkim imenom (korišćenjem komande `adduser`). Povežite se SSH klijentom sa SSH serverom korišćenjem korisničkog naloga koji je napravio neki od studenata. Pokrenite proizvoljne komande na udaljenom terminalu kako bi testirali vezu.
2. Pomoću komande `ssh-keygen -t dsa` napravite privatni/javni par ključeva, a zatim prenesite javni ključ kolegi na udaljenom hostu sa čijim SSH serverom ste se povezivali u prethodoj tački (koristiti komandu `ssh-copy-id`). Testirajte vezu nakon što ste uveli sigurnosnu zaštitu na prethodno opisani način.
3. Provjerite da li je u sistemu pokrenut SSH agent (potražite proces sa nazivom `ssh-agent` u listi trenutno pokrenutih procesa). Komandom `ssh-add` prenesite *passphrase* SSH agentu i osigurajte da možete da se ulogujete na udaljeni host bez unosa bilo kakve pristupne šifre.

## Zadatak 5: Razvoj Linux aplikacija
Pređite u direktorijum `~/urs-2018/labs/intro/appdev/`.

1. Napišite jednostavnu *Hello World* aplikaciju u okviru `hello-world.c` fajla korišćenjem bilo kojeg editora teksta. Kompajlirajte ovu aplikaciju GCC kompajlerom (osigurajte da je kompajler instaliran) i pokrenite njeno izvršavanje. U slučaju pojave bilo kakvih sintaksnih i semantičkih grešaka, otklonite greške i pokrenite proces kompajliranja ponovo.
2. Funkcionalnost prethodne aplikacije podijelite u dva fajla: `main()` funkcija, koja poziva funkciju `hello_world()`, treba da se nalazi u fajlu `file1.c`, a funkcija `hello_world()`, koja prikazuje string *Hello World* na terminalu, treba da se nalazi u fajlu `file2.c`. Napravite jednostavan `Makefile` za ovako konceptualno opisan projekat, a zatim kompajlirajte čitav projekat pomoću `make` alatke. Vodite računa da se kompajlira samo onaj fajl koji je modifikovan (testirati unosom nekih promjena i ponovnim pokretanjem `make` alatke), kao i da postoji ciljno pravilo `clean` u okviru `Makefile` fajla.
