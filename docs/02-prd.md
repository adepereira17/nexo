# NEXO — Product Requirements Document (PRD)

**Projeto:** NEXO  
**Documento:** 02 — Product Requirements Document  
**Versão:** 1.0  
**Status:** Planejamento  
**Categoria:** Fintech / Personal Finance / AI Assistant  
**Plataforma:** Aplicação web responsiva  
**Público-alvo:** Jovens adultos  
**Abordagem de desenvolvimento:** Vibe Coding

---

## 1. Objetivo do documento

Este documento define os requisitos funcionais, não funcionais, regras de negócio e critérios de aceitação do NEXO.

O PRD servirá como referência para orientar a geração do protótipo utilizando ferramentas de inteligência artificial, garantindo coerência entre a visão do produto e sua implementação visual.

O documento também estabelece limites para evitar funcionalidades não solicitadas, comportamentos inconsistentes e informações financeiras incorretas.

## 2. Visão do produto

O NEXO é um aplicativo de gestão e inteligência financeira pessoal que utiliza inteligência artificial para transformar dados financeiros em informações compreensíveis e contextualizadas.

A aplicação combina cinco pilares:

1. Dashboard financeiro.

2. Gestão de movimentações.

3. Agente Financeiro Inteligente.

4. Metas financeiras.

5. Análise de comportamento financeiro.

O principal diferencial é a capacidade de interpretar informações financeiras e identificar padrões, oferecendo ao usuário uma visão mais clara sobre sua situação financeira.

## 3. Objetivos de negócio e experiência

### 3.1. Objetivos principais

- Simplificar a organização financeira pessoal.

- Facilitar a compreensão das receitas e despesas.

- Identificar padrões de comportamento financeiro.

- Incentivar o planejamento e acompanhamento de objetivos.

- Utilizar IA para contextualizar informações financeiras.

- Proporcionar uma experiência simples e acessível.

### 3.2. Resultados esperados

Ao utilizar o NEXO, o usuário deverá conseguir compreender:

- Quanto recebeu em determinado período.

- Quanto gastou.

- Quanto possui de saldo calculado.

- Quais categorias concentram seus gastos.

- Como sua situação financeira evoluiu.

- Como estão suas metas.

- Quais padrões merecem atenção.

## 4. Escopo funcional do MVP

O MVP será composto por cinco módulos principais.

### RF-01 — Dashboard Financeiro

**Descrição:** apresentar uma visão consolidada da situação financeira do usuário.

**Requisitos:**

- RF-01.1: Exibir total de receitas do período.

- RF-01.2: Exibir total de despesas do período.

- RF-01.3: Exibir saldo calculado.

- RF-01.4: Apresentar distribuição de despesas por categoria.

- RF-01.5: Apresentar evolução financeira por período.

- RF-01.6: Permitir seleção de período de consulta.

- RF-01.7: Apresentar resumo das metas financeiras.

- RF-01.8: Disponibilizar acesso ao Agente Financeiro.

**Critérios de aceitação:**

- Os indicadores devem corresponder às movimentações registradas.

- Os valores devem respeitar as regras de cálculo financeiro.

- A alteração do período deve atualizar os indicadores e gráficos.

- Gráficos devem possuir legendas e informações compreensíveis.

- Estados sem movimentações devem apresentar mensagens apropriadas.

### RF-02 — Gestão de movimentações

**Descrição:** permitir o registro e gerenciamento de receitas e despesas.

**Requisitos:**

- RF-02.1: Registrar receitas.

- RF-02.2: Registrar despesas.

- RF-02.3: Informar descrição, valor, data e categoria.

- RF-02.4: Editar movimentações existentes.

- RF-02.5: Excluir movimentações mediante confirmação.

- RF-02.6: Consultar histórico de movimentações.

- RF-02.7: Filtrar movimentações por período, tipo e categoria.

- RF-02.8: Exibir valores formatados em Real brasileiro (BRL).

**Categorias iniciais de despesas:**

- Alimentação.

- Moradia.

- Transporte.

- Saúde.

- Educação.

- Lazer.

- Compras.

- Serviços e assinaturas.

- Outros.

**Categorias iniciais de receitas:**

- Salário.

- Trabalho autônomo.

- Freelance.

- Rendimentos.

- Outros.

**Critérios de aceitação:**

