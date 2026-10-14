# Plano de Gerenciamento de Riscos — TimeShift

**Projeto:** TimeShift — Sistema Inteligente de Redistribuição do Tempo Digital  
**Responsável:** Kairon Giron  
**Status:** Planejamento  
**Versão:** 1.0

## 1. Objetivo

Estabelecer procedimentos para identificar, analisar, priorizar, tratar e monitorar os riscos que possam comprometer o desenvolvimento, a qualidade, a segurança e os objetivos do TimeShift.

O gerenciamento de riscos busca antecipar problemas, reduzir seus impactos e apoiar decisões durante as etapas de pesquisa, desenvolvimento, integração e validação do sistema.

## 2. Escopo do gerenciamento de riscos

O gerenciamento contempla os riscos técnicos, relacionados aos dados, de segurança e privacidade, de qualidade, de produto e de execução do projeto.

O plano será aplicado desde o planejamento até a validação do protótipo, podendo ser atualizado conforme novas informações forem obtidas.

O TimeShift tem como objetivo analisar padrões de comportamento digital e auxiliar o usuário a redistribuir conscientemente seu tempo de acordo com objetivos pessoais. O sistema não tem como finalidade diagnosticar condições de saúde, substituir profissionais ou impor bloqueios compulsórios ao uso de plataformas digitais.

A integração direta com redes sociais e o acesso automático aos dados dessas plataformas não fazem parte do escopo inicial.

## 3. Metodologia

Os riscos serão identificados a partir da análise dos requisitos, das decisões arquiteturais, das características dos dados, das limitações técnicas e das atividades previstas no cronograma.

Cada risco será avaliado considerando dois critérios:

- **Probabilidade:** possibilidade de o risco ocorrer.
- **Impacto:** intensidade das consequências caso o risco se concretize.

A classificação será realizada por meio da multiplicação dos valores atribuídos aos dois critérios.

### 3.1 Escala de probabilidade e impacto

| Valor | Probabilidade | Impacto |
|---|---|---|
| 1 | Muito baixa | Insignificante |
| 2 | Baixa | Pequeno |
| 3 | Média | Moderado |
| 4 | Alta | Grave |
| 5 | Muito alta | Crítico |

### 3.2 Classificação dos riscos

O nível de risco será calculado pela fórmula:

**Nível de risco = Probabilidade × Impacto**

| Pontuação | Classificação | Tratamento |
|---|---|---|
| 1–4 | Baixo | Monitorar |
| 5–9 | Moderado | Planejar medidas preventivas |
| 10–16 | Alto | Priorizar ações de mitigação |
| 17–25 | Crítico | Exigir tratamento prioritário antes de prosseguir com a atividade afetada |

A classificação deverá ser reavaliada sempre que houver mudanças relevantes no projeto, nos requisitos ou nas condições técnicas.

## 4. Registro e análise dos riscos

Os riscos identificados para o TimeShift estão relacionados abaixo. As probabilidades representam estimativas iniciais de planejamento e deverão ser revisadas durante o desenvolvimento.

| ID | Risco identificado | Prob. | Impacto | Nível |
|---|---|---:|---:|---:|
| R01 | Dados insuficientes, inconsistentes ou pouco representativos | 4 | 4 | 16 — Alto |
| R02 | Modelo de Machine Learning com desempenho inadequado em novos dados | 3 | 5 | 15 — Alto |
| R03 | Interpretação incorreta de correlações como relações de causa e efeito | 3 | 5 | 15 — Alto |
| R04 | Recomendações incompatíveis com os objetivos ou a rotina do usuário | 3 | 4 | 12 — Alto |
| R05 | Exposição indevida de dados pessoais ou falhas de segurança | 2 | 5 | 10 — Alto |
| R06 | Aumento do escopo e inclusão prematura de funcionalidades | 4 | 3 | 12 — Alto |
| R07 | Atrasos no desenvolvimento e na validação do protótipo | 4 | 3 | 12 — Alto |
| R08 | Dificuldades na integração entre o modelo, as regras de negócio e a aplicação | 3 | 4 | 12 — Alto |
| R09 | Ausência de critérios adequados para validar a utilidade das recomendações | 3 | 4 | 12 — Alto |
| R10 | Dependência excessiva dos resultados de um único modelo ou conjunto de dados | 3 | 4 | 12 — Alto |

