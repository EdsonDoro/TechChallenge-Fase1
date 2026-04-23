📊 Tech Challenge - NPS Preditivo

🎯 Objetivo

Este projeto tem como objetivo analisar os fatores que impactam a satisfação dos clientes (NPS) em um e-commerce e propor uma abordagem preditiva capaz de antecipar a experiência do cliente antes da coleta da pesquisa.

A análise busca responder:

Quais fatores operacionais impactam o NPS?
O que leva um cliente a se tornar promotor ou detrator?
Como a empresa pode agir de forma preventiva para melhorar a experiência?
🧠 Contexto de Negócio

Com o crescimento acelerado do e-commerce, a empresa passou a lidar com maior volume de pedidos e interações com clientes.

Apesar disso, observou-se uma alta variabilidade no NPS entre clientes com perfis operacionais semelhantes.

Isso levanta a seguinte questão:

Como transformar dados operacionais em ações práticas para melhorar a experiência do cliente antes da coleta do NPS?

📂 Base de Dados

A base contém dados históricos relacionados a:

👤 Cliente (idade, região, tempo de relacionamento)
🛒 Pedido (valor, quantidade de itens, descontos)
🚚 Logística (tempo de entrega, atraso, tentativas)
📞 Atendimento (contatos, tempo de resolução, reclamações)
⭐ Satisfação (CSAT e NPS)
🎯 Variável alvo

nps_score (escala de 0 a 10)
🔍 Metodologia

O projeto foi estruturado em quatro etapas principais:

1. Entendimento do negócio

Análise do problema e definição dos objetivos estratégicos.

2. Definição da variável alvo

Utilização do NPS como proxy de satisfação do cliente.

3. Análise Exploratória de Dados (EDA)

Investigação de padrões e identificação dos principais drivers de satisfação.

4. Modelagem preditiva (opcional)

Proposta de modelo para antecipar o NPS antes da pesquisa.

📊 Principais Insights

A análise exploratória revelou que:

🚨 Atrasos na entrega são o principal fator de insatisfação
📉 Reclamações e contatos com suporte reduzem significativamente o NPS
⏳ Tempo de resolução elevado impacta negativamente a experiência
🔁 Clientes que realizam recompra tendem a ter NPS mais alto
⚠️ Ponto crítico identificado

A combinação de atraso na entrega + necessidade de suporte gera uma queda acentuada na satisfação do cliente.

📈 Visualizações

O projeto inclui:

Distribuição do NPS
Segmentação de clientes (Promotores, Neutros e Detratores)
Mapa de correlação entre variáveis
Análise de impacto do atraso na entrega
NPS médio por região
Comparação de indicadores por nível de satisfação
🤖 Modelo Preditivo (Opcional)

Foi proposta uma abordagem de classificação para prever a satisfação do cliente.

🎯 Objetivo

Antecipar clientes com risco de se tornarem detratores.

🔧 Abordagem

Classificação:
Promotor (9–10)
Neutro (7–8)
Detrator (0–6)
🤖 Modelo utilizado

Random Forest
📏 Métricas de avaliação

Accuracy
F1-score
Matriz de confusão
💡 Recomendações para o Negócio

Com base nos insights obtidos:

🚀 Logística

Reduzir atrasos de entrega (principal driver de insatisfação)
🚀 Atendimento

Diminuir tempo de resolução
Melhorar resolução no primeiro contato
🚀 Experiência do cliente

Reduzir volume de reclamações
Melhorar comunicação com o cliente
🚀 Estratégia de dados

Implementar modelo preditivo para atuação preventiva
⚠️ Limitações

O NPS é uma métrica reativa, coletada após a experiência
Correlação não implica causalidade
Ausência de dados qualitativos (motivo das reclamações)
Possível viés na coleta da pesquisa
🚀 Como Executar o Projeto

1. Clone o repositório

git clone https://github.com/EdsonDoro/TechChallenge-Fase1.git

cd tech-challenge-nps

2. Instale as dependências

pip install -r requirements.txt

3. Execute o notebook

jupyter notebook notebooks/tech_challenge_nps_analise_estruturada.ipynb

📁 Estrutura do Projeto

tech-challenge-nps/

│

├── data/

│   ├── raw/

│   └── processed/

│

├── notebooks/

│   └── tech_challenge_nps_analise_estruturada.ipynb

│

├── reports/

│   └── figures/

│

├── models/

│

├── README.md

└── requirements.txt

📈 Próximos Passos

Implementação do modelo em ambiente produtivo
Criação de dashboard de monitoramento (ex: Power BI)
Integração com sistemas de atendimento e logística
Evolução para modelos mais robustos (XGBoost, ML Ops)
👤 Autor

Projeto desenvolvido como parte do Tech Challenge - Fase 1 (Pós-Tech).

 

 

 

 

 

📌 1. Entendimento do Negócio

❓ Qual problema de negócio está sendo resolvido?

A empresa enfrenta alta variabilidade no NPS entre clientes, mesmo com indicadores operacionais semelhantes.

O problema central é:

Identificar quais fatores operacionais impactam a satisfação do cliente e permitir ações preventivas antes da coleta do NPS.

