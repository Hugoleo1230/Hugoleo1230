# Olá, eu sou o Hugo Leonardo! 👋

<p align="center">
  <img src="https://img.shields.io/badge/Idade-14%20Anos-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Foco-Jovem%20Aprendiz-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Objetivo-Game%20Dev-purple?style=for-the-badge" />
</p>
name: Generate Snake

on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:

permissions:
  contents: write

jobs:
  generate:
    runs-on: ubuntu-latest

    steps:
      - name: Generate snake
        uses: Platane/snk@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-snake.svg
            dist/github-snake-dark.svg?palette=github-dark

      - name: Push snake
        uses: crazy-max/ghaction-github-pages@v4
        with:
          build_dir: dist
        env:
          GH_PAT: ${{ secrets.GITHUB_TOKEN
---

## 🚀 Sobre Mim

Sou um estudante de 14 anos apaixonado por tecnologia e em busca da minha primeira oportunidade no mercado de trabalho como **Jovem Aprendiz**. 

- 🏫 **Educação:** Estudante na *Escola Américo Marco Antônio* há 4 anos.
- 🎯 **Objetivo de Carreira:** No futuro, pretendo atuar profissionalmente na área de **Programação e Desenvolvimento de Jogos**.
- ⚽ **Fora da Tecnologia:** Pratico futebol, esporte que me ensinou na prática o valor da disciplina, do foco e do trabalho em equipe.

---

## 📚 Estudos & Capacitação (Em andamento)

Atualmente, venho me dedicando intensamente aos estudos técnicos:

- 💻 **Tecnologia da Informação (TI)** – *Há 8 meses*
- 🇺🇸 **Inglês** – *Há 8 meses*

---

## 🛠️ Tecnologias & Interesses

<p left>
  <img src="https://img.shields.io/badge/Logic-L%C3%B3gica%20de%20Programa%C3%A7%C3%A3o-informational?style=flat-square&logo=github" />
  <img src="https://img.shields.io/badge/GameDev-Desenvolvimento%20de%20Jogos-orange?style=flat-square&logo=unity" />
  <img src="https://img.shields.io/badge/English-Em%20Aprendizado-blue?style=flat-square" />
</p>

---

## 📫 Contato

- ✉️ **E-mail:** [Seu E-mail Aqui]
- 💼 **LinkedIn:** [Seu Link do LinkedIn Aqui]

---
*“Determinado a aprender diariamente e pronto para contribuir com o crescimento de grandes equipes.”*