## 5. Estratégias de resposta aos riscos

### R01 — Qualidade e representatividade dos dados

**Estratégia:** Mitigar.

**Ações preventivas:**
- Verificar dados ausentes, inconsistências, duplicidades e distribuição das variáveis.
- Documentar a origem, as limitações e as características do conjunto de dados.
- Avaliar se os dados disponíveis representam adequadamente os cenários considerados pelo sistema.
- Evitar generalizações para populações ou situações que não tenham sido avaliadas.

**Resposta caso ocorra:** Revisar o tratamento dos dados, restringir as conclusões e avaliar a necessidade de dados adicionais.

### R02 — Desempenho inadequado do modelo

**Estratégia:** Mitigar.

**Ações preventivas:**
- Avaliar o modelo com métricas adequadas, incluindo precisão, revocação e F1-score, além da acurácia.
- Verificar possíveis problemas de sobreajuste, vazamento de dados e desequilíbrio entre classes.
- Manter a separação entre dados de treinamento e dados de avaliação.
- Comparar o SVM com alternativas quando houver justificativa técnica.

**Resposta caso ocorra:** Investigar as causas do desempenho insatisfatório, revisar o processamento e os parâmetros e reavaliar o modelo antes de utilizá-lo no sistema.

### R03 — Interpretação incorreta de correlações

**Estratégia:** Mitigar.

**Ações preventivas:**
- Diferenciar associações estatísticas de relações causais.
- Documentar as limitações das conclusões extraídas dos dados.
- Evitar afirmações que atribuam causalidade sem evidências apropriadas.
- Apresentar resultados como indicadores de apoio à reflexão, não como verdades definitivas sobre o usuário.

**Resposta caso ocorra:** Corrigir as interpretações e as mensagens apresentadas, revisando as conclusões afetadas.

### R04 — Recomendações inadequadas

**Estratégia:** Mitigar.

**Ações preventivas:**
- Considerar os objetivos pessoais informados pelo usuário.
- Permitir que o usuário avalie e ajuste as sugestões recebidas.
- Definir regras de negócio explícitas para geração das recomendações.
- Evitar recomendações prescritivas baseadas exclusivamente em classificações estatísticas.

**Resposta caso ocorra:** Revisar as regras de recomendação, identificar os cenários problemáticos e realizar novos testes.

### R05 — Segurança e privacidade

**Estratégia:** Mitigar.

**Ações preventivas:**
- Coletar apenas os dados necessários para as funcionalidades previstas.
- Definir controles de acesso e medidas de proteção compatíveis com os dados tratados.
- Evitar a exposição de informações pessoais em registros, mensagens de erro e documentação pública.
- Avaliar os requisitos aplicáveis da Lei Geral de Proteção de Dados Pessoais (LGPD).
- Definir regras de armazenamento, retenção e exclusão de dados antes de utilizar informações pessoais reais.

**Resposta caso ocorra:** Conter o incidente, avaliar os dados e sistemas afetados, corrigir a vulnerabilidade e cumprir os procedimentos de resposta e comunicação aplicáveis.

### R06 — Aumento do escopo

**Estratégia:** Evitar ou mitigar.

**Ações preventivas:**
- Utilizar o documento de escopo como referência para decisões de implementação.
- Registrar novas funcionalidades como propostas de alteração.
- Avaliar o impacto das alterações sobre prazo, complexidade e qualidade.
- Priorizar os requisitos essenciais para a primeira versão.

**Resposta caso ocorra:** Reavaliar as prioridades e adiar funcionalidades não essenciais, mantendo o foco nos objetivos definidos para o MVP.

### R07 — Atrasos no desenvolvimento

**Estratégia:** Mitigar.

