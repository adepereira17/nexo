# 06. Registro de Decisões do Projeto (Decision Log)

**Projeto:** NEXO — Assistente Inteligente de Finanças Pessoais  
**Versão:** 1.0  
**Status:** Planejamento  
**Objetivo:** Registrar decisões arquiteturais, funcionais, visuais e técnicas que orientam o desenvolvimento do protótipo.

---

## 1. Objetivo do documento

O Decision Log centraliza as principais decisões tomadas durante o planejamento do NEXO.

Cada decisão deverá apresentar:

- Contexto: qual problema ou necessidade motivou a decisão.

- Decisão: qual caminho foi escolhido.

- Justificativa: por que essa alternativa foi selecionada.

- Consequências: quais impactos são esperados.

- Status: situação atual da decisão.

As decisões poderão ser revisadas quando surgirem novas necessidades, desde que as alterações sejam documentadas.

## 2. Decisões de produto

### DEC-001 — Nome do produto

**Decisão:** utilizar NEXO como nome provisório.

**Justificativa:** representa a conexão entre informações financeiras, inteligência e tomada de decisões.

**Consequência:** identidade visual, documentação e prompts utilizarão NEXO durante o desenvolvimento.

**Status:** Aprovada, sujeita à verificação de disponibilidade de marca e domínio antes de qualquer lançamento público.

### DEC-002 — Público-alvo

**Decisão:** jovens adultos que estão começando a organizar suas finanças pessoais.

**Justificativa:** permite desenvolver uma experiência acessível, educativa e adequada a pessoas com diferentes níveis de familiaridade com organização financeira.

**Consequência:** linguagem simples, navegação intuitiva e explicações sem excesso de termos técnicos.

**Status:** Aprovada.

### DEC-003 — Diferencial do produto

**Decisão:** priorizar inteligência financeira e análise contextual.

**Justificativa:** um aplicativo que apenas registra receitas e despesas possui diferenciação limitada. O NEXO deverá transformar dados em informações compreensíveis.

**Consequência:** o agente financeiro será parte central da experiência, integrado aos demais módulos.

**Status:** Aprovada.

### DEC-004 — Posicionamento do agente

**Decisão:** o NEXO AI será um assistente integrado à aplicação, não a interface exclusiva do produto.

**Justificativa:** o usuário precisa conseguir consultar indicadores, movimentações, análises e metas sem depender de uma conversa com a IA.

**Consequência:** o agente terá área própria e pontos de acesso contextual no dashboard e nos demais módulos.

**Status:** Aprovada.

## 3. Decisões arquiteturais

### DEC-005 — Abordagem de desenvolvimento

**Decisão:** utilizar Vibe Coding como metodologia de construção do protótipo, com apoio de ferramentas de IA.

**Justificativa:** o desafio busca demonstrar a capacidade de orientar, avaliar e corrigir soluções produzidas por inteligência artificial.

**Consequência:** prompts, resultados, correções e decisões relevantes deverão ser documentados.

**Status:** Aprovada.

### DEC-006 — Ferramenta de prototipação

**Decisão:** utilizar Lovable para construir o protótipo interativo.

**Justificativa:** permite transformar requisitos e instruções em uma aplicação visual e navegável.

**Consequência:** os prompts deverão ser planejados antes da execução, respeitando as limitações do plano utilizado.

**Status:** Aprovada.

### DEC-007 — Arquitetura conceitual

**Decisão:** organizar a aplicação em três camadas lógicas:

1. Interface: componentes, páginas, formulários e gráficos.

2. Aplicação e regras de negócio: movimentações, cálculos, metas e análises.

3. Inteligência: interpretação contextual e respostas do NEXO AI.

**Justificativa:** separa responsabilidades e reduz a dependência de cálculos financeiros realizados pela IA.

**Consequência:** regras financeiras deverão permanecer sob responsabilidade da aplicação.

**Status:** Aprovada.

### DEC-008 — Fonte de dados

**Decisão:** utilizar uma base demonstrativa única e coerente.

**Justificativa:** dashboard, movimentações, análises, metas e agente precisam trabalhar com as mesmas informações.

**Consequência:** evitar dados independentes e números fictícios desconectados entre telas.

**Status:** Aprovada.

### DEC-009 — Persistência

**Decisão:** não exigir backend ou banco de dados remoto no MVP.

**Justificativa:** o objetivo é demonstrar o conceito e as interações do produto, não construir uma infraestrutura de produção.

**Consequência:** utilizar estado local e armazenamento do navegador quando viável. A persistência efetivamente implementada deverá ser documentada.

**Status:** Aprovada.

### DEC-010 — Cálculos financeiros

**Decisão:** cálculos financeiros serão determinísticos e executados pela aplicação.

**Justificativa:** valores monetários precisam ser consistentes e verificáveis. A IA não deverá ser responsável por calcular saldos oficiais.

**Consequência:** o agente receberá indicadores e dados estruturados para interpretação.

**Status:** Aprovada.

### DEC-011 — Integrações externas

**Decisão:** não implementar Open Finance, integrações bancárias ou operações financeiras reais no MVP.

**Justificativa:** essas funcionalidades aumentariam a complexidade e não são necessárias para demonstrar a proposta central.

**Consequência:** todos os dados financeiros serão demonstrativos.

**Status:** Aprovada.

## 4. Decisões de experiência e interface

### DEC-012 — Identidade visual

**Decisão:** utilizar uma identidade moderna, minimalista e profissional, com tema claro inicial.

**Paleta definida:**

| Elemento     | Cor     |
| ------------ | ------- |
| Azul-marinho | #111827 |
| Roxo         | #8B5CF6 |
| Verde-lima   | #A3E635 |
| Fundo claro  | #F8FAFC |

