<div align="center">

# 🎮 jQuery Pokédex

**A simple Pokémon encyclopedia built with Flask & jQuery**

My first web project — built during university while learning how to fetch and consume a REST API with jQuery's `$.ajax`.

![Flask](https://img.shields.io/badge/Flask-2.2-000000?style=flat-square&logo=flask&logoColor=white)
![jQuery](https://img.shields.io/badge/jQuery-3.7-0769AD?style=flat-square&logo=jquery&logoColor=white)
![PokeAPI](https://img.shields.io/badge/API-PokeAPI-E83E8C?style=flat-square&logo=pokeapi&logoColor=white)
![Vercel](https://img.shields.io/badge/Deployed-Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

</div>

---

## 🚀 Live Demo

**[jquery-pokedex.vercel.app](https://jquery-pokedex.vercel.app/)**

> Yes, the subdomain is spelled `jquery-pokemon` instead of `jquery-pokedex` — and it is staying that way on purpose. 🙃

---

## ✨ Features

- **Pokémon Grid** — browse 20 Pokémon per page, fetched live from [PokeAPI](https://pokeapi.co)
- **Pagination** — navigate through every page, with ellipsis markers around the current page
- **Detail Modal** — click a Pokémon card to fetch and show its abilities and types
- **Sidebar Search** — full list of 1,320+ Pokémon with instant client-side filtering
- **Responsive Layout** — grid and modal adapt down to small phone screens

---

## 🛠 Tech Stack

| Layer | Technology |
|:-:|:-:|
| Backend | Flask (Python) |
| Frontend | jQuery 3.7, HTML, CSS |
| Data | [PokeAPI](https://pokeapi.co) (public REST API) |
| Hosting | Vercel |

---

## 🧭 From jQuery to React

This repo is a snapshot of where I started.

Back then, `$.ajax` was how I reached the outside world — a `success` callback felt like magic the first time a Pokémon name appeared on screen. There is no build step, no state management, and no component model: just a template, a script tag, and a lot of string concatenation.

Since then, I have moved on to **React 19 + Laravel 12**, where data fetching, state, and rendering are handled very differently. You can see where that path led in my [Buku Pejabat](https://github.com/qhnaf/bukupejabat-portfolio) project — a full-stack application with role-based auth, PDF generation, and a component-driven frontend.

I keep this project around to measure the distance.

---

## ⚠️ Known Limitations

Honesty over polish — this is what it is:

- **Missing sprites** — Pokémon images for entries #52 through #66 do not render (noted in the app's own warning popup)
- **Sidebar images** — clicking a Pokémon from the sidebar list does not show its picture
- **Dead routes** — `/home2` and `/list` still exist in `app.py` but their templates were removed, so they return a 500
- **Unused dependencies** — a few packages in `requirements.txt` are leftovers from earlier experiments

---

## ▶️ Getting Started

```bash
git clone https://github.com/qhnaf/jquery-pokedex.git
cd jquery-pokedex
pip install -r requirements.txt
python app.py
```

Then open [http://localhost:5000](http://localhost:5000).

No environment variables required — the app talks directly to PokeAPI from the browser.

---

<div align="center">

Built by [Ahnaf](https://github.com/qhnaf) while learning the web.

</div>