- Não permitir valores negativos ou iguais a zero.

- Não permitir movimentações sem valor, data e tipo.

- Toda movimentação deve possuir uma categoria.

- Alterações e exclusões devem atualizar os indicadores financeiros.

- O histórico deve apresentar informações organizadas cronologicamente.

### RF-03 — Agente Financeiro Inteligente

**Descrição:** disponibilizar um agente de IA capaz de interpretar informações financeiras estruturadas e apresentar análises contextualizadas.

**Requisitos:**

- RF-03.1: Disponibilizar uma interface de conversação.

- RF-03.2: Responder perguntas sobre receitas e despesas.

- RF-03.3: Interpretar dados do período selecionado.

- RF-03.4: Identificar categorias com maior participação nas despesas.

- RF-03.5: Comparar períodos financeiros.

- RF-03.6: Identificar padrões de comportamento.

- RF-03.7: Apresentar sugestões educativas de organização financeira.

- RF-03.8: Informar quando não houver dados suficientes.

- RF-03.9: Apresentar contexto utilizado nas análises.

- RF-03.10: Diferenciar informações calculadas de interpretações produzidas pela IA.

**Exemplos de perguntas:**

- Quanto gastei neste mês?

- Qual categoria representa meus maiores gastos?

- Minhas despesas aumentaram em relação ao mês anterior?

- Quanto consegui economizar?

- Como está o andamento da minha meta?

- Quais despesas merecem minha atenção?

**Critérios de aceitação:**

- As respostas devem utilizar os dados financeiros disponíveis.

- A IA não pode inventar movimentações, valores ou saldos.

- Comparações devem utilizar períodos equivalentes.

- Na ausência de dados, o agente deve informar a limitação.

- As respostas devem utilizar linguagem acessível.

- Sugestões devem ser educativas e contextualizadas.

- O agente não deve executar movimentações financeiras sem autorização explícita do usuário.

### RF-04 — Metas financeiras

**Descrição:** permitir que o usuário estabeleça objetivos financeiros e acompanhe seu progresso.

**Requisitos:**

- RF-04.1: Criar uma meta financeira.

- RF-04.2: Informar nome, valor desejado e prazo.

- RF-04.3: Informar valor inicial acumulado.

- RF-04.4: Atualizar o progresso da meta.

- RF-04.5: Apresentar percentual de conclusão.

- RF-04.6: Permitir editar e excluir metas.

- RF-04.7: Exibir metas no dashboard.

- RF-04.8: Permitir que o agente interprete o andamento das metas.

**Critérios de aceitação:**

- O progresso deve ser calculado corretamente.

- O percentual não deve ultrapassar 100% na representação visual.

- Valores acumulados não podem ser negativos.

- Metas concluídas devem possuir indicação visual.

- Alterações devem atualizar os indicadores correspondentes.

### RF-05 — Análise de comportamento financeiro

**Descrição:** apresentar informações sobre hábitos financeiros a partir das movimentações registradas.

**Requisitos:**

- RF-05.1: Identificar categorias com maior participação nas despesas.

- RF-05.2: Comparar despesas entre períodos.

- RF-05.3: Identificar variações relevantes.

- RF-05.4: Apresentar evolução das receitas e despesas.

- RF-05.5: Identificar concentração de gastos.

- RF-05.6: Gerar observações contextualizadas com apoio da IA.

- RF-05.7: Disponibilizar indicadores de acompanhamento.

**Critérios de aceitação:**

- As análises devem considerar exclusivamente os dados disponíveis.

- Comparações devem apresentar os períodos utilizados.

- Variações percentuais devem possuir base de cálculo válida.

- Ausência de histórico deve ser informada.

- O sistema não deve apresentar conclusões sem evidências suficientes.

## 5. Regras de negócio

As regras de negócio devem ser respeitadas independentemente da interface ou ferramenta utilizada para construir o protótipo.

### RN-01 — Cálculo do saldo

O saldo do período será calculado pela diferença entre receitas e despesas:

**Saldo = Total de receitas − Total de despesas**

### RN-02 — Cálculo de receitas

Somente movimentações classificadas como receitas devem compor o total de receitas.

### RN-03 — Cálculo de despesas

Somente movimentações classificadas como despesas devem compor o total de despesas.

### RN-04 — Transferências

Transferências entre contas do mesmo usuário não devem ser contabilizadas como receitas ou despesas.

