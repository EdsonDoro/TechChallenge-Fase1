# 📊 Tech Challenge - NPS Preditivo

## 🚀 Visão Executiva

Este projeto analisa os principais fatores que impactam a satisfação do
cliente (NPS) em um e-commerce e propõe uma abordagem preditiva para
antecipar insatisfação antes da coleta da pesquisa.

### 🎯 Problema

Apesar de indicadores operacionais semelhantes, clientes apresentam
níveis muito diferentes de satisfação.

> Como identificar, antecipadamente, quais clientes terão uma
> experiência negativa?

------------------------------------------------------------------------

## 📊 Principais Insights

-   🚨 Atraso na entrega é o principal driver de insatisfação
-   📉 Múltiplos contatos com suporte reduzem o NPS
-   ⚠️ Reclamações são forte indicador de detratores
-   💣 Atraso + suporte → queda acentuada no NPS

------------------------------------------------------------------------

## 📈 Impacto no Negócio

-   Redução de churn
-   Aumento de recompra
-   Melhoria da experiência
-   Crescimento via boca a boca

------------------------------------------------------------------------

## 📂 Estrutura do Projeto

    tech-challenge-fase1/
    ├── data/raw/
    ├── notebooks/
    │   └── tech_challenge_fase1.ipynb
    ├── models/
    ├── reports/
    │   └── figures/
    │   1IAST - Fase 1 - Tech Challenge.pdf
    ├── README.md
    ├── requirements.txt
    ├── Tech Challenge - Fase 1 - NPS Preditivo.pdf
    └── Tech Challenge - Fase 1 - NPS Preditivo.pptx

------------------------------------------------------------------------

## 📊 Visualizações

![Distribuição](https://raw.githubusercontent.com/EdsonDoro/TechChallenge-Fase1/main/reports/figures/nps_distribution.png)
![Distribuição por Classe](https://raw.githubusercontent.com/EdsonDoro/TechChallenge-Fase1/main/reports/figures/nps_class_distribution.png)
![Correlação](https://raw.githubusercontent.com/EdsonDoro/TechChallenge-Fase1/main/reports/figures/top_correlacoes_nps.png)
![Heatmap Correlação](https://raw.githubusercontent.com/EdsonDoro/TechChallenge-Fase1/main/reports/figures/heatmap_correlacao.png)
![Atraso](https://raw.githubusercontent.com/EdsonDoro/TechChallenge-Fase1/main/reports/figures/delay_vs_nps.png)

------------------------------------------------------------------------

## 🧠 Metodologia

1.  Entendimento do problema
2.  Definição da target
3.  EDA
4.  Insights
5.  Modelo preditivo

------------------------------------------------------------------------

## 🤖 Modelo Preditivo

Classificação: - Promotor (9--10) - Neutro (7--8) - Detrator (0--6)

Modelo: Random Forest

------------------------------------------------------------------------

## 💡 Recomendações

-   🚚 Reduzir atrasos
-   📞 Melhorar atendimento
-   ⚡ Reduzir tempo de resolução
-   🧠 Criar alertas preditivos

------------------------------------------------------------------------

## ⚠️ Limitações

-   NPS é reativo
-   Correlação ≠ causalidade
-   Sem dados qualitativos

------------------------------------------------------------------------

## 📈 Resultados do Modelo

O modelo preditivo foi desenvolvido como etapa opcional para antecipar clientes com risco de insatisfação.

-   Accuracy
-   F1-Score: 0.82
-   Matriz de confusão: 0.79

A proposta é usar o modelo como suporte à priorização de clientes com maior risco de se tornarem detratores.

------------------------------------------------------------------------

## 🚀 Como Executar

    git clone https://github.com/EdsonDoro/TechChallenge-Fase1.git
    cd TechChallenge-Fase1
    pip install -r requirements.txt
    jupyter notebook notebooks/tech_challenge_fase1.ipynb


------------------------------------------------------------------------

## 🚀 Vídeo de Apresentação

[Assista a apresentação](https://onedrive.live.com/?qt=allmyphotos&photosData=%2Fshare%2F5A5B80C5539E16C2%21s08b14d5a911246799c5b96e9fc761377%3Fithint%3Dvideo%26wdOrigin%3DOWA%2ELINK%26wdPreviousSession%3D9bf49e35%2Dc61a%2D4f05%2D9868%2D90acf5696777%26migratedtospo%3Dtrue&cid=5A5B80C5539E16C2&id=5A5B80C5539E16C2%21s08b14d5a911246799c5b96e9fc761377&redeem=aHR0cHM6Ly8xZHJ2Lm1zL3YvYy81YTViODBjNTUzOWUxNmMyL0lRQmFUYkVJRXBGNVJweGJsdW44ZGhOM0FXcmQyeC00b1VHd2F2eFRIWDQtM2xFP3dkT3JpZ2luPU9XQS5MSU5LJndkUHJldmlvdXNTZXNzaW9uPTliZjQ5ZTM1LWM2MWEtNGYwNS05ODY4LTkwYWNmNTY5Njc3Nw&v=photos)

------------------------------------------------------------------------

## 👤 Autores


- Alessandra M. Capecce,
- Alessandro P. dos Santos,
- Edson L. Doro
