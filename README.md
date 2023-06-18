# Duurzaam, groen en sociaal Strandeiland
Team repo: https://github.com/RainbowJM/strandeiland
---
# Table of contents

---
## Introduction
The Meesterproef is the final client-project of the half year minor programme about Web Design and Development in Amsterdam. 
Bachelor Communication and Multimedia Design, Amsterdam University of Applied Science.

In the coming years, a completely new neighborhood will be created on the east side of Amsterdam: Strandeiland. 
Ambitions are high: the neighborhood must be energy-generating, greener than the first version of IJburg, residents must be able to live pleasantly with each other and equality of opportunity must be improved.

## Duurzaam, groen en sociaal Strandeiland
The Participatieteam wants to add a new functionality for the `hallostrandeiland.nl` website where people can submit new proposals for the new Strandeiland neighborhood. This will promote communication between future residents of Strandeiland and the project managers of the municipality of Amsterdam. The goal is to use Hallo Strandeiland to collect good ideas and proposals, improve them and get the beautiful and feasible ones realized.

### User stories
The user stories are written in Dutch. The user stories are written in the following format: 
- Als toekomstig bewoner, wil ik mijn voorstel voor een duurzamer, groener en socialer strandeiland kunnen delen, zodat dit onderzocht en hopelijk gerealiseerd kan worden.

- Als toekomstig bewoner, wil ik een reactie kunnen geven op voorstellen van andere toekomstige bewoners, zodat we kunnen samenwerken aan het vormgeven van de voorstellen.

- Als projectmanager van de gemeente, wil ik voorstellen van toekomstige bewoners kunnen filteren op thema's, zodat ik per thema kan bekijken of er ideeën bijzitten die kunnen bijdragen aan een lagere ecologische footprint, of betere sociale cohesie van de wijk.

### Briefing
The briefing is the first meeting we had as group with Michel Vogler from CrossmarX. Before the briefing we made a mind map with all the information we already had about the project. You can find this mind map below.

... (pic of the mind map)
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
After the briefing we made a debriefing. We wrote down all the information we got from the briefing. We also wrote down the questions we still had. You can find the debriefing below.

[Debriefing](https://github.com/RainbowJM/strandeiland/wiki/Debriefing)

## Week 1
The kick-off presentation of the final project for this minor was given by the teachers. We were given detailed information about the planned schedule for the next five weeks. We had briefing with the product owner. After that we made a briefing with the product owner and we started working on a the first iteration of our prototype. 

### Brainstorm
We started with a brainstorm to get a better understanding of the project. 
Based on that we made a MoSCoW list.

... (pic of the MoSCoW list)

### Design
For this week we wanted a first version of the overview page, detail page make a wish form. 
So we started where everyone designed their idea's of options of how the page should look like.

... (pic of the design)

After that we brainstormed together to create a first version of the design by putting all the idea's together.

The overview page:
... (pic of the design)

The detail page:
... (pic of the design)

The make a wish form:
... (pic of the design)

### API
In the project description it was mentioned that we had to use an API. 
That I will be provided by the school self. 
But after a meeting that we had with the teacher that was responsible for the API, I got that assignment to make the API. 
The API will be used by both teams.

I made the API in supabase. The step by step guide can be found in the blog that I wrote. [Supabase](https://medium.com/@jevona.magdalena/unleashing-the-power-of-supabase-your-ultimate-guide-to-modern-database-development-with-express-872dbb3b6e)

The process of naming everything took a while, because I wanted to make sure that everything was clear.
So that everyone could understand what the API was doing. 
And how it has to be used.
... (pic of the naming)

...(pic first version datamodel)

...(pic second version datamodel)

The second version was the version that I went for in the end.
I made The tables and tested if the API worked with Postman.
... (pic of the postman)

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

For a more detailed infomation about the daily stand-ups, sprint reviews and retrospectives you can go to the [wiki](https://github.com/RainbowJM/strandeiland/wiki/Daily-Stand-ups--&-Retrospective)