Essa funcionalidade poderá ser implementada em uma evolução futura, mas a regra deve ser considerada na modelagem conceitual.

### RN-05 — Precisão monetária

- Utilizar BRL como moeda padrão.

- Exibir valores no padrão brasileiro.

- Evitar erros de arredondamento.

- Realizar cálculos monetários utilizando representação decimal ou valores inteiros em centavos.

- Não depender de cálculos aproximados realizados pela IA.

### RN-06 — Períodos

As movimentações devem respeitar suas respectivas datas.

O período selecionado deve ser aplicado aos indicadores, gráficos e análises correspondentes.

### RN-07 — Comparação financeira

Comparações mensais devem utilizar períodos equivalentes.

Quando não houver dados suficientes para comparação, o sistema deve informar a indisponibilidade da análise.

### RN-08 — Metas financeiras

O progresso será calculado pela relação entre valor acumulado e valor desejado.

**Progresso (%) = (Valor acumulado ÷ Valor desejado) × 100**

O valor desejado deve ser maior que zero.

### RN-09 — Integridade dos dados

Os indicadores do dashboard devem ser derivados das movimentações registradas, evitando valores duplicados ou divergentes.

### RN-10 — Responsabilidade da IA

A IA não é responsável pelos cálculos financeiros oficiais do sistema.

Ela recebe informações estruturadas e utiliza esses dados para elaborar interpretações e explicações.

### RN-11 — Dados insuficientes

O agente deve informar quando não possuir dados suficientes para responder com segurança.

### RN-12 — Transparência

Toda análise deve deixar claro quando se trata de um dado registrado, um cálculo do sistema ou uma interpretação da IA.

## 6. Requisitos não funcionais

### RNF-01 — Usabilidade

A interface deve ser intuitiva, com navegação simples e textos acessíveis.

### RNF-02 — Responsividade

A aplicação deve funcionar adequadamente em dispositivos desktop, tablets e smartphones.

### RNF-03 — Acessibilidade

- Contraste adequado.

- Navegação compreensível.

- Identificação textual de informações importantes.

- Campos com rótulos claros.

- Estados de foco visíveis.

- Não utilizar apenas cores para comunicar situações.

### RNF-04 — Desempenho

A interface deve apresentar carregamento e transições fluidas, evitando elementos desnecessários.

### RNF-05 — Consistência

Os valores financeiros devem ser apresentados de maneira uniforme em todas as telas.

### RNF-06 — Privacidade

O protótipo utilizará exclusivamente dados fictícios.

Não deverão ser inseridas credenciais bancárias, informações financeiras reais ou dados pessoais sensíveis.

### RNF-07 — Segurança

A solução não deve expor credenciais ou chaves de API no código disponibilizado ao usuário.

### RNF-08 — Compatibilidade

Priorizar navegadores modernos, com experiência consistente entre desktop e dispositivos móveis.

### RNF-09 — Clareza visual

Gráficos, indicadores e informações devem possuir hierarquia visual adequada e não sobrecarregar a interface.

## 7. Fluxos principais

### Fluxo 1 — Consulta financeira

1. Usuário acessa o NEXO.

2. Visualiza o dashboard.

3. Seleciona o período desejado.

4. Consulta receitas, despesas e saldo.

5. Acessa análises detalhadas ou consulta o agente.

### Fluxo 2 — Registro de movimentação

1. Usuário acessa movimentações.

2. Seleciona receita ou despesa.

3. Informa os dados.

4. Seleciona a categoria.

5. Confirma o registro.

6. O sistema atualiza os indicadores financeiros.

### Fluxo 3 — Análise com IA

1. Usuário acessa o Agente Financeiro.

2. Envia uma pergunta.

3. O sistema disponibiliza os dados relevantes.

4. O agente interpreta as informações.

5. A resposta é apresentada com contexto.

6. O usuário pode aprofundar a análise.

### Fluxo 4 — Criação de meta

1. Usuário acessa metas financeiras.

2. Cria um objetivo.

3. Informa valor desejado e prazo.

4. Define o valor inicial acumulado.

5. Confirma a criação.

6. O sistema apresenta o progresso.

### Fluxo 5 — Análise de comportamento

1. Usuário acessa análises.

2. Seleciona o período.

3. O sistema consolida os dados.

