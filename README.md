# 💬 Chat WebSocket em Go

Este é um simples servidor de **chat em tempo real** utilizando **WebSocket com Golang**. O objetivo é demonstrar uma implementação básica de comunicação bidirecional entre clientes e servidor usando o pacote [`gorilla/websocket`](https://github.com/gorilla/websocket)

---

## 🚀 Funcionalidades

- Comunicação em tempo real via WebSocket
- Servidor HTTP simples embutido (`net/http`)
- Broadcast de mensagens para todos os clientes conectados
- Interface web mínima em HTML/JS

---

## 🧠 Conceitos utilizados

- WebSocket (`Upgrade` de HTTP para WS)
- Conexões simultâneas com `map[*websocket.Conn]bool`
- Canal (`chan`) para envio de mensagens
- Servidor HTTP servindo arquivos estáticos e rota `/ws` para conexão WebSocket

---

## 📁 Estrutura do Projeto

```

chat\_websocket\_golang/
├── main.go          # Código principal do servidor WebSocket
└── index.html       # Interface web simples para testes

````

---

## ⚙️ Como rodar

### 1. Clone o projeto

```bash
git clone https://github.com/seu-usuario/chat_websocket_golang.git
cd chat_websocket_golang
````

### 2. Inicie o módulo Go e instale dependências

```bash
go mod init chat_websocket_golang
go get github.com/gorilla/websocket
```

### 3. Execute o servidor

```bash
go run main.go
```

O servidor estará disponível em:
📍 `http://localhost:8081`

---

## 🧪 Testando

Abra o arquivo `index.html` no navegador ou acesse diretamente se ele estiver na mesma pasta do `main.go`.

Você pode abrir em múltiplas abas ou janelas para simular múltiplos usuários trocando mensagens em tempo real.

---

## 🛠️ Requisitos

* Go 1.16 ou superior
* Navegador moderno (para suporte ao WebSocket)

---

## 📦 Dependência principal

* [`github.com/gorilla/websocket`](https://github.com/gorilla/websocket) – biblioteca robusta para WebSocket no Go.

---

## 🙋‍♂️ Autor

Feito com 💻 por **João Paulo**
Se quiser contribuir ou melhorar este exemplo, pull requests são bem-vindos!
