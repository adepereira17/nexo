# 05. MVP, Priorização e Estratégia de Validação

**Projeto:** NEXO — Assistente Inteligente de Finanças Pessoais  
**Versão:** 1.0  
**Status:** Planejamento  
**Objetivo:** Definir o escopo do MVP, priorizar funcionalidades e estabelecer critérios objetivos para validar o protótipo desenvolvido com Vibe Coding.

---

## 1. Objetivo do MVP

O MVP do NEXO deverá demonstrar como uma aplicação de finanças pessoais pode combinar gestão financeira, visualização de dados e inteligência artificial em uma experiência integrada.

O objetivo não é construir uma plataforma financeira de produção, mas apresentar um protótipo interativo que permita avaliar:

- Organização e visualização das finanças pessoais.

- Registro e gerenciamento de movimentações.

- Acompanhamento de metas financeiras.

- Identificação de padrões de receitas e despesas.

- Interação com um assistente financeiro inteligente.

- Coerência entre dados, cálculos e respostas do agente.

O diferencial do produto deverá estar na capacidade de transformar informações financeiras em explicações compreensíveis e orientações educativas.

## 2. Escopo funcional do MVP

As funcionalidades serão divididas em três níveis de prioridade.

### 2.1. Prioridade P0 — Essencial

Funcionalidades indispensáveis para demonstrar a proposta central do NEXO.

| Módulo        | Funcionalidade                                                      |
| ------------- | ------------------------------------------------------------------- |
| Dashboard     | Exibir receitas, despesas e saldo do período.                       |
| Dashboard     | Apresentar gráficos de distribuição de despesas.                    |
| Dashboard     | Exibir evolução financeira e metas em andamento.                    |
| Movimentações | Listar receitas e despesas.                                         |
| Movimentações | Cadastrar movimentações com descrição, valor, data e categoria.     |
| Movimentações | Editar e excluir movimentações demonstrativas.                      |
| Metas         | Exibir metas financeiras e progresso.                               |
| Metas         | Permitir cadastrar e atualizar metas no protótipo.                  |
| Análises      | Apresentar distribuição por categoria e comparativos.               |
| NEXO AI       | Disponibilizar interface de conversação.                            |
| NEXO AI       | Responder perguntas utilizando o contexto financeiro demonstrativo. |

### 2.2. Prioridade P1 — Importante

Funcionalidades que enriquecem a experiência e reforçam o diferencial do produto.

- Filtros por período e categoria.

- Comparação entre períodos.

- Identificação de variações relevantes nas despesas.

- Sugestões educativas relacionadas aos hábitos financeiros.

- Alertas contextuais sobre metas e movimentações.

- Histórico de interações com o agente durante a sessão.

- Estados vazios e mensagens de orientação.

### 2.3. Prioridade P2 — Evolução futura

Funcionalidades que não devem comprometer a conclusão do MVP.

- Integração com instituições financeiras.

- Open Finance.

- Sincronização entre dispositivos.

- Autenticação e gerenciamento de usuários.

- Persistência em banco de dados remoto.

- Notificações externas.

- Relatórios exportáveis.

- Integrações financeiras reais.

- Personalização avançada do agente.

Esses recursos ficam fora do escopo inicial.

## 3. Funcionalidades reais e simulações

Como o projeto será construído no Lovable, é importante diferenciar uma interação demonstrável de uma funcionalidade de produção.

O protótipo deverá priorizar interações reais no frontend, utilizando dados fictícios e estado local quando possível.

| Recurso             | Comportamento esperado no protótipo                                                                                       |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| Dashboard           | Atualizar indicadores conforme os dados disponíveis no estado da aplicação.                                               |
| Movimentações       | Permitir cadastro, edição e exclusão durante a demonstração.                                                              |
| Filtros             | Alterar os registros exibidos conforme os critérios selecionados.                                                         |
| Metas               | Atualizar o progresso conforme os valores demonstrativos.                                                                 |
| Gráficos            | Refletir os dados utilizados nos cálculos.                                                                                |
| Agente NEXO AI      | Demonstrar respostas contextualizadas, conforme a implementação disponível.                                               |
| Histórico do agente | Manter as mensagens durante a sessão, se implementado.                                                                    |
| Persistência        | Não presumir armazenamento permanente. O protótipo poderá utilizar estado local ou armazenamento do navegador, se viável. |

