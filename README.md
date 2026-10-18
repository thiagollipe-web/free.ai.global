# FREE.A.I — Hub Global de IAs 100% Gratuitas

[FREE.A.I](https://img.shields.io/badge/FREE.A.I-100%25%20FREE-00E5FF?style=for-the-badge)
[IAs](https://img.shields.io/badge/IAs-73%20mapeadas-A855F7?style=for-the-badge)
[Sem PRO](https://img.shields.io/badge/Sem%20PRO-Sem%20Cartão-00FFC6?style=for-the-badge)
[Licença](https://img.shields.io/badge/License-MIT-white?style=for-the-badge)

> **Só IAs que são 100% FREE de verdade. Zero ChatGPT com limite, zero Claude com banner de upgrade.**

Um hub moderno, flutuante e open-source que reúne **73 inteligências artificiais gratuitas de todo o mundo** — China, EUA, Europa — com logos oficiais, balões explicativos e links diretos.

**🔗 Demo:** Abra o arquivo `index.html` (artefato gerado) no navegador.

---

## ✨ O que é?

O FREE.A.I nasceu da frustração com listas que dizem "grátis" mas mostram "seu limite acabou, assine o PRO". Aqui a regra é clara:

- ✅ **100% FREE** = open-source, sem plano PRO, sem cartão, ilimitado (ex: DeepSeek, Qwen, Kimi, Pollinations, Craiyon)
- ✅ **FREE GENEROSO** = free tier que funciona de verdade sem pedir cartão (ex: Leonardo 150/dia, Runway créditos mensais)

Excluímos propositalmente: ChatGPT, Claude, Gemini, Copilot e similares que bloqueiam após poucas mensagens.

## 🌍 Varredura Global

| Região | Quantidade | Exemplos |
| :--- | :--- | :--- |
| 🇨🇳 China | 9 | DeepSeek, Qwen3, Kimi 200k, GLM-4.5, Doubao (ByteDance), Yuanbao (Tencent), Minimax, Yi, InternLM |
| 🇺🇸 EUA | 35+ | Meta AI Llama 3.3, Groq 800 tok/s, Venice privado, Duck.ai anônimo, HuggingChat, CapCut, Pollinations |
| 🇪🇺 Europa | 3 | Mistral Le Chat (FR), etc |
| 🌐 Open World | 26 | Craiyon, Raphael, Flux, Stable Diffusion, etc |

**Total: 73 IAs verificadas em Outubro 2026**

## 📂 Categorias

- 💬 **CHAT GERAL MUNDO (20)** - Chatbots para conversa, raciocínio e pesquisa
- 💻 **CÓDIGO & DEV (12)** - DeepSeek Coder, Qwen Coder, Blackbox, Phind, Codeium FREE FOREVER, Supermaven, Tabby
- 🎨 **IMAGEM & DESIGN (15)** - Craiyon ilimitado, Pollinations API open, Raphael, Flux Schnell, Mage.space, Dezgo, SeaArt
- 🎬 **VÍDEO & ANIMAÇÃO (10)** - CapCut sem watermark, Stable Video Diffusion, Clipchamp Microsoft, Haiper, PixVerse, Luma, Pika
- 🎧 **ÁUDIO, VOZ E MÚSICA (8)** - TTSMaker 600 vozes ilimitado, MusicGen Meta, Riffusion, Stable Audio, Adobe Enhance
- 📚 **ESTUDO & PESQUISA (8)** - NotebookLM Google, Elicit, Consensus, SciSpace, Grammarly

## 🎨 Design

- **Layout flutuante moderno** com glassmorphism
- **Cores frias vivas:** cyan `#00E5FF`, azul `#5B8DEF`, roxo `#A855F7`, mint `#00FFC6`
- **Fundo:** `#050814` com 4 blobs desfocados animados (float 8s)
- **Logo FREE.A.I:** pill glass, FREE com tracking 0.2em, .A.I com gradiente cyan→roxo
- **Logo-box:** 64x64px, fundo branco, radius 16px, shadow, hover `scale(1.1) + rotate(3deg)`
- **Balões explicativos (?)** com: O que faz, Por que é 100% free, Ideal para, Diferencial, País

## 🚀 Tecnologias

- HTML5 + CSS3 + JavaScript (Vanilla)
- React (build do artefato) + TailwindCSS
- Sem dependências externas (exceto Google Fonts Sora + Inter)
- 100% client-side, sem backend
- Lazy loading + fallback de logos

## 📦 Como usar

### Opção 1: Abrir direto
```bash
# Baixe o index.html do release e abra no navegador
open index.html
```

### Opção 2: Clonar e rodar
```bash
git clone https://github.com/seu-usuario/free-a-i.git
cd free-a-i
# Se for a versão React/TSX
npm install
npm run dev
```

### Opção 3: Deploy no GitHub Pages / Vercel
1. Faça upload do `index.html`
2. Ative GitHub Pages em Settings → Pages → Branch: main
3. Pronto: `seu-usuario.github.io/free-a-i`

## 🔍 Funcionalidades

- [x] Busca em tempo real (nome, descrição, país, finalidade)
- [x] Filtros por categoria + toggle "Só 100% FREE"
- [x] Contador dinâmico "X encontradas de 73"
- [x] 73 cards com logos oficiais (12 locais + 61 favicons)
- [x] Tooltip rico com balão explicativo
- [x] Botão "Acessar agora →" com link direto `_blank`
- [x] Responsivo mobile + desktop
- [x] 0 bugs de script (corrigido console.error override)

## 📊 Exemplo de Card

```json
{
  "nome": "DeepSeek Chat",
  "url": "https://chat.deepseek.com",
  "pais": "🇨🇳 China",
  "badge": "100% FREE",
  "categoria": "CHAT GERAL",
  "desc": "R1 reasoning e V3 ilimitados",
  "oqueFaz": "Chat geral com raciocínio profundo...",
  "porQueFree": "Open-source financiado por hedge fund...",
  "logo": "deepseek.png"
}
```

## 🤝 Contribuir

Encontrou uma IA 100% free que não está na lista? Abra uma PR!

1. Fork o repo
2. Crie branch `feat/nova-ia-nome`
3. Adicione no array `IAS` em `App.tsx`
4. Teste local
5. Abra PR com descrição e link

**Critérios para entrar:**
- Não pedir cartão de crédito no free
- Não ter banner "limite atingido, assine PRO" agressivo
- Ser open-source OU ter free tier realmente utilizável

## 🗺️ Roadmap

- [ ] Adicionar filtro por país
- [ ] Modo claro/escuro
- [ ] Exportar lista em JSON/CSV
- [ ] API pública `/api/ias.json`
- [ ] PWA instalável
- [ ] IAs brasileiras (Maritaca AI, etc)

## 📄 Licença

MIT — pode usar livremente, só mantenha os créditos.

## 🙏 Créditos

Curadoria e design por **Thiago Fillipe Soares** + Meta AI.

Logos são propriedade de seus respectivos donos. Uso apenas para identificação (fair use).

---

### ⭐ Dê uma estrela se esse hub te salvou de pagar PRO à toa!

**FREE.A.I — Porque IA boa não precisa ser paga.**
