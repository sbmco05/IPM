# Grupo 8

* Aluno1: Juliana Silva
* Aluno2: Sofia Couto
* Aluno3: Soraia Pereira

## Como correr o projeto

O projeto está dividido em duas partes:

- **backend/**: contém os ficheiros de dados em CSV/JSON e o script para gerar a base consolidada;
- **projeto/**: contém a aplicação web em Vue + Vite.

### 1. Requisitos

- **Node.js** 20.19 ou superior;
- **npm**;
- **Python 3** (apenas se quiser regenerar o ficheiro de dados do backend).

### 2. Instalar dependências da aplicação

Entrar na pasta do frontend e instalar os pacotes:

```bash
cd projeto
npm install
```

### 3. Executar a aplicação em modo de desenvolvimento

```bash
npm run dev
```

Depois, abrir o endereço mostrado no terminal, normalmente:

```bash
http://localhost:5173
```

### 4. Gerar build para produção

```bash
npm run build
```

Para pré-visualizar o build gerado:

```bash
npm run preview
```

### 5. Recriar os dados do backend, se necessário

Se for preciso regenerar o ficheiro `db.json` a partir dos dados em `backend/db/`, executar:

```bash
cd backend
python3 build_jsondb.py db
```

Isto cria ou atualiza o ficheiro `db.json` com base nos dados existentes na pasta `db/`.
