# Last.Month

Servidor Express que serve o card do Last.Month e gera downloads do card em PNG (usando Puppeteer).

## Pré-requisitos

- [Node.js](https://nodejs.org/) (recomendado: versão 18 ou superior, LTS)
- npm (já vem junto com o Node.js)

## Instalando o Node.js

### Windows

1. Acesse [nodejs.org](https://nodejs.org/) e baixe o instalador **LTS**.
2. Execute o instalador baixado e siga os passos (Next, Next, Finish), mantendo as opções padrão.
3. Abra o **Prompt de Comando** (ou PowerShell) e confirme a instalação:
   ```
   node -v
   npm -v
   ```
   Se aparecerem os números das versões, deu certo.

### macOS

1. Acesse [nodejs.org](https://nodejs.org/) e baixe o instalador **LTS** para macOS.
2. Execute o `.pkg` baixado e siga os passos.
3. Abra o **Terminal** e confirme:
   ```
   node -v
   npm -v
   ```

   Alternativa via [Homebrew](https://brew.sh/):
   ```
   brew install node
   ```

### Linux (Ubuntu/Debian)

```
curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash -
sudo apt-get install -y nodejs
```

Confirme a instalação:
```
node -v
npm -v
```

## Instalando as dependências do projeto

Dentro da pasta do projeto (onde está o `package.json`), rode:

```
npm install
```

Isso vai instalar o `express` e o `puppeteer` (o Puppeteer baixa também uma versão do Chromium, então essa etapa pode demorar um pouco).

## Iniciando o servidor

```
npm start
```

O terminal vai mostrar:

```
Servidor rodando em http://localhost:3000
```

Basta abrir esse endereço no navegador.

> Quer usar outra porta? Defina a variável de ambiente `PORT` antes de iniciar, por exemplo:
> ```
> PORT=8080 npm start
> ```

## Estrutura do projeto

```
.
├── LastfmCard.html   # Página/card servido pelo Express
├── server.js         # Servidor Express (rotas e geração do PNG)
├── package.json
└── package-lock.json
```

(colocar screenshot do card aqui)
