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

## Instalando as dependências do projeto

Dentro da pasta do projeto (onde está o `package.json`), rode no terminal:

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


![Card do Last.Month](assets/screenshot.png)