Atualmente, o NPS é medido apenas após a jornada, o que limita a capacidade de antecipar insatisfações e agir proativamente.

❓ Por que o NPS é importante para um e-commerce?

O NPS é um dos principais indicadores de:

Lealdade do cliente
Qualidade da experiência
Probabilidade de recompra
Além disso, ele impacta diretamente:

Crescimento orgânico (boca a boca)
Retenção de clientes
Receita de longo prazo
❓ Quais áreas se beneficiam desses insights?

As principais áreas impactadas são:

Logística: melhoria no prazo de entrega e redução de atrasos
Atendimento: redução de contatos e tempo de resolução
Produto: melhoria na experiência de compra
Pricing: ajuste de percepção de valor
Estratégia: priorização de investimentos com base em impacto no cliente
❓ Como o NPS impacta o negócio?

📌 Recompra

Clientes com NPS alto tendem a comprar novamente com maior frequência.

📌 Boca a boca

Promotores recomendam a marca, enquanto detratores podem prejudicar a reputação.

📌 Market share

Empresas com melhor experiência do cliente ganham vantagem competitiva.

❓ Quais indicadores complementares poderiam ser usados?

CSAT (satisfação imediata)
SLA logístico (tempo e atraso de entrega)
Taxa de recompra
Churn rate
Benchmark de NPS de concorrentes
Tempo médio de atendimento
📌 2. Definição da Target

❓ Qual variável representa a satisfação do cliente?

A variável escolhida é:
👉 nps_score

❓ Por que ela foi escolhida?

Representa diretamente a percepção do cliente
É amplamente utilizada no mercado
Permite segmentação clara (promotores, neutros e detratores)
❓ Em que momento da jornada ela é coletada?

O NPS é coletado após o encerramento da jornada de compra, ou seja, depois da entrega e da experiência completa do cliente.

❓ Existe risco no uso dessa variável?

Sim, existem alguns riscos:

É uma métrica reativa, não preventiva
Pode sofrer viés emocional (experiência recente)
Não explica diretamente o motivo da nota
📌 3. Análise Exploratória de Dados (EDA)

❓ Quais fatores parecem mais críticos para a satisfação?

Os principais fatores identificados foram:

Atraso na entrega
Número de reclamações
Quantidade de contatos com atendimento
Tempo de resolução de problemas
👉 Esses fatores têm forte impacto negativo no NPS.

❓ O que mais gera detratores?

Os principais drivers de detratores são:

Entregas atrasadas
Alto número de reclamações
Necessidade de múltiplos contatos com suporte
Demora na resolução de problemas
❓ Existe algum ponto de ruptura na experiência?

Sim.

Foi identificado que:

Qualquer atraso na entrega já impacta negativamente o NPS
A combinação de atraso + suporte necessário gera queda acentuada na satisfação
👉 Isso caracteriza um “ponto crítico” na jornada do cliente.

❓ Que tipo de cliente tende a ter NPS mais alto ou mais baixo?

Clientes com NPS alto:

Recebem pedidos no prazo
Não precisam acionar suporte
Possuem poucas ou nenhuma reclamação
Tendem a recomprar
Clientes com NPS baixo:

Sofrem atraso na entrega
Possuem múltiplas interações com atendimento
Registram reclamações
Enfrentam demora na resolução
📌 4. Proposta de Modelo Preditivo

❓ Qual estratégia você adotaria?

A estratégia recomendada é um modelo de classificação, segmentando clientes em:

Promotores
Neutros
Detratores
❓ Por que essa abordagem?

Mais alinhada com decisões de negócio
Permite ações práticas (ex: tratar detratores)
Facilita interpretação para áreas não técnicas
❓ Definição da variável alvo

Transformar o nps_score em categorias:

0–6 → Detrator
7–8 → Neutro
9–10 → Promotor
❓ Variáveis de entrada

Logística:
delivery_delay_days
delivery_time_days
Atendimento:
complaints_count
customer_service_contacts
resolution_time_days
Pedido:
order_value
items_quantity
Cliente:
customer_tenure_months
customer_region
❓ Separação dos dados

Treino: 70%
Teste: 30%
❓ Modelo escolhido

Random Forest
Motivo:

Boa performance
Interpretação razoável
Robustez a variáveis diversas
❓ Avaliação do modelo

Accuracy
F1-score
Matriz de confusão
❓ Como usar na prática?

O modelo pode ser utilizado para:

Identificar clientes com risco de insatisfação antes da pesquisa
Acionar equipes de logística ou atendimento
Priorizar pedidos críticos
👉 Exemplo:

Cliente com atraso + reclamação → alerta automático → ação preventiva

📌 5. Recomendações para o Negócio

Com base nos insights:

🚀 Reduzir atrasos logísticos

Principal fator de insatisfação

🚀 Melhorar atendimento

Reduzir tempo de resolução
Resolver no primeiro contato
🚀 Diminuir reclamações

Melhor comunicação
Gestão de expectativas
🚀 Implementar modelo preditivo

Antecipar detratores
Agir antes da pesquisa
📌 6. Limitações e Riscos

NPS é coletado após a experiência
Não captura motivos qualitativos
Correlação não implica causalidade
Possível viés na amostra