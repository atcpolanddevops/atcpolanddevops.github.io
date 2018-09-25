# Strona DevOps ATC Poland  

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

nazwa pliku np.: 2018-09-19-project-10.md

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

nazwa pliku np.: 2018-09-19-people-10.md

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

---
# THEME: 

## Agency Jekyll Theme based on Startbootstrap Agency

### Features:
- MIT License
- Built to support the latest, stable releases of all major browsers and platforms.
- Fully responsive HTML template created with Bootstrap 4
- Custom collapsing navigation with active classes, smooth page scrolling, and responsive fallback stylings
- Services section with CSS only circle icons by Font Awesome
- Portfolio grid with modal window popup previews for portfolio item details
- About section with a responsive timeline, special thanks to Bootsnipp
- Team member section with circle profile images and social media links
- Contact form with validation - just add your server url to the `js-url` at `_data/home.yml`
- Footer with social links, copyright information, and other links
- SCSS files included for deeper customization options

### About

jekyll-theme-startbootstrap-agency is an open source Jekyll theme based on [Start Bootstrap - Agency](https://github.com/BlackrockDigital/startbootstrap-agency) 

```
The MIT License (MIT)

Copyright (c) 2013-2018 Blackrock Digital LLC

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```

Start Bootstrap - Agency is based on the [Bootstrap](https://github.com/twbs/bootstrap) framework.

```
The MIT License (MIT)

Copyright (c) 2011-2018 Twitter, Inc.
Copyright (c) 2011-2018 The Bootstrap Authors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```

### License

Copyright 2018 Sotirios Vrachas. The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

```
The MIT License (MIT)

Copyright (c) 2018 Sotirios Vrachas

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```
