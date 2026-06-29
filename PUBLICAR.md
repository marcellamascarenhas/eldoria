# Como Publicar — GitHub e itch.io

## 📦 Estrutura que você precisa ter localmente

```
eldoria/
├── eldoria.py
├── README.md
├── ASSETS.md
├── CHANGELOG.md
├── LICENSE
├── requirements.txt
├── .gitignore
├── NewRocker-Regular.ttf
├── Capa_Eldoria.jpeg
│
├── [todos os .png dos sprites, estruturas e itens]
└── [todos os .mp3 de áudio — opcionais]
```

---

## 🐙 Publicar no GitHub

### 1. Criar o repositório

1. Acesse [github.com](https://github.com) e faça login
2. Clique em **"New repository"**
3. Preencha:
   - **Repository name:** `eldoria`
   - **Description:** `Jogo de estratégia por turnos em Python + Pygame`
   - Marque **Public**
   - **NÃO** marque "Add a README" (você já tem um)
4. Clique em **"Create repository"**

### 2. Subir os arquivos

```bash
# Na pasta do projeto:
git init
git add .
git commit -m "feat: versão inicial de Eldoria"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/eldoria.git
git push -u origin main
```

### 3. Configurar o repositório (opcional mas recomendado)

- **Topics:** `python`, `pygame`, `game`, `strategy`, `turn-based`, `rpg`
- **About → Website:** cole o link do itch.io após publicar lá
- Adicione uma **screenshot** como Social Preview em *Settings → Social preview*

---

## 🎮 Publicar no itch.io

### 1. Preparar o arquivo para download

Crie um `.zip` com **todos** os arquivos do projeto:

```bash
# Windows (PowerShell):
Compress-Archive -Path eldoria\* -DestinationPath eldoria_v1.0.zip

# macOS / Linux:
zip -r eldoria_v1.0.zip eldoria/
```

O `.zip` deve conter diretamente `eldoria.py` (sem subpasta extra dentro).

### 2. Criar a página no itch.io

1. Acesse [itch.io](https://itch.io) e faça login
2. Clique em **"Upload new project"**
3. Preencha os campos:

   | Campo | Valor sugerido |
   |-------|---------------|
   | **Title** | Eldoria |
   | **Project URL** | `eldoria-game` |
   | **Kind of project** | Downloadable |
   | **Classification** | Games |
   | **Genre** | Strategy |
   | **Tags** | python, pygame, turn-based, strategy, fantasy, rpg |

4. Em **Uploads**, clique em **"Upload files"** e suba o `eldoria_v1.0.zip`
   - Marque **"This file is for Windows"** E **"This file is for Linux"** E **"This file is for macOS"** (é Python, roda em todos)

5. Em **Description**, cole o conteúdo de `docs/descricao_itchio.txt`

6. Em **Screenshots**, suba pelo menos 2–3 capturas de tela do jogo

7. Em **Cover image**, suba a `Capa_Eldoria.jpeg`

8. **Pricing:** marque *"No payments"* ou *"Pay what you want"* (com preço mínimo 0)

9. Clique em **"Save & view page"** para revisar, depois **"Publish"**

### 3. Adicionar instruções de instalação na página

Na descrição do itch.io, adicione uma seção clara:

```
📥 COMO INSTALAR

1. Baixe e extraia o arquivo .zip
2. Instale Python 3.8+ em python.org
3. Instale o Pygame: abra o terminal e digite:
      pip install pygame
4. Execute: python eldoria.py
```

---

## ✅ Checklist final

### GitHub
- [ ] `README.md` com capturas de tela
- [ ] `LICENSE` incluída
- [ ] `.gitignore` configurado
- [ ] `requirements.txt` presente
- [ ] Topics e descrição preenchidos

### itch.io
- [ ] Capa / cover image carregada
- [ ] Screenshots (mínimo 2)
- [ ] Descrição completa com controles
- [ ] Instruções de instalação visíveis
- [ ] Tags preenchidas
- [ ] Arquivo `.zip` testado antes de subir (rode o jogo pelo zip para confirmar)
