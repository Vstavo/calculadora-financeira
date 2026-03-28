## Simulador de Maturação de Whisky

Este programa foi desenvolvido em **HTML e JavaScript** para simular o processo de maturação de um barril de whisky. O objetivo é estimar quanto volume será perdido por evaporação ao longo do tempo e qual será o valor final do whisky restante.

### Funcionamento do Programa

O usuário deve inserir algumas informações relacionadas ao processo de maturação:

* **Temperatura média (°C)** – influencia a velocidade do envelhecimento.
* **Tempo de maturação (anos)** – período que o whisky ficará no barril.
* **Volume inicial (litros)** – quantidade inicial de whisky no barril.
* **Taxa de evaporação (% ao ano)** – porcentagem de líquido que evapora a cada ano.
* **Valor por litro (R$)** – preço estimado do whisky por litro.
* **Umidade do ambiente (%)** – influencia qual componente evapora mais (água ou álcool).

Após preencher os campos, o usuário clica no botão **"Calcular resultado"**. O JavaScript executa uma função que realiza os cálculos e mostra os resultados na tela.

### Cálculos Realizados

O programa realiza quatro cálculos principais:

**1. Valor inicial do barril**

Calcula o valor total do whisky antes da maturação.

Valor inicial = Volume inicial × Valor por litro

---

**2. Perda total por evaporação**

Calcula quanto líquido evapora durante o período de maturação.

Perda = Volume inicial × (Taxa de evaporação / 100) × Tempo

---

**3. Volume final**

Mostra quanto whisky ainda restará no barril após a evaporação.

Volume final = Volume inicial − Perda

---

**4. Valor final estimado**

Calcula o valor do whisky restante após o processo de maturação.

Valor final = Volume final × Valor por litro

---

### Análise das Condições de Maturação

Além dos cálculos, o programa também analisa **temperatura** e **umidade**, exibindo mensagens explicativas.

**Temperatura**

* Entre **15°C e 20°C** → considerada ideal para maturação.
* Entre **10°C e 30°C** → aceitável.
* Abaixo de **10°C** ou acima de **30°C** → condição ruim para maturação.

**Umidade**

* **55% a 70%** → evaporação equilibrada.
* **Abaixo de 55%** → evapora mais água, aumentando o teor alcoólico.
* **Acima de 70%** → evapora mais álcool, diminuindo o teor alcoólico.

### Objetivo do Simulador

O simulador demonstra de forma simples como fatores ambientais podem influenciar o envelhecimento do whisky em barris. Ele permite visualizar:

* a perda de volume ao longo dos anos,
* o impacto financeiro da evaporação,
* e as condições ideais de maturação.
