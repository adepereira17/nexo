# NEXO — Experiência do Usuário (UX/UI) e Fluxo de Navegação

**Projeto:** NEXO  
**Documento:** 04 — UX/UI e Experiência do Usuário  
**Versão:** 1.0  
**Status:** Planejamento  
**Plataforma:** Aplicação web responsiva

---

## 1. Objetivo

Definir a experiência de utilização, a arquitetura de navegação, a organização das telas e as diretrizes visuais do NEXO.

Este documento servirá como referência para a construção do protótipo no Lovable.

O objetivo é garantir uma experiência consistente, acessível e funcional, alinhada à proposta de inteligência financeira pessoal.

## 2. Diretrizes de experiência

A experiência deverá seguir os seguintes princípios:

### 2.1. Clareza

Informações financeiras devem ser apresentadas de maneira objetiva, com hierarquia visual e linguagem acessível.

### 2.2. Simplicidade

As principais operações devem exigir poucos passos, evitando formulários e navegação desnecessariamente complexos.

### 2.3. Contextualização

O usuário deve compreender o significado dos indicadores apresentados.

### 2.4. Consistência

Componentes, cores, tipografia, ícones e padrões de interação devem seguir um sistema visual uniforme.

### 2.5. Inteligência integrada

O agente NEXO AI deverá estar acessível durante a experiência, sem substituir a navegação tradicional.

### 2.6. Responsividade

A experiência deverá se adaptar a diferentes resoluções, priorizando desktop e oferecendo excelente utilização em smartphones.

## 3. Identidade visual

### 3.1. Conceito

A identidade visual deverá transmitir tecnologia, inteligência, confiança e modernidade.

O produto não deve parecer um banco tradicional nem uma plataforma de investimentos especulativos.

### 3.2. Paleta de cores

| Elemento   | Cor     | Aplicação                           |
| ---------- | ------- | ----------------------------------- |
| Primary    | #111827 | Fundo escuro e elementos principais |
| Secondary  | #252B3B | Superfícies secundárias             |
| Accent     | #8B5CF6 | Inteligência artificial e destaques |
| Success    | #A3E635 | Progresso e resultados positivos    |
| Background | #F8FAFC | Fundo claro                         |
| Surface    | #FFFFFF | Cards e componentes                 |
| Text       | #1F2937 | Textos principais                   |
| Muted      | #64748B | Textos secundários                  |
| Danger     | #EF4444 | Alertas e situações negativas       |

A aplicação deverá priorizar uma interface clara, com possibilidade de evolução para tema escuro.

### 3.3. Tipografia

Utilizar Inter ou Manrope.

Hierarquia:

- Títulos principais: 24–32 px.

- Títulos de seção: 18–22 px.

- Textos principais: 14–16 px.

- Textos auxiliares: 12–14 px.

- Indicadores financeiros: destaque visual conforme importância.

### 3.4. Componentes visuais

- Cards com bordas discretas.

- Cantos arredondados moderados.

- Ícones consistentes.

- Gráficos minimalistas.

- Espaçamento uniforme.

- Botões com hierarquia clara.

- Feedback visual para operações.

## 4. Arquitetura de navegação

A aplicação deverá possuir uma navegação principal composta por:

1. Dashboard.

2. Movimentações.

3. Análises.

4. Metas.

5. NEXO AI.

### Desktop

Utilizar sidebar lateral com identificação do produto e navegação principal.

A área central será reservada ao conteúdo da página.

O cabeçalho deverá apresentar o título da página, período selecionado quando aplicável e ações contextuais.

### Mobile

Substituir a sidebar por uma navegação compacta, utilizando menu inferior ou menu recolhível.

Priorizar o acesso rápido ao dashboard, movimentações e agente financeiro.

## 5. Mapa de telas

### Tela 01 — Dashboard

**Objetivo:** oferecer uma visão geral da situação financeira.

Componentes:

- Saudação e identificação do usuário fictício.

- Seletor de período.

- Card de saldo.

