# TEKNISK DOKUMENTATION - A Good Case - Gruppe 2 

## Kort om projektet

Dette projekt har vi lavet i forbindelse med Tema 9, hvor vu har re-designet hjemmesiden for agoodcase.dk ved at bruge hendholdsvis HTML, CSS og JavaScript. Indholdet til hjemmesiden bliver indhentet fra et rest API.

## Links:

- Netflify:
https://agoodcaseg2.netlify.app/

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
-  **Button.astro** – Komponent - HTML, CSS for buttons på produktliste siden
-  **Card.astro** - Komponent - HTML, CSS og JavaScript for cards på produktliste siden
-  **Footer.astro** - Komponent - HTML, CSS footer bruges på alle sider
-  **Header.astro** - Komponent - HTML, CSS og Javascript navigation som bruges på alle sider
-  **Hero.astro** - Komponent - HTML og CSS bruges på forsiden
-  **MitIdPopUp.astro** - Komponent - HTML, CSS og JavaScript for alders bekræftelses popup
-  **TopBaner.astro** - Komponent - HTML, CSS banner over navigationen som bruges på alle sider
-  **Layout.astro** - Layout - HTML og CSS her er vores fonte bl.a. indsat
-  **index.astro** - Forsiden
-  **list.astro** - Produktliste siden
-  **[slug].astro** - Produktside - HTML, CSS og Javascript. [slug] bruges i filnavnet til at lave dynamiske ruter i Astro. Det fungerer som en variabel i URL’en, så én side kan vise forskelligt indhold baseret på hvilken værdi der kommer fra URL’en. På den måde kan man bruge én komponent til alle produkter i stedet for at lave en side per produkt.

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

**Et objekt kan fx se sådan ud:** 

```
{data.id}
{data.image}
{data.brand}
{data.title}
{data.type}
{data.price}

```

### Felter vi bruger
```
- id
- title
- brand
- price
```

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

Vi har tænkt bæredygtighed ind i projektet ved bl.a. ikke at bruge videoer på siden. 
Derudover har vi også genbrugt koder og komprimeret billeder (vi har kun benyttet os af svg og webp filer)


## Mulige forbedringer

Hvis vi skulle arbejde videre med projektet, kunne vi forbedre det ved at tilføje:

- Error handling - 404 side



