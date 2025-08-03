<h2 align="left">Hi 👋! My name is Aravind </h2>

###

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Aravind-avii&hide_title=false&hide_rank=false&show_icons=true&include_all_commits=true&count_private=true&disable_animations=false&theme=dracula&locale=en&hide_border=false" height="150" alt="stats graph"  />
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=Aravind-avii&locale=en&hide_title=false&layout=compact&card_width=320&langs_count=5&theme=dracula&hide_border=false" height="150" alt="languages graph"  />
</div>

###


###

<div align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="30" alt="javascript logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" height="30" alt="typescript logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" height="30" alt="react logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" height="30" alt="html5 logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" height="30" alt="css3 logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" height="30" alt="python logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/csharp/csharp-original.svg" height="30" alt="csharp logo"  />
</div>

###

<div align="left">
  <a href="mailto:aravindb2104@gmail.com">
    <img src="https://img.shields.io/static/v1?message=aravindb2104@gmail.com&logo=gmail&label=&color=D14836&logoColor=white&labelColor=&style=for-the-badge" height="35" alt="gmail logo" />
  </a>
  <a href="https://www.linkedin.com/in/bandaru-aravind-690557253" target="_blank">
    <img src="https://img.shields.io/static/v1?message=LinkedIn&logo=linkedin&label=&color=0077B5&logoColor=white&labelColor=&style=for-the-badge" height="35" alt="linkedin logo" />
  </a>
</div>


###

<br clear="both">

### 🐍 GitHub Contribution Snake

<img src="https://github.com/Aravind-avii/Aravind-avii/blob/output/github-contribution-grid-snake.svg" alt="Snake animation" />

name: Generate Snake Animation

on:
  schedule:
    - cron: "0 0 * * *"  # Runs every day at midnight UTC
  workflow_dispatch:      # Allows manual trigger

jobs:
  generate:
    runs-on: ubuntu-latest
    steps:
      - name: Generate Snake SVG
        uses: Platane/snk@v3
        with:
          github_user_name: Aravind-avii
          outputs: |
            dist/github-contribution-grid-snake.svg

      - name: Push Snake to output branch
        uses: crazy-max/ghaction-github-pages@v3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

###