4. Apresenta gráficos e indicadores.

5. O agente pode contextualizar os resultados.

## 8. Modelo conceitual de dados

O protótipo deverá considerar as seguintes entidades:

### Usuário

- Identificador.

- Nome de exibição.

- Preferências de interface.

### Movimentação

- Identificador.

- Descrição.

- Tipo.

- Valor.

- Data.

- Categoria.

- Observações opcionais.

### Categoria

- Identificador.

- Nome.

- Tipo.

- Descrição opcional.

### Meta financeira

- Identificador.

- Nome.

- Valor desejado.

- Valor acumulado.

- Prazo.

- Status.

### Conversa

- Identificador.

- Data de criação.

- Mensagens.

- Contexto da análise.

Esse modelo é conceitual e não determina uma tecnologia de banco de dados ou uma infraestrutura específica.

## 9. Dados para demonstração

O protótipo deverá utilizar dados fictícios, porém coerentes entre si.

Os dados devem contemplar:

- Diferentes fontes de receitas.

- Despesas em categorias variadas.

- Movimentações em diferentes datas.

- Histórico suficiente para comparações mensais.

- Metas financeiras em diferentes estágios.

- Exemplos de variação de despesas.

Os dados utilizados pelo dashboard, gráficos e agente devem possuir uma única fonte lógica de referência, evitando inconsistências entre módulos.

## 10. Fora do escopo do MVP

Não serão implementados nesta versão:

- Integração bancária via Open Finance.

- Conexão com contas bancárias reais.

- Pagamentos e transferências financeiras.

- Cartões de crédito reais.

- Contratação de produtos financeiros.

- Recomendações personalizadas de investimento.

- Compra e venda de ativos.

- Gestão financeira empresarial.

- Compartilhamento de contas entre usuários.

- Infraestrutura de produção e autenticação bancária.

## 11. Critérios gerais de qualidade

O protótipo será avaliado considerando:

| Critério                | Resultado esperado                         |
| ----------------------- | ------------------------------------------ |
| Coerência funcional     | Funcionalidades alinhadas ao PRD           |
| Precisão financeira     | Cálculos consistentes                      |
| Inteligência artificial | Análises contextualizadas                  |
| Experiência do usuário  | Navegação intuitiva                        |
| Consistência visual     | Identidade uniforme                        |
| Responsividade          | Adaptação a diferentes dispositivos        |
| Transparência           | Diferenciação entre dados e interpretações |
| Integridade             | Informações coerentes entre os módulos     |

## 12. Priorização das funcionalidades

Classificação utilizada:

- **P0:** indispensável para demonstrar o MVP.

- **P1:** importante para a experiência completa.

- **P2:** evolução futura.

| Funcionalidade                     | Prioridade |
| ---------------------------------- | ---------- |
| Dashboard financeiro               | P0         |
| Cadastro e edição de movimentações | P0         |
| Agente Financeiro                  | P0         |
| Metas financeiras                  | P0         |
| Análise de comportamento           | P0         |
| Filtros e comparativos             | P1         |
| Histórico de conversas             | P1         |
| Alertas inteligentes               | P2         |
| Importação de extratos             | P2         |
| Integrações bancárias              | P2         |

## 13. Definição de conclusão do MVP

O MVP será considerado concluído quando:

1. Os cinco módulos principais estiverem representados no protótipo.

2. Os fluxos principais puderem ser demonstrados.

3. Os dados fictícios estiverem integrados conceitualmente entre os módulos.

4. Os cálculos financeiros apresentarem resultados coerentes.

5. O agente conseguir interpretar informações financeiras disponíveis.

6. A interface apresentar consistência visual e responsividade.

7. As limitações do protótipo estiverem documentadas.

8. O resultado estiver alinhado à visão do produto.

## 14. Premissas de implementação

O desenvolvimento será conduzido por meio de Vibe Coding, utilizando o PRD como referência principal.

As ferramentas de IA poderão propor soluções técnicas e visuais, mas todas as sugestões deverão ser avaliadas quanto à coerência com os requisitos estabelecidos.

Nenhuma funcionalidade adicional deverá ser considerada parte do MVP sem uma decisão explícita de escopo.

---

**Documento:** 02 — PRD  
**Projeto:** NEXO  
**Versão:** 1.0  
**Status:** Base para engenharia de prompts e prototipação
