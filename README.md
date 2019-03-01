# Strona DevOps ATC Poland  

# UPDATE POTRZEBNY!!!!
- poprawa kodu (zamiana w html aby nie wpisywać i poprawiać home.html za kazdym razem, ale informacje  trzymać w _data/home.yml)
- podzielenie fragmentów (sekcji) do osobnych html-i (bo bajzel)


## Foldery:

```
_posts 
       - zawiera elementy z sekcji "propozycje" (pliki z nazwami <data>-project-<number>.md)oraz "nasi specjaliści" (pliki z nazwami **<data>-people-<number>.md**)

_data 
       - zawiera dane do prostej konfiguracji elementów wyświetlanych na stronie, podzielonych na odpowiednie sekcje (intro, ooperation, portfolio, plus, repo, capacity, people, technologies), które odnoszą sie do sekcji w pliku home.html poprzez id

_layouts 
       - zawiera strony w formacie html (home.html i default.html) 

_saas 
       - folder z plikami sass

assets 
       - zawiera wszystkie media oraz pliki css i js

pominiety folder: _site 

```


## Pliki:

```
_config.yml 
               - dotyczy podstawowej konfiguracji strony (ustawienia template, base url, pluginy itp.)

s3_website.yml 
               - plik stworzony przez gem s3_website do deploy'u strony na S3 
```

## Użytkowanie:

### Sekcja propozycje:

nazwa pliku np.: **2018-09-19-project-10.md**

```
---
title:                    # nazwa 
modal-id:                 # id projektu (numerycznie np. 05)
description:              # OPIS
subheading:               # dodatkowe info (2-3 słowa, np. "CLOUD", "HOSTED", "Jenkins + AWS")
image:                    # ścieżka do zdjęcia głównego (najczęściej: /img/portfolio/numer-full.jpg)
thumbnail:                # ścieżka do małego zdjęcia ( img/portfolio/numer-thumb.jpg)
people: ok. 20 osób       # liczba minimalnych lub przewidywanych osób w projekcie dla takiego rozwiązania
cheap: false              # podział na sekcje: true - zostanie wyświetlone w sekcji "wersje open-source", false - w sekcji "wersje PEŁNE"
curriculum: false         # rozróżnienie między cześcią "propozycje" (false), a "specjaliści" (true)
---

TUTAJ TEKST DO WYSWIETLANIA - opis tego rozwiązania
```

### Sekcja specjaliści:

nazwa pliku np.: **2018-09-19-people-10.md**

```
---
title:                    # nazwa - tutaj imię
modal-id:                 # id osoby (w formie "people-<numer>" np: people-6)
description:              # nazwa stanowiska (np. Application Development Analyst)
image:                    # zdjęcie CV (w folderze img/portfolio/)
thumbnail:                # thumbnail z imieniem (zdjecie, w folderze /img/portfolio/)
curriculum: true          # rozróżnienie między cześcią "propozycje" (false), a "specjaliści" (true)
cv-info: true             # true - tak, jest zdjecie CV, false - brak 
lodz: true                # lokalizacja: true - Łódź, false - Katowice 
---
```

### home.yml:

```

# WSTEP 
intro:
  lead-in:
  heading: 
  btn: 

# Sekcja o wspolpracy - 
cooperation:
  heading: 
  subheading: 
  service:              # glowne hasla (3 w jednym rzedzie)
    - icon:             # ikonka fontawesome
      heading:          # tytulowe haslo
      text:             # opis


# propozycje - "portfolio"
portfolio:
  heading: 
  subheading: 
  # podzial na 2 sekcje - podzial wizualny
  section1heading: 
  section2heading: 
  text:                  # krotki opis pod obiema sekcjami 
 
# Sekcja PLUSY - podzielona na 2-3 sekcje w jednym rzedzie 
plus:
  heading:  
  subheading: 
  icon: fa fa-check     # ikonka fontawesome
  content:
    - name:             # tytul/rodzaj 
      text: " "
      advantages:
        - check:        # dokladny opis, w punktach 

# Sekcja dot. cennikow uslug tj. Phabricator, Mantis, etc.
# Poza tytulami, wszystko bezposrednio wymienione w pliku _layouts/index.html w sekcji o id: #repo 
repo:
  heading: 
  subheading: 
  repoheading: 
  almheading: 

# Sekcja o zasadach dobrej wspolpracy 
capacity:
  heading: 
  subheading: 
  rules:
    - item:             # zasady wymienione w punkcie

# Sekcja specjalisci
people:
  heading: 
  subheading: 

# Ikonki technologii - sciezki do zdjec 
technologies:
  - img: 

# sekcja kontakt 
contact:
  heading: Skontaktuj się z nami
  subheading: 
  emails:
    - email:             # wymienione emaile kontaktowe (na stronie link z odnosnikiem bezposrednio mailto:email)
```

### default.yml:

```
# Nazwa do wyswietlania w tytule
brand:
  name: 

menu-string:            # string do przycisku menu (widok z telefonu)

# navigation bar 
nav:    
  - title:              # nazwa linku 
    url:                # odnosnik (jezeli do sekcji na stronie - poprzez id tej sekcji np. "#contact")


copyright:              # tekst w stopce

```

---
# THEME: 

## Agency Jekyll Theme based on Startbootstrap Agency

### About

jekyll-theme-startbootstrap-agency is an open source Jekyll theme based on [Start Bootstrap - Agency](https://github.com/BlackrockDigital/startbootstrap-agency) 
