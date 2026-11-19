# Astro Starter Kit: Minimal

```sh
npm create astro@latest
```

Vi bruger "npm create" som en genvejt til at køre en startpakke, der opretter vores projekt.

Vi skriver derefter @latest, for at fortælle npm, at den skal hente den nyeste udgivne version af create-astro i stedet for en ældre standardversion.

Vi bruger create-astro som et lille hjælpeprogram fra Astro, som kører i terminalen.

## 🚀 Project Structure

Inde i vores mappestruktur, ville i se følgende struktur:

├── public/
├── src/
│ └── assets/
└── Detailview-billeder/
└── footer-iconer/
└── forsiden-billeder/
│ └── componenter/
│ │ └── cards-udstyr
│ │ └── Footer
│ │ └── Header
│ │ └── Herodetailview
│ │ └── Kontaktdetail
│ │ └── Kontaktcard
│ │ └── Udstyrlist
│ └── Layout/
│ └── Pagelayout
│ └── pages/
│ └── udstyr/
│ │ └── singlepage.astro
│ └── index.astro
│ └── kontaktliste.astro
│ └── udstyrsliste.astro
│ └── styles/
│ └── global.css
│
└── package.json

Vores mappestruktur genereres fra create-astro, hvor guiden allerede indeholder filer og mapper på forhånd. Ud fra denne guide har vi udarbejdet vores egen mappestruktur.

Her var der blandt andet public og src (med pages indeni) i forvejen. Ud fra det oprettede vi selv vores assets-mappe til billeder, en layout-mappe til pagelayout samt en udstyr-mappe under pages til vores singlepage-sider, som vi skulle bruge til vores dynamiske site.

Astro fungerer på den måde, at den behandler og samler vores src-filer for at skabe det endelige site.

## 🚀 komponenter

Under vores opgave har vi benyttet ov af flere komponenter, til vires forskellige sider. Fordelen ved komponenter, er at de fungeere som en grundlæggende byggesten i et astro projekt.

I vores projekt, har vi både brugt komponenter som genanvendelige UI-elementer, både ved produktliste, kontakt siden og på vores header og footer.

Her har vi benyttet props til at sende data ind i vores komponent. Her har vi f.eks brugt prop til vise forskellige værdier som mails og telefonnumre:

```sh
const { mail, telefon} = Astro.props;

```

<p>{mail}</p>
<p>{telefon}</p>
```
Når vi sætter mail og telefon ind som props kan det samme komponet genbruges med forskellige kontaktoplysninger.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).

```

```
