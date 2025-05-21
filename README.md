# 🚀 Hard-skill-test---LRGE-Systems — Extensão Chrome com Gravação de Áudio

## 🎯 Descrição do Desafio

Desenvolver uma **extensão para Google Chrome** capaz de **gravar simultaneamente o áudio da aba ativa e o áudio do microfone do usuário**.

📥 Ao finalizar a gravação, a extensão deverá gerar e baixar automaticamente o arquivo de áudio mesclado.

---

## ✅ Funcionalidades Obrigatórias

### 🧠 Funcionalidade Principal
- 🔊 Capturar áudio da aba ativa.
- 🎙️ Capturar áudio do microfone.
- 🔗 Mesclar os dois fluxos de áudio.
- 💾 Realizar o download automático do arquivo final gravado (`.wav` ou `.mp3`).

### 🖥️ Interface (Popup da Extensão)
1. Tela de Login
   - Campos: email + senha (funcionalidade mockada).
2. Tela Principal
   - ✅ Botão Iniciar Gravação.
   - ⏹️ Botão Parar Gravação.
   - 🔄 Status da gravação.

---

## ⚙️ Requisitos Técnicos

- ✅ JavaScript ou TypeScript (**Diferencial:** React + TypeScript).
- ✅ Uso das APIs nativas do Chrome.
- ✅ Processamento e mesclagem dos áudios usando `WebAudioAPI` ou `AudioContext`.
- ✅ Download automático do áudio gerado.
- ✅ Interface limpa, responsiva e funcional.
- ✅ Compatível com Manifest V3.

---

## 📦 Estrutura Sugerida

```
chrome-extension/
├── manifest.json
├── public/
│   └── icons/
├── popup/ (React app)
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── App.tsx
│   │   ├── index.tsx
│   │   └── styles/
│   └── dist/ (build)
├── background/
│   ├── background.ts
├── scripts/
│   ├── recorder.ts
├── README.md
```

---

## 🐳 Diferenciais

- ✅ React + TypeScript no popup.
- ✅ Organização modular de componentes.
- ✅ Build otimizado com Vite, CRA ou Next.js (modo export).
- ✅ Layout com TailwindCSS, Shadcn/UI, ou ChakraUI.
- ✅ Controle de estados com Zustand, Redux ou Context API.

---

## 🚀 Fluxo de Funcionamento

**1. Abrir popup da extensão**  
⬇️  
**2. Tela de Login (simulada, sem autenticação real)**  
⬇️  
**3. Tela principal com botão de Gravar/Parar**  
⬇️  
**4. Ao iniciar:** Captura simultânea de áudio da aba + microfone  
⬇️  
**5. Ao parar:** Mescla dos dois áudios  
⬇️  
**6. Geração do arquivo de áudio (.wav ou .mp3)**  
⬇️  
**7. Download automático no navegador**

---

## 🏗️ Requisitos de Entrega

- ✅ Código-fonte.
- ✅ README com:
  - Instruções de build (`yarn build` ou `npm run build`).
  - Como carregar a extensão no Chrome (`chrome://extensions` → Load unpacked).
- ✅ Print ou GIF de demonstração (opcional, valorizado).

---

## 🔥 Critérios de Avaliação

| Critério               | Peso |
|------------------------|------|
| Funcionalidade completa| ⭐⭐⭐⭐ |
| Uso correto das APIs    | ⭐⭐⭐⭐ |
| Código organizado       | ⭐⭐⭐  |
| Uso de React + TS       | ⭐⭐⭐⭐ (Diferencial) |
| UX/UI popup             | ⭐⭐  |
| Tratamento de erros     | ⭐⭐  |
| Documentação            | ⭐⭐⭐ |

---

## 📜 Observações

- 🚫 Não é permitido usar bibliotecas prontas para gravação de abas (como extensions externas ou APIs pagas).
- ✅ A mesclagem dos dois fluxos de áudio (**aba + microfone**) deve ser feita manualmente usando as APIs do browser.
- ✔️ O áudio final deve ser entregue em formato `.wav` ou `.mp3` via **download automático**.

---

## ✨ Boa Sorte 🚀
