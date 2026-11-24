# werkenbijunilever.nl

Statische satire-site, gehost op GitHub Pages. Geen build-stap: `index.html` + `assets/`.

## Live zetten
1. Maak een GitHub-repo (bijv. `werkenbijunilever`), push deze map naar `main`.
2. Repo > Settings > Pages > Source: `Deploy from a branch`, branch `main`, map `/ (root)`.
3. Vul bij Custom domain `werkenbijunilever.nl` in en vink "Enforce HTTPS" aan zodra dat kan.

## DNS bij Hostnet
Verwijder bestaande A/AAAA/CNAME-records voor `@` en `www` die naar de oude hosting wijzen, en zet:

| Naam | Type  | Waarde |
|------|-------|--------|
| @    | A     | 185.199.108.153 |
| @    | A     | 185.199.109.153 |
| @    | A     | 185.199.110.153 |
| @    | A     | 185.199.111.153 |
| www  | CNAME | `<jouw-github-gebruikersnaam>.github.io.` |

Controleer de IP-adressen nog even in de GitHub-docs, die kunnen wijzigen. Zeg het hostingpakket pas op als de site via GitHub live staat.
