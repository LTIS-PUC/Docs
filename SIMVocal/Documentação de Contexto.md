# Documentação de Contexto

 A simulação clínica é uma metodologia ativa essencial na formação de profissionais de saúde, permitindo o treinamento seguro de habilidades técnicas e comportamentais em ambientes controlados. Simuladores físicos de alta fidelidade, como os manequins desenvolvidos pela Laerdal, são amplamente utilizados nos laboratórios e departamentos médicos universitários para reproduzir condições clínicas complexas por meio de sinais fisiológicos (frequência cardíaca, respiração, respostas a intervenções farmacológicas, entre outros).

 Apesar da alta fidelidade fisiológica, esses simuladores apresentam uma limitação significativa na dimensão da comunicação humana: a interação verbal com o paciente. A fala do manequim geralmente restringe-se a gemidos pré-gravados ou depende da intervenção manual direta de um ator, que precisa atuar improvisando a "voz" do paciente durante a prática.

 O SIMVocal (Simulador Interativo Médico Vocal) foi idealizado para suprir essa lacuna tecnológica. O sistema integra-se ao ambiente de simulação clínica permitindo o cadastro de casos clínicos estruturados com árvores de respostas pré-definidas. Dessa forma, o simulador passa a interagir verbalmente com os alunos de forma padronizada, respondendo a perguntas essenciais para a anamnese e diagnóstico, elevando o realismo e o rigor da avaliação médica.

# Problema

O diagnóstico médico depende fundamentalmente de uma anamnese bem executada. Contudo, os simuladores clínicos tradicionais, ao não possuírem um sistema nativo de respostas estruturadas, geram os seguintes desafios:

## Ausência de Automação Verbal Estruturada: 
Os manequins não respondem autonomamente a perguntas vitais formuladas pelos alunos (ex: "Qual o seu nome?", "Onde dói?").

## Falta de Padronização Avaliativa: 
Quando o instrutor improvisa as respostas verbalmente, turmas diferentes podem receber informações com níveis de detalhamento distintos para o mesmo caso clínico, prejudicando a isonomia da avaliação.

## Sobrecarga da Equipe Docente: 
A necessidade de o professor atuar duplamente como avaliador e "ator" (voz do paciente) divide a atenção durante a simulação.

## Inviabilidade de IA Generativa Aberta: 
O uso de respostas 100% automatizadas geradas por IA em tempo real apresenta risco de "alucinações" (invenção de sintomas não previstos), o que invalidaria o cenário clínico planejado.

# Objetivos

# Objetivo Geral
Desenvolver uma plataforma de software (cliente-servidor) que permita o cadastro, gerenciamento e execução de casos clínicos com respostas verbais pré-definidas, dotando simuladores físicos da capacidade de responder de forma padronizada às perguntas dos alunos em tempo real.

# Objetivos Específicos
## Gerenciamento de Casos: 
Fornecer uma interface para o cadastro de cenários clínicos por parte dos professores.

## Mapeamento de Gatilhos e Respostas: 
Permitir o vínculo entre perguntas esperadas (gatilhos) e respostas específicas pré-cadastradas (em áudio ou texto sintetizado) para garantir a padronização.

## Captura de Áudio Local: 
Implementar um cliente local capaz de captar a voz do aluno de forma clara durante o cenário.

## Processamento e Correspondência: 
Estabelecer uma comunicação assíncrona onde a API recebe a pergunta do aluno, identifica a intenção e aciona a resposta exata planejada no roteiro.

## Padronização Educacional: 
Facilitar a reutilização de cenários por diferentes professores, garantindo uniformidade nas práticas laboratoriais.

# Objetivos específicos

Criar e manter um banco institucional de questões avaliativas;

Permitir o cadastro, edição, visualização e exclusão de questões;

Possibilitar a categorização das questões por disciplinas, conteúdos e objetivos de aprendizagem;

Facilitar a criação de provas e simulados de forma estruturada;

Permitir a organização das questões por níveis de dificuldade ou competências avaliadas;

Apoiar a criação de simulados voltados à preparação para exames como o ENAMED;

Oferecer uma interface intuitiva que facilite o uso do sistema pelos profissionais responsáveis pela elaboração das avaliações.

# Justificativa

A comunicação empática e a coleta precisa de informações são pilares da prática em saúde. Treinar a intervenção fisiológica sem treinar a abordagem ao paciente resulta em uma formação clínica fragmentada.

O SIMVocal inova ao transformar o manequim em um paciente interativo de forma controlada. A escolha por respostas pré-definidas garante a segurança pedagógica necessária para o ambiente universitário. Além do ganho imersivo para o aluno, a plataforma otimiza o tempo dos professores, cria um repositório centralizado de casos para a instituição e garante que todos os estudantes sejam avaliados sob o mesmo rigor e roteiro de informações.

O Gemini disse
Verdade, Carlos! Faltou mesmo essa seção fundamental para fechar o documento com chave de ouro.

Como o sistema vai rodar dentro de um contexto educacional bem específico (laboratórios de simulação realística em departamentos médicos universitários), o público-alvo precisa deixar claro quem opera o sistema no backend e quem interage com ele na prática.

Aqui está o bloco do Público-alvo formatado no mesmo padrão do restante da documentação para você adicionar logo após a "Justificativa":

# Público-alvo

O público-alvo do SIMVocal é composto por dois perfis distintos que atuam no ecossistema de simulação realística universitária:

## 1. Usuários Operacionais e Gestores (Interação com a Interface/API):

Professores e Instrutores Clínicos: Docentes responsáveis por planejar as aulas práticas, estruturar as anamneses e cadastrar as árvores de perguntas e respostas pré-definidas para cada cenário clínico.

Técnicos e Analistas de Laboratório de Simulação: Profissionais de tecnologia e apoio operacional que preparam os manequins da Laerdal, garantem a comunicação do cliente local (C++) com a API e ativam os casos clínicos no sistema antes do início das aulas.

Coordenadores Acadêmicos: Gestores que buscam padronizar as avaliações práticas (como o OSCE - Exame Clínico Objetivo Estruturado) e consolidar um banco institucional de casos clínicos padronizados.

## 2. Beneficiários Finais (Interação por Voz):

Estudantes da Área da Saúde (Medicina, Enfermagem e afins): Alunos que realizam o treinamento prático presencial. Eles interagem verbalmente com o manequim, formulando perguntas essenciais para o diagnóstico e ouvindo as respostas automatizadas, com o objetivo de aprimorar suas habilidades de comunicação, empatia e raciocínio clínico sob pressão.