**Regra importante:** não apresentar uma simulação como se fosse uma integração real. Caso o agente utilize respostas predefinidas ou dados mockados, isso deverá ser documentado como limitação do protótipo.

## 4. Base de dados demonstrativa

O MVP deverá utilizar uma única base de dados fictícia e coerente.

Não devemos criar dados independentes para cada tela. Dashboard, movimentações, análises, metas e agente precisam consultar a mesma fonte lógica.

### 4.1. Perfil demonstrativo

Criar um perfil fictício de jovem adulto que esteja começando a organizar suas finanças.

O perfil deverá conter:

- Receitas mensais.

- Despesas recorrentes.

- Despesas variáveis.

- Categorias de movimentação.

- Histórico de movimentações.

- Metas financeiras em andamento.

Não utilizar dados pessoais reais.

### 4.2. Categorias sugeridas

**Receitas**

- Salário.

- Renda extra.

- Outros recebimentos.

**Despesas**

- Moradia.

- Alimentação.

- Transporte.

- Educação.

- Saúde.

- Lazer.

- Assinaturas.

- Outros gastos.

### 4.3. Regras de consistência

A base demonstrativa deverá obedecer às seguintes regras:

1. Receitas e despesas precisam possuir valores positivos.

2. O tipo da movimentação determina se o valor será somado ou subtraído.

3. O saldo deve corresponder à diferença entre receitas e despesas.

4. Os gráficos devem refletir os registros existentes.

5. Os filtros devem afetar os indicadores e as listagens correspondentes.

6. O progresso das metas deve ser compatível com os valores registrados.

7. O agente não poderá apresentar informações inexistentes na base.

8. Os períodos comparados precisam utilizar intervalos equivalentes.

**Fórmula do saldo:**

Saldo = Total de receitas − Total de despesas.

A aplicação será responsável pelos cálculos financeiros. O agente deverá interpretar os resultados, não inventar ou substituir os valores oficiais.

## 5. Cenários de validação

O protótipo deverá ser testado com situações que representem o uso esperado.

### Cenário 01 — Visão geral financeira

**Objetivo:** validar a consistência do dashboard.

Verificar:

- Total de receitas.

- Total de despesas.

- Saldo disponível.

- Distribuição por categoria.

- Evolução financeira.

- Metas em andamento.

**Critério de aprovação:** todos os indicadores devem corresponder à base demonstrativa.

### Cenário 02 — Cadastro de movimentação

**Objetivo:** validar o gerenciamento financeiro.

Verificar:

- Cadastro de receita.

- Cadastro de despesa.

- Edição de movimentação.

- Exclusão de movimentação.

- Atualização dos indicadores após cada operação.

**Critério de aprovação:** as alterações devem refletir corretamente nas demais áreas do protótipo.

### Cenário 03 — Análise de despesas

**Objetivo:** verificar se a aplicação consegue apresentar informações úteis.

Verificar:

- Categoria com maior participação.

- Distribuição percentual.

- Comparação entre períodos.

- Identificação de variações.

**Critério de aprovação:** os resultados devem ser coerentes com os dados disponíveis e com os períodos selecionados.

### Cenário 04 — Acompanhamento de metas

**Objetivo:** validar o acompanhamento dos objetivos financeiros.

Verificar:

- Cadastro de meta.

- Valor desejado.

- Valor acumulado.

- Percentual de progresso.

- Atualização após alterações nos dados.

**Critério de aprovação:** o progresso deve ser calculado corretamente e apresentado de forma compreensível.

### Cenário 05 — Interação com o NEXO AI

**Objetivo:** avaliar a capacidade do agente de interpretar informações financeiras.

Perguntas demonstrativas:

- Como está minha situação financeira neste mês?

- Qual categoria representa a maior parte das minhas despesas?

- O que mudou em relação ao mês anterior?

- Quais despesas merecem minha atenção?

- Como está o andamento das minhas metas?

**Critério de aprovação:** as respostas devem utilizar os dados disponíveis, apresentar explicações claras e respeitar as limitações definidas no Documento 03.

### Cenário 06 — Dados insuficientes

**Objetivo:** avaliar o comportamento diante de informações incompletas.

Situações:

- Período sem movimentações.

- Categoria sem registros.

- Meta sem valor acumulado.

- Comparação sem histórico suficiente.

**Critério de aprovação:** a aplicação e o agente devem informar as limitações dos dados, sem inventar resultados.

