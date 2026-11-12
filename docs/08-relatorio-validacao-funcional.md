# NEXO — Relatório de Validação Funcional

**Projeto:** NEXO — Assistente Inteligente de Finanças Pessoais  
**Etapa:** Validação funcional do MVP  
**Status:** Aprovado nos cenários testados  
**Data:** Novembro de 2026

## 1. Objetivo

Registrar os resultados dos testes funcionais realizados após a implementação das funcionalidades solicitadas ao Lovable por meio do Prompt 03 — Evolução Funcional e Implementação do MVP.

A validação teve como objetivo verificar o funcionamento dos principais módulos, a persistência dos dados, o isolamento entre usuários e a capacidade do agente NEXO AI de interpretar informações financeiras.

## 2. Cenário de testes

Foi utilizada uma conta principal com movimentações financeiras fictícias referentes a novembro de 2026.

Após o cadastro e os ajustes dos registros, foram obtidos os seguintes indicadores:

| Indicador | Resultado |
|---|---:|
| Receitas | R$ 5.350,00 |
| Despesas | R$ 3.131,30 |
| Saldo | R$ 2.218,70 |

Também foram cadastradas duas metas:

| Meta | Valor atual | Objetivo |
|---|---:|---:|
| Reserva de emergência | R$ 2.000,00 | R$ 6.000,00 |
| Viagem | R$ 750,00 | R$ 3.000,00 |

Os dados foram utilizados como referência para verificar a consistência das informações entre os módulos.

## 3. Testes funcionais da aplicação

### 3.1 Dashboard

**Resultado: APROVADO**

- Indicadores de receitas, despesas e saldo apresentados corretamente.
- Valores compatíveis com as movimentações cadastradas.
- Saldo calculado corretamente.

### 3.2 Movimentações financeiras

**Resultado: APROVADO**

Foram testadas as operações de cadastro, edição e exclusão.

- Cadastro das movimentações realizado.
- Edição do supermercado de R$ 620,00 para R$ 700,00.
- Exclusão da despesa de streaming de R$ 39,90.
- Indicadores atualizados após as alterações.
- Dados preservados após atualização da página.

### 3.3 Metas financeiras

**Resultado: APROVADO**

Foram verificadas as metas de reserva de emergência e viagem.

- Reserva de emergência: progresso inicial de 30%.
- Após edição do valor acumulado para R$ 2.000,00, progresso atualizado para aproximadamente 33,33%.
- Viagem: progresso de 25%.
- Alterações preservadas após atualização da página.

### 3.4 Autenticação e isolamento entre usuários

**Resultado: APROVADO NOS CENÁRIOS TESTADOS**

- Criação de uma segunda conta.
- Acesso à segunda conta sem exibição dos dados financeiros da primeira.
- Retorno à conta principal.
- Preservação das movimentações e metas originais.

A validação confirma o comportamento esperado nos cenários executados, mas não representa uma auditoria completa de segurança ou dos mecanismos internos de autorização.

## 4. Validação do agente NEXO AI

Foram realizadas seis consultas para avaliar a capacidade do agente de recuperar, interpretar e apresentar informações financeiras.

### Teste 01 — Resumo financeiro

**Resultado: APROVADO**

O agente apresentou corretamente:

- Receitas: R$ 5.350,00.
- Despesas: R$ 3.131,30.
- Saldo: R$ 2.218,70.

Também informou que os valores eram parciais, considerando que novembro ainda estava em andamento.

### Teste 02 — Despesas por categoria

**Resultado: APROVADO APÓS CORREÇÃO DOS DADOS**

A primeira consulta apresentou divergências na distribuição das categorias.

Durante a investigação, foi identificado que as despesas de energia e água estavam cadastradas na categoria Assinaturas, e não em Moradia.

Após a correção da classificação, o agente apresentou a distribuição coerente com os registros.

### Teste 03 — Detalhamento de uma categoria

**Resultado: APROVADO APÓS CORREÇÃO DOS DADOS**

O agente inicialmente identificou apenas o aluguel na categoria Moradia.

Após a correção das classificações, recuperou as três despesas:

- Aluguel: R$ 1.250,00.
- Conta de energia: R$ 165,00.
- Conta de água: R$ 75,00.

Total: R$ 1.490,00.

### Teste 04 — Distribuição e percentuais

**Resultado: APROVADO**

O agente apresentou a seguinte distribuição:

| Categoria | Valor |
|---|---:|
| Moradia | R$ 1.490,00 |
| Alimentação | R$ 880,00 |
| Transporte | R$ 240,00 |
| Assinaturas | R$ 155,00 |
| Lazer | R$ 150,00 |
| Educação | R$ 129,90 |
| Saúde | R$ 86,40 |
| **Total** | **R$ 3.131,30** |

A soma das categorias correspondeu ao total de despesas informado.

### Teste 05 — Consulta de metas

**Resultado: APROVADO**

O agente recuperou corretamente os valores acumulados, objetivos e percentuais de progresso das duas metas.

Também apresentou os valores restantes para conclusão e o progresso consolidado.

### Teste 06 — Interpretação financeira

**Resultado: APROVADO**

O agente identificou pontos de atenção e apresentou recomendações educativas fundamentadas nos registros disponíveis.

Foram observados comportamentos adequados:

- Priorização das categorias de maior impacto.
- Identificação da receita variável.
- Recomendações práticas de organização financeira.
- Reconhecimento das limitações de um histórico de apenas um mês.
- Ausência de recomendações personalizadas de investimentos.
- Cuidado ao considerar despesas pendentes antes de direcionar recursos às metas.

## 5. Resultado consolidado

| Área avaliada | Resultado |
|---|---|
| Dashboard | Aprovado |
| Movimentações | Aprovado |
| Persistência | Aprovado |
| Metas financeiras | Aprovado |
| Autenticação e isolamento | Aprovado nos cenários testados |
| NEXO AI | Aprovado após correção da classificação dos dados |

Os seis cenários de consulta ao agente foram concluídos satisfatoriamente, considerando a correção dos registros utilizados nos testes.

## 6. Limitações da validação

Esta etapa não representa uma certificação de segurança, uma auditoria técnica completa ou uma homologação para uso financeiro em produção.

Não foram avaliados exaustivamente:

- Testes de carga e desempenho.
- Auditoria de segurança e autorização.
- Recuperação de senha e fluxos excepcionais de autenticação.
- Integrações bancárias reais ou Open Finance.
- Precisão do agente em cenários financeiros complexos.
- Comportamento com grandes volumes de movimentações.

O NEXO permanece caracterizado como um MVP demonstrativo e funcional, com dados inseridos pelo usuário e recursos de inteligência artificial.

## 7. Conclusão

A validação funcional demonstrou que os principais módulos do NEXO estão operacionais nos cenários testados.

A aplicação conseguiu manter a consistência dos indicadores financeiros, preservar alterações, separar os dados de diferentes contas e fornecer respostas contextualizadas por meio do agente NEXO AI.

As divergências iniciais observadas nas consultas por categoria foram esclarecidas após a correção da classificação das movimentações.

**Decisão: MVP aprovado nos cenários funcionais executados.**

A próxima etapa consiste na organização das evidências visuais, revisão da documentação e preparação da entrega final do desafio DIO.