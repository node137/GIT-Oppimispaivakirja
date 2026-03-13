# Oppimispäiväkirja: Hajautettu git

__Mikä osion tehtävissä oli vaikeaa ja mikä helppoa? Mikä auttoi minua oppimaan? Miten selvitin esteet, jotka vaikuttivat tehtävän suorittamiseen?__

Tämäkin osio oli suhteellisen helppo sillä työssäni ohjelmistokehittäjänä olen joutunut GITiä käyttämään aktiivisesti päivittäin tiimityöskentelyssä.

## Osiossa käyttämäni Git-komennot

### Harjoitus 5: Etärepositorio ja GitHub

| Komento | Kuvaus |
| ---------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| `git remote add origin https://github.com/node137/GitCourse26.git` | Liittää paikallisen repositorion GitHubissa luotuun tyhjään etärepositorioona nimellä origin |
| `git remote -v` | Näyttää listauksen määritetyistä etärepositorioista ja niiden osoitteista |
| `git push -u origin master` | Puskee paikallisen master-haaran GitHubiin ja asettaa seurannan |
| `git branch` | Näyttää pakaillisen gitin haarat (etärepossa vain master) |
| `git fetch` | Hakee tiedot etärepositorion muutoksista paikalliseen muistiin (ei muuta työtiedostoja) |
| `git checkout origin/master` | Siirtyy tarkastelemaan etärepositorion tilaa |
| `git checkout master` | Palaa takaisin paikalliseen master-haaraan |
| `git status` | Tarkistaa paikallisen haaran tilan suhteessa etärepositorioon |
| `git merge origin/master` | Yhdistää etärepositoriosta noudetut muutokset paikalliseen haaraan |
| `git tag harjoitus5` | Lisää tunnisteen harjoitus5 viimeisimpään talletukseen |
