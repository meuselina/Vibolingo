<div align="center">

# Vibolingo

**Duolingo for the way software gets built now.**
Five minutes a day. Real, working apps. No CS degree required.

<img src="media/badge-hackathon.png" height="40" alt="2nd place at the CODE Hackathon" />&nbsp;
<a href="https://meuselina.github.io/Vibolingo/"><img src="media/button-live-demo.png" height="40" alt="Try the live demo" /></a>&nbsp;
<img src="media/badge-javascript.png" height="40" alt="Built with JavaScript" />

<sub>Concept prototype, not a live product</sub>

<img src="media/lesson-demo.gif" width="300" alt="Clicking through a full Vibolingo lesson" />

</div>

## The problem

Everyone can generate code now. Almost no one can direct it.
Millions of people are "vibe coding": describing an app to an AI and shipping whatever it hands back, without knowing whether it is safe or any good.

## The idea

Vibolingo teaches people to *direct* AI the way Duolingo teaches a language: short daily lessons, streaks, XP and leagues.

## A lesson in three checks

The demo walks through a full lesson, "Ship a waitlist page":

| Step | What you practice | Example |
|---|---|---|
| **Prompt quality** | Writing a sharp prompt | "Make me an app." vs. a prompt that names the headline, the signup form and the colors |
| **Vibe check** | Spotting risky AI code | "Would you ship this?" A signup function with a live API key in the code |
| **Iterating** | Giving useful feedback | "try again" vs. telling the AI what is wrong and what you want instead |

At the end you earn XP, keep your hearts and extend your streak.

![Vibolingo screens](screenshots.jpg)

## Screens

| Screen | What it shows |
|---|---|
| `Main.dc.html` | App pitch |
| `Home.dc.html` | Learning path with units like "Prompting Like a Pro" |
| `Lesson.dc.html` | A lesson: change a live tip calculator app by telling the AI what to do |
| `VibeCheck.dc.html` | "Would you ship this?" Spot problems in AI generated code, e.g. a hard coded API key |
| `Streak.dc.html` | Streak and weekly league |
| `Profile.dc.html` | Profile with shipped apps |
| `Icon.dc.html` | App icon |
| `Demo.dc.html` | Clickable demo |
| `index.html` | Start page linking all screens |

## Run locally

The screens load their components at runtime, so they need a small web server (opening the files directly does not work):

```bash
git clone https://github.com/meuselina/Vibolingo.git
cd Vibolingo
python3 -m http.server 8000
```

Then open http://localhost:8000 for the overview of all screens.

## Built with

HTML, CSS, JavaScript · hosted on GitHub Pages
