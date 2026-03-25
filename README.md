
# 🚐 MRL Log — Controle de Saídas

> Sistema de controle de entregas e saídas para transportadoras, com autenticação, relatórios e integração com WhatsApp.

---

## 📋 Sobre o Projeto

O **MRL Log** é uma aplicação web progressiva (PWA) desenvolvida para gerenciar saídas e entregas de motoristas. Permite registrar, filtrar e exportar dados de saídas por motorista, loja, período e peso, com geração de relatórios em PDF, Excel e envio via WhatsApp.

---

## ✨ Funcionalidades

- 🔐 **Autenticação** via Firebase (email e senha)
- ➕ **Cadastro de saídas** com motorista, loja, valor, peso, NFs e data
- 🔍 **Filtros** por período, motorista e loja
- 📊 **Gráficos** de saídas, peso e lucro por motorista
- 📄 **Exportação em PDF** com resumo do período
- 📊 **Exportação em Excel** (.xlsx)
- 💬 **Envio de relatório via WhatsApp**
- 🤖 **IA de Voz** para preenchimento por fala (`vozIA.js`)
- 💬 **Chat com cliente** (`chatcliente.html`)
- 📱 **PWA** — instalável no celular como app nativo

---

## 🛠️ Tecnologias

| Tecnologia | Uso |
|---|---|
| HTML / CSS / JavaScript | Frontend (sem framework) |
| Firebase Firestore | Banco de dados em tempo real |
| Firebase Authentication | Login e controle de acesso |
| jsPDF + AutoTable | Geração de PDF |
| SheetJS (XLSX) | Exportação para Excel |
| Chart.js | Gráficos de desempenho |
| Font Awesome | Ícones |
| Google Fonts (Orbitron, Rajdhani) | Tipografia |

---

## 📁 Estrutura de Arquivos

```
/
├── index.html          # Página principal
├── script.js           # Lógica principal + Firebase
├── styles.css          # Estilo principal (tema ArcaneOS)
├── vozIA.js            # IA de voz
├── chatcliente.html    # Chat com clientes
├── scriptChat.js       # Lógica do chat
├── stylesChat.css      # Estilo do chat
├── service-worker.js   # PWA - cache offline
├── manifest.json       # PWA - configuração do app
├── favicon.svg         # Ícone do site
└── icons/              # Ícones para PWA (192x192, 512x512)
```

---

## 🚀 Como Usar

1. Acesse o link do projeto pelo navegador
2. Faça login com seu email e senha cadastrados
3. Preencha os dados da saída e clique em **Adicionar Saída**
4. Use os filtros para buscar por período, motorista ou loja
5. Exporte os dados pelo menu flutuante (**+**) no canto inferior direito

---

## 🔒 Segurança

- API Key do Firebase protegida por **restrição de domínio** no Google Cloud Console
- Regras do Firestore exigem autenticação (`request.auth != null`)
- Nenhum dado é acessível sem login

---

## 📱 Instalação como App (PWA)

No celular, ao acessar o site pelo Chrome ou Safari, toque em **"Adicionar à tela inicial"** para instalar o MRL Log como um aplicativo nativo, com ícone e tela de abertura.

---

## 👤 Autor

Desenvolvido por **Leandro** — [@leandrocirilojs](https://github.com/leandrocirilojs)
