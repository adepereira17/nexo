# PROMPT 03 — EVOLUÇÃO FUNCIONAL DO NEXO E IMPLEMENTAÇÃO DO MVP

## 1. Contexto

Continue o desenvolvimento do projeto NEXO utilizando como base a aplicação existente, os documentos de planejamento e os dois prompts anteriormente fornecidos:

- Prompt Mestre.
- Estrutura Visual e Navegação.

O NEXO é uma aplicação de gestão financeira pessoal com inteligência artificial, voltada principalmente para jovens adultos que desejam organizar suas finanças, compreender seus hábitos e planejar melhor seus objetivos.

A primeira entrega visual e estrutural foi validada e aprovada.

Agora, o objetivo é evoluir a aplicação para uma versão funcional do MVP.

## 2. Diretriz principal

Antes de implementar, analise a estrutura existente, as tecnologias utilizadas, os serviços integrados e os recursos já disponíveis.

Não reconstrua a aplicação do zero.

Preserve integralmente:

- Identidade visual do NEXO.
- Paleta de cores.
- Tipografia.
- Layout e navegação.
- Responsividade.
- Componentes visuais aprovados.
- Organização dos cinco módulos existentes.

A implementação deve aproveitar ao máximo a estrutura atual.

Não faça alterações visuais desnecessárias.

## 3. Autenticação de usuários

Implemente um sistema funcional de autenticação.

Requisitos:

- Tela de cadastro de usuários.
- Tela de login.
- Logout.
- Validação de campos.
- Tratamento de credenciais inválidas.
- Proteção das páginas internas.
- Persistência da sessão.
- Separação dos dados financeiros por usuário autenticado.

Utilize uma solução de autenticação adequada à arquitetura existente.

Se houver integração com Supabase ou outro serviço, avalie sua utilização antes de introduzir uma nova tecnologia.

As senhas nunca devem ser armazenadas em texto puro.

Não simule autenticação apenas com variáveis locais ou verificações superficiais no frontend.

## 4. Movimentações financeiras

Transforme o módulo Movimentações em uma funcionalidade real.

Implemente:

- Cadastro de receitas.
- Cadastro de despesas.
- Edição de movimentações.
- Exclusão de movimentações.
- Descrição.
- Valor.
- Categoria.
- Data.
- Tipo de movimentação.
- Validação dos dados.
- Filtros e listagem funcional.

Requisitos adicionais:

- Utilizar precisão adequada para valores monetários.
- Impedir registros com valores inválidos.
- Exibir feedback de sucesso e erro.
- Atualizar as informações após operações de cadastro, edição e exclusão.
- Garantir que cada usuário visualize somente seus próprios registros.

## 5. Integração dos módulos financeiros

Os módulos devem utilizar uma fonte de dados consistente.

### Dashboard

- Calcular receitas, despesas e saldo com base nas movimentações cadastradas.
- Atualizar indicadores automaticamente.
- Atualizar gráficos conforme os dados disponíveis.
- Manter filtros de período funcionais.
- Apresentar estados vazios quando não existirem registros.

### Análises

- Utilizar movimentações reais.
- Apresentar indicadores e comparativos coerentes.
- Atualizar gráficos conforme os filtros selecionados.
- Não apresentar conclusões baseadas em dados inexistentes.

### Metas

- Permitir criar e acompanhar objetivos financeiros.
- Registrar nome, valor desejado e progresso.
- Persistir as metas por usuário.
- Apresentar indicadores de progresso coerentes.

## 6. Remoção dos dados demonstrativos

Remova os dados fictícios utilizados na primeira versão.

A aplicação deve iniciar com uma experiência limpa para cada novo usuário.

Requisitos:

- Não apresentar receitas, despesas ou saldos fictícios como dados reais.
- Não manter movimentações demonstrativas misturadas aos registros dos usuários.
- Exibir mensagens e estados vazios adequados.
- Orientar o usuário sobre como começar a utilizar cada módulo.

Preserve os dados estruturais necessários à aplicação, sem apagar configurações, componentes ou funcionalidades.

## 7. NEXO AI — Versão beta funcional

O assistente inteligente faz parte da proposta central do produto e precisa deixar de ser apenas uma interface visual.

Implemente uma primeira versão funcional do NEXO AI.

Requisitos:

- Habilitar envio e recebimento de mensagens.
- Apresentar histórico da conversa durante a sessão.
- Oferecer sugestões de perguntas.
- Utilizar informações financeiras do usuário autenticado como contexto, respeitando as permissões.
- Interpretar receitas, despesas, categorias e metas.
- Produzir explicações educativas sobre hábitos financeiros.
- Auxiliar na compreensão de padrões e no planejamento de objetivos.

Regras de confiabilidade:

- Os cálculos oficiais devem ser realizados pelo sistema, não pela IA.
- O assistente não pode inventar saldos, movimentações ou metas.
- Não deve apresentar promessas de rentabilidade.
- Não deve fornecer recomendações personalizadas de investimentos.
- Deve reconhecer quando não possui informações suficientes.
- Deve informar que está em versão beta.

Utilize uma integração de IA compatível com a arquitetura existente, preferencialmente aproveitando recursos já disponíveis na plataforma.

Não exponha chaves de API no frontend ou no código público.

Se for necessária configuração externa, identifique claramente o que precisa ser configurado.

Não apresente respostas simuladas como se fossem respostas de uma IA real.

## 8. Segurança e qualidade

Verifique os seguintes pontos:

- Isolamento dos dados entre usuários.
- Proteção das rotas privadas.
- Validação de entradas.
- Tratamento de erros.
- Persistência dos registros.
- Segurança das credenciais.
- Consistência dos dados financeiros.
- Ausência de erros relevantes no console.

Não considere a ocultação de elementos na interface como mecanismo de segurança.

## 9. Critérios de aceitação

A implementação será considerada concluída quando for possível:

1. Criar uma conta.
2. Entrar e sair da aplicação.
3. Manter uma sessão autenticada.
4. Cadastrar receitas e despesas.
5. Editar e excluir movimentações.
6. Consultar os dados cadastrados no Dashboard.
7. Visualizar análises atualizadas.
8. Criar e acompanhar metas.
9. Utilizar o NEXO AI em uma versão beta funcional.
10. Verificar que usuários diferentes não compartilham seus dados financeiros.

Todas as funcionalidades devem ser testadas considerando os fluxos principais.

## 10. Método de execução

Trabalhe de forma organizada e incremental.

Antes de implementar, identifique possíveis incompatibilidades entre a arquitetura atual e os requisitos.

Priorize a reutilização dos componentes existentes.

Não altere funcionalidades já aprovadas sem necessidade.

Não adicione módulos, integrações ou recursos fora do escopo definido.

Não considere uma funcionalidade concluída apenas porque sua interface foi criada.

Ao concluir, apresente um relatório contendo:

- Tecnologias utilizadas.
- Serviços e integrações configurados.
- Funcionalidades implementadas.
- Funcionalidades que dependem de configuração externa.
- Estrutura de dados e persistência.
- Medidas de segurança adotadas.
- Testes executados e seus resultados.
- Problemas encontrados.
- Limitações conhecidas.
- Itens que ainda precisam de intervenção.

Se algum requisito não puder ser implementado, explique o motivo e não apresente uma implementação fictícia como concluída.

**Resultado esperado:** uma evolução funcional do NEXO, preservando a primeira entrega aprovada e transformando os módulos existentes em uma experiência integrada de gestão financeira pessoal com autenticação e assistência inteligente.