**Ações preventivas:**
- Dividir o trabalho em tarefas menores, com critérios de conclusão verificáveis.
- Priorizar dependências técnicas e atividades de maior incerteza.
- Acompanhar o progresso em relação à lista de tarefas.
- Reservar tempo para correções, testes e documentação.

**Resposta caso ocorra:** Replanejar as atividades, revisar prioridades e ajustar as entregas sem eliminar etapas essenciais de validação.

### R08 — Dificuldades de integração

**Estratégia:** Mitigar.

**Ações preventivas:**
- Definir previamente as responsabilidades de cada componente.
- Estabelecer formatos de entrada e saída entre o modelo, as regras de negócio e a aplicação.
- Implementar e testar componentes progressivamente.
- Criar testes para os principais fluxos de integração.

**Resposta caso ocorra:** Isolar o componente com falha, verificar contratos e dependências e corrigir os problemas antes de avançar para a integração completa.

### R09 — Falta de validação da utilidade do sistema

**Estratégia:** Mitigar.

**Ações preventivas:**
- Definir critérios de aceitação para as funcionalidades.
- Avaliar a coerência das recomendações com os objetivos informados.
- Diferenciar métricas de desempenho do modelo de indicadores de utilidade do produto.
- Planejar testes funcionais e avaliações com usuários quando viáveis.

**Resposta caso ocorra:** Suspender conclusões sobre a eficácia do produto, definir critérios de avaliação e executar testes antes de afirmar que as recomendações são úteis.

### R10 — Dependência excessiva de um modelo ou conjunto de dados

**Estratégia:** Mitigar.

**Ações preventivas:**
- Documentar as condições em que o modelo foi treinado e avaliado.
- Evitar tratar o SVM atual como solução definitiva.
- Separar a lógica de recomendação da implementação específica do modelo, quando tecnicamente viável.
- Avaliar alternativas caso as limitações dos dados ou do algoritmo comprometam os objetivos do sistema.

**Resposta caso ocorra:** Reavaliar a abordagem técnica e substituir ou complementar o modelo, se os resultados e os requisitos justificarem a mudança.

## 6. Monitoramento e controle

O registro de riscos deverá ser revisado durante a conclusão das etapas do projeto e sempre que uma alteração relevante for identificada.

O monitoramento deverá considerar:

- Surgimento de novos riscos.
- Mudanças na probabilidade ou no impacto dos riscos existentes.
- Efetividade das ações preventivas e corretivas.
- Identificação de problemas que já tenham se concretizado.
- Necessidade de revisão do escopo, do cronograma ou dos critérios de qualidade.

Os riscos classificados como altos ou críticos deverão receber atenção prioritária. Quando um risco se concretizar, ele deverá ser tratado como problema ativo, com registro da ocorrência, das medidas adotadas e dos resultados obtidos.

## 7. Responsabilidades

O responsável pelo projeto deverá conduzir a identificação, a avaliação, o registro e o acompanhamento dos riscos, além de definir e executar as medidas de tratamento compatíveis com suas atribuições.

Quando necessário, decisões que afetem significativamente o escopo, a arquitetura ou os objetivos do projeto deverão ser documentadas antes da implementação.

## 8. Atualização do plano

Este documento poderá ser atualizado conforme o avanço do TimeShift, especialmente após a definição da arquitetura, a implementação das regras de negócio, a integração do modelo e a execução dos primeiros testes.

Toda alteração relevante deverá ser registrada no repositório do projeto, preservando o histórico de evolução da documentação.

## 9. Considerações finais

O gerenciamento de riscos é uma atividade contínua e deverá acompanhar todas as etapas do TimeShift. A identificação antecipada de problemas permitirá reduzir retrabalho, melhorar a tomada de decisões e aumentar a confiabilidade das entregas.

A avaliação positiva de um modelo de Machine Learning não será considerada, isoladamente, evidência suficiente de que o sistema atende aos seus objetivos. A qualidade dos dados, a segurança, a coerência das recomendações e a validação do produto deverão ser consideradas em conjunto.

O plano deverá permanecer alinhado ao escopo aprovado e ser atualizado conforme novas evidências forem obtidas durante o desenvolvimento.
