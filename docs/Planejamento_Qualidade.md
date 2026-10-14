# Plano de Gerenciamento da Qualidade — TimeShift

## 1. Objetivo

O objetivo deste plano é definir critérios, procedimentos e práticas para assegurar a qualidade do desenvolvimento do TimeShift — Sistema Inteligente de Redistribuição do Tempo Digital.

O gerenciamento da qualidade busca garantir que o sistema atenda aos requisitos definidos, apresente comportamento consistente, utilize adequadamente os dados disponíveis e ofereça funcionalidades coerentes com seus objetivos.

A qualidade será considerada durante todo o ciclo de desenvolvimento, desde o planejamento e a definição dos requisitos até a implementação, os testes e a validação do sistema.

## 2. Escopo do Gerenciamento da Qualidade

O gerenciamento da qualidade abrangerá os seguintes aspectos:

- **Qualidade funcional:** verificar se as funcionalidades implementadas atendem aos requisitos estabelecidos.
- **Qualidade técnica:** avaliar a organização, a legibilidade, a manutenção e a confiabilidade do código.
- **Qualidade dos dados:** verificar consistência, integridade, tratamento de valores ausentes e limitações do conjunto de dados utilizado.
- **Qualidade do modelo de Machine Learning:** avaliar o desempenho e a capacidade de generalização do modelo por meio de métricas apropriadas.
- **Qualidade das recomendações:** verificar se as sugestões geradas são coerentes com os objetivos informados pelo usuário e com as limitações dos dados.
- **Segurança e privacidade:** considerar medidas de proteção das informações e os requisitos aplicáveis de proteção de dados pessoais.
- **Usabilidade:** avaliar a clareza da interface, a facilidade de navegação e a compreensão dos resultados apresentados.
- **Documentação:** manter os documentos técnicos e de planejamento atualizados e consistentes com a implementação.

A avaliação será proporcional ao estágio de desenvolvimento do projeto e às funcionalidades efetivamente implementadas.

## 3. Responsabilidades

O responsável pelo projeto deverá coordenar as atividades de gerenciamento da qualidade, incluindo a definição dos critérios de aceitação, a execução ou organização dos testes, o registro dos resultados e o tratamento das não conformidades identificadas.

Caso novos integrantes sejam incorporados ao projeto, as responsabilidades poderão ser distribuídas conforme suas atribuições.

As atividades de qualidade deverão ser registradas de forma que seja possível identificar os critérios utilizados, os resultados obtidos e as correções realizadas.

## 4. Processo de Gerenciamento da Qualidade

### 4.1 Planejamento da qualidade

O planejamento da qualidade será realizado com base nos requisitos, no escopo e nos objetivos definidos para o TimeShift.

Para cada funcionalidade relevante, deverão ser estabelecidos critérios de aceitação que permitam verificar objetivamente se o resultado atende ao comportamento esperado.

Os critérios deverão ser definidos antes da conclusão das funcionalidades, sempre que possível, reduzindo ambiguidades e evitando que a avaliação dependa exclusivamente de julgamentos subjetivos.

### 4.2 Garantia da qualidade

A garantia da qualidade compreenderá práticas preventivas destinadas a reduzir a ocorrência de falhas durante o desenvolvimento.

Serão consideradas as seguintes práticas:

- Manter uma estrutura de código organizada e responsabilidades bem definidas entre os componentes.
- Adotar padrões consistentes de nomenclatura, formatação e documentação.
- Utilizar controle de versão para acompanhar as alterações realizadas no projeto.
- Revisar os requisitos antes da implementação das funcionalidades.
- Registrar decisões técnicas relevantes e limitações conhecidas.
- Verificar se as alterações permanecem alinhadas ao escopo aprovado.
- Planejar testes para as funcionalidades e os componentes críticos.

A adoção de ferramentas específicas de análise estática, integração contínua ou automação de testes dependerá das necessidades técnicas e da evolução do projeto.

### 4.3 Controle da qualidade

O controle da qualidade será realizado por meio da verificação dos resultados produzidos durante o desenvolvimento.

As atividades poderão incluir:

- Testes funcionais das funcionalidades implementadas.
- Testes unitários para componentes com regras de negócio relevantes.
- Testes de integração entre componentes.
- Verificação do tratamento de erros e entradas inválidas.
- Avaliação da consistência dos dados processados.
- Testes de segurança compatíveis com a arquitetura e os dados tratados.
- Verificação da documentação em relação ao comportamento real do sistema.

Os resultados deverão ser registrados, e as falhas identificadas deverão ser corrigidas e submetidas a novos testes antes da aprovação da funcionalidade afetada.

