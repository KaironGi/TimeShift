# TAP — TimeShift 

### 1. Identificação do Projeto 

Nome: TimeShift — Sistema Inteligente de Redistribuição do Tempo Digital 
Área: Tecnologia, Ciência de Dados e Bem-Estar Digital 
Tipo: Projeto de desenvolvimento de software baseado em dados
Gerente do Projeto: Kairon Giron 
Status atual: Planejamento e documentação para desenvolvimento 

### 2. Objetivo do Projeto 

O TimeShift tem como objetivo desenvolver um sistema inteligente capaz de 
analisar padrões de comportamento digital e auxiliar o usuário na 
redistribuição consciente do seu tempo, considerando seus objetivos pessoais 
e sua rotina. 
A proposta não consiste simplesmente em reduzir o tempo de utilização das redes 
sociais. O sistema deverá utilizar informações sobre o comportamento digital do 
usuário para identificar padrões e apresentar oportunidades de reorganização do 
tempo de acordo com objetivos definidos pelo próprio usuário, como: 
• estudos;  
• exercícios físicos;  
• projetos pessoais;  
• atividades profissionais;  
• descanso;  
• outras atividades relevantes.  
O sistema deverá atuar como uma ferramenta de consciência e apoio à tomada 
de decisão, e não como mecanismo de controle ou diagnóstico. 

### 3. Situação Atual do Projeto 

O projeto encontra-se em uma etapa posterior à pesquisa e validação 
experimental. 
As etapas de investigação relacionadas ao conjunto de dados e à aplicação inicial 
de Machine Learning já foram realizadas. 
Foram analisados 4.500 registros e 15 variáveis relacionadas a aspectos como: 
• utilização de redes sociais;  
• sono;  
• estresse;  
• saúde mental;  
• desempenho acadêmico.  
A variável-alvo Overall_Impact apresentou três classificações: 
• Beneficial  
• Neutral  
• Negative  
Foi utilizado um modelo Support Vector Machine (SVM) com kernel RBF, 
utilizando 80% dos dados para treinamento e 20% para avaliação. 
Os resultados obtidos foram: 
Métrica 
Resultado 
Registros 
Variáveis 
Treinamento 
Teste 
Acurácia 
4.500 
15 
3.600 registros 
900 registros 
96,67% 
F1-Score Macro 93,32% 
A análise descritiva também identificou diferenças no uso diário médio das redes 
sociais entre as categorias: 
Classificação Uso médio diário 
Beneficial 
Neutral 
Negative 
4,42 h 
8,50 h 
12,25 h 
Os resultados indicaram a existência de padrões relevantes entre 
comportamento digital e impacto na rotina, fornecendo uma base quantitativa 
para a proposta do sistema. 
Esses resultados representam uma associação observada nos dados utilizados e 
não estabelecem causalidade. 

### 4. Justificativa 

A utilização crescente de tecnologias digitais tornou o gerenciamento do tempo 
uma questão relevante para usuários que precisam conciliar redes sociais, 
estudos, trabalho, atividades físicas, projetos pessoais e descanso. 
O problema identificado não está necessariamente no uso das redes sociais em 
si, mas na dificuldade de compreender como o tempo digital está distribuído e 
como esse comportamento se relaciona com outras atividades da rotina. 
Atualmente, muitas soluções trabalham principalmente com métricas simples de 
tempo de tela ou bloqueio de aplicativos. 
O TimeShift propõe uma abordagem diferente: utilizar dados comportamentais 
para identificar padrões e transformar essas informações em recomendações 
contextualizadas, considerando os objetivos definidos pelo próprio usuário. 
A pesquisa experimental realizada durante a concepção do projeto apresentou 
resultados que sustentam a continuidade da investigação e o desenvolvimento de 
uma prova de conceito. 
Dessa forma, a criação do TimeShift é justificada pela oportunidade de 
transformar os resultados obtidos na etapa de pesquisa em uma solução de 
software capaz de aplicar esses conceitos em um contexto de utilização 
prática. 

### 5. Principais Metas do Projeto 

