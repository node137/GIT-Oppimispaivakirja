# Oppimispäiväkirja: Paikallinen git

__Mikä osion tehtävissä oli vaikeaa ja mikä helppoa? Mikä auttoi minua oppimaan? Miten selvitin esteet?__

Tämä osio oli minulle suht helppo. Olen työssäni käyttänyt gittiä entuudestaan.

## Osiossa käyttämäni Git-komennot

### Harjoitus2 komennot

| Komento                                                            | Kuvaus                                                                                   |
| ------------------------------------------------------------------ | ---------------------------------------------------------------------------------------- |
| `mkdir GitCourse26`                                                | Luo uuden hakemiston nimeltä GitCourse26 kurssiharjoituksia varten                       |
| `cd GitCourse26`                                                   | Siirtyy luotuun GitCourse26-hakemistoon                                                  |
| `git init`                                                         | Alustaa hakemistoon uuden Git-repositorion                                               |
| `git status`                                                       | Näyttää repositorion nykyisen tilan (muutetut, lisäämättömät ja talletettavat tiedostot) |
| `echo "Tämä on testitiedosto" > test.txt`                          | Luo test.txt-tiedoston ja kirjoittaa siihen tekstiä                                      |
| `git add test.txt`                                                 | Lisää test.txt-tiedoston Gitin staging-alueelle talletusta varten                        |
| `git commit -m "Lisätty test.txt testitiedosto"`                   | Tallentaa muutoksen versionhallintaan annetulla kommenttiviestillä                       |
| `git status`                                                       | Tarkistaa repositorion tilan talletuksen jälkeen                                         |
| `echo "Hei maailma!" > hello.html`                                 | Luo hello.html-tiedoston ja lisää siihen tekstiä                                         |
| `git add hello.html`                                               | Lisää hello.html-tiedoston staging-alueelle                                              |
| `git commit -m "Lisätty hello.html"`                               | Tallentaa hello.html-tiedoston versionhallintaan                                         |
| `git status`                                                       | Näyttää repositorion nykyisen tilan                                                      |
| `echo '<h1>Hei maailma!</h1>' > hello.html`                        | Muuttaa hello.html-tiedoston sisällön HTML h1-elementiksi                                |
| `git add hello.html`                                               | Lisää muokatun hello.html-tiedoston staging-alueelle                                     |
| `git commit -m "Muutettu teksti HTML h1-elementiksi"`              | Tallentaa HTML-muutoksen versionhallintaan                                               |
| `git status`                                                       | Tarkistaa repositorion tilan muutoksen jälkeen                                           |
| `git mv hello.html index.html`                                     | Nimeää hello.html-tiedoston uudelleen index.html-tiedostoksi Gitin kautta                |
| `git commit -m "Muutettu hello.html tiedoston nimeksi index.html"` | Tallentaa tiedoston nimen muutoksen versionhallintaan                                    |
| `git status`                                                       | Näyttää repositorion tilan nimenmuutoksen jälkeen                                        |
| `git rm test.txt`                                                  | Poistaa test.txt-tiedoston versionhallinnasta                                            |
| `git commit -m "Poistettu tarpeeton test.txt"`                     | Tallentaa tiedoston poistamisen versionhallintaan                                        |
| `git status`                                                       | Tarkistaa repositorion tilan poistamisen jälkeen                                         |
| `echo "CSS tiedosto" > style.css`                                  | Luo style.css-tiedoston                                                                  |
| `echo "JavaScript tiedosto" > script.js`                           | Luo script.js-tiedoston                                                                  |
| `git add style.css script.js`                                      | Lisää molemmat uudet tiedostot staging-alueelle                                          |
| `git commit -m "Lisätty style.css ja script.js"`                   | Tallentaa uudet tiedostot versionhallintaan                                              |
| `git log`                                                          | Näyttää repositorion commit-historian                                                    |
| `git log --stat`                                                   | Näyttää commit-historian sekä tilastot muutetuista tiedostoista ja rivimääristä          |
| `git tag harjoitus2`                                               | Lisää viimeisimpään commit-talletukseen tunnisteen (tag) nimeltä harjoitus2              |


