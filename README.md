# LABORATÓRIO DE PROGRAMAÇÃO


Automação da conciliação e do suporte no sistema DigitalConsig com IA
Visão geral
Esta proposta apresenta um projeto de automação para a empresa DigitalCard, responsável pelo sistema DigitalConsig, com foco em dois pontos centrais observados no estágio: a conciliação de valores consignados e o suporte operacional aos usuários.[file:1] O objetivo geral é propor um sistema automatizado para reduzir erros, tempo de execução e demanda repetitiva de atendimento, combinando rotinas de software, automação de processos e um assistente de suporte com IA.[file:1][cite:10]
Título
Automação da conciliação e do suporte no sistema DigitalConsig com IA.
Objetivo geral
Propor um sistema automatizado para reduzir erros, tempo de execução e demanda repetitiva de atendimento no DigitalConsig, por meio da automação da conciliação financeira e da implantação de um assistente virtual com IA para suporte aos usuários.[file:1][cite:8][cite:13]
Justificativa
O relatório de estágio mostra que a rotina operacional da empresa envolve tarefas críticas e repetitivas, especialmente na conferência de holerites, tratamento de arquivos enviados pelo RH, comparação de valores em planilhas, importação para o sistema e ajuste de divergências antes da liberação para bancos e prefeituras.[file:1] O mesmo relatório informa que o suporte técnico ocorre todos os dias, incluindo recuperação de senhas, dúvidas operacionais, problemas de login, margens negativas e apoio a consignatárias na emissão de relatórios.[file:1]
Esse cenário cria um ambiente com alta dependência de trabalho manual, atenção constante e risco operacional, tanto que o relatório afirma que divergências não corrigidas podem gerar prejuízo financeiro e que o atendimento simultâneo à conciliação compromete a concentração da equipe.[file:1] Além disso, o próprio documento recomenda uma central de ajuda mais robusta e automatizada, com portal de autoatendimento e separação entre atendimento e conciliação, o que reforça a pertinência de uma solução tecnológica para esse contexto.[file:1]
Descrição da solução
A solução proposta é composta por dois módulos integrados, que podem ser implantados de forma gradual para reduzir riscos e facilitar a adoção interna.[file:1]
Módulo 1: automação da conciliação
Este módulo automatiza a leitura dos arquivos enviados pelo RH, o tratamento dos dados, a comparação com os registros do DigitalConsig e a geração de relatórios de divergências.[file:1] Na prática, o sistema receberia arquivos TXT ou CSV, estruturaria os dados automaticamente, validaria campos essenciais, compararia valores de empréstimos, margens e identificação de servidores, e sinalizaria inconsistências para análise humana apenas nos casos necessários.[file:1][cite:10][cite:16]
As principais funções desse módulo seriam:
Importação automática de arquivos do RH.
Padronização e limpeza dos dados.
Cruzamento com dados já existentes no sistema.
Identificação de divergências de valores, cadastro e margem.
Emissão de relatório para conferência e liberação final.
Histórico das inconsistências para auditoria.
A literatura sobre RPA aplicada à reconciliação mostra que a automação dessas rotinas tende a melhorar precisão, velocidade e padronização, além de liberar os profissionais para análise de exceções em vez de repetir tarefas operacionais.[cite:10][cite:13][cite:16]
Módulo 2: assistente de suporte com IA/chatbot
Este módulo é o foco principal da proposta complementar e consiste em um chatbot treinado com a base de conhecimento da empresa para responder dúvidas frequentes de servidores públicos, consignatárias e operadores internos.[file:1] Pelo relatório, grande parte dos atendimentos está ligada a temas recorrentes, como recuperação de senha, problemas de acesso, margem negativa, dúvidas sobre relatórios e uso geral do sistema.[file:1]
O chatbot poderia funcionar em um portal web, WhatsApp corporativo ou área interna do DigitalConsig, com respostas guiadas e linguagem simples.[cite:8][cite:14] Em casos simples, a IA resolveria o problema de forma imediata; em casos mais complexos, o sistema abriria chamado e encaminharia o atendimento para um colaborador humano, com resumo automático da conversa.[cite:8][cite:11]
As principais funções do módulo seriam:
Responder dúvidas frequentes 24 horas por dia.
Orientar recuperação de senha e procedimentos de login.
Explicar motivos comuns para margem negativa.
Guiar emissão de relatórios e uso de funções básicas.
Abrir chamados automaticamente quando necessário.
Sugerir artigos de ajuda com base na pergunta do usuário.
Registrar histórico de atendimentos para análise futura.
Soluções de atendimento com IA são adotadas justamente para reduzir filas, padronizar respostas e melhorar o tempo médio de resolução em demandas repetitivas.[cite:8][cite:11][cite:14]
Tecnologias sugeridas
A proposta pode ser implementada com tecnologias acessíveis e compatíveis com um projeto acadêmico aplicado.
Camada	Tecnologias indicadas	Finalidade
Tratamento de dados	Python, Pandas	Ler, limpar, comparar e validar arquivos da conciliação
Automação de tarefas	Power Automate, UiPath ou scripts Python	Automatizar importações, rotinas repetitivas e notificações
Banco de dados	PostgreSQL ou MySQL	Armazenar usuários, logs, divergências e histórico de suporte
IA conversacional	OpenAI API, Azure AI ou Dialogflow	Interpretar perguntas e responder com base na base de conhecimento
Interface web	Flask, Django ou Streamlit	Disponibilizar painel, chatbot e relatórios
Integração	API REST ou conexão com banco interno	Comunicação com o DigitalConsig e demais rotinas
Python é especialmente indicado porque permite rápida prototipagem, integração com planilhas e criação de regras de negócio para comparação de dados.[cite:10] Já o uso de RPA é recomendado quando a empresa precisa automatizar tarefas repetitivas em sistemas já existentes sem alterar profundamente a infraestrutura atual.[cite:13][cite:16]
Viabilidade técnica e financeira
A proposta é tecnicamente viável porque o processo já está mapeado no relatório e possui entradas bem definidas, como arquivos do RH, planilhas tratadas e verificações recorrentes no sistema DigitalConsig.[file:1] Isso reduz a complexidade do projeto, já que a automação seria aplicada sobre um fluxo conhecido, em vez de exigir a criação de um processo totalmente novo.[file:1]
Do ponto de vista financeiro, a viabilidade também é favorável, principalmente se a implantação ocorrer por etapas e com ferramentas de baixo custo inicial.[cite:10][cite:13] Um protótipo funcional pode ser criado com software livre, banco de dados gratuito e interface web simples, deixando integrações mais avançadas e escalabilidade para uma segunda fase.[cite:10]
A adoção gradual melhora a aceitação da equipe e reduz riscos de parada operacional. Esse modelo também facilita testes controlados, validação com usuários reais e mensuração de ganhos antes de novos investimentos.[file:1]
Custos estimados
Os custos podem ser divididos em três cenários, o que ajuda a demonstrar maturidade da proposta e adequação à realidade da empresa.
Cenário	Estrutura	Faixa estimada
Baixo custo	Python, banco open source, chatbot básico com perguntas frequentes, interface web simples	Baixo investimento inicial, concentrado em desenvolvimento interno
Custo intermediário	Inclusão de API de IA, hospedagem em nuvem, automações com RPA e painel gerencial	Investimento moderado com melhor escalabilidade
Custo mais alto	Integração completa com sistemas internos, múltiplos canais de atendimento, analytics e segurança ampliada	Investimento maior, indicado para expansão futura
Para fins acadêmicos, o cenário mais adequado é o de baixo custo, com protótipo funcional e viabilidade comprovada.[cite:10] O principal custo real tende a estar nas horas de desenvolvimento, documentação, testes e eventual consumo de API de IA, enquanto as ferramentas centrais podem ser gratuitas ou acessíveis em planos iniciais.[cite:8][cite:13]
Benefícios esperados
A implementação da solução deve gerar ganhos operacionais, financeiros e de qualidade no atendimento.
Redução do tempo gasto na conciliação manual.[file:1][cite:10]
Diminuição de erros causados por cansaço, interrupções e conferências repetitivas.[file:1][cite:13]
Melhoria do foco da equipe durante períodos críticos de fechamento e validação.[file:1]
Atendimento mais rápido e padronizado para dúvidas frequentes.[cite:8][cite:11]
Disponibilidade de suporte fora do horário comercial para questões simples.[cite:8][cite:14]
Criação de histórico para auditoria, indicadores e melhoria contínua.[cite:11][cite:13]
Maior satisfação dos usuários do sistema, com menos dependência de atendimento manual.[cite:11][cite:14]
Além desses benefícios, a proposta fortalece a governança do processo, pois transforma conhecimento tácito da equipe em regras documentadas e fluxos automatizados.[file:1][cite:13]
Cronograma de implantação
A implantação pode ser feita em etapas curtas, com foco em validação contínua.
Fase	Duração estimada	Atividades principais
1. Levantamento	1 a 2 semanas	Mapear fluxos, arquivos, regras de negócio e dúvidas frequentes
2. Protótipo da conciliação	2 a 4 semanas	Criar importação, tratamento e comparação automática dos dados
3. Base de conhecimento	1 a 2 semanas	Estruturar perguntas frequentes, fluxos e respostas do chatbot
4. Protótipo do chatbot	2 a 3 semanas	Implantar assistente em ambiente de teste com respostas guiadas
5. Integração e testes	2 semanas	Validar com usuários, medir erros, tempo e taxa de resolução
6. Implantação gradual	1 a 2 semanas	Colocar em produção por grupos ou processos específicos
7. Monitoramento	Contínuo	Ajustar regras, ampliar base de conhecimento e acompanhar indicadores
Esse cronograma é compatível com um projeto de implantação incremental e permite entregar valor já nas primeiras fases, especialmente se o primeiro foco for a automação da conciliação e o segundo a triagem do suporte.[file:1]
Conclusão
A proposta de automação da conciliação e do suporte no sistema DigitalConsig com IA é adequada ao contexto descrito no relatório de estágio, porque responde diretamente aos problemas observados na rotina da empresa: excesso de trabalho manual, alta repetição de atendimentos, risco de erro e sobrecarga operacional.[file:1] Ao combinar tratamento automatizado de dados, RPA, banco de dados, interface web e assistente virtual com IA, o projeto se mostra tecnicamente viável, financeiramente escalável e academicamente relevante.[cite:8][cite:10][cite:13]
Como trabalho de faculdade, a proposta é forte porque parte de uma necessidade real da empresa, aplica conceitos de Sistemas de Informação e demonstra como IA e software podem gerar melhoria concreta em processos organizacionais.[file:1]
