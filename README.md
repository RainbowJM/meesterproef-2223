# Duurzaam, groen en sociaal Strandeiland <!-- omit in toc -->

[Team repo](https://github.com/RainbowJM/strandeiland) <!-- omit in toc -->
---
# Table of contents <!-- omit in toc -->
  
- [Introduction](#introduction)
- [Duurzaam, groen en sociaal Strandeiland](#duurzaam-groen-en-sociaal-strandeiland)
  - [User stories](#user-stories)
  - [Briefing](#briefing)
  - [The debriefing](#the-debriefing)
- [Week 1](#week-1)
  - [Brainstorm](#brainstorm)
  - [Design](#design)
  - [API](#api)
  - [Chat](#chat)
- [Week 2](#week-2)
  - [API](#api-1)
  - [Chat](#chat-1)
- [Week 3](#week-3)
  - [API](#api-2)
  - [Chat](#chat-2)
  - [Service worker](#service-worker)
  - [Design](#design-1)
- [Week 4](#week-4)
  - [Modules](#modules)
  - [Database](#database)
  - [User detail page](#user-detail-page)
  - [Code refactor](#code-refactor)
- [Week 5](#week-5)
  - [Fetching data](#fetching-data)
  - [Code refactor](#code-refactor-1)
  - [Testing](#testing)
  - [LightHouse testing](#lighthouse-testing)
- [Feedback](#feedback)
  - [Feedback week 1](#feedback-week-1)
    - [Feedback design review - 31 mei 2023](#feedback-design-review---31-mei-2023)
    - [Feedback debriefing - 1 juni 2023](#feedback-debriefing---1-juni-2023)
    - [Feedback Sprint review - 2 juni 2023](#feedback-sprint-review---2-juni-2023)
    - [Retrospetive](#retrospetive)
  - [Feedback week 2](#feedback-week-2)
    - [Feedback Code Review - 7 juni 2023](#feedback-code-review---7-juni-2023)
    - [Feedback Sprint Review - 9 juni 2023](#feedback-sprint-review---9-juni-2023)
    - [Retrospetive](#retrospetive-1)
  - [Feedback Week 3](#feedback-week-3)
    - [Feedback Code Review - 14 juni 2023](#feedback-code-review---14-juni-2023)
    - [Feedback Sprint Review - 15 juni 2023](#feedback-sprint-review---15-juni-2023)
    - [Feedback Design Review - 15 juni 2023](#feedback-design-review---15-juni-2023)
    - [Retrospetive](#retrospetive-2)
  - [Feedback Week 4](#feedback-week-4)
    - [Feedback Code Review - 21 juni 2023](#feedback-code-review---21-juni-2023)
    - [Feedback Design Review - 22 juni 2023](#feedback-design-review---22-juni-2023)
    - [Feedback Sprint Review - 23 juni 2023](#feedback-sprint-review---23-juni-2023)
    - [Retrospetive](#retrospetive-3)
- [General retrospective](#general-retrospective)
- [Course Applied](#course-applied)
  - [CSS to the Rescue](#css-to-the-rescue)
  - [Web App From Scratch](#web-app-from-scratch)
  - [Browser Technologies](#browser-technologies)
  - [Progressive Web Apps](#progressive-web-apps)
  - [Human Centred Design](#human-centred-design)
  - [Real Time Web](#real-time-web)
- [Sources](#sources)

---
## Introduction
The Meesterproef is the final client-project of the half year minor programme about Web Design and Development in Amsterdam. 
Bachelor Communication and Multimedia Design, Amsterdam University of Applied Science.

In the coming years, a completely new neighborhood will be created on the east side of Amsterdam: Strandeiland. 
Ambitions are high: the neighborhood must be energy-generating, greener than the first version of IJburg, residents must be able to live pleasantly with each other and equality of opportunity must be improved.

## Duurzaam, groen en sociaal Strandeiland
The Participatieteam wants to add a new functionality for the `hallostrandeiland.nl` website where people can submit new proposals for the new Strandeiland neighborhood. 
This will promote communication between future residents of Strandeiland and the project managers of the municipality of Amsterdam. 
The goal is to use Hallo Strandeiland to collect good ideas and proposals, improve them and get the beautiful and feasible ones realized.

### User stories
The user stories are written in Dutch. The user stories are written in the following format: 
- Als toekomstig bewoner, wil ik mijn voorstel voor een duurzamer, groener en socialer strandeiland kunnen delen, zodat dit onderzocht en hopelijk gerealiseerd kan worden.

- Als toekomstig bewoner, wil ik een reactie kunnen geven op voorstellen van andere toekomstige bewoners, zodat we kunnen samenwerken aan het vormgeven van de voorstellen.

- Als projectmanager van de gemeente, wil ik voorstellen van toekomstige bewoners kunnen filteren op thema's, zodat ik per thema kan bekijken of er ideeën bijzitten die kunnen bijdragen aan een lagere ecologische footprint, of betere sociale cohesie van de wijk.

### Briefing
The briefing is the first meeting we had as group with Michel Vogler from CrossmarX. Before the briefing we made a mind map with all the information we already had about the project. You can find this mind map below.

<img width="832" alt="Screenshot 2023-06-18 at 13 32 31" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/a8841440-5b8c-4e7b-9946-147c5e334fa5">

Below are the questions we asked Michel Vogler:
- Wat wil de opdrachtgever met deze opdracht?
- Eigen repo op github of repo van het bedrijf zelf? (vanuit school moet github)
- Prototype start from scratch?
- Wat is de doelstelling?
- Wat zijn de randvoorwaarden?
- Heeft het project relatie met een andere project?
- Voor desktop alleen? of desktop en mobile?
- Hosten jullie het zelf?
- Is er al een design? Is er een huisstijl? Is de huisstijl van de hello strandeiland?
- Moet het een progressive web app worden? (zodat de app downloadbaar is)
- Hoe moeten de voorstellen eruit komen te zien? Moet het een soort document worden of tekst met eventueel een afbeelding?
- Hoe ziet u het onderdeel van de projectmanager voor zich? Bewoners en projectmanager een account of alleen projectmanager een account.
- Zijn er specifieke thema’s, zoals lagere ecologische footprint en betere sociale cohesie van de wijk of moeten gebruikers deze zelf aan kunnen maken bij het voorstel?
- Wanneer er meerdere voorstellen zijn geüpload, wilt u deze dan op een pagina zien waar u kunt filteren of onder verschillende tabbladen wilt met de verschillende thema’s?
- In hoeverre verschilt dit project met hallostrandeiland.nl, aangezien je daar ook berichten hebt waar je een reactie bij kan plaatsen?
- Hebben jullie het logo en beeldmateriaal, zodat wij dit kunnen gebruiken?

### The debriefing
After the briefing we made a debriefing. We wrote down all the information we got from the briefing. 
We also wrote down the questions we still had. You can find the debriefing below.

[Debriefing](https://github.com/RainbowJM/strandeiland/wiki/Debriefing)

## Week 1
The kick-off presentation of the final project for this minor was given by the teachers. 
We were given detailed information about the planned schedule for the next five weeks. 
We had briefing with the product owner. 
After that we made a briefing with the product owner and we started working on a the first iteration of our prototype. 

### Brainstorm
We started with a brainstorm to get a better understanding of the project. 
Based on that we made a MoSCoW list.

<img width="833" alt="Screenshot 2023-06-18 at 13 34 55" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/97f33ad1-a6fb-457c-8f26-df40aaae0f0d">

### Design
For this week we wanted a first version of the overview page, detail page make a wish form. 
So we started where everyone designed their idea's of options of how the page should look like.

<img width="435" alt="Screenshot 2023-06-25 at 22 36 59" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/bfec2e36-d0d3-4446-9a0f-8d0839b6f4a8">

<img width="471" alt="Screenshot 2023-06-25 at 22 37 09" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/51c3276c-0d4c-4bd6-9cde-417ec896cfba">

<img width="421" alt="Screenshot 2023-06-25 at 22 36 46" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/23dfe4f3-a8ec-4290-aac9-cb9b329b1d58">

After that we brainstormed together to create a first version of the design by putting all the idea's together.

The overview page:

<img width="365" alt="Screenshot 2023-06-16 at 16 16 42" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/36b594a5-6d57-41d2-8a71-cd0fb8300ad8">

The detail page:

<img width="441" alt="Screenshot 2023-06-18 at 18 23 09" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/440d7fd7-11ba-4c6b-9294-d181be533f02">

The make a wish form:

<img width="308" alt="Screenshot 2023-06-16 at 16 19 28" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/185fc2b7-8038-48d5-84cc-ac759047b978">

### API
In the project description it was mentioned that we had to use an API. 
That I will be provided by the school self. 
But after a meeting that we had with the teacher that was responsible for the API, I got that assignment to make the API. 
The API will be used by both teams.

I made the API in supabase. The step by step guide can be found in the blog that I wrote. [Supabase](https://medium.com/@jevona.magdalena/unleashing-the-power-of-supabase-your-ultimate-guide-to-modern-database-development-with-express-872dbb3b6e)

The process of naming everything took a while, because I wanted to make sure that everything was clear.
So that everyone could understand what the API was doing. 
And how it has to be used.

<img width="876" alt="Screenshot 2023-06-18 at 18 28 02" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/8f7cbef5-ee3f-4324-9fd5-571c40912b74">

<img width="514" alt="Screenshot 2023-06-18 at 18 28 27" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/68be055a-c4d5-43fc-b035-bf1282a0a7ae">

![image](https://github.com/RainbowJM/meesterproef-2223/assets/59873140/d290fc2e-a601-4a66-b3e7-417aa78563b9)

The second version was the version that I went for in the end.

One thing about the API that I was not sure about was the authentication.
So at the code review section I asked Justus(one if the teachers) about it.
He told me that there is different ways to do it. 
But in this minor we don't have to do it. the focus is not on security.
So I decided to leave the security part out of the API.

### Chat
The chat is a part of the project that we saw as a innotive part of the project.

So for the first sprint we wanted to show the product owner what a real-time chat would look like.

Here is some code:
```javascript
const express = require("express");
const app = express();
const http = require("http").createServer(app);
const path = require("path");
const io = require("socket.io")(http);
const port = process.env.PORT || 6954;
const bodyParser = require("body-parser");
const historySize = 100;
let history = [];

app.set("view engine", "ejs");
app.set("views", "./views");

app.use(express.static(path.resolve("public")));
app.use(bodyParser.urlencoded({ extended: true }));
app.use(bodyParser.json());

app.get("/chat", (req, res) => {
  res.render("chat", {
    title: "Chat",
  });
});


io.on("connection", (socket) => {
  console.log("user connected");

  socket.emit("history", history);

  socket.on("message", (message) => {
    // Add the message to the history.
    while (history.length > historySize) {
      // Remove the oldest message.
      history.shift();
    }
    // Add the message to the history.
    history.push(message);

    // Emit the message to all connected users.
    io.emit("message", {
      message: message.message,
      id: socket.id,
      time: message.time,
    });
  });

  socket.on("disconnect", () => {
    console.log(`user ${socket.id} disconnected`);
  });
});

http.listen(port, () => {
  console.log(`Example app listening on  http://localhost:${port}`);
});
```
```javascript
// ------------------ variables -------------------------------------------------------
const socket = io();
const messages = document.querySelector("section ul");
const submitMessage = document.querySelector("#message-button");
const input = document.querySelector("#message-input");
const filterMenu = document.querySelector(".filter-menu");
const themeFilterBtn = document.querySelector(".thema-btn");
const themeSelect = document.getElementById("thema");
const theMenuButton = document.querySelector(".menuButton");
const theNav = document.querySelector(".navigation-links");
const theImage = document.querySelector(".menuContainer img");
const asideItems = document.querySelectorAll(".helping-item");
const tabs = document.querySelectorAll("[data-filter-target]");
const tabContents = document.querySelectorAll("[data-filter-content]");
const filterThemeBtn = document.querySelector(".filter-theme-btn");
const filterSortBtn = document.querySelector(".filter-sort-btn");
const closeFilterBtn = document.querySelector(".close-filter");
let last;


// ------------------ logic -------------------------------------------------------

if (submitMessage) {
  submitMessage.addEventListener("click", (event) => {
    event.preventDefault();

    // Get the current time.
    const hour = new Date().toLocaleTimeString("nl-NL", {
      hour: "2-digit",
      minute: "2-digit",
    });

    if (input.value) {
      // Emit the message to all connected users.
      socket.emit("message", {
        message: input.value,
        // name: nameTitle.textContent,
        time: hour,
      });

      // Add the message to the chat.
      add(input.value, hour, socket.id, true);

      input.value = "";
    }
  });
}

// ------------------ sockets -------------------------------------------------------

socket.on("message", (message) => {
  if (message.id != socket.id) {
    add(message.message, message.time, message.id);
  }
});

socket.on("history", (history) => {
  history.forEach((message) => {
    add(message.message, message.time, message.id);
  });
});

// ------------------ functions -------------------------------------------------------
function add(message, time, id, self) {
  let styling = "";

  // Add styling to the message if you are the sender.
  if (self) {
    styling = "self";
  } else {
    if (last == id) {
      styling = "multiple";
    }
  }

  messages.appendChild(
    Object.assign(document.createElement("li"), {
      className: styling,
      innerHTML: `<section id='message'>
    <span class="message">${message}</span>
    <span class="time">${time}</span> 
    </section>`,
    })
  );
  // Scroll to the bottom of the chat.
  messages.scrollTop = messages.scrollHeight;
  last = id;
}
```

## Week 2
### API
This week I finished the API.
I made the tables and tested if the API worked with Postman.

<img width="809" alt="Screenshot 2023-06-18 at 18 26 45" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/3839d93d-1276-47bf-b8b9-7c007738b420">

So it was ready to be used in code. 
That was again a new challenge for me. Cuz it it was to diffent teams which had two diffent ways of working.
And when they had issues with implementing the API I had to help them.
But this for sure was a good learning moment for me.
I got to knwo better was of working with the API, new functionalities that I didn't know about.
I explored more with supabase.

Also I started to add dummy data to the API.
I started with the themes.
For this one we had a section where both teams came together to discuss the themes that we wanted to add.

We came up with the following themes:

<img width="415" alt="Screenshot 2023-06-18 at 22 38 41" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/8830d2c6-e177-49c9-88f2-fc4087ad7040">

<img width="372" alt="Screenshot 2023-06-14 at 18 45 51" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/a19ac15a-74aa-4e15-b330-5873c8a7e635">

### Chat
The for design of the chat was that you can pin messgae in the chat and they will appear on the right side.

<img width="1345" alt="Screenshot 2023-06-09 at 13 28 38" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/49308006-3df8-46c4-9cd3-dfa290a12728">

So I started with the implemtation of the chat, with the correct design and functionality.
Sadly for this sprint couldn't finish the part of the pinning of the messages.
But on the bring side, after the review the product owner changed his mind and didn't want the pinning of the messages anymore.
So that was not so bad that I didn't finish it.
But for the following sprint we had to redesign the whole chat aspect of the project.

## Week 3
### API
The API was done but it was empty, it didnt had any data.
At the code review we got feedback that we should add dummy data to the API.
To start implementing teh fetch of the data in to our project.

When I was adding dummy dat ato the database I realised that I had to change the structure of the database.
So that is when I created teh new datamodel and implemented it in to the API.

![meesterproef (1)](https://github.com/RainbowJM/meesterproef-2223/assets/59873140/16c42c4e-5f92-4936-b395-f86dd3226835)

<img width="453" alt="Screenshot 2023-06-22 at 21 41 01" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/f1a44fb4-67f9-46aa-a57f-78fac04a95e4">

<img width="296" alt="Screenshot 2023-06-20 at 22 19 55" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/c59693c6-5a7e-4044-ae1c-928002df0b82">

So now de project has actual data to work with.

<img width="1280" alt="Screenshot 2023-06-21 at 18 26 33" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/9d61a1bb-8abf-4132-9b27-4ccb09985305">

### Chat
For this sprint we had to redesign the chat. 
We decided to go with reacties inset of chat, but still in real-time.

<img width="1352" alt="Screenshot 2023-06-18 at 23 23 53" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/3d9f9518-5ec3-47a2-a246-98b2068dd6a8">

```js
require('dotenv').config()
const express = require("express");
const app = express();
const http = require("http").createServer(app);
const path = require("path");
const io = require("socket.io")(http);
const port = process.env.PORT || 6954;
const bodyParser = require("body-parser");
const { createClient } = require('@supabase/supabase-js');
const supabase = createClient(
    'https://yyufywjwwwmgfjmenluv.supabase.co',
    `${process.env.SUPABASE_KEY}`);
const historySize = 100;
let history = [];

app.set("view engine", "ejs");
app.set("views", "./views");

app.use(express.static(path.resolve("public")));
app.use(bodyParser.urlencoded({ extended: true }));
app.use(bodyParser.json());

app.get('/detailPage-1', (req, res) => {
    res.render('detailPage-1',{
    title: "Detail",
  });
});

io.on("connection", (socket) => {
  console.log("user connected");

  socket.emit("history", history);

  socket.on("message", (message) => {
    // Add the message to the history.
    while (history.length > historySize) {
      // Remove the oldest message.
      history.shift();
    }
    // Add the message to the history.
    history.push(message);

    // Emit the message to all connected users.
    io.emit("message", {
      message: message.message,
      name: message.name,
      id: socket.id,
      time: message.time,
    });
  });

  socket.on("disconnect", () => {
    console.log(`user ${socket.id} disconnected`);
  });
});

http.listen(port, () => {
  console.log(`Example app listening on  http://localhost:${port}`);
});
```
```js
// ------------------ variables -------------------------------------------------------
import {
  messages,
  submitMessage,
  input,
  tabs,
  filterMenu,
  themeFilterBtn,
  themeSelect,
  asideItems,
  theMenuButton,
} from "./modules/variables.js";
import { toggleFilterMenu } from "./modules/filter.js";
import { toggleMenu } from "./modules/navigationMenu.js";

const socket = io();
let last;


// ------------------ logic -------------------------------------------------------
if (submitMessage) {
  submitMessage.addEventListener("click", (event) => {
    event.preventDefault();

    // Get the current time.
    const date = new Date().toLocaleString("nl-NL", {
      weekday: "short",
      day: "numeric",
      month: "short",
      year: "numeric",
      hour: "2-digit",
      minute: "2-digit",
    });

    if (input.value) {
      // Emit the message to all connected users.
      socket.emit("message", {
        message: input.value,
        // name has to be fetch from database
        name: "Jane Doe",
        time: date,
      });

      // Add the message to the chat.
      add(input.value, 'Jane Doe', date, socket.id);

      input.value = "";
    }
  });
}
// ------------------ sockets -------------------------------------------------------

socket.on("message", (message) => {
  if (message.id != socket.id) {
    add(message.message, message.name, message.time, message.id);
  }
});

socket.on("history", (history) => {
  history.forEach((message) => {
    add(message.message, message.name, message.time, message.id);
  });
});

// ------------------ functions -------------------------------------------------------
function add(message, name, time, id) {
  messages.appendChild(
    Object.assign(document.createElement("li"), {
      innerHTML: `<section id='message'>
      <img src="/images/bob.jpeg" alt="avatar" class="avatar">
      <div class="message-name-time">
      <p class="name">${name}</p> 
      <span class="message">${message}</span>
      <span class="time">${time}</span> 
      </div>
      </section>`,
    })
  );
  // Scroll to the bottom of the chat.
  messages.scrollTop = messages.scrollHeight;
  last = id;
}
```
```css
#chat {
  height: 20em;
  position: relative;
  background-color: var(--white);
  display: flex;
  flex-direction: column;
  grid-column-start: 1;
}

#chat h2{
text-align: center;
}

.chat-section {
  overflow-y: scroll;
  height: 67%;
}

form {
  position: absolute;
  bottom: 0;
  width: 100%;
  margin: 0 1em 0.5em 1em;
}

form input[type="text"] {
  font-family: Poppins, system-ui;
  background: var(--light-grey);
  border: none;
  border-radius: 25px;
  width: 90%;
  padding: 15px 20px;
}

form button {
  height: 50px;
  width: 50px;
  background: var(--blue);
  border: none;
  /* border: solid 2px var(--yellow); */
  border-radius: 50%;
  justify-content: center;
  align-items: center;
  cursor: pointer;
}

#chat li {
  font-size: small;
  display: flex;
  flex-direction: column;
  margin-top: 8px;
  margin-bottom: 8px;
}

#chat li #name {
  font-weight: bold;
  margin-top: 0;
  margin-bottom: 8px;
  background-color: var(--yellow);
  display: none;
}

#chat li #message {
  background: var(--light-grey);
  border-radius: 25px;
  width: 97%;
  padding: 10px 25px;
  height: 5em;
  font-size: medium;
  word-wrap: break-word;
  margin: 0 10px 0 10px;
  display: flex;
}

div.message-name-time{
  display: flex;
  flex-direction: column;
}

#chat li #message span::first-letter {
  text-transform: uppercase;
}

#chat li.self #message {
  background: var(--light-grey);
  border-radius: 25px;
  margin-left: auto;
  /* border: 1.5px solid var(--yellow); */
  margin: 0 10px 0 10px;
}

#chat li #message p {
  word-break: break-word;
  display: inline;
  margin: 0;
  text-align: start;
  font-weight: bold;
  font-size: medium;
  background-color: var(--yellow);
  width: fit-content;
  padding: 0.05em;
}

#chat li #message .time {
  font-size: smaller;
  float: right;
  color: grey;
  font-style: italic;
}

#chat li.self #message .time {
  color: grey;

}

img.avatar{
  height: 4em;
  width: 4em;
  border-radius: 5em;
  margin-right: 0.5em;
}
```
### Service worker
Started with adding the manifest.json and service worker.
And also you can download the app to your homescreen.

```json
{
    "theme_color": "#009ce0",
    "background_color": "#f0f0eb",
    "display": "standalone",
    "scope": "/",
    "start_url": "/",
    "manifest_version": 1,
    "orientation": "portrait",
    "name": "Strandeiland",
    "short_name": "Strandeiland",
    "icons": [
        {
            "src": "/images/icon-192x192.png",
            "sizes": "192x192",
            "type": "image/png"
        },
        {
            "src": "/images/icon-256x256.png",
            "sizes": "256x256",
            "type": "image/png"
        },
        {
            "src": "/images/icon-384x384.png",
            "sizes": "384x384",
            "type": "image/png"
        },
        {
            "src": "/images/icon-512x512.png",
            "sizes": "512x512",
            "type": "image/png"
        }
    ]
}
```
```js
const cacheName = 'cache-v1';
const runtimeCacheName = 'runtime-cache'
const assets = [
    '/',
    '/css/style.css',
    '/css/detail-page.css',
    '/css/form.css',
    '/css/global.css',
    '/css/overview-page.css',
    '/css/sent.css',
    '/css/offline.css',
    '/images/favicon.ico',
    '/offline',
];


self.addEventListener('install', event => {
    console.log('Installed service worker');

    event.waitUntil(
        caches.open(cacheName)
            .then(cache => {
                cache.addAll(assets)
                    .then(() => self.skipWaiting());
            })
    );
});

self.addEventListener('activate', event => {
    console.log('Activating service worker')
    event.waitUntil(
        caches.keys()
            .then(names => {
                return Promise.all(names
                    .filter(name => name !== cacheName && name !== runtimeCacheName)
                    .map(key => caches.delete(key)))
            })
    )
});

self.addEventListener('fetch', event => {
    console.log('Fetch event: ', event.request.url);
    if (isCoreGetRequest(event.request)) {
        event.respondWith(
            caches.open(cacheName)
                .then(cache => cache.match(event.request.url))
        );
    } else if (isHtmlGetRequest(event.request)) {
        event.respondWith(
            caches.open(runtimeCacheName)
                .then(cache => cache.match(event.request.url))
                .then(response => response ? response : fetchAndCache(event.request, runtimeCacheName))
                .catch(e => {
                    return caches.open(cacheName)
                        .then(cache => cache.match('/offline'))
                })
        );
    }
});

function isCoreGetRequest(request) {
    return request.method === 'GET' && assets.includes(getPathName(request.url));
}

function isHtmlGetRequest(request) {
    return request.method === 'GET' && 
    (request.headers.get('accept') !== null && request.headers.get('accept').indexOf('text/html') > -1);
}

function fetchAndCache(request, cacheName) {
    return fetch(request)
        .then(response => {
            if (!response.ok) {
                throw new TypeError('Bad response status');
            }
            const clone = response.clone();
            caches.open(cacheName).then((cache) => cache.put(request, clone));
            limitCacheSize(cacheName,5);
            return response;
        })
}

function getPathName(requestUrl) {
    const url = new URL(requestUrl);
    return url.pathname;
}
```

### Design
A few sprint back we got the feedback to add a page where you can see the details of the user.

This sprint I made a mini design for it.

<img width="622" alt="Screenshot 2023-06-25 at 22 52 59" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/80445970-b9b7-44f9-88c2-ff4e5701a452">

Based on the feedback we got about the color palette, we adde more colors to use in our design.

<img width="131" alt="Screenshot 2023-06-25 at 22 53 10" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/370a5016-036b-4561-a830-eaf92dac9699">

We tested the colors with the accessibility testing tool, before we made the final decision.

<img width="480" alt="Screenshot 2023-06-25 at 22 54 06" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/e00b4ccb-8e99-4e06-b01d-d29bf82b1121">

## Week 4
### Modules
In the code reviews a got the feedback from Joost to refactor `app.js` and `server.js` into modules.
And I did that with `app.js` by using  `express router`

```js
require("dotenv").config();
const express = require("express");
const app = express();
const { createClient } = require("@supabase/supabase-js");
const supabase = createClient(
  `${process.env.SUPABASE_URL}`,
  `${process.env.SUPABASE_KEY}`
);
const _ = require("lodash");
const router = express.Router();

router.get("/", async (req, res) => {
  const { data: themeData, themeError } = await supabase.from("theme").select();
  const { data: themeSuggestions, themeSuggestionsError } = await supabase
    .from("suggestion_theme")
    .select();
  const { data: suggestionsData, error: suggestionsError } = await supabase
    .from("suggestion")
    .select();
  const { data: latestSuggestionsData, latestSuggestionsError } = await supabase
    .from("suggestion")
    .select()
    .order("created_at", { ascending: false })
    .limit(3);
  const { count, error } = await supabase
    .from("suggestion")
    .select("*", { count: "exact", head: true });
  const { data: residentSuggestionData, residentSuggestionError } =
    await supabase.from("resident_suggestion").select();
  const { data: residentData, residentError } = await supabase
    .from("resident")
    .select();

  // Randomize the suggestionsData array
  const shuffledSuggestionsData = _.shuffle(suggestionsData);

  for (const suggestion of shuffledSuggestionsData) {
    const relatedTheme = themeSuggestions.find(
      (ts) => ts.suggestionId === suggestion.id
    );

    if (relatedTheme) {
      const theme = themeData.find((t) => t.id === relatedTheme.themaId);

      if (theme) {
        suggestion.theme = theme;
      }
    }
  }

  for (const latestSuggestion of latestSuggestionsData) {
    const latestRelatedTheme = themeSuggestions.find(
      (ts) => ts.suggestionId === latestSuggestion.id
    );

    if (latestRelatedTheme) {
      const theme = themeData.find((t) => t.id === latestRelatedTheme.themaId);

      if (theme) {
        latestSuggestion.theme = theme;
      }
    }
  }

  for (const latestSuggestion of latestSuggestionsData) {
    for (const residentSuggestion of residentSuggestionData) {
      if (latestSuggestion.id === residentSuggestion.suggestion_id) {
        for (const resident of residentData) {
          if (resident.id === residentSuggestion.resident_id) {
            latestSuggestion.amb = resident;
          }
        }
      }
    }
  }

  if (
    themeError ||
    suggestionsError ||
    latestSuggestionsError ||
    themeSuggestionsError
  ) {
    console.error(
      "Error:",
      themeError ||
        suggestionsError ||
        latestSuggestionsError ||
        themeSuggestionsError
    );
  } else {
    res.render("index", {
      title: "Wensen",
      themes: themeData,
      suggestions: shuffledSuggestionsData,
      latestSuggestions: latestSuggestionsData,
      totalSuggestions: count,
    });
  }
});

router.get("/wens/:id", async (req, res) => {
  const suggestionId = req.params.id;
  const { data: suggestionData, error } = await supabase
    .from("suggestion")
    .select()
    .eq("id", suggestionId)
    .single();

  let defaultTime = suggestionData.created_at;
  let date = new Date(defaultTime).toLocaleDateString("nl-NL", {
    day: "numeric",
    month: "long",
    year: "numeric",
    hour: "2-digit",
    minute: "2-digit",
  });

  const { data: residentSuggestionData, residentSuggestionError } =
    await supabase.from("resident_suggestion").select();

  const { data: residentData, residentError } = await supabase
    .from("resident")
    .select();

  const { data: themeData, themeError } = await supabase.from("theme").select();

  const { data: suggestionThemeData, suggestionThemeError } = await supabase
    .from("suggestion_theme")
    .select();

  let listSuggestions = [];
  let theme = [];
  for (const residentSuggestion of residentSuggestionData) {
    for (const resident of residentData) {
      if (residentSuggestion.resident_id === resident.id) {
        if (residentSuggestion.suggestion_id === suggestionData.id) {
          suggestionData.resident = resident;
          listSuggestions.push(suggestionData);
        }
      }
    }
  }

  for (const suggestion of listSuggestions) {
    let relatedThemes = [];
    for (const ts of suggestionThemeData) {
      if (ts.suggestionId === suggestion.id) {
        relatedThemes.push(ts);
      }
    }
    for (const relatedTheme of relatedThemes) {
      for (const t of themeData) {
        if (t.id === relatedTheme.themaId) {
          theme.push(t);
        }
      }
    }
  }

  if (
    error ||
    residentSuggestionError ||
    residentError ||
    themeError ||
    suggestionThemeError
  ) {
    console.error(
      "Error fetching suggestion:",
      error ||
        residentSuggestionError ||
        residentError ||
        themeError ||
        suggestionThemeError
    );
  } else {
    res.render("suggestion", {
      title: "Wens",
      suggestion: suggestionData,
      time: date,
      themes: theme,
    });
  }
});

router.get("/user/:first_name", async (req, res) => {
  const firstName = req.params.first_name;
  const { data: userData, error: userError } = await supabase
    .from("resident")
    .select()
    .eq("first_name", firstName)
    .single();

  let defaultTime = userData.created_at;
  let date = new Date(defaultTime).toLocaleDateString("nl-NL", {
    day: "numeric",
    month: "long",
    year: "numeric",
    hour: "2-digit",
    minute: "2-digit",
  });

  const { data: residentSuggestionData, residentSuggestionError } =
    await supabase.from("resident_suggestion").select();

  const { data: suggestionData, suggestionError } = await supabase
    .from("suggestion")
    .select();

  let int = 0;
  let listSuggestions = [];
  let theme = [];
  for (const suggestion of suggestionData) {
    for (const residentSuggestion of residentSuggestionData) {
      if (suggestion.id === residentSuggestion.suggestion_id) {
        if (userData.id === residentSuggestion.resident_id) {
          int++;
          listSuggestions.push(suggestion);
        }
      }
    }
  }

  const { data: themeData, themeError } = await supabase.from("theme").select();

  const { data: suggestionThemeData, suggestionThemeError } = await supabase
    .from("suggestion_theme")
    .select();
  for (const suggestion of listSuggestions) {
    let relatedThemes = [];
    for (const ts of suggestionThemeData) {
      if (ts.suggestionId === suggestion.id) {
        relatedThemes.push(ts);
      }
    }
    for (const relatedTheme of relatedThemes) {
      for (const t of themeData) {
        if (t.id === relatedTheme.themaId) {
          theme.push(t);
        }
      }
    }
  }
  if (
    userError ||
    residentSuggestionError ||
    suggestionError ||
    themeError ||
    suggestionThemeError
  ) {
    console.error(
      "Error:",
      userError ||
        residentSuggestionError ||
        suggestionError ||
        themeError ||
        suggestionThemeError
    );
  } else {
    res.render("user", {
      title: "Gebruiker",
      user: userData,
      time: date,
      amount: int,
      suggestions: listSuggestions,
      themes: theme,
    });
  }
});

router.post("/form", async (req, res) => {
  try {
    const { data, error } = await supabase
      .from("suggestion")
      .insert([
        {
          title: req.body.title,
          description: req.body.description,
          image: req.body.imageLink,
        },
      ])
      .select();

    const insertId = data.length > 0 ? data[0].id : null;
    if (error || !insertId) {
      throw error;
    }

    console.log([parseInt(req.body.theme)]);
    const themes = req.body.theme;

    const themeInsertPromises = themes.map(async (theme) => {
      const { data: themeData, error: themeError } = await supabase
        .from("theme")
        .select("id")
        .eq("id", theme)
        .single();
      if (themeError) {
        throw themeError;
      }

      const { error: suggestionThemeError } = await supabase
        .from("suggestion_theme")
        .insert([
          {
            suggestionId: insertId,
            themaId: themeData.id,
          },
        ]);
      if (suggestionThemeError) {
        throw suggestionThemeError;
      }
    });

    await Promise.all(themeInsertPromises);
    res.render("sent", {
      title: "sent",
    });
  } catch (error) {
    res
      .status(500)
      .json({ error: "Het toevoegen van de wens ging fout, probeer opnieuw" });
    console.log(error);
    return;
  }
});

router.get("/sent", (req, res) => {
  res.render("sent", {
    title: "Bevesting",
  });
});

router.get("/form", (req, res) => {
  res.render("form", {
    title: "Formulier",
  });
});

router.get("/offline", (req, res) => {
  res.render("offline", {
    title: "Offline",
  });
});

module.exports = router;
```
This is the router file that I created that contains all the routes that we needed for the application.
It gets called in the `app.js` file as follows:

```js
const router = require('./routes/route')
app.use('/', router);
```

### Database
While we were fetching data from the database, I noticed that the database was missing some data. 
Each time that I noticed that something was missing, I added it to the database.
And also since both team was testeing of the data they were fetch and sending to the database was correct, I had to constantly clear the database. 
Otherwise I would crach everyones application.

### User detail page
The product owner give the suggestion to add a user page detail if we had the time. I took this task up on me to design the page.
I started with a small design in Figma. 
I used the colors from the color palette and the font from the house style, also used the same icons as on the overview page. 

<img width="639" alt="Screenshot 2023-06-25 at 22 57 25" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/2ec52751-0bed-455e-aa60-3ed727ca2c81">

```js
router.get("/user/:first_name", async (req, res) => {
  const firstName = req.params.first_name;
  const { data: userData, error: userError } = await supabase
    .from("resident")
    .select()
    .eq("first_name", firstName)
    .single();

  let defaultTime = userData.created_at;
  let date = new Date(defaultTime).toLocaleDateString("nl-NL", {
    day: "numeric",
    month: "long",
    year: "numeric",
    hour: "2-digit",
    minute: "2-digit",
  });

  const { data: residentSuggestionData, residentSuggestionError } =
    await supabase.from("resident_suggestion").select();

  const { data: suggestionData, suggestionError } = await supabase
    .from("suggestion")
    .select();

  let int = 0;
  let listSuggestions = [];
  let theme = [];
  for (const suggestion of suggestionData) {
    for (const residentSuggestion of residentSuggestionData) {
      if (suggestion.id === residentSuggestion.suggestion_id) {
        if (userData.id === residentSuggestion.resident_id) {
          int++;
          listSuggestions.push(suggestion);
        }
      }
    }
  }

  const { data: themeData, themeError } = await supabase.from("theme").select();

  const { data: suggestionThemeData, suggestionThemeError } = await supabase
    .from("suggestion_theme")
    .select();
  for (const suggestion of listSuggestions) {
    let relatedThemes = [];
    for (const ts of suggestionThemeData) {
      if (ts.suggestionId === suggestion.id) {
        relatedThemes.push(ts);
      }
    }
    for (const relatedTheme of relatedThemes) {
      for (const t of themeData) {
        if (t.id === relatedTheme.themaId) {
          theme.push(t);
        }
      }
    }
  }
  if (
    userError ||
    residentSuggestionError ||
    suggestionError ||
    themeError ||
    suggestionThemeError
  ) {
    console.error(
      "Error:",
      userError ||
        residentSuggestionError ||
        suggestionError ||
        themeError ||
        suggestionThemeError
    );
  } else {
    res.render("user", {
      title: "Gebruiker",
      user: userData,
      time: date,
      amount: int,
      suggestions: listSuggestions,
      themes: theme,
    });
  }
});
```
This is the router file that I created for the user detail page.

### Code refactor
As team we took the time to refactor our code.
We focus on cleaning up our code, removing all the console logs and comments that we didn't need anymore.
Check if we stayed consistent with our naming conventions.
and renaming some of the functions to make it more clear what they do.

## Week 5
### Fetching data
For some final touch I fetch the theme for each suggestion and added it to the detailpage and the user detail page.

in the previous iteration I did fetch the theme for each suggestion, but obly one theme. 
And some suggestion has more then one theme

<img width="1276" alt="Screenshot 2023-06-23 at 20 05 55" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/2dda3a9f-cd7a-42ed-a400-c8185a44dfa7">

<img width="1263" alt="Screenshot 2023-06-23 at 20 24 15" src="https://github.com/RainbowJM/meesterproef-2223/assets/59873140/d27f3eb2-fb04-42fb-8ec1-b2ed96b56101">


### Code refactor

### Testing
This week I focus on testing the whole applicattion, note where there were bug or things that we could so better.



### LightHouse testing
---

## Feedback
### Feedback week 1
#### Feedback design review - 31 mei 2023
- More interaction
- Deviate from the house style
- Discuss whether the chat is really useful
- Give each theme a color
- Give the detailpage with certain theme a color
- Animated slogan

#### Feedback debriefing - 1 juni 2023
We sent our first version of the debrief to our coach and the client. 
We received feedback that we have modified together. 
Feedback (in Dutch):
- Hebben we toegang tot het platform CrossMarX? Is dat nodig?
- Is er content/data beschikbaar?
- Hoe gaan IJburg bewoners op het platform? Voornamelijk Mobiel? Responsive?
- Hoe krijgt de gemeente en projectleiders de ideeen en voorstellen te zien/horen?
- Hebben we een huisstijldocument? Of moeten we dat samenstellen aan de hand van de bestaande website
- Is de huisstijlgids grafisch of zijn er al web elementen en componenten gedefinieerd (living styleguide)?
- Kunnen we inlog testen? Hebben we test user accounts? Is dat nodig?
- Hebben we toegang tot de gebruikers? Testdagen plannen? (liefst door de opdrachtgever)
- Projectleiders ontbreken in de lijst gebruikers?
- Welke data kunnen/willen de bewoners posten? titel, text, categorie, platje, filmpje?
- Wat betekent API (vanuit school)? Wie gaat dat doen?
- Ik zie niet goed wat de relatie is tussen het project wat jullie gaan ontwerpen en maken en de CrossmarX software

#### Feedback Sprint review - 2 juni 2023
- We can define the theme with sustainability development goals or Donut economics
- Other words for 'trekker' and 'delers' can be; ambassador, support
- Overview of people sharing the proposal
- Can deviate with the house style, but should express strandeiland feeling
- Can you see who is online in chat
- Bit complicated about chat, it might get too much, he really wants to see the important messages back.
- Be able to select multiple themes in the form
- Product owner wants to see the chat and also see messages (important messages)
- Make a separate page where you put the chat on a separate page
- Themes should be looked at properly, strandeiland does not exist yet, so playground etc is not going to be useful
- All the things that go wrong at the moment, you can prevent those in advance, he wants to see such wishes

#### Retrospetive 
That was all for the first Sprint of the project.
We did a debrieving and already sent it to the product owner. 
I worked on the API started from scratch, made the datamodel. 
Working on the API and the datamodel was a bit of a rollorcoaster, because it was my second time making a API with supabase.
And this thime the API was a bit more complicated.
But I learned a lot from it.
Think what are the best name for each of the table and their relationships to each other. 
Did a little bit of coding for the chat in the detail page.

I think we work well together as a group, and there is clear communication and division of labor.

For a more detailed infomation about the daily stand-ups, sprint reviews and retrospectives you can go to the [wiki](https://github.com/RainbowJM/strandeiland/wiki/Daily-Stand-ups--&-Retrospective) & [project board](https://github.com/users/RainbowJM/projects/1)

### Feedback week 2
#### Feedback Code Review - 7 juni 2023
This was the first code review, we had to show our code to the other group and they had to give feedback on it. 
I got some good feedback on my code, but also some things I could improve on.

- Feature branches
- Create issues and link them in the project board
- Using Github to keep a to do list
- Break down Javascript and ejs templating and rewrite into modules

We were already working with branches, but everyone had one branch where they were working in.
That means that everey feature was in one branch, and that is not really good.
And we were already working with issues, but we were not linking them in the project board.  
When making pull request, so that was for sure a good thing to do.

#### Feedback Sprint Review - 9 juni 2023
- Making it clearer that the filter can expand
- Search based on keyword
- New design for detail page
- New design for the chat - more functionalities and change the name
- Different ways to upload image in wish form
- Change proposal to wish
- Pull menu to be different and not on the side
- The wish create butuon should have an activating call to action

#### Retrospetive 
That was all for the second Sprint of the project.
This week I focused on finishing the API and the datamodel.
I also worked on the chat, style it and made it work with the basic functionalities.
The pull request was a bit of a struggle, because I had to merge the branches and there was alot of merge conflict, cuz we were not working in modules yet.
When we started working with modules all of that was fixed.
There was lest merge conflict and the code was more readable.
Added also service worker to the project, so that it can work offline.

I think we work well together as a group, and there is clear communication and division of labor.

For a more detailed infomation about the daily stand-ups, sprint reviews and retrospectives you can go to the [wiki](https://github.com/RainbowJM/strandeiland/wiki/Daily-Stand-ups--&-Retrospective) & [project board](https://github.com/users/RainbowJM/projects/1)


### Feedback Week 3
#### Feedback Code Review - 14 juni 2023
- The code is well structured and uncluttered
- Splits up the app.js file into modules
- Add dummy data to the database for the API
  
#### Feedback Sprint Review - 15 juni 2023
- On the overview page change the order of sorting and filtering
- Online views on the post, is it everyone who is online on the community page or are only users who are currently on the page.
- Green circle (when user is online) is not clear enough

#### Feedback Design Review - 15 juni 2023
- For the form page need to pay attention to hierachy which components belong together
- The input section for image can be changed to a pop up.
- Pay attention to the hierarchy of the overview page
- Change a catchy image for the banner on the overview page
- Add animation to the sending of reactions
- A catchy banner image that gives more context.
- Playing more with the layout of the overview pages
- Add more color to the color palette

#### Retrospetive 
That was all for the third Sprint of the project.
This week I stared working with chnge the design of teh chat.
And implementeing this in to the code.
After the code review we had, I first finished the new chat in code and then started to add dummy data to the database.
While doing this I changed the datamodel again.
After that I did a design for the user detail page.

I think we work well together as a group, and there is clear communication and division of labor.

For a more detailed infomation about the daily stand-ups, sprint reviews and retrospectives you can go to the [wiki](https://github.com/RainbowJM/strandeiland/wiki/Daily-Stand-ups--&-Retrospective) & [project board](https://github.com/users/RainbowJM/projects/1)

### Feedback Week 4
#### Feedback Code Review - 21 juni 2023
- The code is well structured and uncluttered
- Good file names
- Remove console.log
- remove not needed comments
- Split `app.js` into multiple files
- Do performance test
- Do accessibility test
- Prioritize tasks
- Check for the correct head structuring in html
- Check if you are using the correct html elements

#### Feedback Design Review - 22 juni 2023
- Let the wish button rotate a bit when hovered
- Try the select menu 
- Try using grid auto fit 
  
#### Feedback Sprint Review - 23 juni 2023
- Show what the page looks like when sorted by themes
- Change the call button action 
- Show a data visualization which themes are used the most
- Filter sorting should be underneath the most recent wishes
- Enforce max 3 themes in the form
- See if we can flip the image or make it a bit higher
- Visualization how you can see which themes are most common

#### Retrospetive
Out of all the other weeks this was the week that we worked extra very hard on the project.
we wanted to have the majority of the functionalities done by the end of this week.
And we achieved that.
I worked on the design of the user detail page and then set it in to the code.
When the code design was one, I worked on fetching data from the database and displaying it on the page.
Also help Keisha with the filter and the sorting of the wishes. But sadly we could make it work.
During the code review we asked about it, we good as feedback that we should try to visualize the filter and sorting.
And skip the functionality for now.
So we did that, and it looks really good.
During this project I was/am the "pull request master" so I had to merge all the branches and fix the merge conflicts.
On the final day before the sprint review, we got a major merge conflict, that took me hours to fix.
Had to make hard descisions, but in the end it worked out.
Finally I have been walking through the application and fixed some bugs.

I think we work well together as a group, and there is clear communication and division of labor.

For a more detailed infomation about the daily stand-ups, sprint reviews and retrospectives you can go to the [wiki](https://github.com/RainbowJM/strandeiland/wiki/Daily-Stand-ups--&-Retrospective) & [project board](https://github.com/users/RainbowJM/projects/1)

---
## General retrospective


---

## Course Applied
### CSS to the Rescue
In this project you can defintely see that I have experimented with new CSS techniques. When I started with this minor I only new `div` and only used `id` and `class` as selector. But now I now more about the CSS selector and the possibility. This meesterproef project is defintily a good example. Check week 2 en week 4 for more information.
I experiment with CSS.  
I worked with new techniques like grid, :has() selectors and css animations.
It was for sure a challenge to work with grid, but I made it work.
I also used the :has() selector, which is not supported by all browsers. But I used it in a way that it is not a problem if it is not supported, by adding a fall back.

Check [Week 3](#week-3) and [Week 4](#week-4) for more information.

### Web App From Scratch
For this application to get the data to display on the pages, I used the API that was made for this project. [Strandeiland API](https://yyufywjwwwmgfjmenluv.supabase.co/rest/v1/)

I used Supabase to retrieve data and display it on the page. 
From the database I retrieved the first name, last name, description, date and image.

In terms of code structure, I worked with modules. We split our `app.js` file into a `route.js` file and `script.js` file has each functionality a separate file. 
Our CSS and HTML was also done in components. 
For the html we used a template engine called ejs. 
Repetitive HTML code was placed in a partials file and called in the ejs file. 
For the css, each page got it's own css file.

I wanted to make the `script.js` smaller, but due to time this was not possible.

Check [Week 1](#week-1), [Week 2](#week-2) and [Week 3](#week-3) for more information.

### Browser Technologies
One thing we learned in browser technologies is that we need to make sure that our application works as well as possible on all kinds of devices.
And under any conditions. 
So the application should be accessibility for everyone. 
So I started with testing my part, the user detail page, see if it works on all kinds of devices. 
Furthermore, we did a color contrast test to see if there is enough color contrast between the foreground and background. 

I alsot worked a bit on feature detection, for each function I wrote I put in an `if()` statements. 
If the feature does not exist then the code is not executed.

The basic functionality of the wish summary page is to write a semantic html structure. 
Writing good html can make it easier for people who use screen readers to operate the page. 
A progressive enhancement is formatting the HTML document with css. 
The page becomes more beautiful and clearer for the user.

Check [Week 1](#week-1), [Week 2](#week-2), [Week 3](#week-3) and [Week 4](#week-4) for more information.

### Progressive Web Apps
We used a template engine called ejs. 
In Progressive Web App was the first time that I worked with the template engine ejs and it was also the first time that I worked with express.

In Web App From Scratch we learned about working in modules and in Progressive Web Apps we went deeper in to it. 

I applied what we learned of service worker in this project, when I applied it we started noticing that as soon as you change pages the service worker will go to offline mode. 

The offline mode is for when you don't have internet, but in our case we had internet but yet it was going to the offline page.
I was very challenging to figure out how to fix this.

The fixes was in the `fetch`, I had to add a `catch` to the `fetch` and then it worked.

Also the part of client side rendering I did. 
This was to make sure that the page is loaded faster.
For this task I decided to try something new, in the course they one of the recommendation was to use gulp.
This will take care of the minifying of your code and other things.
But I did use it for the minifying of the code, during the course.
But for this project I implemented it and also learned how to work with it.

Check [Week 3](#week-3) and [Week 5](#week-5) for more information.

### Human Centred Design
We did a briefing and debriefing where we got to know more about the client and the project.
The idea of Human Centres Design is tha you will create a product that is based on the user goals. 
And that you will test the product with the user each time.
This is something that I have definitely been doing the last five weeks.
At the end of each iteration we tested the prototype with the product owner, who in this case is the client.

At the end of each iteration the team and I had a meeting with the client. 
Where we showed the prototype and the client gave feedback.
Based on the feedback we made a new prototype for the next iteration.

Check [Week 1](#week-1) and [Feedback](#feedback) for more information.

### Real Time Web
I implemetend a real-time feature in the application. 
The feature is that the reaction that are placed are done by `socket.io`.
There is a socket connection where the client and server can communicate with each other.
When a user places a reaction, the server will send the reaction to all the clients that are connected to the socket.

Futhermore I made the API that we are using for this project.
I used Supabase to create the API.
It took more time that I expected to create the API, but I learned a lot from it.
It was my second time making an API using Supabase.
And this time it was a lot more complicated than the first time, more complex queries and more tables.

But I defintely learned new things, I did not know that you can create bucket with Supabase.
And that when you fetch data that supabase had its own `on` functions, that you can use to listen to changes in the database.
Or to check equal of data.

And it making on the database self was at first a complicated task, because I had to make sure that the data was correct.
And that the data was in the right format. and had everything that was needed.

Check [Week 1](#week-1), [Week 2](#week-2), [Week 3](#week-3) and [Week 4](#week-4) for more information.

---
## Sources
- How do I fetch Multiple Specific Rows in Supabase JS? (n.d.). Stack Overflow. https://stackoverflow.com/questions/75717077/how-do-i-fetch-multiple-specific-rows-in-supabase-js
- How to get “COUNT(*)” in Supabase. (n.d.). Stack Overflow. https://stackoverflow.com/questions/65612167/how-to-get-count-in-supabase
- Vanilla JavaScript search - how to show results only when button is clicked? (n.d.). Stack Overflow. https://stackoverflow.com/questions/69117827/vanilla-javascript-search-how-to-show-results-only-when-button-is-clicked
- How to get the selected radio button’s value? (n.d.). Stack Overflow. https://stackoverflow.com/questions/9618504/how-to-get-the-selected-radio-button-s-value
- How do I get Date(); to show the time in JavaScript right? (n.d.). Stack Overflow. https://stackoverflow.com/questions/46754181/how-do-i-get-date-to-show-the-time-in-javascript-right
- How to make “fit-content” work across browsers? (n.d.). Stack Overflow. https://stackoverflow.com/questions/54740433/how-to-make-fit-content-work-across-browsers
- Rotate Parent but not child on hover. (n.d.). Stack Overflow. https://stackoverflow.com/questions/48651589/rotate-parent-but-not-child-on-hover
- EJS - pass data to partial view and use it in every view/page. How can i do that? (n.d.). Stack Overflow. https://stackoverflow.com/questions/60551806/ejs-pass-data-to-partial-view-and-use-it-in-every-view-page-how-can-i-do-that
- iterating over JSON object in ejs partial. (n.d.). Stack Overflow. https://stackoverflow.com/questions/37279927/iterating-over-json-object-in-ejs-partial
- Fading out text on overflow with css if the text is bigger than allowed. (n.d.). Stack Overflow. https://stackoverflow.com/questions/22808040/fading-out-text-on-overflow-with-css-if-the-text-is-bigger-than-allowed
- ::-webkit-scrollbar - CSS: Cascading Style Sheets | MDN. (2023, April 1). https://developer.mozilla.org/en-US/docs/Web/CSS/::-webkit-scrollbar
- Advanced Form Control Styling With Selectmenu And Anchoring API — Smashing Magazine. (2023, June 1). Smashing Magazine. https://www.smashingmagazine.com/2023/06/advanced-form-control-styling-selectmenu-anchoring-api/
- Lazy loading - Web performance | MDN. (2023, March 30). https://developer.mozilla.org/en-US/docs/Web/Performance/Lazy_loading
- Brosset, P. (2022, October 25). The selectmenu HTML Tag | CSS-Tricks. CSS-Tricks. https://css-tricks.com/the-selectmenu-element/
- Fetch data | Supabase. (n.d.). https://supabase.com/docs/reference/javascript/crawlers/select
- Isheanesu. (2022). How To SELECT, COUNT and JOIN Supabase Data. DEV Community. https://dev.to/thisisisheanesu/how-to-select-count-and-join-supabase-data-3ihk
- House, C. (2023). A Complete Guide to CSS Grid | CSS-Tricks. CSS-Tricks. https://css-tricks.com/snippets/css/complete-guide-grid/
- Onyejiaku, T. K. (2023). What is req.query in Express.js? Educative: Interactive Courses for Software Developers. https://www.educative.io/answers/what-is-reqquery-in-expressjs
- Hallo IJburg - houdt je verbonden. (n.d.). halloijburg.nl. https://halloijburg.nl/
- Hallo Strandeiland. (n.d.). hallostrandeiland.nl. https://hallostrandeiland.nl/
- Supabase Javascript Client - Using filters. (n.d.). https://supabase.com/docs/reference/javascript/using-filters
- How To Create Vertical Tabs. (n.d.). https://www.w3schools.com/howto/howto_js_vertical_tabs.asp
- how to use font awesome icons in HTML. (n.d.). Stack Overflow. https://stackoverflow.com/questions/71146319/how-to-use-font-awesome-icons-in-html
- CSS scroll snap - CSS: Cascading Style Sheets | MDN. (2023, May 29). https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_scroll_snap
- Kohler, M. (2020, June 18). Practical CSS Scroll Snapping | CSS-Tricks. CSS-Tricks. https://css-tricks.com/practical-css-scroll-snapping/
- Using Each Loop in EJS Template and Express JS. (2021, July 8). The freeCodeCamp Forum. https://forum.freecodecamp.org/t/using-each-loop-in-ejs-template-and-express-js/468398/2
- suggestion | Meesterproef | Strandeiland | Supabase. (n.d.). https://supabase.com/dashboard/project/yyufywjwwwmgfjmenluv/editor/28660?sort=id%3Adesc
- API | Supabase. (n.d.). https://supabase.com/dashboard/project/yyufywjwwwmgfjmenluv/api
- Magdalena, J. (2023, June 16). Unleashing the Power of Supabase: Your Ultimate Guide to Modern Database Development With Express. Medium. https://medium.com/@jevona.magdalena/unleashing-the-power-of-supabase-your-ultimate-guide-to-modern-database-development-with-express-872dbb3b6e
- Service Worker API - Web APIs | MDN. (2023, April 13). https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API
