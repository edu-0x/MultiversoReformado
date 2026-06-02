# 🌌 Multiverso Nerd - Organização de Dados

## 📖 Sobre o Projeto

O Multiverso Nerd entrou em colapso e todos os personagens foram armazenados em uma base de dados desorganizada.

Este projeto tem como objetivo organizar esses dados, aplicando técnicas de **higienização** e **normalização** utilizando MongoDB.

---

## 🎯 Objetivo

- Limpar dados inconsistentes
- Padronizar informações
- Organizar a base em coleções estruturadas

---

## 📂 Problemas Encontrados

A base de dados apresentava:

- Duplicidade de personagens (ex: Batman e Bat Man)
- Tipos de dados inconsistentes (string e número)
- Valores nulos ou "N/A"
- Campos despadronizados
- Dados incompletos

---

## 🧹 Etapa 1 — Higienização de Dados

Foi criada uma nova coleção com dados limpos:
```js
db.nerd_universe_clean
```

✅ Processos realizados:

- Padronização de nomes de campos
- Correção de maiúsculas e minúsculas
- Remoção de espaços extras
- Conversão de tipos de dados
- Tratamento de valores nulos
- Remoção de duplicidades
- Limpeza de valores inválidos

---

## 📤 Exportação
```json
mongoexport --collection=nerd_universe_clean --out=nerd_universe_clean.json --jsonArray
```
---

## 🧱 Etapa 2 — Normalização
Os dados foram organizados nas seguintes coleções:

- 👤 characters → informações principais
- 🌌 universes → universos dos personagens
- 🧬 species → espécies
- ⚙️ equipment → equipamentos
- 🎬 movies → filmes/séries

## 🚀 Tecnologias Utilizadas

- MongoDB
- JavaScript (Mongo Shell)
- JSON
---

## 📁 Entregáveis

- Arquivo: nerd_universe_clean.json
- Scripts de higienização
- Scripts de normalização
---

## ✅ Resultado Final
A base de dados foi:

- Limpa ✅
- Padronizada ✅
- Estruturada ✅

O multiverso está organizado novamente! 🌌✨
  
  