**Justificativa:** transmitir organização, tecnologia e clareza sem sobrecarregar a experiência.

**Consequência:** os componentes deverão seguir uma linguagem visual consistente.

**Status:** Aprovada.

### DEC-013 — Navegação principal

**Decisão:** organizar a navegação em cinco módulos:

1. Dashboard.

2. Movimentações.

3. Análises.

4. Metas.

5. NEXO AI.

**Justificativa:** separar responsabilidades e facilitar a localização das funcionalidades.

**Consequência:** manter navegação consistente em desktop e dispositivos móveis.

**Status:** Aprovada.

### DEC-014 — Responsividade e acessibilidade

**Decisão:** desenvolver uma experiência adaptável a desktop, tablet e dispositivos móveis.

**Justificativa:** o produto deve permanecer utilizável em diferentes contextos.

**Consequência:** priorizar hierarquia visual, contraste, controles identificáveis e navegação acessível.

**Status:** Aprovada.

## 5. Decisões sobre inteligência artificial

### DEC-015 — Responsabilidade do agente

**Decisão:** o NEXO AI será responsável por interpretar dados, identificar padrões e oferecer orientações educativas.

**Justificativa:** a inteligência artificial deve agregar contexto, não substituir as regras de negócio.

**Consequência:** respostas deverão utilizar informações disponíveis e reconhecer limitações.

**Status:** Aprovada.

### DEC-016 — Limites de atuação

**Decisão:** o agente não deverá oferecer recomendações personalizadas de investimentos, promessas de rentabilidade ou executar operações financeiras.

**Justificativa:** manter o produto no campo da organização e educação financeira.

**Consequência:** perguntas fora do escopo deverão receber respostas transparentes e direcionamento adequado.

**Status:** Aprovada.

### DEC-017 — Tratamento de dados insuficientes

**Decisão:** o agente deverá reconhecer quando não possui informações suficientes.

**Justificativa:** respostas inventadas comprometem a confiança no produto.

**Consequência:** apresentar ressalvas, solicitar informações adicionais quando necessário ou informar que não é possível realizar determinada análise.

**Status:** Aprovada.

## 6. Decisões de escopo

### DEC-018 — Priorização do MVP

**Decisão:** utilizar três níveis de prioridade:

- P0: funcionalidades essenciais.

- P1: funcionalidades importantes.

- P2: evoluções futuras.

**Justificativa:** manter o foco no objetivo central e evitar expansão desnecessária do escopo.

**Consequência:** funcionalidades P2 não deverão consumir o esforço inicial de construção.

**Status:** Aprovada.

### DEC-019 — Dados fictícios

**Decisão:** utilizar exclusivamente dados demonstrativos no protótipo.

**Justificativa:** não há necessidade de utilizar informações financeiras reais para validar a experiência.

**Consequência:** os dados deverão ser coerentes, consistentes e identificados como demonstrativos.

**Status:** Aprovada.

### DEC-020 — Critérios de conclusão

**Decisão:** avaliar o protótipo por critérios funcionais, financeiros, visuais e de inteligência contextual.

**Justificativa:** qualidade não deve ser medida apenas pela aparência da interface.

**Consequência:** executar os cenários definidos no Documento 05 antes de considerar o MVP concluído.

**Status:** Aprovada.

## 7. Pendências para as próximas etapas

As decisões abaixo ainda dependem de validação durante a implementação.

| ID      | Pendência                                                    | Quando resolver                   |
| ------- | ------------------------------------------------------------ | --------------------------------- |
| PEN-001 | Verificar disponibilidade do nome NEXO para uso público.     | Antes de publicação comercial.    |
| PEN-002 | Definir a estrutura definitiva dos dados mockados.           | Antes da construção do protótipo. |
| PEN-003 | Definir como o agente receberá o contexto financeiro.        | Durante a engenharia de prompts.  |
| PEN-004 | Avaliar quais interações podem ser implementadas no Lovable. | Durante a construção.             |
| PEN-005 | Validar consistência dos cálculos e gráficos.                | Durante os testes.                |
| PEN-006 | Registrar limitações reais da versão construída.             | Na documentação final.            |

## 8. Controle de alterações

Toda alteração relevante deverá ser registrada neste documento.

Modelo para novas decisões:

**ID:** DEC-XXX  
**Data:** DD/MM/AAAA  
**Contexto:** descrição da necessidade.  
**Decisão:** alternativa escolhida.  
**Justificativa:** motivo da escolha.  
**Consequências:** impactos esperados.  
**Status:** proposta, aprovada, rejeitada ou substituída.

Decisões substituídas não deverão ser apagadas. O histórico deverá permanecer disponível para consulta.

## 9. Encerramento do planejamento

Com este documento, a fase de planejamento do NEXO está formalmente concluída.

Os seis documentos da Wiki estabelecem:

- Visão e posicionamento do produto.

- Requisitos funcionais e não funcionais.

- Comportamento esperado do agente financeiro.

- Experiência do usuário e identidade visual.

- Escopo do MVP e critérios de validação.

- Decisões arquiteturais e funcionais.

**Próxima fase:** Engenharia de Prompts e Construção do Protótipo.

O desenvolvimento deverá seguir os requisitos e decisões documentados, utilizando a IA como ferramenta de execução, enquanto as decisões de produto, arquitetura e qualidade permanecem sob controle do projeto.

**Princípio de desenvolvimento:** a IA pode acelerar a construção, mas a responsabilidade pela qualidade do produto continua sendo de quem o especifica, avalia e valida.
