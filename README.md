<div align="center">

<!-- Animated wave banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=220&section=header&text=Hey%20There!%20I'm%20Manju%20%F0%9F%91%8B&fontSize=42&fontColor=00F5FF&animation=twinkling&fontAlignY=38&desc=Software%20%26%20Web%20Developer&descAlignY=58&descSize=20&descColor=FF00E5" width="100%"/>

<!-- Typing SVG -->
<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=26&duration=2500&pause=1000&color=39FF14&center=true&vCenter=true&width=600&lines=Building+cool+things+for+the+web+%F0%9F%9A%80;Clean+code+%2B+bold+design;Always+learning+%2C+always+shipping;Welcome+to+my+profile+%E2%9C%A8" alt="Typing SVG" />
</a>

<br/>

<!-- Social badges -->
<a href="https://github.com/manju-17-ctrl">
  <img src="https://img.shields.io/badge/GitHub-manju--17--ctrl-0f0c29?style=for-the-badge&logo=github&logoColor=39FF14&labelColor=000000" />
</a>
<img src="https://komarev.com/ghpvc/?username=manju-17-ctrl&style=for-the-badge&color=ff00e5&labelColor=000000&label=PROFILE+VIEWS" />

</div>

<br/>

## ⚡ About Me

<img align="right" width="320" src="https://raw.githubusercontent.com/DenverCoder1/DenverCoder1/main/discord-status.svg" style="display:none;" />

```yaml
name: Manju
role: Software / Web Developer
focus: [ "Frontend", "Backend", "Full-Stack" ]
currently_learning: "Always leveling up 🔼"
fun_fact: "I turn ☕ into 💻"
```

- 🔭 Currently building cool web projects
- 🌱 Constantly sharpening my dev skills
- 💬 Ask me about web development
- ⚡ Fun fact: I debug faster than I explain what the bug was

<br/>

## 🛠️ Tech Stack

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=39FF14)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=00F5FF)
![JavaScript](https://img.shields.io/badge/JavaScript-000000?style=for-the-badge&logo=javascript&logoColor=F7DF1E)
![React](https://img.shields.io/badge/React-000000?style=for-the-badge&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-000000?style=for-the-badge&logo=node.js&logoColor=39FF14)
![Python](https://img.shields.io/badge/Python-000000?style=for-the-badge&logo=python&logoColor=FFE873)
![Git](https://img.shields.io/badge/Git-000000?style=for-the-badge&logo=git&logoColor=FF00E5)
![VSCode](https://img.shields.io/badge/VS%20Code-000000?style=for-the-badge&logo=visualstudiocode&logoColor=00F5FF)

</div>

<br/>

## 📊 GitHub Stats

<div align="center">

<img height="180em" src="https://github-readme-stats.vercel.app/api?username=manju-17-ctrl&show_icons=true&theme=radical&hide_border=true&bg_color=0D1117&title_color=FF00E5&icon_color=39FF14&text_color=C9D1D9"/>
<img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=manju-17-ctrl&layout=compact&theme=radical&hide_border=true&bg_color=0D1117&title_color=FF00E5&text_color=C9D1D9"/>

<br/>

<img src="https://streak-stats.demolab.com?user=manju-17-ctrl&theme=radical&hide_border=true&background=0D1117&ring=39FF14&fire=FF00E5&currStreakLabel=00F5FF"/>

</div>

<br/>

## 🏆 Trophies

<div align="center">
<img src="https://github-profile-trophy.vercel.app/?username=manju-17-ctrl&theme=radical&no-frame=true&no-bg=true&margin-w=8&row=1" />
</div>

<br/>

## 📈 Contribution Graph

<div align="center">
<img src="https://github-readme-activity-graph.vercel.app/graph?username=manju-17-ctrl&theme=redical&bg_color=0D1117&color=39FF14&line=FF00E5&point=00F5FF&hide_border=true" width="95%"/>
</div>

<br/>

## 🐍 Contribution Snake

<div align="center">
<img src="https://raw.githubusercontent.com/manju-17-ctrl/manju-17-ctrl/output/github-contribution-grid-snake-dark.svg" width="95%"/>
</div>

> ⚠️ The snake animation above needs a one-time GitHub Actions setup (I've included the workflow file below) — it won't render until that's added to your profile repo.

<br/>

## 🤝 Connect With Me

<div align="center">

<a href="https://github.com/manju-17-ctrl"><img src="https://img.shields.io/badge/GitHub-Follow-000000?style=for-the-badge&logo=github&logoColor=39FF14"/></a>
<a href="#"><img src="https://img.shields.io/badge/LinkedIn-Connect-000000?style=for-the-badge&logo=linkedin&logoColor=00F5FF"/></a>
<a href="#"><img src="https://img.shields.io/badge/Twitter-Follow-000000?style=for-the-badge&logo=twitter&logoColor=FF00E5"/></a>
<a href="#"><img src="https://img.shields.io/badge/Portfolio-Visit-000000?style=for-the-badge&logo=googlechrome&logoColor=39FF14"/></a>

</div>
name: Generate Snake Animation

on:
  schedule:
    - cron: "0 0 * * *"    # runs once a day
  workflow_dispatch: {}      # lets you trigger it manually
  push:
    branches:
      - main

jobs:
  generate:
    permissions:
      contents: write
    runs-on: ubuntu-latest
    steps:
      - name: Generate the snake game from GitHub contribution grid
        uses: Platane/snk@v3
        with:
          github_user_name: manju-17-ctrl
          outputs: |
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark
            dist/github-contribution-grid-snake.svg

      - name: Push output to the output branch
        uses: crazy-max/ghaction-github-pages@v4
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

<br/>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:24243e,50:302b63,100:0f0c29&height=120&section=footer"/>
</div>

<div align="center">
<i>⭐️ Thanks for stopping by — feel free to explore my repos!</i>
</div>
