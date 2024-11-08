✨ Hi there, I'm Mariana Lazarini!

🇧🇷 Estudante de Engenharia da Computação - IFSP

🇺🇸 Studying Computer Engineer - IFSP

<div>
  <a href="https://MarianaLazarini">
    <img height="180em" src="https://github-readme-stats.vercel.app/api?username=MarianaLazarini&show_icons=true&theme=dracula&include_all_commits=true&count_private=true"/>
    <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MarianaLazarini&layout=compact&langs_count=8&theme=dracula"/>
</div>

  <div style="display: inline_block"><br>
  <img align="center" alt="C" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/c/c-original.svg">
  <img align="center" alt="C++" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-original.svg">
  <img align="center" alt="C#" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/csharp/csharp-original.svg">
  <img align="center" alt="Java" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg">
  <img align="center" alt="Java Script Icon" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg">
  <img align="center" alt="Canva Icon" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/canva/canva-original.svg">
</div>
  
  ##
 
<div> 
  <a href="https://www.linkedin.com/in/mariana-lazarini-01347222a/?originalSubdomain=br" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a>
      <a href="https://www.instagram.com/marianalazarini_/" target="_blank"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
    <a href="marisolazarini@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"></a>


name: Generate Datas

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: rafaballerini
          svg_out_path: dist/github-contribution-grid-snake.svg

  - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
      
