# 📖 Bíblia JFA — Gerador de APK

Este repositório compila automaticamente o APK da Bíblia JFA usando GitHub Actions + Capacitor.
O TTS (Leitura em Voz) funciona perfeitamente neste APK.

---

## 🚀 PASSO A PASSO

### 1. Preparar os arquivos da Bíblia

Coloque seus arquivos na pasta `www/`:
- `www/index.html` → renomeie seu `Biblia.html` para `index.html`
- `www/Biblia_data.js` → o arquivo de dados da Bíblia

A pasta `www/` deve ficar assim:
```
www/
  index.html
  Biblia_data.js
```

---

### 2. Fazer upload no GitHub

1. Acesse seu repositório no GitHub
2. Clique em **"Add file" → "Upload files"**
3. Faça upload de TODOS os arquivos e pastas deste projeto
4. Clique em **"Commit changes"**

---

### 3. Aguardar a compilação

1. Clique na aba **"Actions"** no seu repositório
2. Você verá o workflow **"Build APK - Bíblia JFA"** rodando
3. Aguarde cerca de **5 a 10 minutos**
4. Quando aparecer ✅ verde, clique nele

---

### 4. Baixar o APK

1. Na página do workflow concluído, role para baixo
2. Você verá **"Artifacts"** → **"Biblia-JFA-APK"**
3. Clique para baixar o arquivo `.zip`
4. Extraia o `.zip` — dentro estará o `app-debug.apk`
5. Transfira para o celular e instale

> ⚠️ Para instalar: vá em Configurações → Segurança → Permitir fontes desconhecidas

---

## 🔄 Atualizar o app no futuro

Sempre que quiser atualizar:
1. Acesse o repositório no GitHub
2. Vá na pasta `www/`
3. Clique no arquivo que quer atualizar → **"Edit"** ou faça novo upload
4. Commit → GitHub Actions compila automaticamente
5. Baixe o novo APK em Actions → Artifacts

---

## ✅ O que funciona neste APK

- ✅ Leitura em Voz (TTS) — WebSpeech API totalmente suportada
- ✅ Todos os 66 livros offline
- ✅ Destaques, notas, favoritos (localStorage)
- ✅ Plano de leitura 365 dias
- ✅ Busca, referências cruzadas
- ✅ Tema claro/escuro
- ✅ Internet para ResponsiveVoice (voz de qualidade)

---

## ❓ Dúvidas

Se o workflow falhar, verifique:
- A pasta `www/` contém `index.html` e `Biblia_data.js`?
- O upload foi feito corretamente?
