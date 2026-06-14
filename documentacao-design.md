# 🎨 Documentação de Design – Sprint 2

## Projeto ORIZON

Sistema inteligente de monitoramento de segurança industrial utilizando Visão Computacional para detecção de EPIs, geração de ocorrências e apoio à tomada de decisão através de dashboards gerenciais.

---

# 📑 Sumário

* [1. Mapa de Telas](#1-mapa-de-telas)
* [2. Descrição das Telas](#2-descrição-das-telas)
* [3. Decisões de UX](#3-decisões-de-ux)
* [4. Mapeamento entre Telas e Casos de Uso](#4-mapeamento-entre-telas-e-casos-de-uso)
* [5. Considerações Finais](#5-considerações-finais)

---

# 1. Mapa de Telas

O sistema possui dois perfis de acesso: **Técnico de Segurança** e **Supervisor**.

```text
Login
│
├── Telas Técnico
│   ├── Painel Técnico
│   ├── Cadastro de EPI
│   ├── Config de Máquina
│   └── Alertas
│
└── Telas Supervisor
    ├── Painel Supervisor
    └── Relatórios
```

---

# 2. Descrição das Telas

## 🔐 Tela de Login

### Objetivo

Permitir a autenticação dos usuários no sistema.

### Funcionalidades

* Login por e-mail
* Login por senha
* Redirecionamento conforme perfil

### Protótipo

<img width="1702" height="1433" alt="Painel Técnico" src="https://github.com/user-attachments/assets/e26fdd8c-4102-468d-a7f5-28f40bdb6223" />

---

## 👷 Painel Técnico de Segurança

### Objetivo

Centralizar as funcionalidades operacionais do sistema.

### Funcionalidades

* Gerenciar EPIs
* Gerenciar Máquinas
* Gerenciar Alertas

### Protótipo

<img width="1440" height="1433" alt="Image" src="https://github.com/user-attachments/assets/58767cd1-ece0-4626-a795-cd04053dc89d" />

---

## 🦺 Cadastro de EPI

### Objetivo

Cadastrar e manter os Equipamentos de Proteção Individual monitorados pelo sistema.

### Funcionalidades

* Cadastro de novos EPIs
* Atualização de EPIs
* Consulta de EPIs cadastrados

### Protótipo

<img width="1440" height="1238" alt="Image" src="https://github.com/user-attachments/assets/1b628210-6d9c-41a6-b8c8-f0e9e4ccc9ab" />

---

## ⚙️ Cadastro de Máquina

### Objetivo

Cadastrar máquinas e definir os EPIs obrigatórios para cada área monitorada.

### Funcionalidades

* Cadastro de máquinas
* Associação de EPIs obrigatórios
* Definição de áreas monitoradas

### Protótipo

<img width="1440" height="1473" alt="Image" src="https://github.com/user-attachments/assets/c28cff22-fa1f-4e91-b932-2716581a6fda" />

---

## 🚨 Alertas

### Objetivo

Apresentar ocorrências identificadas automaticamente pela visão computacional.

### Funcionalidades

* Consulta de alertas
* Acompanhamento de infrações

### Protótipo

<img width="1440" height="991" alt="Image" src="https://github.com/user-attachments/assets/0be9aac3-ca27-4ea7-a1c7-a5fdf8898d4a" />

---

## 📊 Painel Supervisor

### Objetivo

Disponibilizar indicadores e métricas para acompanhamento da segurança industrial.

### Funcionalidades

* Visualização de dashboards
* Indicadores de ocorrências
* Funcionários com infrações

### Protótipo

<img width="1440" height="1524" alt="Image" src="https://github.com/user-attachments/assets/beef8968-e5a2-4ea9-a88e-71a04e7d26d0" />

---

## 📈 Relatórios

### Objetivo

Gerar relatórios de conformidade para apoio à tomada de decisão.

### Funcionalidades

* Filtro por período
* Filtro por setor
* Consolidação de ocorrências

### Protótipo

<img width="1440" height="1524" alt="Image" src="https://github.com/user-attachments/assets/b049606f-3f27-41d8-a933-2b248f3c24a5" />

---

# 3. Decisões de UX

A interface foi desenvolvida com foco em simplicidade, usabilidade e rápida visualização das informações críticas.

Foi adotada uma identidade visual moderna com cores escuras e elementos de destaque para alertas e indicadores de risco, facilitando a identificação de situações críticas no ambiente industrial.

A navegação foi segmentada por perfil de usuário para garantir que cada ator tenha acesso apenas às funcionalidades relacionadas às suas responsabilidades.

Os dashboards utilizam cards, tabelas e gráficos para facilitar a interpretação dos dados e apoiar a tomada de decisão.

---

# 4. Mapeamento entre Telas e Casos de Uso

| ID   | Caso de Uso                          | Tela                               |
| ---- | ------------------------------------ | ---------------------------------- |
| UC01 | Realizar Login                       | Login                              |
| UC02 | Cadastrar Máquina                    | Cadastro de Máquina                |
| UC03 | Cadastrar EPI                        | Cadastro de EPI                    |
| UC04 | Definir EPIs por Máquina             | Cadastro de Máquina                |
| UC05 | Configurar Áreas Monitoradas         | Cadastro de Máquina                |
| UC06 | Consultar Ocorrências                | Painel Técnico / Painel Supervisor |
| UC07 | Gerenciar Alertas                    | Alertas                            |
| UC08 | Visualizar Dashboard                 | Painel Supervisor                  |
| UC09 | Visualizar Relatórios                | Relatórios                         |
| UC10 | Consultar Funcionários com Infrações | Painel Supervisor/ Alertas         |

---

# 5. Considerações Finais

O protótipo foi desenvolvido para representar as principais funcionalidades do sistema ORIZON, mantendo alinhamento com os requisitos levantados, diagramas UML e casos de uso definidos na Sprint 1.

A proposta busca demonstrar a viabilidade de uma solução de segurança industrial baseada em Visão Computacional, capaz de identificar irregularidades relacionadas ao uso de EPIs, registrar ocorrências automaticamente e fornecer informações estratégicas para supervisão e tomada de decisão.