Agora sim, aqui devemos separar o que já foi alcançado do que o projeto 
pretende alcançar daqui para frente. 
Meta 1 — Consolidar os resultados da pesquisa 
Status: Concluída. 
Documentar os resultados obtidos na análise dos dados e no experimento 
utilizando Machine Learning, estabelecendo a fundamentação quantitativa do 
projeto. 
Meta 2 — Transformar a pesquisa em uma solução de software 
Status: Próxima etapa. 
Utilizar os conhecimentos obtidos durante a pesquisa para desenvolver o sistema 
TimeShift. 
O objetivo é transformar: 
dados → padrões → interpretação → reorganização do tempo 
em funcionalidades concretas. 
Meta 3 — Permitir definição de objetivos pessoais 
O sistema deverá permitir que o usuário estabeleça objetivos para os quais deseja 
direcionar seu tempo, como: 
• estudar;  
• treinar;  
• desenvolver projetos;  
• trabalhar;  
• descansar;  
• aprender novas habilidades.  
Isso é fundamental porque o TimeShift não deve simplesmente recomendar: 
"Use menos redes sociais." 
A proposta é algo mais próximo de: 
"Você possui determinado padrão de utilização digital. Considerando o objetivo 
que definiu, existem oportunidades de redistribuição desse tempo." 
Meta 4 — Desenvolver um mecanismo de análise personalizada 
O sistema deverá evoluir da análise genérica realizada no dataset para uma 
abordagem capaz de trabalhar com dados e objetivos individuais. 
Essa é uma diferença importante entre a pesquisa já realizada e o software que 
vamos construir. 
O dataset respondeu: 
"Existem padrões gerais nos dados?" 
O TimeShift deverá buscar responder: 
"O que esses padrões significam para este usuário específico?" 
Meta 5 — Desenvolver um protótipo funcional 
A primeira versão deverá priorizar: 
simplicidade + funcionamento + validação da ideia.
Meta 6 — Validar a utilização prática 
Após o desenvolvimento inicial, avaliar se o sistema consegue transformar os 
dados disponíveis em informações compreensíveis e úteis para o usuário. 
Essa etapa será necessária porque um modelo com 96,67% de acurácia não 
significa automaticamente que o produto será útil. 
Essa distinção precisa permanecer explícita na documentação. 

### 6. Entregáveis 

Documentação 
• Termo de Abertura do Projeto;  
• Matriz RACI;  
• definição dos stakeholders;  
• requisitos;  
• escopo;  
• riscos;  
• cronograma;  
• arquitetura;  
• regras de negócio;  
• casos de uso;  
• critérios de aceitação.  
Sistema 
• estrutura inicial do projeto;  
• backend;  
• banco de dados;  
• lógica de processamento;  
• mecanismo de análise;  
• interface;  
• sistema de objetivos;  
• mecanismo de recomendações;  
• dashboard/visualização;  
• testes.  

### 7. Escopo de Alto Nível 

Dentro do escopo 
O TimeShift deverá contemplar: 
• cadastro/autenticação do usuário;  
• registro ou obtenção dos dados necessários;  
• processamento das informações;  
• análise dos padrões;  
• definição de objetivos pessoais;  
• comparação entre comportamento atual e objetivos;  
• identificação de oportunidades de redistribuição;  
• apresentação dos resultados;  
• histórico das análises;  
• acompanhamento da evolução.  
Fora do escopo inicial 
Não fará parte da primeira versão: 
• diagnóstico médico;  
• diagnóstico psicológico;  
• tratamento de dependência digital;  
• prescrição terapêutica;  
• controle compulsório de aplicativos;  
• bloqueio obrigatório de redes sociais;  
• integração com todas as plataformas existentes;  
• substituição de profissionais de saúde.  

### 8. Critérios de Sucesso 

O projeto será considerado bem-sucedido quando: 
1. O sistema estiver funcional.  
2. O fluxo principal puder ser executado de ponta a ponta.  
3. O usuário puder definir seus próprios objetivos.  
4. O sistema conseguir analisar os dados disponíveis.  
5. Os resultados forem apresentados de forma compreensível.  
6. As recomendações estiverem relacionadas aos objetivos definidos pelo 
usuário.  
7. O sistema não apresentar conclusões causais a partir de correlações.  
8. A arquitetura permitir evolução futura.  
9. A solução puder ser submetida a testes com usuários reais em uma etapa 
posterior.  

### 9. Principais Riscos 

Risco 
Transformar correlação em 
causalidade 
Recomendações genéricas 
Escopo excessivo 
Dados reais insuficientes 
Baixo engajamento 
Interface complexa 
Dependência excessiva do 
modelo ML 
Problemas de privacidade 
Impacto Estratégia 
Alto 
Alto 
Alto 
Alto 
Restringir linguagem e regras de 
interpretação 
Baseá-las nos objetivos individuais 
Definir MVP 
Separar modelo experimental de 
aplicação futura 
Médio/Alto Planejar feedback e 
acompanhamento 
Médio 
Alto 
Alto 
Priorizar clareza 
Separar ML, regras de negócio e 
apresentação 
Minimizar e proteger dados pessoais 