###Harjoitus3 komennot
| Komento                                                      | Kuvaus                                                                              |
| ------------------------------------------------------------ | ----------------------------------------------------------------------------------- |
| `git status`                                                 | Näyttää repositorion nykyisen tilan ennen muutoksia                                 |
| `echo "Lisätty teksti" >> index.html`                        | Lisää tekstiä olemassa olevaan index.html-tiedostoon                                |
| `echo "Uusi tiedosto" > uusi.txt`                            | Luo uuden tiedoston nimeltä uusi.txt                                                |
| `echo "Toinen tiedosto" > toinen.txt`                        | Luo toisen uuden tiedoston                                                          |
| `git status`                                                 | Näyttää tehdyt muutokset työtilassa                                                 |
| `git add .`                                                  | Lisää kaikki muutokset staging-alueelle seuraavaa talletusta varten                 |
| `git status`                                                 | Näyttää että muutokset ovat staging-alueella                                        |
| `git restore --staged uusi.txt`                              | Poistaa yksittäisen tiedoston staging-alueelta mutta säilyttää muutoksen työtilassa |
| `git status`                                                 | Tarkistaa staging-alueen tilanteen                                                  |
| `git restore --staged .`                                     | Poistaa kaikki loput tiedostot staging-alueelta                                     |
| `git status`                                                 | Näyttää että muutokset ovat työtilassa mutta eivät staging-alueella                 |
| `git restore index.html`                                     | Peruuta talletetun tiedoston muutokset työtilasta ja palauttaa viimeisimmän version |
| `git status`                                                 | Tarkistaa tilanteen muutoksen jälkeen                                               |
| `git restore .`                                              | Peruuta kaikki loput työtilaan tehdyt muutokset talletetuissa tiedostoissa          |
| `git status`                                                 | Näyttää jäljellä olevat muutokset (uudet tiedostot ovat edelleen untracked)         |
| `echo "Lisää sisältöä" >> index.html`                        | Tekee uuden muutoksen talletettuun tiedostoon                                       |
| `git add .`                                                  | Lisää kaikki muutokset staging-alueelle                                             |
| `git commit -m "Lisätty uusia muutoksia harjoitus 3 varten"` | Tallentaa muutokset versionhallintaan                                               |
| `git log`                                                    | Näyttää commit-historian ennen peruuttamista                                        |
| `git revert HEAD`                                            | Luo uuden commitin joka kumoaa viimeisimmän commitin muutokset                      |
| `git log`                                                    | Näyttää commit-historian jossa näkyy myös revert-commit                             |
| `git tag harjoitus3`                                         | Lisää viimeisimpään commit-talletukseen tunnisteen nimeltä harjoitus3               |

### Harjoitus4 komennot
| Komento                                                          | Kuvaus                                                                                      |
| ---------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| `git status`                                                     | Näyttää repositorion nykyisen tilan ennen muutoksia                                         |
| `nano index.html`                                                | Avaa index.html-tiedoston muokattavaksi HTML-perusrakenteen lisäämistä varten               |
| `git add index.html`                                             | Lisää muokatun index.html-tiedoston staging-alueelle                                        |
| `git commit -m "Lisätty HTML sivun perusrakenne"`                | Tallentaa HTML-rakenteen muutokset master-haaraan                                           |
| `git branch tyylit`                                              | Luo uuden ominaisuushaaran nimeltä tyylit                                                   |
| `git checkout tyylit`                                            | Vaihtaa aktiiviseksi haaraksi tyylit                                                        |
| `nano styles.css`                                                | Luo ja avaa styles.css-tiedoston, johon lisätään CSS-tyylit                                 |
| `nano index.html`                                                | Muokkaa index.html-tiedostoa ja lisää head-osioon CSS-linkitys                              |
| `git add styles.css index.html`                                  | Lisää CSS-tiedoston ja HTML-muutoksen staging-alueelle                                      |
| `git commit -m "Lisätty CSS tyylit ja linkitys HTML tiedostoon"` | Tallentaa tyylimuutokset tyylit-haaraan                                                     |
| `git checkout master`                                            | Vaihtaa takaisin päähaaraan master                                                          |
| `git checkout tyylit`                                            | Vaihtaa takaisin tyylit-haaraan tarkistaaksesi erot                                         |
| `git checkout master`                                            | Palaa jälleen master-haaraan ennen yhdistämistä                                             |
| `git merge --no-ff tyylit`                                       | Yhdistää tyylit-haaran master-haaraan ja säilyttää yhdistämisen näkyvänä commit-historiassa |
| `git log --oneline --graph`                                      | Näyttää commit-historian graafisesti haarojen yhdistämisen kanssa                           |
| `git tag harjoitus4`  | Lisää viimeisimpään commit-talletukseen tunnisteen nimeltä harjoitus4 |