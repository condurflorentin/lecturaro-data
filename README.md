# LecturăRO data

Acest folder conține setul de date remote pentru aplicație:

- `autori.xml`: autori, localizare pe hartă și opere reprezentative
- `scoruri.json`: scoruri de similaritate între opere canonice
- `opere.json`: catalog JSON cu operele canonice și metadatele lor

Linkuri raw de folosit după publicarea pe GitHub:

```text
https://raw.githubusercontent.com/USERNAME/lecturaro-data/main/autori.xml
https://raw.githubusercontent.com/USERNAME/lecturaro-data/main/scoruri.json
https://raw.githubusercontent.com/USERNAME/lecturaro-data/main/opere.json
```

Recomandare pentru proiect:

1. `autori.xml` sincronizează autorii și operele canonice în SQLite
2. `scoruri.json` aduce similaritățile pre-calculate între opere
3. textul adăugat de utilizator se leagă de un `autor` și de o `operă de referință`
4. pagina de similaritate afișează doar recomandări din interiorul aceluiași autor

Formatul nou din `scoruri.json` păstrează și `text1` / `text2` pentru compatibilitate, dar include și `opera1_id` / `opera2_id` pentru o integrare mai curată.