- Card de receitas.

- Card de despesas.

- Gráfico de evolução financeira.

- Gráfico de despesas por categoria.

- Resumo de movimentações recentes.

- Resumo de metas.

- Destaque com análise do NEXO AI.

### Tela 02 — Movimentações

**Objetivo:** gerenciar receitas e despesas.

Componentes:

- Título e descrição da página.

- Botão de nova movimentação.

- Filtros por período.

- Filtros por tipo.

- Filtros por categoria.

- Lista ou tabela de movimentações.

- Identificação visual de receitas e despesas.

- Ações de edição e exclusão.

### Tela 03 — Análises

**Objetivo:** apresentar informações sobre o comportamento financeiro.

Componentes:

- Seletor de período.

- Indicadores financeiros.

- Comparativo entre períodos.

- Gráfico de evolução das despesas.

- Distribuição por categoria.

- Identificação de variações.

- Observações produzidas pelo agente.

- Acesso à análise conversacional.

### Tela 04 — Metas financeiras

**Objetivo:** permitir o acompanhamento de objetivos financeiros.

Componentes:

- Resumo das metas.

- Botão para criar meta.

- Cards individuais.

- Nome e valor desejado.

- Valor acumulado.

- Barra de progresso.

- Percentual de conclusão.

- Prazo.

- Status da meta.

### Tela 05 — NEXO AI

**Objetivo:** disponibilizar uma experiência conversacional de inteligência financeira.

Componentes:

- Identificação do agente.

- Histórico da conversa.

- Área de mensagens.

- Campo de entrada.

- Botão de envio.

- Sugestões de perguntas.

- Indicador de processamento.

- Contexto da análise.

- Mensagens de ausência de dados.

Sugestões iniciais:

- Como estão minhas finanças?

- Onde estou gastando mais?

- Compare meus últimos meses.

- Como estão minhas metas?

- Quais padrões você identificou?

## 6. Fluxos de interação

### 6.1. Consulta ao dashboard

1. Usuário acessa a aplicação.

2. Dashboard apresenta indicadores financeiros.

3. Usuário seleciona o período.

4. Indicadores e gráficos são atualizados.

5. Usuário pode acessar detalhes ou solicitar uma análise ao agente.

### 6.2. Cadastro de movimentação

1. Usuário acessa movimentações.

2. Seleciona nova movimentação.

3. Escolhe receita ou despesa.

4. Informa descrição, valor, data e categoria.

5. Confirma o registro.

6. Sistema apresenta confirmação.

7. Indicadores financeiros são atualizados.

### 6.3. Criação de meta

1. Usuário acessa metas.

2. Seleciona nova meta.

3. Informa nome, valor desejado e prazo.

4. Define o valor inicial acumulado.

5. Confirma a criação.

6. Aplicação apresenta o progresso.

### 6.4. Consulta ao agente

1. Usuário acessa NEXO AI.

2. Seleciona uma pergunta sugerida ou digita sua própria pergunta.

3. Sistema disponibiliza o contexto financeiro.

4. Agente processa os dados.

5. Resposta é apresentada.

6. Usuário pode continuar a conversa.

## 7. Componentes reutilizáveis

A interface deverá utilizar componentes compartilhados para manter consistência.

### Componentes financeiros

- FinancialSummaryCard.

- IncomeExpenseChart.

- CategoryDistributionChart.

- TransactionList.

- TransactionForm.

- GoalCard.

- GoalProgress.

- PeriodSelector.

### Componentes de inteligência artificial

- AIMessage.

- ChatInput.

- ChatMessage.

- SuggestedQuestions.

- AIInsightCard.

- AIProcessingIndicator.

- AIEmptyState.

### Componentes gerais

- Sidebar.

- MobileNavigation.

- PageHeader.

- Modal.

- ConfirmationDialog.

- EmptyState.

- LoadingState.

- ErrorState.

- ToastNotification.

Os nomes são referências conceituais, não exigências de implementação.

## 8. Estados de interface

