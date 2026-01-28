# PricingCore
Pricing Core é um motor de precificação de derivativos financeiros implementado em C++, baseado em simulação Monte Carlo sob Movimento Browniano Geométrico (GBM).

Motor de precificação de opções europeias utilizando **Simulação Monte Carlo** em **C++**.

Projeto focado em:
- matemática correta
- código limpo e modular
- uso eficiente de C++ para computação numérica

---

## Visão Geral

O **PricingCore** estima o valor justo de opções **Call** e **Put** sob o modelo de **Movimento Browniano Geométrico (GBM)**, aproximando a esperança matemática do payoff por Monte Carlo.

---

## Modelo

\[
S_T = S_0 \cdot \exp\left((r - \frac{1}{2}\sigma^2)T + \sigma\sqrt{T}Z\right),
\quad Z \sim \mathcal{N}(0,1)
\]

\[
Preço = e^{-rT} \cdot \mathbb{E}[\max(S_T - K, 0)]
\]
