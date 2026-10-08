# 1. Visão Geral

### TimeShift: Sistema Inteligente de Redistribuição do Tempo Digital é uma proposta de sistema voltada à utilização mais consciente do tempo digital.
A solução pretende auxiliar o usuário a refletir sobre a distribuição de seu tempo entre atividades digitais e outras atividades de sua rotina, utilizando informações fornecidas pelo próprio usuário.
A proposta surgiu a partir de uma investigação exploratória realizada sobre 4.500 registros relacionados a comportamento digital, sono, estresse, saúde mental e desempenho acadêmico.
Os resultados dessa investigação serviram como base para a definição do problema e para a concepção do TimeShift.
Em sua primeira versão, o sistema não realizará integração automática com redes sociais, sistemas operacionais ou aplicativos externos.
Dessa forma, as informações utilizadas pelo protótipo serão fornecidas manualmente pelo usuário ou inseridas para fins de demonstração e validação da proposta.
Diferencial: em vez de simplesmente recomendar a redução do uso de redes sociais, o TimeShift propõe analisar a distribuição do tempo digital em relação aos objetivos
e à rotina do usuário, buscando identificar oportunidades de redistribuição desse tempo.
________________________________________

### 2. Funcionalidades Principais

Registro manual do tempo digital:
O usuário poderá informar o tempo dedicado a diferentes atividades digitais, como redes sociais, entretenimento, estudos ou outras categorias definidas pelo sistema.
Registro de informações da rotina:
O usuário poderá informar dados relacionados à sua rotina que sejam relevantes para a análise, como tempo de sono, nível de estresse e desempenho em atividades.
Visualização dos registros:
O sistema deverá apresentar os dados registrados pelo usuário por meio de indicadores e gráficos.
Identificação de padrões:
A solução poderá analisar os registros fornecidos pelo usuário e identificar padrões de distribuição do tempo digital.


Análise baseada em dados:
Os conceitos e critérios utilizados pelo sistema serão fundamentados na análise exploratória realizada durante o projeto e nos modelos de Machine Learning estudados.
Sugestões de redistribuição:
A partir das informações disponíveis, o sistema poderá apresentar sugestões de redistribuição do tempo, considerando as categorias e objetivos informados pelo usuário.
Acompanhamento da evolução:
O usuário poderá visualizar alterações em seus registros ao longo do tempo e acompanhar a evolução de seus hábitos.
________________________________________

### 3. Plataforma Alvo

Protótipo Web.
A primeira versão será desenvolvida como um protótipo web, sem integração automática com redes sociais, sistemas operacionais ou aplicativos externos.
________________________________________

### 4. Requisitos Técnicos
Análise e Processamento de Dados
Utilização de Python para processamento, exploração e preparação dos dados.
Possível utilização de bibliotecas como:
•	Pandas; 
•	NumPy; 
•	Scikit-learn; 
•	Matplotlib; 
•	SciPy, quando aplicável. 

Machine Learning
Utilização de algoritmos de aprendizado de máquina para classificação e análise dos padrões identificados.
O estudo realizado utiliza SVM para classificação dos impactos relacionados ao comportamento digital.

Backend
O protótipo deverá possuir uma camada responsável pelo processamento das informações, aplicação das regras de análise e integração com o modelo de Machine Learning.

Banco de Dados
Caso necessário para o protótipo, deverá ser utilizado banco de dados para armazenamento estruturado das informações do usuário, registros comportamentais e resultados das análises.

Interface
A interface deverá apresentar:
•	indicadores de comportamento digital; 
•	resultados das análises; 
•	padrões identificados; 
•	recomendações de redistribuição; 
•	evolução dos indicadores. 

Visualização de Dados
Os dados deverão ser apresentados por meio de gráficos, indicadores e outros recursos visuais que facilitem a interpretação dos resultados.

Segurança e Privacidade
A solução deverá considerar princípios de segurança e privacidade no tratamento dos dados, especialmente por envolver informações relacionadas a comportamento, bem-estar e rotina dos usuários.
Caso seja implementado como produto real, deverão ser avaliados requisitos de conformidade com a LGPD.

________________________________________

### 5. Modelo de Negócio

Não definido no escopo atual.
O TimeShift encontra-se, neste momento, em uma etapa acadêmica de pesquisa, planejamento e desenvolvimento de protótipo. Portanto, não será definido neste projeto um modelo comercial, preços ou planos de assinatura.
Uma eventual transformação do projeto em produto poderá avaliar posteriormente modelos como:
•	aplicação gratuita com recursos premium; 
•	assinatura; 
•	licenciamento; 
•	parceria com instituições de ensino; 
•	solução corporativa de bem-estar digital. 
Essas possibilidades não fazem parte do escopo atual.
________________________________________

### 6. Restrições e Limitações

•	NÃO haverá integração automática com redes sociais na primeira versão. 
•	NÃO haverá coleta automática de tempo de tela. 
•	NÃO haverá acesso automático aos aplicativos utilizados pelo usuário. 
•	NÃO haverá coleta automática de dados de smartphones ou computadores. 
•	NÃO haverá integração com APIs de redes sociais no escopo inicial. 
•	NÃO haverá integração com wearables na primeira versão. 
•	Os dados utilizados inicialmente serão informados manualmente pelo usuário ou utilizados em cenários de demonstração. 
•	Os resultados do estudo com 4.500 registros não representam necessariamente o comportamento individual de cada usuário. 
•	O sistema não realizará diagnóstico médico ou psicológico. 
•	O sistema não substituirá acompanhamento profissional. 
•	Os resultados não deverão ser interpretados como diagnóstico ou recomendação clínica. 
________________________________________

### 7. Perfis de Usuário
Usuário Final
Pessoa que utiliza o TimeShift para acompanhar seu comportamento digital, visualizar indicadores e receber recomendações relacionadas à redistribuição do seu tempo.
Administrador do Sistema
Responsável pelo gerenciamento técnico da aplicação, configurações do sistema e manutenção dos dados e serviços.
Pesquisador/Analista
Perfil destinado à análise dos dados, avaliação dos modelos e acompanhamento dos resultados da solução.
Para o protótipo acadêmico, esses perfis podem ser apenas conceituais. Não é necessário desenvolver um sistema completo de permissões caso isso não faça parte do escopo definido.
________________________________________

### 8. Futuras Atualizações

Integração com sistemas operacionais: coleta automática de tempo de tela e utilização de aplicativos.
Integração com redes sociais: possibilidade de utilização de dados disponibilizados por plataformas externas, quando tecnicamente possível e permitido.
Integração com dispositivos vestíveis: utilização de dados complementares provenientes de smartwatches e outros dispositivos.
Coleta automática de dados: substituição progressiva da entrada manual por mecanismos automatizados.
________________________________________