## 5. Critérios de Qualidade

Os seguintes critérios serão utilizados como referência para avaliar a qualidade do TimeShift.

### 5.1 Requisitos funcionais

As funcionalidades deverão apresentar o comportamento especificado nos requisitos e respeitar os limites definidos para a versão em desenvolvimento.

**Critérios de aceitação:**
- Os fluxos principais executam conforme o comportamento esperado.
- As entradas inválidas ou incompletas recebem tratamento adequado.
- Os resultados apresentados correspondem às informações processadas.
- As funcionalidades não introduzem comportamentos incompatíveis com os requisitos existentes.

### 5.2 Qualidade do código

O código deverá favorecer a legibilidade, a manutenção e a separação adequada de responsabilidades.

**Critérios de aceitação:**
- Os componentes possuem responsabilidades identificáveis.
- As regras de negócio não são duplicadas desnecessariamente.
- Os erros relevantes são tratados explicitamente.
- As alterações podem ser rastreadas pelo controle de versão.
- Os componentes críticos possuem testes compatíveis com seus riscos e complexidade.

### 5.3 Qualidade dos dados

Os dados utilizados pelo modelo e pelas funcionalidades deverão passar por verificações de consistência e integridade.

**Critérios de aceitação:**
- Valores ausentes são identificados e tratados de forma documentada.
- Tipos de dados e categorias são verificados.
- Possíveis duplicidades e inconsistências são avaliadas.
- O processamento não utiliza informações indisponíveis ou inválidas sem tratamento.
- As limitações e a origem dos dados são documentadas.

A qualidade dos dados será considerada uma condição necessária para a interpretação dos resultados do modelo.

### 5.4 Qualidade do modelo de Machine Learning

O modelo deverá ser avaliado com métricas adequadas à tarefa de classificação e às características dos dados utilizados.

**Critérios de aceitação:**
- O treinamento e a avaliação utilizam conjuntos de dados separados adequadamente.
- O processamento dos dados evita vazamento de informações entre treinamento e avaliação.
- São consideradas métricas como acurácia, precisão, revocação e F1-score.
- O desempenho por classe é analisado para identificar possíveis desequilíbrios.
- Os resultados e as limitações do modelo são documentados.

A acurácia de 96,67% obtida no estudo preliminar com SVM será tratada como um resultado experimental, não como garantia de desempenho na aplicação final.

Os limites mínimos de desempenho deverão ser definidos após a consolidação dos requisitos e a avaliação das consequências de erros de classificação. Nenhuma métrica isolada será considerada suficiente para comprovar a qualidade do produto.

### 5.5 Qualidade das recomendações

As recomendações deverão apoiar a redistribuição consciente do tempo digital, respeitando os objetivos informados pelo usuário e as limitações dos dados disponíveis.

**Critérios de aceitação:**
- As recomendações seguem regras de negócio documentadas.
- Os resultados são apresentados de forma compreensível.
- O sistema não apresenta inferências estatísticas como certezas individuais.
- As sugestões não são tratadas como diagnósticos médicos ou psicológicos.
- O usuário mantém autonomia para avaliar e decidir se deseja seguir as sugestões.

### 5.6 Segurança e privacidade

A aplicação deverá considerar a proteção das informações processadas e os riscos relacionados ao acesso, armazenamento e exposição de dados.

**Critérios de aceitação:**
- O acesso a funcionalidades e informações é compatível com as permissões definidas.
- Informações sensíveis não são expostas desnecessariamente em mensagens de erro ou registros.
- Os dados coletados são limitados às necessidades justificadas do sistema.
- Os procedimentos de armazenamento, retenção e exclusão são definidos quando houver tratamento de dados pessoais.
- Os requisitos aplicáveis da Lei Geral de Proteção de Dados Pessoais (LGPD) são considerados.

As medidas específicas deverão ser ajustadas à arquitetura adotada e ao tipo de informação efetivamente tratado.

### 5.7 Usabilidade e acessibilidade

A interface deverá permitir que o usuário compreenda as funcionalidades, navegue pelos fluxos principais e interprete os resultados apresentados.

**Critérios de aceitação:**
- Os principais fluxos podem ser executados sem ambiguidades relevantes.
- Os textos, mensagens e instruções são claros.
- Os erros apresentados orientam o usuário sobre como proceder, quando aplicável.
- A interface considera legibilidade, contraste e navegação consistente.
- Aspectos de acessibilidade são avaliados durante os testes da interface.

### 5.8 Qualidade da documentação

A documentação deverá representar fielmente o estado atual do projeto.

