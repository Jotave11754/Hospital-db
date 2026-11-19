# Consultas SQL – Banco de Dados Hospitalar

Trabalho prático com **10 consultas SQL** sobre um banco de dados hospitalar. Os exercícios exploram funções de agregação (`SUM`, `AVG`, `COUNT`), agrupamento (`GROUP BY`), filtros (`WHERE`, `LIKE`, `IN`) e junções (`JOIN`) entre as tabelas do domínio: convênios, consultas, especialidades, médicos, pacientes, internações (diárias e quartos) e prescrições de medicamentos.

## Objetivo

Responder a situações-problema de diferentes setores do hospital (financeiro, coordenação clínica, infraestrutura, diretoria, cobrança, farmácia, auditoria, regulação e atendimento) por meio de consultas SQL.

## Conceitos praticados

- Funções de agregação: `SUM`, `AVG`, `COUNT`
- Agrupamento com `GROUP BY` (um ou mais campos)
- Filtros com `WHERE`, `LIKE` e `IN`
- Junções (`INNER JOIN`) entre múltiplas tabelas
- Filtros por padrão de texto (início, meio e fim de string)

## Exercícios

### 1. Faturamento total de consultas por convênio
**Setor:** Financeiro
Levantar o valor total arrecadado em consultas para os convênios que possuem **"Saúde"** no nome, acompanhando o faturamento por parceiro.

### 2. Média do valor de consulta por especialidade médica
**Setor:** Coordenação clínica
Calcular a média do valor das consultas realizadas apenas nas especialidades ligadas à **Cardiologia**.

### 3. Valor médio das diárias por tipo de quarto
**Setor:** Gerência de infraestrutura hospitalar
Analisar o valor médio da diária praticado nas internações em acomodações do tipo **"Apartamento"** ou **"UTI"**.

### 4. Total de consultas realizadas por médico
**Setor:** Diretoria de atendimento
Listar o nome dos médicos e a soma total dos valores de suas consultas, considerando apenas consultas com status **"Realizada"** ou **"Finalizada"**.

### 5. Soma de diárias por paciente com sobrenome "Silva"
**Setor:** Cobrança
Identificar a soma acumulada do valor das diárias de internação de todos os pacientes com sobrenome **"Silva"**.

### 6. Contagem de prescrições por status da consulta
**Setor:** Farmácia hospitalar
Obter a quantidade total de medicamentos prescritos, agrupada pelo status da consulta correspondente, considerando apenas prescrições de **"Dipirona"** ou **"Paracetamol"**.

### 7. Média de valor de consultas por convênio e especialidade
**Setor:** Auditoria
Em negociação contratual, saber o valor médio pago por consulta cruzando os convênios que contêm **"Unimed"** com a especialidade do médico.

### 8. Média de diária de internação por convênio em quartos de UTI
**Setor:** Regulação hospitalar
Calcular o valor médio gasto em diárias de internação, agrupado por convênio, considerando unicamente quartos classificados como **"UTI"**.

### 9. Medicamentos prescritos por médico em consultas realizadas
**Setor:** Comissão de farmácia e terapêutica
Descobrir a quantidade total de itens prescritos por médico nas consultas marcadas como **"Realizada"**.

### 10. Valor total e média de consultas por paciente
**Setor:** Atendimento ao cliente
Gerar um extrato financeiro simples com a soma e a média dos valores gastos em consultas por pacientes cujo nome começa com a letra **"M"**.

## Estrutura do repositório

```
.
├── README.md
└── consultas.sql   # scripts das 10 consultas
```

## Como executar

1. Abra o seu cliente SQL (por exemplo, MySQL Workbench).
2. Crie e popule o banco de dados do hospital.
3. Execute o arquivo `consultas.sql`, ou cada consulta individualmente.
