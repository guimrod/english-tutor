# English Tutor — Deploy no Cloudflare Pages

## Arquivos do projeto
- `index.html` — app completo
- `sw.js` — service worker (PWA instalável)
- `manifest.json` — configuração do app

---

## Passo a passo (tudo pelo iPhone)

### 1. Criar conta no GitHub
- Acesse **github.com** no Chrome
- Crie uma conta gratuita (se não tiver)

### 2. Criar repositório
- Toque em **"+"** → **"New repository"**
- Nome: `english-tutor`
- Deixe **Public**
- Toque em **"Create repository"**

### 3. Subir os arquivos
No repositório criado, toque em **"uploading an existing file"**:
- Faça upload do `index.html`
- Repita para `sw.js`
- Repita para `manifest.json`
- Cada arquivo: toque em **"Commit changes"**

### 4. Criar conta no Cloudflare Pages
- Acesse **pages.cloudflare.com**
- Crie conta gratuita
- Toque em **"Create a project"**
- Escolha **"Connect to Git"** → autorize o GitHub
- Selecione o repositório `english-tutor`
- Configurações: deixe tudo padrão (não precisa de build command)
- Toque em **"Save and Deploy"**

### 5. Acessar o app
- O Cloudflare vai gerar uma URL tipo `english-tutor-xyz.pages.dev`
- Abra essa URL no **Chrome do iPhone**
- Na primeira vez: coloque sua chave do Groq (de console.groq.com)

### 6. Instalar como app no iPhone
- No Chrome, toque nos **três pontos** (⋮) → **"Adicionar à tela inicial"**
- Pronto — ícone aparece na tela inicial igual um app nativo

---

## Chave do Groq (gratuita)
1. Acesse **console.groq.com**
2. Faça login (Google, GitHub ou email)
3. Vá em **"API Keys"** → **"Create API Key"**
4. Copie a chave (começa com `gsk_...`) e cole no app na primeira abertura

A chave fica salva só no seu iPhone — nunca sai do dispositivo.

Limite gratuito: 30 requisições/minuto, 14.400/dia no modelo Llama 3.3 70B — bem mais generoso que o Gemini free tier.

---

## Recursos do app
- Tutor que conduz a conversa e nunca pede pra você escolher o tema
- Você pode redirecionar: "let's do more of this" / "focus on linking words"
- Modo Imersão de Cena (situações reais)
- Modo Decifra o Nativo (frases como nativos falam)
- Correção integrada + nota curta no final
- Memória entre sessões (erros, temas, nível)
- Progressão A2 → B1 → B2 → C1 → C2
- Revisão espaçada de erros recorrentes
- Microfone (Chrome no iPhone) + texto
- Voz do tutor (botão 🔊 opcional)