**Critérios de aceitação:**
- Os documentos refletem o escopo e as decisões vigentes.
- As alterações relevantes são registradas.
- Os procedimentos de execução e teste são documentados quando aplicáveis.
- As limitações conhecidas são explicitadas.
- Os documentos de planejamento são revisados quando mudanças relevantes afetam suas definições.

## 6. Estratégia de Testes

Os testes serão conduzidos de forma progressiva, conforme os componentes e as funcionalidades forem implementados.

### 6.1 Testes unitários

Verificarão componentes isolados, especialmente funções de processamento de dados, validações e regras de negócio.

### 6.2 Testes de integração

Verificarão a comunicação entre componentes, incluindo o processamento dos dados, a aplicação das regras de negócio e a integração com o modelo de Machine Learning, quando implementada.

### 6.3 Testes funcionais

Verificarão se as funcionalidades atendem aos requisitos e aos critérios de aceitação definidos.

### 6.4 Testes de dados e do modelo

Verificarão o tratamento dos dados, a consistência do processamento e o desempenho do modelo por meio de métricas adequadas.

### 6.5 Testes de segurança e usabilidade

Avaliarão os controles de acesso e a exposição de informações, quando aplicáveis, além da clareza da interface e da compreensão dos resultados.

A seleção e a profundidade dos testes dependerão da implementação, da arquitetura e da criticidade de cada funcionalidade.

## 7. Tratamento de Não Conformidades

Uma não conformidade será caracterizada pela identificação de um resultado, comportamento ou artefato que não atenda a um requisito ou critério de qualidade definido.

Quando uma não conformidade for identificada, deverão ser realizadas as seguintes atividades:

1. Registrar a falha e o comportamento observado.
2. Identificar o requisito ou critério não atendido.
3. Avaliar a causa e os possíveis impactos.
4. Definir e implementar uma ação corretiva.
5. Executar novamente os testes pertinentes.
6. Registrar o resultado da correção.

Falhas que comprometam a segurança, a integridade dos dados ou o funcionamento dos fluxos essenciais deverão receber prioridade de tratamento.

## 8. Monitoramento e Indicadores de Qualidade

O monitoramento será realizado por meio de indicadores compatíveis com a etapa de desenvolvimento.

Poderão ser utilizados:

- **Taxa de aprovação nos testes:** proporção de testes executados com resultado satisfatório.
- **Quantidade de defeitos identificados:** número de falhas registradas durante os testes.
- **Taxa de resolução de defeitos:** proporção de defeitos corrigidos em relação aos defeitos registrados no período analisado.
- **Cobertura de testes:** proporção do código ou dos elementos definidos como relevantes que são exercitados pelos testes automatizados.
- **Métricas do modelo:** acurácia, precisão, revocação e F1-score.
- **Conformidade com os requisitos:** proporção dos requisitos avaliados que atendem aos critérios de aceitação.

Os indicadores deverão ser interpretados em conjunto. Uma alta taxa de aprovação, por exemplo, não garante a ausência de falhas se os testes forem insuficientes ou pouco representativos.

Metas quantitativas específicas serão estabelecidas quando houver requisitos consolidados e uma base de avaliação adequada.

## 9. Revisão e Atualização do Plano

Este plano deverá ser revisado durante a evolução do TimeShift, especialmente quando ocorrerem:

- Alterações relevantes no escopo ou nos requisitos.
- Mudanças na arquitetura ou nas tecnologias utilizadas.
- Integração de novos componentes.
- Identificação de falhas recorrentes.
- Mudanças nas características dos dados.
- Resultados insatisfatórios na avaliação do modelo.
- Identificação de novos requisitos de segurança, privacidade ou acessibilidade.

As revisões deverão manter o documento alinhado ao estado real do projeto e aos critérios de qualidade necessários para sua validação.

## 10. Considerações Finais

O gerenciamento da qualidade do TimeShift será conduzido de forma contínua, integrando prevenção, verificação, correção e melhoria.

O atendimento aos requisitos funcionais e técnicos será necessário, mas não suficiente para demonstrar a qualidade do sistema. A confiabilidade dos dados, as limitações do modelo, a coerência das recomendações, a proteção das informações e a experiência do usuário também deverão ser consideradas.

A aprovação de uma funcionalidade dependerá de critérios verificáveis e resultados registrados, evitando que a qualidade seja determinada apenas pela percepção subjetiva de que o sistema está funcionando.

Dessa forma, este plano servirá como referência para orientar o desenvolvimento e apoiar a avaliação da qualidade das entregas do TimeShift.