## 6. Indicadores de qualidade

A avaliação do MVP deverá considerar os seguintes aspectos:

| Indicador               | Resultado esperado                                                |
| ----------------------- | ----------------------------------------------------------------- |
| Consistência financeira | Valores corretos em todas as telas.                               |
| Integridade dos dados   | Alterações refletidas nos módulos relacionados.                   |
| Usabilidade             | Navegação intuitiva e operações compreensíveis.                   |
| Responsividade          | Experiência adequada em desktop e dispositivos móveis.            |
| Acessibilidade          | Contraste, hierarquia visual e identificação dos controles.       |
| Inteligência contextual | Respostas coerentes com os dados disponíveis.                     |
| Tratamento de erros     | Mensagens claras para entradas inválidas e situações inesperadas. |
| Coerência visual        | Identidade visual consistente em todos os módulos.                |

## 7. Roteiro de validação

A validação será realizada em cinco etapas.

**Etapa 1 — Inspeção visual**

- Verificar identidade visual.

- Conferir hierarquia das informações.

- Avaliar navegação.

- Testar responsividade.

**Etapa 2 — Validação funcional**

- Cadastrar movimentações.

- Editar e excluir registros.

- Aplicar filtros.

- Atualizar metas.

**Etapa 3 — Validação financeira**

- Conferir cálculos.

- Comparar indicadores com os registros.

- Verificar gráficos.

- Conferir distribuição de valores por categoria.

**Etapa 4 — Validação do agente**

- Executar perguntas previstas.

- Verificar coerência das respostas.

- Testar ausência de dados.

- Verificar limites e linguagem educativa.

**Etapa 5 — Revisão geral**

- Identificar inconsistências.

- Corrigir problemas prioritários.

- Registrar limitações.

- Capturar evidências da versão final.

## 8. Riscos e medidas preventivas

| Risco                               | Medida preventiva                                          |
| ----------------------------------- | ---------------------------------------------------------- |
| Protótipo visual sem funcionalidade | Priorizar interações demonstráveis.                        |
| Dados inconsistentes                | Utilizar uma fonte lógica única.                           |
| Cálculos incorretos                 | Centralizar regras financeiras na aplicação.               |
| Respostas inventadas pelo agente    | Fornecer contexto estruturado e limitar afirmações.        |
| Excesso de funcionalidades          | Respeitar a priorização P0, P1 e P2.                       |
| Limitação de interações no Lovable  | Planejar prompts e agrupar alterações relacionadas.        |
| Perda de contexto entre telas       | Definir previamente os dados e contratos conceituais.      |
| Aparência genérica                  | Reforçar identidade visual e consistência dos componentes. |

## 9. Critérios de aprovação do MVP

O MVP será considerado satisfatório quando:

- Os cinco módulos principais estiverem disponíveis.

- A navegação entre módulos funcionar.

- O dashboard apresentar indicadores coerentes.

- O gerenciamento de movimentações funcionar no escopo demonstrativo.

- As análises refletirem os dados disponíveis.

- As metas apresentarem progresso consistente.

- O agente responder utilizando contexto financeiro.

- O agente respeitar suas limitações.

- O protótipo apresentar estados vazios e tratamento básico de erros.

- A experiência funcionar em diferentes tamanhos de tela.

- As principais limitações estiverem documentadas.

- As evidências da validação estiverem registradas.

## 10. Limitações conhecidas

O NEXO desenvolvido nesta etapa será um protótipo conceitual e interativo.

Não deverá ser apresentado como:

- Aplicação financeira pronta para uso real.

- Plataforma conectada a bancos.

- Sistema com dados financeiros reais.

- Consultor de investimentos.

- Sistema com segurança e persistência equivalentes a uma aplicação de produção.

A implementação deverá deixar claro o que é funcional, simulado ou apenas demonstrativo.

## 11. Resultado esperado

Ao final desta etapa, teremos um MVP com escopo delimitado, critérios de qualidade e cenários de validação definidos.

O resultado deverá demonstrar não apenas a capacidade de gerar uma interface com IA, mas também a capacidade de planejar um produto, definir regras de negócio, avaliar resultados e corrigir inconsistências.

**Princípio central:** o NEXO não deve apenas exibir números. Deve ajudar o usuário a compreender o que esses números representam.

---

**Próximo documento:** 06 — Registro de Decisões do Projeto (Decision Log).
