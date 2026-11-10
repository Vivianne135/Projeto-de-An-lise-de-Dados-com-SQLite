# Projeto-de-An-lise-de-Dados-com-SQL

### 📌 Este projeto demonstra a aplicação prática de comandos e consultas em SQL utilizando o SQLite. O objetivo é simular um ambiente de banco de dados corporativo estruturado em tabelas relacionais (clientes, produtos e vendas), explorando desde a extração simples de dados até o cruzamento avançado de informações para suporte à tomada de decisão.

## 🗄️ Arquitetura do Banco de Dados 
O modelo relacional é composto por três entidades principais: 
 
1. **`clientes`**: Armazena informações cadastrais, dados demográficos (idade, localização) e histórico de registo dos consumidores. 
2. **`produtos`**: Contém o catálogo detalhado de itens, com foco em gestão de stock, custos de armazenagem, margens de lucro e fornecedores. 
3. **`vendas` (Tabela Fato):** Regista as transações comerciais diárias, conectando clientes e produtos, detalhando quantidades, preços, faturamento e lucros obtidos

## Durante o desenvolvimento deste projeto, foram aplicadas as seguintes técnicas e comandos SQL:

**SELEÇÃO E FILTRAGEM BASICA:**

Uso do comando SELECT * FROM para explorar bases de dados e aplicação de filtos por estado.

Este print mostra uma interface de gerenciamento de banco de dados uma IDE de SQL rodando em SQLite. Aqui começamos a importar as planilhas, nesse caso iniciamos com a de vendas.
<img width="1360" height="639" alt="sqllite 1" src="https://github.com/user-attachments/assets/6fec64e8-122f-4d6c-9a54-6a11273b713d" />

**PROJEÇÃO E RENOMEAÇÃO DE COLUNAS (AS):**

Nesta etapa do projeto organizamos o resultado das consultas renomeando colunas para uma melhor legibilidade executiva (ex: SELECT id_cliente AS CLIENTE, estado AS ESTADO.
<img width="1361" height="635" alt="sqllite 2" src="https://github.com/user-attachments/assets/59175035-9e29-4ef4-b799-9df52a1f2f87" />


**ORDENAÇÃO E LIMITAÇÃO DE RESULTADOS:**

Ordenação de dados em ordem decrescente utilizando ORDER BY ... DESC e restrição do volume de exibição com LIMIT para identificar rapidamente os maiores volumes de vendas ou os produtos mais movimentados.
<img width="1361" height="631" alt="sqllite 3" src="https://github.com/user-attachments/assets/aae3e616-ad74-46e9-bab1-5ed85100d6eb" />


**FILTRAGEM COM CONDICIONAIS NUMERICOS:**

Utilização de operadores lógicos de comparação (> 100) para auditar produtos com níveis elevados de stock nas prateleiras e armazéns.
<img width="1363" height="634" alt="sqllite 6 filtros" src="https://github.com/user-attachments/assets/796f9fc7-28c1-4305-bc06-3f0f7ba3c8ca" />


**CRUZAMENTO DE TABELAS RELACIONAIS (INNER JOIN):**

Conexão lógica entre a tabela de fatos de vendas e as tabelas dimensionais de produtos e clientes utilizando chaves estrangeiras. Isso permitiu unir dados de transações com informações detalhadas de clientes (como e-mail, celular e idade) e especificações dos produtos comercializados numa única visão analítica.
<img width="1363" height="630" alt="sqllite 7 juntar tabelas" src="https://github.com/user-attachments/assets/801e5b37-8c50-4234-a5a7-b4608c4b7013" />


## O QUE APRENDI COM ESSE PROJETO:

**Gestão e Importação de Dados:**
Capacidade de estruturar e importar bases de dados tabulares para um ambiente de SGBD (SQLite).

**Manipulação e Filtragem de Dados:**
Domínio de comandos fundamentais como SELECT, aplicação de filtros direcionados com WHERE e operadores lógicos de comparação numérica para auditoria de stocks.

**Formatação e Legibilidade de Relatórios:**
Utilização do comando AS (Alias) para renomear colunas e entregar resultados com um layout executivo, limpo e profissional.

**Organização e Performance Analítica:**
Aplicação de ordenações (ORDER BY ... DESC) e limites (LIMIT) para extração rápida de Top Rankings e indicadores comerciais chave.

**Modelagem Relacional Avançada:**
Execução bem-sucedida de cruzamentos entre tabelas utilizando INNER JOIN, conectando chaves estrangeiras para unificar dados transacionais, cadastrais e de inventário numa única visão analítica.

### **CONCLUSÃO:**
Este projeto demonstrou como a linguagem SQL é uma ferramenta indispensável para o Analista de Dados. A habilidade de estruturar tabelas e consultar bases relacionais transforma dados brutos em respostas rápidas e estratégicas, essenciais para a tomada de decisões corporativas em ambientes de e-commerce e varejo.

