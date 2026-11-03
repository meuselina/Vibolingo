<div align="center">

# Vibolingo

**Duolingo for the way software gets built now.**
Five minutes a day. Real, working apps. No CS degree required.

![2nd place](https://img.shields.io/badge/%F0%9F%8F%86%202nd%20place-CODE%20Hackathon-f59e0b?style=for-the-badge)
![HTML](https://img.shields.io/badge/HTML-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-663399?style=for-the-badge&logo=css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

**[Try the live demo](https://meuselina.github.io/Vibolingo/)** · concept prototype, not a live product

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
