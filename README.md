# Ghid de Utilizare GitHub Desktop pentru Jurnal de Drumeții

Acest proiect conține documentația completă și instrucțiunile pas cu pas pentru gestionarea repository-urilor de hărți și obținerea link-urilor directe (RAW) necesare pentru publicarea pe blogul **www.jurnaldedrumetii.ro**.

## 1. Crearea unui Repository Nou în GitHub Desktop
1. Deschideți aplicația **GitHub Desktop**.
2. Navigați în meniul superior la `File` -> `New repository...` (sau folosiți comanda rapidă `Ctrl + N` / `Cmd + N`).
3. Completați detaliile solicitate în fereastra pop-up:
   * **Name:** Introduceți numele proiectului (de exemplu: `proiect-harti`).
   * **Local Path:** Selectați directorul din calculator unde doriți salvarea fizică a fișierelor.
   * **Initialize this repository with a README:** Bifați obligatoriu această opțiune pentru a genera structura inițială.
4. Faceți click pe butonul **Create repository**.

## 2. Structurarea Folderelor și Adăugarea Hărților
Deoarece GitHub Desktop monitorizează exclusiv fișierele și nu folderele goale, structura trebuie creată prin managerul de fișiere nativ al sistemului de operare:
1. În GitHub Desktop, apăsați pe butonul **Show in Explorer** (Windows) sau **Show in Finder** (macOS).
2. În fereastra deschisă, creați un folder nou numit `harti` (Click dreapta -> `New Folder`).
3. Adăugați fișierele cu trasee sau hărți în acest folder (formate acceptate: `.gpx`, `.kml`, `.geojson`, `.png` etc.).

> ⚠️ **Notă importantă:** Dacă un folder este complet gol, Git îl va ignora. Pentru a păstra un folder gol în structură până la adăugarea hărților propriu-zise, creați în interiorul lui un fișier gol numit `.gitkeep`.

## 3. Salvarea Modificărilor (Commit) și Sincronizarea Online
1. Reveniți în aplicația **GitHub Desktop**. Modificările vor apărea automat în panoul din stânga, la secțiunea **Changes**.
2. În colțul din stânga jos, completați câmpul **Summary** (titlul modificării), de exemplu: `Adaugat folderul pentru harti`.
3. Faceți click pe butonul albastru **Commit to main** (sau `Commit to master`).
4. Pentru a trimite fișierele pe serverul GitHub, apăsați butonul **Publish repository** (la prima publicare) sau **Push origin** (pentru actualizări ulterioare) amplasat în bara superioară.

## 4. Obținerea Link-ului RAW pentru Blog
Pentru a integra track-urile sau hărțile direct în articolele de pe blog, aveți nevoie de link-ul de tip RAW:
1. În GitHub Desktop, accesați meniul `Repository` -> `View on GitHub` (Scurtătură: `Ctrl + Shift + G` / `Cmd + Shift + G`).
2. În interfața web deschisă în browser, navigați în folderul `harti` și dați click pe fișierul dorit.
3. În colțul din dreapta-sus al ferestrei cu conținutul fișierului, apăsați pe butonul **Raw**.
4. Copiați adresa URL completă din bara de navigare a browserului. Un URL corect va începe întotdeauna cu structura: `https://raw.githubusercontent.com/...`

## 5. Integrarea în Blog (Cod HTML Recomandat)
Link-ul RAW obținut poate fi folosit direct în platforma de blogging pentru descărcare sau vizualizare:

**Buton de descărcare directă pentru vizitatori:**
```html
<a href="URL_RAW_COPIAT" download>Descarcă traseul GPX</a>
