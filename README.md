<h1 align="center">👋 Olá, eu sou xddogDev!</h1>

<p align="center">
  💻 Desenvolvedor de bots • 🌐 Criador de sistemas • 🚀 Apaixonado por código
</p>

---

### 👨‍💻 Sobre mim

- 🔭 Trabalhando em: bots para Discord e projetos web
- 🌱 Aprendendo: Node.js, MongoDB, Discord.js
- 💬 Me chame pra trocar ideia sobre bots e APIs!
- ⚡ Fun fact: Sempre tenho um projeto secreto em andamento 👀

---

### 🛠️ Tecnologias e Ferramentas

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![Discord.js](https://img.shields.io/badge/Discord.js-5865F2?style=for-the-badge&logo=discord&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

---

### 📊 Estatísticas

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=xddogDev&show_icons=true&theme=radical" width="45%"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=xddogDev&layout=compact&theme=radical" width="45%"/>
</div>

---

### 📫 Onde me encontrar

- Discord: `xddogDev#1234`
- Email: ryanalexandreredes@gmail.com
- Comunidade: [maralto](https://discord.gg/maralto)

# Nome da Actions:  
name: Snake Game

# Controlador do tempo que sera feito a atualização dos arquivos.
on:
  schedule:
      # Será atualizado a cada 5 horas.
    - cron: "0 */5 * * *"

# Permite executar na na lista de Actions (utilizado para testes de build).
  workflow_dispatch:

# Regras
jobs:
  build:
    runs-on: ubuntu-latest
    steps:

    # Checks repo under $GITHUB_WORKSHOP, so your job can access it
      - uses: actions/checkout@v2

    # Repositorio que será utilizado para gerar os arquivos.
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: nomeUsuario #Seu usuario
          gif_out_path: dist/github-contribution-grid-snake.gif
          svg_out_path: dist/github-contribution-grid-snake.svg

      - run: git status

      # Para as atualizações.
      - name: Push changes
        uses: ad-m/github-push-action@master
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          branch: master
          force: true

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          # the output branch we mentioned above
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}


