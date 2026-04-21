# TEKNISK DOKUMENTATION - A Good Case - Gruppe 2 

## Kort om projektet

Dette projekt har vi lavet i forbindelse med Tema 9, hvor vu har re-designet hjemmesiden for agoodcase.dk ved at bruge hendholdsvis HTML, CSS og JavaScript. Indholdet til hjemmesiden bliver indhentet fra et rest API.

## Links:

- GitHub Pages: 


- Projektets GitHub Repository:
https://github.com/fashionrus-yoli/aYOLIcase

- Figma:
https://www.figma.com/design/csvTzxcR9ihXPYrqEEkjTB/A-good-case?node-id=1-4&t=PFL2ipvhfhropnof-1

- Trello Board:
https://trello.com/b/cwn4ZZxz/a-good-case


## Gruppemedlemmer:
- Luna Victoria Bungkird Christiansen - luch0005@stud.ek.dk
- Ophélie Breit Zoungrana Bedsted - opbe0001@stud.ek.dk
- Ida Dam - Idda0001@stud.ek.dk
- Yvonne Yuna Quach - yvqu0001@stud.ek.dk

# Projektstruktur
```
AYOLICASE/
├── .astro/..
├── .vscode/..
├── node_modules/..
├── public/
│   ├── css/
|   |    └── variabler.css
|   └── favicon.ico
|   └── favicon.svg
├── src/
│   ├── assets/
|   |    └── alderpopup.svg
|   |    └── Arrow.svg
|   |    └── ArrowBig.svg
|   |    └── astro.svg
|   |    └── background.svg
|   |    └── bag.svg
|   |    └── flasker-hero.webp
|   |    └── humle.webp
|   |    └── logo_gold.svg
|   |    └── logo.svg
|   |    └── MitID_blue.svg
|   |    └── MitID_white.svg
|   |    └── mitidbaggrund.svg
|   |    └── profile.svg
|   |    └── search.svg
|   |    └── Star.svg
│   ├── components/
|   |    └── AlderPopup.astro
|   |    └── Button.astro
|   |    └── Card.astro
|   |    └── Fotter.astro
|   |    └── Header.astro
|   |    └── Hero.astro
|   |    └── MitIdPopUp.astro
|   |    └── TopBanner.astro
│   ├── layouts/
|   |    └── Layou.astro
│   ├── pages/
|   |    └── products/
|   |    |    └── [slug].astro
|   |    └── index.astro
|   |    └── list.astro
|   |    └── product.astro
├── astro.config.mjs
├── package-lock.json
├──package.json
├── README.md
└── tsconfig.json
```

## Filbeskrivelser SKAL LAVES
-  **AlderpPopup.astro** – Komponent - HTML, CSS og JavaScript for MitID bekræftelses popup
-  **Button.astro** – 
-  **Card.astro** -
-  **Footer.astro** -
-  **Header.astro** -
-  **Hero.astro** -
-  **MitIdPopUp.astro** - Komponent - HTML, CSS og JavaScript for alders bekræftelses popup
-  **TopBaner.astro** -
-  **Layout.astro** -
-  **[slug].astro** -
-  **index.astro** - Forsiden
-  **list.astro** - Produkt liste siden
-  **product.astro** - Produkt side

## Hvordan koden fungerer SKAL LAVES


**Flow:**



## Navngivning 

Vi har navngivet vores filer, variabler og funktioner for at det lettest muligt giver mening ift. hvad koden gør.

### Eksempler på variabler 

```
const {
  delay = 2000,
  title = "Bekræft din alder",
  subtitle = "*Bekræftes igen med MitID inden checkout",
  message = "Er du 18 eller ældre?",
  followupTitle = "",
  followupMessage = "Du kan desværre ikke fortsætte. Genindlæs siden, hvis du vil starte forfra.",
} = Astro.props;
```

### Eksempler på funktioner 

```
function openPopup() {
    overlay?.removeAttribute("hidden");
    document.body.classList.add("popup-open");
  }
```
Vi har brugt camelCase i JavaScript, fordi det gør koden mere ensartet og lettere at læse.

## Data og JSON-struktur

Vi henter data fra et API i JSON-format.

**Et objekt kan fx se sådan ud:** SKAL LAVES

```json

```

### Felter vi bruger SKAL LAVES


### HTML-Validering: SKAL LAVES
- `type="text"` -validerer tekst input
- `required` -feltet skal udfyldes
- `<textarea>` -tekstfeldt til længere tekst

# Git og branches 
Vi har brugt GitHub til at kode denne hjemmeside sammen. 
Vi har dertil arbjedet med branches så vi kunne være flere om at kode på samme tid. 

### Eksempler på branches 
- header-fix
- ophe-retter-hero
- card_and_button_mobile

### Workflow

1. Lave en branch med et navn der stemmer overens med den opgave man er gået igang med
2. Kode et feature
3. Committe ændringer
4. Pushe til GitHub
5. Merge til main når det virker

## Bæredygtighed SKAL LAVES

Vi har tænkt bæredygtighed ind i projektet ved at holde page weight under 250 kb samt en enkel informationasarkitektur.

**Tiltag:** SKAL LAVES

- Ingen videoer
- Genbruge af kode
- Optimerede billeder: svg + webp

## Udfordringer undervejs SKAL LAVES
Der har selvfølgelig været småfejl undervejs eksempelvis som.....


**Løsninger:** SKAL LAVES

- .....


## Mulige forbedringer SKAL LAVES

Hvis vi skulle arbejde videre med projektet, kunne vi forbedre det ved at tilføje:

- At få søgefunktion til at virke, lige nu er det bare implementeret på sitet af æstetiske årsager
- Error handling - 404 side



