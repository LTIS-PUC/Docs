# 2. Especificação do Projeto

A definição exata do problema e os pontos mais relevantes a serem tratados neste projeto foi consolidada com base na análise das necessidades institucionais relacionadas à elaboração de avaliações acadêmicas. Esse levantamento foi realizado por meio da observação dos processos atuais de criação de provas e simulados, bem como pela identificação das dificuldades enfrentadas por professores e gestores acadêmicos.
Os detalhes levantados nesse processo foram organizados de forma a orientar o desenvolvimento do sistema ADAMED, com foco na centralização de questões, padronização das avaliações e apoio à criação de simulados voltados à preparação para exames como o ENAMED.


## Requisitos do Projeto

O escopo funcional do projeto é definido por meio dos requisitos funcionais que descrevem as possibilidades de interação dos usuários, bem como os requisitos não funcionais que descrevem os aspectos gerais que o sistema deverá apresentar. Estes requisitos são apresentados a seguir.

### Requisitos Funcionais

A tabela a seguir apresenta os requisitos do projeto, identificando a prioridade em que os mesmos devem ser entregues.

| ID    | Descrição                                                                                         | Prioridade |
|-------|---------------------------------------------------------------------------------------------------|------------|
| RF-01 | O sistema deve permitir o cadastro de questões avaliativas | Alta       |
| RF-02 | O sistema deve permitir a edição e exclusão de questões | Alta     |
| RF-03 | O sistema deve permitir categorizar questões por disciplina | Alta     |
| RF-04 | O sistema deve permitir associar questões a objetivos de aprendizagem | Alta     |
| RF-05 | O sistema deve permitir definir nível de dificuldade das questões  | Alta      |
| RF-06 | O sistema deve permitir cadastrar alternativas e definir a resposta correta | Alta     |
| RF-07 | O sistema deve permitir criar provas a partir do banco de questões | Alta      |
| RF-08 | O sistema deve permitir criar simulados acadêmicos | Alta      |
| RF-09 | O sistema deve permitir selecionar questões manualmente | Alta      |
| RF-10 | O sistema deve permitir gerar provas automaticamente por critérios | Alta      |
| RF-11 | O sistema deve permitir definir tempo limite para provas e simulados | Alta      |
| RF-12 | O sistema deve permitir buscar e filtrar questões por disciplina, tema e dificuldade | Alta      |
| RF-13 | O sistema deve permitir aplicar provas para turmas específicas | Alta      |
| RF-14 | O sistema deve permitir definir início e fim da aplicação de provas | Alta      |
| RF-15 | O sistema deve registrar as respostas dos alunos | Alta      |
| RF-16 | O sistema deve permitir envio automático ao término do tempo | Alta      |
| RF-17 | O sistema deve corrigir automaticamente provas objetivas | Alta      |
| RF-18 | O sistema deve calcular a nota do aluno | Alta      |
| RF-19 | O sistema deve gerar relatórios de desempenho | Alta      |
| RF-20 | O sistema deve permitir embaralhar questões automaticamente | Média     |
| RF-21 | O sistema deve permitir embaralhar alternativas das questões | Média      |
| RF-22 | O sistema deve permitir salvar provas como rascunho | Alta      |
| RF-23 | O sistema deve permitir clonar provas existentes | Média      |
| RF-24 | O sistema deve permitir reabrir provas em casos específicos | Média      |
| RF-25 | O sistema deve exibir desempenho por disciplina | Média      |
| RF-26 | O sistema deve permitir exportação de resultados em PDF ou Excel | Alta      |
| RF-27 | O aplicativo devera exibir informações sobre time do usuário em sua página de perfil | Média      |
| RF-28 | O sistema deve exibir estatísticas de uso das questões | Média      |
| RF-29 | O sistema deve permitir autenticação de usuários | Alta      |
| RF-30 | O sistema deve permitir diferentes perfis de acesso | Alta      |
| RF-31 | O sistema deve controlar permissões de acesso por perfil | Alta      |
| RF-32 | O sistema deve registrar logs de ações dos usuários | Média      |


### Requisitos não funcionais

A tabela a seguir apresenta os requisitos não funcionais que o projeto deverá atender.

| ID    | Descrição                                                                                          
|-------|-----------------------------------------------------------------------------------------------------------------|
| RNF-01 | O sistema deve ser acessível apenas para usuários autorizados da Pontifícia Universidade Católica de Minas Gerais 
| RNF-02 | O sistema deverá ser responsivo, permitindo a visualização em diferentes dispositivos de forma adequada 
| RNF-03 | O sistema deve garantir a segurança e integridade dos dados
| RNF-04 | O sistema deve apresentar bom desempenho e tempo de resposta adequado 
| RNF-05 | O sistema deve possuir alta disponibilidade para uso contínuo pelos usuários autorizados
| RNF-06 | O sistema deve ser de fácil usabilidade
| RNF-07 | O sistema deve ser escalável e de fácil manutenção
| RNF-08 | O sistema deve ser compatível com navegadores modernos

### Restrições

As questões que limitam a execução desse projeto e que se configuram como obrigações claras para o desenvolvimento do projeto em questão são apresentadas na tabela a seguir.

| ID  | Descrição                                                                                     |
|-----|---------------------------------------------------------------------------------------------|
| RE-01 | O sistema é de uso exclusivo da Pontifícia Universidade Católica de Minas Gerais |
| RE-02 | O projeto deverá seguir o cronograma acadêmico definido pela instituição |
| RE-03 | A equipe não pode subcontratar o desenvolvimento do trabalho |
| RE-04 | O acesso ao sistema é restrito a usuários devidamente autorizados |
| RE-05 | Não é permitida a utilização de dados sensíveis sem autorização institucional |
