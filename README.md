<h1 align="center">👋 Olá, eu sou Ryan!</h1>

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

- Discord: [Fantasma](https://discord.com/users/994037361824518164)
- Email: ryanalexandreredes@gmail.com
- Comunidade: [maralto](https://discord.gg/maralto)

- uses: Platane/snk@v3
  with:
    # github user name to read the contribution graph from (**required**)
    # using action context var `github.repository_owner` or specified user
    github_user_name: ${{ github.repository_owner }}

    # list of files to generate.
    # one file per line. Each output can be customized with options as query string.
    #
    #  supported options:
    #  - palette:     A preset of color, one of [github, github-dark, github-light]
    #  - color_snake: Color of the snake
    #  - color_dots:  Coma separated list of dots color.
    #                 The first one is 0 contribution, then it goes from the low contribution to the highest.
    #                 Exactly 5 colors are expected.
    outputs: |
      dist/github-snake.svg
      dist/github-snake-dark.svg?palette=github-dark
      dist/ocean.gif?color_snake=orange&color_dots=#bfd6f6,#8dbdff,#64a1f4,#4b91f1,#3c7dd9