Todas as telas deverão considerar diferentes estados de utilização.

### 8.1. Estado inicial

Apresentar conteúdo de orientação quando não existirem movimentações.

### 8.2. Estado de carregamento

Utilizar indicadores visuais durante operações e processamento de informações.

### 8.3. Estado vazio

Apresentar mensagens explicativas e ações para iniciar a utilização.

### 8.4. Estado de erro

Informar o problema de maneira compreensível e oferecer possibilidade de recuperação quando aplicável.

### 8.5. Estado de sucesso

Apresentar confirmação após operações realizadas.

### 8.6. Estado sem dados suficientes

O agente deverá explicar por que não consegue produzir determinada análise.

## 9. Responsividade

### Desktop

- Sidebar fixa ou recolhível.

- Dashboard com múltiplas colunas.

- Cards financeiros organizados em grade.

- Gráficos com área adequada.

- Conversação com área confortável de leitura.

### Tablet

- Sidebar compacta ou menu recolhível.

- Cards reorganizados em duas colunas.

- Gráficos adaptáveis.

### Mobile

- Navegação compacta.

- Cards empilhados.

- Gráficos adaptados à largura.

- Formulários com campos acessíveis.

- Conversação otimizada para toque.

- Tabelas substituídas por listas ou cards quando necessário.

## 10. Acessibilidade

- Contraste adequado entre texto e fundo.

- Hierarquia semântica de títulos.

- Rótulos em todos os campos.

- Navegação por teclado.

- Foco visível.

- Botões com áreas de interação adequadas.

- Alternativas textuais para informações importantes.

- Não depender exclusivamente de cores para representar receitas, despesas ou status.

## 11. Diretrizes de interação

- Operações importantes devem solicitar confirmação.

- Exclusões devem possuir confirmação explícita.

- Formulários devem apresentar validação clara.

- Valores devem ser formatados em BRL.

- Alterações devem refletir nos indicadores.

- Filtros devem apresentar o contexto selecionado.

- A navegação deve preservar a compreensão do usuário sobre sua localização no aplicativo.

## 12. Dados visuais de demonstração

O protótipo deverá apresentar dados fictícios, porém coerentes.

Todos os valores exibidos deverão possuir correspondência lógica entre:

- Dashboard.

- Movimentações.

- Análises.

- Metas.

- Respostas do agente.

Não deverão existir indicadores arbitrários ou gráficos sem correspondência com os dados demonstrativos.

## 13. Critérios de aceitação de UX/UI

| Critério       | Resultado esperado                           |
| -------------- | -------------------------------------------- |
| Navegação      | Acesso claro aos cinco módulos               |
| Hierarquia     | Informações organizadas por importância      |
| Consistência   | Componentes visuais uniformes                |
| Responsividade | Adaptação a desktop, tablet e mobile         |
| Acessibilidade | Interações compreensíveis                    |
| Feedback       | Estados de sucesso, erro e carregamento      |
| Inteligência   | Agente integrado à experiência               |
| Coerência      | Informações visuais compatíveis com os dados |

## 14. Diretrizes para construção no Lovable

O Lovable deverá utilizar este documento e o PRD como referências obrigatórias.

As seguintes orientações deverão ser respeitadas:

1. Construir uma aplicação web responsiva.

2. Priorizar o dashboard como página inicial.

3. Implementar navegação entre os cinco módulos.

4. Reutilizar componentes visuais.

5. Manter identidade visual consistente.

6. Utilizar dados fictícios coerentes.

7. Preservar a separação entre cálculos financeiros e inteligência artificial.

8. Implementar estados vazios, carregamento e erro.

9. Evitar elementos decorativos que prejudiquem a usabilidade.

10. Não acrescentar funcionalidades fora do escopo aprovado sem justificativa.

O resultado deverá ser um protótipo navegável que permita demonstrar os principais fluxos do NEXO.

---

**Documento:** 04 — UX/UI e Experiência do Usuário  
**Projeto:** NEXO  
**Versão:** 1.0
