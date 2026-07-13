---
theme: frankfurt
colorSchema: light
layout: cover
class: text-center
title: The Viability of Blockchain Markets
titleTemplate: '%s'
favicon: ./images/defiicon.png
author: Fayçal Drissi
fonts:
  local: Montserrat, Roboto Mono, Roboto Slab
themeConfig:
  paginationX: disabled
  paginationY: disabled
  paginationPagesDisabled: [1]
infoLine: true
date: '18/07/2026'
drawings:
  enabled: false   # hides Slidev's floating pen/annotation toolbar
mdc: true
---

# Viability of blockchain markets

<br>
<br>


### Agostino Capponi, Álvaro Cartea, and Fayçal Drissi

<br>

###  NBER Summer Institute 2026 -- Financial Market Structure 

<br><br><br><br>

#### [https://www.faycaldrissi.com/mempools-talk](https://www.faycaldrissi.com/mempools-talk)



---
section: Blockchain markets
layout: two-cols-header
---

# Blockchains

### A distributed, digital, permissionless ledger that stores and executes transactions
<v-click at="1">

- blockchains replace *institutional trust* with consensus: *algorithmic rules*


</v-click>



::left::

<v-click at="2">

<br>
<br>
<br>

### **Blockchain round** (*slot*) 
- orders collect during block time (≈12s)
</v-click>
<v-click at="3">

- network communications to validate transactions
</v-click>
<v-click at="4">

- transactions are executed
</v-click>
<v-click at="5">

$\implies$ consensus requires **time** to secure the chain: **block time**
</v-click>

::right::

<div style="display:flex; justify-content:center; margin-top: 8px;">
<v-switch at="0">
<template #1>

![blockchain](./images/block1.png){style="height: 250px;"}

</template>
<template #2>

![block1](./images/block1.png){style="height: 250px;"}

</template>
<template #3>

![block2](./images/block2.png){style="height: 250px;"}

</template>
<template #4>

![block3](./images/block3.png){style="height: 250px;"}

</template>
<template #5>

![block4](./images/block4.png){style="height: 250px;"}

</template>
<template #6>

![block4](./images/block4.png){style="height: 250px;"}

</template>
</v-switch>
</div>



<br><br>

---

# Blockchains

### A distributed, digital, permissionless ledger that stores and executes transactions
- consensus requires economic **incentives** $\implies$ **priority fees**

<div style="display:flex; justify-content:center; margin-top: 8px;">

![mempools3](./images/mempool3.png){style="height: 300px;"}

</div>

---
layout: two-cols-header
---

# Consensus shapes microstructure 

::left::

- <u>Traditional markets</u>: continuous trading, cleared over multiple short rounds

<br>
<br>

![continuous_trading](./images/continuous_trading.gif){style="height: 250px;"}

::right::


<v-click>

- <u>Blockchain markets</u>: blockchain round

</v-click>

<v-clicks at="2">

1. liquidity provider deposits liquidity in a smart contract
2. traders submit transactions
3. block is created and market cleared against liquidity pool

</v-clicks>

<div style="display:flex; justify-content:center; margin-top:8px;">
<v-switch at="2">
<template #1>

![bc](./images/bc_1.gif){style="height: 220px;"}

</template>
<template #2>

![bc](./images/bc_2.gif){style="height: 220px;"}

</template>
<template #3>

![bc](./images/bc_3.gif){style="height: 220px;"}

</template>
</v-switch>
</div>

---

# Motivation


### Blockchains promise to coordinate economic activity at scale *without intermediaries*

<br>
<v-click>

### Financial markets are a fundamental test
- the role of DEXs is likely to grow with **asset tokenization**, **central bank digital currencies**, and **cross-border settlement**

<br>
<v-click>

### This paper
- Can the blockchain host *viable* markets?

<v-click>

- how ? a model to understand market outcomes of a **blockchain round** of trading

</v-click>
</v-click>
</v-click>

---

# Literature

<div style="display:flex; gap:30px; font-size:0.62em; line-height:1.38; margin-top:4px;">

<div style="flex:1;">

<div style="font-weight:700; color:#334155; border-bottom:1px solid #cbd5e1; padding-bottom:2px; margin-bottom:5px;">Blockchain &amp; DEX microstructure</div>

<div><b style="color:#1e293b;">Equilibrium liquidity provision</b></div>
<div style="color:#475569; margin-bottom:5px;">Park (2023, <i>MS</i>) · Malinova–Park (2024) · Hasbrouck–Rivera–Saleh (2026, <i>MS</i>) · Lehar–Parlour (2025, <i>JF</i>)</div>

<div><b style="color:#1e293b;">LP losses &amp; other markets</b></div>
<div style="color:#475569; margin-bottom:5px;">Milionis et al. (2022) · Hasbrouck–Rivera–Saleh (2023) · Cartea–Drissi–Monga (2023, 2024, <i>SIAM</i>)</div>

<div><b style="color:#1e293b;">Informed liquidity provision</b></div>
<div style="color:#475569; margin-bottom:5px;">Klein et al. (2023)</div>

<div><b style="color:#1e293b;">Blockchain infrastructure (gas fees)</b></div>
<div style="color:#475569; margin-bottom:5px;">Capponi–Jia–Yu (2024, <i>RFS</i>)</div>

<div><b style="color:#1e293b;">Others</b></div>
<div style="color:#475569; margin-bottom:5px;">Angeris–Evans–Chitra (2021) · Capponi–Iyengar–Sethuraman (2023, <i>F&amp;T</i>)</div>

<div style="font-weight:700; color:#334155; border-bottom:1px solid #cbd5e1; padding-bottom:2px; margin:9px 0 5px;">Classical microstructure</div>
<div style="margin-bottom:4px;"><b style="color:#1e293b;">Information monopolist</b> <span style="color:#64748b;">— Kyle (1985, <i>Econometrica</i>)</span></div>
<div style="margin-bottom:4px;"><b style="color:#1e293b;">Competition on information</b> <span style="color:#64748b;">— Holden–Subrahmanyam (1992, <i>JF</i>), Foster–Viswanathan (1996, <i>JF</i>)</span></div>
<div style="margin-bottom:4px;"><b style="color:#1e293b;">Multi-stage inventory models</b> <span style="color:#64748b;">— Biais (1993, <i>JF</i>), De Frutos–Manzano (2002, <i>JF</i>)</span></div>
<div style="margin-bottom:4px;"><b style="color:#1e293b;">Compete for queue position (not speed)</b> <span style="color:#64748b;">— O'Hara (1998, <i>book</i>)</span></div>
<div style="margin-bottom:4px;"><b style="color:#1e293b;">Information processing costs</b> <span style="color:#64748b;">— Grossman–Stiglitz (1980, <i>AER</i>), Verrecchia (1982, <i>Econometrica</i>), Kyle (1989, <i>RES</i>), Baldauf–Mollner (2020, <i>JF</i>)</span></div>
<div style="margin-bottom:4px;"><b style="color:#1e293b;">DEX ≈ parametrized price schedule in electronic markets</b> <span style="color:#64748b;">— Glosten (1994, <i>JF</i>), Biais–Martimort–Rochet (2000, <i>Econometrica</i>)</span></div>
<div style="margin-bottom:5px;"><b style="color:#1e293b;">Dealer markets / market making</b> <span style="color:#64748b;">— Ho–Stoll (1983, <i>JF</i>), Glosten–Milgrom (1985, <i>JFE</i>)</span></div>

</div>

<div style="flex:1;">

<div style="font-weight:700; color:#334155; border-bottom:1px solid #cbd5e1; padding-bottom:2px; margin-bottom:5px;">Political contests (multi-prize)</div>
<div style="margin-bottom:4px;"><b style="color:#1e293b;">Multi-prize contests</b> <span style="color:#64748b;"> — Lazear–Rosen (1981, <i>JPE</i>), Hillman–Riley (1989), Barut–Kovenock (1998), Klose–Kovenock (2015)</span></div>
<div style="margin-bottom:5px;"><b style="color:#1e293b;">Multi-prize contests with a fixed prize vector</b> <span style="color:#64748b;">— Moldovanu–Sela (2001, <i>AER</i>)</span></div>

<br>

<div style="font-weight:700; color:#334155; border-bottom:1px solid #cbd5e1; padding-bottom:2px; margin:9px 0 5px;">Periodic auctions for markets</div> 
<div><b style="color:#1e293b;">Uniform-price batch auctions</b> <span style="color:#64748b;">— Madhavan (1992, <i>JF</i>), Budish–Cramton–Shim (2015, <i>QJE</i>); we use discriminatory pricing, LP absent</span></div>

<br>


<div style="font-weight:700; color:#334155; border-bottom:1px solid #cbd5e1; padding-bottom:2px; margin:9px 0 5px;">Opening / closing auctions</div>
<div><b style="color:#1e293b;">Information revelation accelerates toward the close</b> <span style="color:#64748b;">— Medrano–Vives (2001, <i>RAND J. Econ</i>)</span></div>

<div style="margin-bottom:4px;"><b style="color:#1e293b;">Transparency &amp; ending times of call auctions</b> <span style="color:#64748b;">— Van Bommel–Hoffmann (2011)</span></div>
<div style="margin-bottom:4px;"><b style="color:#1e293b;">Preopening price discovery &amp; learning (pure-noise hypothesis)</b> <span style="color:#64748b;">— Biais–Hillion–Spatt (1999, <i>JPE</i>)</span></div>


</div>

</div>

---
section: Model
---

# Model


<div style="text-align:center; font-weight:600; color:#1e293b; margin: 20px 0 8px;">

### A static, three-stage game
</div>

<div style="display:flex; align-items:stretch; justify-content:center; gap:6px; margin: 14px 24px 0;">
<div style="flex:1; border:1.5px solid #334155; border-radius:8px; background:white; padding:10px; text-align:center;">
<div style="font-weight:700; color:#1e293b;">Stage 1 · Entry</div>
<div style="font-size:0.78em; color:#334155; margin-top:5px;">M traders pay information cost C</div>
</div>
<div style="align-self:center; color:#94a3b8; font-size:1.5em; padding:0 3px;">→</div>
<div style="flex:1; border:1.5px solid #334155; border-radius:8px; background:white; padding:10px; text-align:center;">
<div style="font-weight:700; color:#1e293b;">Stage 2 · Liquidity</div>
<div style="font-size:0.78em; color:#334155; margin-top:5px;">supplier sets reserves L</div>
</div>
<div style="align-self:center; color:#94a3b8; font-size:1.5em; padding:0 3px;">→</div>
<div style="flex:1.35; border:1.5px solid #334155; border-radius:8px; background:white; padding:10px; text-align:center;">
<div style="font-weight:700; color:#1e293b;">Stage 3 · Trading (PGA)</div>
<div style="font-size:0.78em; color:#334155; margin-top:5px;">informed traders set priority fees Φ and volumes Q</div>
</div>
</div>

<br><br>

<v-click>
<div style="text-align:center; font-weight:600; color:#1e293b; margin: 20px 0 8px;">

### Solved backward
</div>

<div style="display:flex; align-items:stretch; justify-content:center; gap:6px; margin: 0 16px;">
<div style="flex:1; border:1px solid #cbd5e1; border-radius:8px; background:white; padding:9px 8px; text-align:center;">
<div style="font-weight:700; color:#334155;">① priority fees Φ</div>
</div>
<div style="align-self:center; color:#94a3b8; font-size:1.3em;">→</div>
<div style="flex:1; border:1px solid #cbd5e1; border-radius:8px; background:white; padding:9px 8px; text-align:center;">
<div style="font-weight:700; color:#334155;">② volumes Q</div>
</div>
<div style="align-self:center; color:#94a3b8; font-size:1.3em;">→</div>
<div style="flex:1; border:1px solid #cbd5e1; border-radius:8px; background:white; padding:9px 8px; text-align:center;">

<div style="font-weight:700; color:#334155;">③ liquidity L</div>
</div>
<div style="align-self:center; color:#94a3b8; font-size:1.3em;">→</div>
<div style="flex:1; border:1px solid #cbd5e1; border-radius:8px; background:white; padding:9px 8px; text-align:center;">
<div style="font-weight:700; color:#334155;">④ entry M</div>
</div>
</div>
</v-click>


---
layout: two-cols-header
---

# Execution prices

::left::

#### <u>**Linear price schedule**</u>: buying a quantity $Q$ executes at

$$ \underbrace{Q/L}_{\text{slippage}} \;+\; \underbrace{\pi}_{\text{fee}}$$
<!--\qquad\implies\qquad\text{cash paid } = Q\,(Q/L + \pi)-->
Larger liquidity $L$ $\implies$ smaller slippage

<v-click>

<br><br><br>

#### <u>**Linear price update rule**</u>: After a buy of size $Q$, the marginal price moves to

$$ 
\underbrace{2\,Q/L}_\text{price impact}
$$


Larger liquidity $L$ $\implies$ smaller impact

<br><br>

</v-click>

::right::

<v-click>

#### <u>**Why compete ?**</u>

- Trader 1 buys $Q_1$ first, then trader 2 buys $Q_2$

<div style="display:flex; justify-content:center; margin: 10px 0 2px;">
<div style="position:relative; border:1.5px solid #4b5563; border-radius:5px; padding:9px 5px 5px;">
<div style="position:absolute; top:-8px; left:10px; background:white; padding:0 5px; font-size:9px; font-weight:700; color:#4b5563;">block</div>
<div style="display:flex; gap:4px;">
<div style="border:1.5px solid #334155; background:#eef2f6; color:#1e293b; padding:6px 18px; text-align:center; font-size:12px; line-height:1.35;"><b>Trader 1</b><br>buys Q<sub>1</sub></div>
<div style="border:1.5px solid #334155; background:#eef2f6; color:#1e293b; padding:6px 18px; text-align:center; font-size:12px; line-height:1.35;"><b>Trader 2</b><br>buys Q<sub>2</sub></div>
</div>
</div>
</div>
<div style="text-align:center; font-size:0.62em; color:#64748b; margin-top:2px;">execution order →</div>

<v-click>

- Trader 1 pays 
$$Q_1/L + \pi\quad\text{per unit}$$

<v-click>

- Trader 2  pays 
$$\underbrace{2Q_1/L}_{\text{impact from trader 1}} \,+\, \underbrace{Q_2/L}_{\text{own slippage}} \,+\, \pi \quad\text{per unit}$$


</v-click>
</v-click>
</v-click>

---
class: fact-c
---

# Competition among informed traders

### Informed flow arrives just before block creation

- Traders who submit high priority fees submit **late** 
- Competition among informed traders is effectively **blind**


<div style="display:flex; justify-content:center;">

![distribPF](./images/distribPF.png){style="height: 250px; margin-top: 8px;"}

</div>

<div class="fig-cap" style="max-width:4500px;">Priority fee distribution as a function of submission time over a blockchain slot. &nbsp;<br><b>Data</b>: Ethereum public mempool, ≈10 million transactions, 20–21 March 2024 (source: EthPandaOps).</div>

<br>

---

# Competition among informed traders


### <u>Setup</u>
- sealed-bid auction: $M$ buying traders with private valuations $\,v_i \in [0, \overline  v] \sim F$
- DEX liquidity $L$

<div v-click="1">
<br>

###  <u>Expected wealth</u>

</div>

<div style="display:grid; align-items:start;">

<div style="grid-area:1/1;" v-click="[1,2]">

$$
\boxed{\mathbb{E}_{i}\left[W_{i}\right]= \sum_{n=0}^{M-1}\mathbb{E}_{i}\left[\mathbf{1}_{\Phi_{(n)}<\Phi_{i}<\Phi_{(n+1)}}\,W_{i,(n)}\right]}
$$

</div>

<div style="grid-area:1/1;" v-click="2">

$$
\boxed{\mathbb E_i[W_i]=  \underbrace{Q_i\,v_i}_{\text{trading profit}} - \underbrace{Q_i\left(\dfrac{Q_i}{L}+\pi\right)}_{\text{slippage \& DEX fee}} - \underbrace{\Phi_i}_{\text{priority fee}} -\ \ Q_i\times\underbrace{\dfrac{2}{L}\sum_{n=0}^{M-1}\mathbb E_i\big[\mathbf 1_{\Phi_{(n)}<\Phi_i<\Phi_{(n+1)}}\,\Delta_{(n+1:M-1)}\big]}_{\text{adverse impact of competitors}} - \underbrace{C}_{\text{info. cost}}}
$$

</div>

</div>

<div v-click="3">

###  <u>Objective</u>

$$
\boxed{\sup_{\Phi_i, Q_i}\mathbb E_i[W_i] =\sup_{Q_i} \sup_{\Phi_i}\mathbb E_i[W_i]}
$$

</div>


---
section: Results
layout: two-cols-header
---

# <span style="font-size:0.56em; font-weight:600;">① priority fees <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">② volumes</span> <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">③ liquidity</span> <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">④ entry <i>M</i></span></span>


### <u>Setup</u>
- Exogenous private volumes distribution $Q \in [0, \overline  Q] \sim G$
- $M$ buying traders
- DEX liquidity $L$


<br>



::left::

<v-click>


### <u>Trader $i$ chooses the priority fee $\Phi_i$</u>

<br>

$$\sup_{\Phi_i}\ \Bigg\{\ -\underbrace{\Phi_i}_{\text{priority fee}}\ +\ \underbrace{\frac{2\,Q_i}{L}\,\sum_{n=0}^{M-1}\mathbb{E}_{i}\left[ \mathbf{1}_{\{\Phi_{(n)}<\Phi_{i}<\Phi_{(n+1)}\}}\,\Delta_{(1:n)}\right]}_{\text{surplus }=\text{ avoided impact}}\Bigg\}$$

- the surplus grows with volume $Q_i$, with the number of competitors $M$, and with thinner liquidity $L$

</v-click>

::right::

<br>
<br>

<v-click at="1">

<div style="margin: 4px 30px 0;">
<svg viewBox="0 0 600 100" preserveAspectRatio="none" style="width: 100%; height: 94px; display: block;">
  <path d="M 175 58 L 175 44 L 245 44 L 245 30 L 560 30 L 560 58 Z" fill="#334155" fill-opacity="0.14"/>
  <path d="M 0 90 L 35 90 L 35 74 L 105 74 L 105 58 L 175 58 L 175 44 L 245 44 L 245 30 L 600 30" stroke="#334155" stroke-width="1.6" fill="none" vector-effect="non-scaling-stroke"/>
  <line x1="165" y1="58" x2="560" y2="58" stroke="#dc2626" stroke-width="1" stroke-dasharray="5 3" vector-effect="non-scaling-stroke"/>
  <line x1="165" y1="60" x2="165" y2="100" stroke="#dc2626" stroke-width="0.8" stroke-dasharray="2 2" vector-effect="non-scaling-stroke"/>
  <circle cx="165" cy="58" r="4" fill="#dc2626"/>
  <text x="4" y="12" style="font-size: 8px;" fill="#444">price</text>
  <text x="150" y="50" text-anchor="middle" style="font-size: 8px; font-weight: 700;" fill="#dc2626">trader i</text>
  <text x="378" y="46" text-anchor="middle" style="font-size: 8px; font-weight: 700;" fill="#334155">surplus = avoided impact</text>
</svg>

<div style="position: relative; border: 1.5px solid #4b5563; border-radius: 4px; padding: 7px 0 3px; margin-top: 1px;">
<div style="position: absolute; top: -8px; left: 12px; background: white; padding: 0 6px; font-size: 9px; font-weight: 700; color: #4b5563;">block</div>
<div style="display: flex;">
  <div style="flex: 70; border-right: 1px solid #cbd5e1; background: #eef2f6; padding: 3px 1px; text-align: center; font-size: 9px; color: #1e293b;">txn 1 · Φ<sub>(1)</sub></div>
  <div style="flex: 70; border-right: 1px solid #cbd5e1; background: #eef2f6; padding: 3px 1px; text-align: center; font-size: 9px; color: #1e293b;">txn 2 · Φ<sub>(2)</sub></div>
  <div style="flex: 70; border-right: 1px solid #cbd5e1; background: #eef2f6; padding: 3px 1px; text-align: center; font-size: 9px; color: #1e293b;">⋯</div>
  <div style="flex: 70; border-right: 1px solid #cbd5e1; background: #eef2f6; padding: 3px 1px; text-align: center; font-size: 9px; color: #1e293b;">txn N · Φ<sub>(N)</sub></div>
  <div style="flex: 320; background: #f3f4f6; padding: 3px 6px; text-align: center; font-size: 9px; color: #374151;">fee = 0</div>
</div>
</div>

</div>

</v-click>

---


# <span style="font-size:0.56em; font-weight:600;">① priority fees <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">② volumes</span> <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">③ liquidity</span> <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">④ entry <i>M</i></span></span>



<br><br>

$$
\Phi^\star\left(Q_{i}\right)=\frac{2}{L}\left(M-1\right)\int_{0}^{Q_{i}}x^{2}\,dG\left(x\right)
$$


<br><br><br>

<div class="prop-box">

### Equilibrium fee

1. larger volume $Q_i$ $\Rightarrow$ larger fee $\Phi^\star(Q_i)$
2. priority fees **increase with competition** $M$ 
3. priority fees **decrease with liquidity** $L$

</div>

---
class: fact-c
---

# <span style="font-size:0.56em; font-weight:600;">① priority fees <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">② volumes</span> <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">③ liquidity</span> <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">④ entry <i>M</i></span></span>


### When price formation happens on-chain: 
- absolute volume **decreases** with queue position
<!--$\ \implies\,$ aggressive, high-volume traders secure the earliest positions-->
<br>

<div style="display:flex; justify-content:center;">

![abs](./images/tradingvolumes_abs.png){style="height: 190px; margin-top: 8px;"}

</div>

<div class="fig-cap" style="max-width:360px;">Distribution of normalized absolute volume as a function of queue position. &nbsp;<b>Data</b>: 75 Uniswap v3 pools whose asset is <i>not</i> on Binance: 317,901 trades in 36,692 blocks, 2021–2026.</div>

<br>

---

# <span style="font-size:0.56em; font-weight:600;"><span style="opacity:0.45;">① priority fees</span> <span style="opacity:0.4;">→</span> ② volumes <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">③ liquidity</span> <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">④ entry <i>M</i></span></span>

### <u>Setup</u>
- $M$ buying traders with private valuations $\,v_i \in [0, \overline  v] \sim F$
- DEX liquidity $L$

<br>
<br>

<v-click>

### <u>Trader $i$ chooses volume $Q_i$, anticipating the fee </u>
<br>

$$\sup_{Q_i}\ \Bigg\{\underbrace{Q_i\,v_i}_{\text{profit}}-\underbrace{Q_i\left(Q_i/L+\pi\right)}_{\text{slippage}}-\underbrace{\Phi^\star(Q_i)}_{\text{priority fee}}-\underbrace{\dfrac{2Q_i}{L}(M-1)\!\int_{v_i}^{\overline v}\! x\,dF(x)}_{\text{impact of trades with better queue positions}}\ \Bigg\}$$

- profit incentivises **higher** volume $Q_i$
- slippage, fees, and impact incentivise **lower**  $Q_i$

</v-click>

---
layout: two-cols-header
---

# <span style="font-size:0.56em; font-weight:600;"><span style="opacity:0.45;">① priority fees</span> <span style="opacity:0.4;">→</span> ② volumes <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">③ liquidity</span> <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">④ entry <i>M</i></span></span>

<br>

$$Q^\star(v_i)
= L \times \frac{1}{2}\Bigg(\underbrace{\left(\overline v - \pi\right)e^{-(M-1)\left(1-F(v_i)\right)}}_{\text{profit net of fees}}
- \underbrace{\int_{v_i}^{\overline v} e^{-(M-1)\left(F(u)-F(v_i)\right)}\,du}_\text{impact of competing orders} \Bigg)
$$

<br>

::left::

<div class="prop-box">

#### Equilibrium volume

- increasing in valuation $v$ and liquidity $L$
- decreasing in number of traders $M$

<br>
</div>

<br>

::right::

<v-click>

<div class="prop-box">


#### Endogenous selection

- Only aggressive traders trade: there is a participation cutoff $\underline v(M)$

- the cutoff **rises with competition** $\ \lim_{M\to\infty}\underline v(M)=\overline v$

</div>

</v-click>


---
class: fact-c
---

# <span style="font-size:0.56em; font-weight:600;"><span style="opacity:0.45;">① priority fees</span> <span style="opacity:0.4;">→</span> ② volumes <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">③ liquidity</span> <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">④ entry <i>M</i></span></span>


### When price formation is on-chain and off-chain
- price changes in blockchain markets are more extreme
<br><br>
<div style="display:flex; justify-content:center; margin-top:10px;">
<table class="overshoot-tbl" style="font-size:0.72em;">
<thead>
<tr>
<th style="text-align:left;">Asset</th>
<th colspan="2" class="cmid">Blockchain (bp)</th>
<th colspan="2" class="cmid">Binance (bp)</th>
</tr>
<tr>
<th></th><th>std</th><th>99%</th><th>std</th><th>99%</th>
</tr>
</thead>
<tbody>
<tr><td>ETH/BTC</td><td><b>7.72</b></td><td><b>30.71</b></td><td>6.00</td><td>23.26</td></tr>
<tr><td>ETH</td><td><b>8.71</b></td><td><b>29.86</b></td><td>6.87</td><td>26.10</td></tr>
<tr><td>BTC</td><td><b>24.94</b></td><td><b>89.33</b></td><td>17.83</td><td>69.27</td></tr>
<tr><td>LINK</td><td><b>27.35</b></td><td><b>79.51</b></td><td>13.45</td><td>48.35</td></tr>
<tr><td>UNI</td><td><b>29.41</b></td><td><b>81.29</b></td><td>18.29</td><td>78.74</td></tr>
<tr><td>APE</td><td><b>36.34</b></td><td>99.50</td><td>28.63</td><td><b>108.52</b></td></tr>
<tr><td>MATIC</td><td><b>43.07</b></td><td><b>99.61</b></td><td>18.77</td><td>73.19</td></tr>
<tr><td>1INCH</td><td><b>84.11</b></td><td><b>182.40</b></td><td>34.84</td><td>119.70</td></tr>
</tbody>
</table>
</div>

<div class="fig-cap" style="max-width:640px;">Distribution of absolute one-block returns in bp (1 Jan 2021 – 31 Dec 2023). &nbsp;<b>Data</b>: 8 assets priced both on-chain (Uniswap v3) and on Binance: ETH/BTC 148,624 transations · ETH 1,703,611 · BTC 24,967 · LINK 31,663 · UNI 14,606 · APE 41,902 · MATIC 13,928 · 1INCH 3,751.</div>



---

# <span style="font-size:0.56em; font-weight:600;"><span style="opacity:0.45;">① priority fees</span> <span style="opacity:0.4;">→</span> ② volumes <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">③ liquidity</span> <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">④ entry <i>M</i></span></span>


### <u>Consequences</u>

<div style="display:flex; gap:26px; align-items:flex-start; margin-top:6px;">
<div style="flex:1; min-width:0;">

- Information is **truncated** as competition increases

<br>
<v-click>


<div class="prop-box">

End-of-block price is pushed to extremes as competition increases 
$$\quad \lim_{M\to\infty}\underbrace{\dfrac{M(\underline v(M)-\pi)}{M-1}}_{\text{end-of-block price}\ }\ \ =\ \ \overline v-\pi$$

</div>

</v-click>

</div>
<div style="flex:1; min-width:0; display:flex; justify-content:center; align-items:flex-start;">

<div style="max-width:410px; width:100%;">
<svg viewBox="0 0 600 480" preserveAspectRatio="xMidYMid meet" style="width: 100%; height: auto; display: block;">
  <defs><marker id="arrM" markerWidth="7" markerHeight="7" refX="5" refY="2.5" orient="auto"><path d="M0,0 L5,2.5 L0,5 z" fill="#dc2626"/></marker></defs>
  <line x1="75" y1="410" x2="585" y2="410" stroke="#444" stroke-width="1.2"/>
  <line x1="75" y1="30" x2="75" y2="410" stroke="#444" stroke-width="1.2"/>
  <text x="82" y="26" text-anchor="start" style="font-size: 21px;" fill="#444">density</text>
  <text x="330" y="467" text-anchor="middle" style="font-size: 21px;" fill="#444">valuation</text>
  <text x="75" y="435" text-anchor="middle" style="font-size: 21px;" fill="#444">0</text>
  <text x="575" y="435" text-anchor="middle" style="font-size: 21px;" fill="#444">v&#772;</text>
  <path d="M 325 410 L 325 318 L 375 351 L 425 377 L 475 395 L 525 406 L 575 410 Z" fill="#334155" fill-opacity="0.15"/>
  <path d="M 75 40 L 125 110 L 175 173 L 225 229 L 275 277 L 325 318 L 375 351 L 425 377 L 475 395 L 525 406 L 575 410" stroke="#334155" stroke-width="2.5" fill="none"/>
  <line x1="325" y1="318" x2="325" y2="410" stroke="#dc2626" stroke-width="2"/>
  <text x="325" y="435" text-anchor="middle" style="font-size: 21px;" fill="#dc2626"><tspan style="text-decoration: underline;">v</tspan>(M)</text>
  <line x1="405" y1="367" x2="405" y2="410" stroke="#dc2626" stroke-width="1.5" stroke-dasharray="5,4"/>
  <line x1="333" y1="392" x2="397" y2="392" stroke="#dc2626" stroke-width="2" marker-end="url(#arrM)"/>
  <text x="365" y="380" text-anchor="middle" style="font-size: 23px; font-style: italic;" fill="#dc2626">M &#8593;</text>
  <text x="455" y="288" text-anchor="middle" style="font-size: 21px;" fill="#334155">active traders</text>
</svg>
</div>

</div>
</div>



---
class: fact-c
---

# <span style="font-size:0.56em; font-weight:600;"><span style="opacity:0.45;">① priority fees</span> <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">② volumes</span> <span style="opacity:0.4;">→</span> ③ liquidity <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">④ entry <i>M</i></span></span>


### Equilibrium structure of a block
- Early trades take the same direction
- Back of block $\to$ two-sided **noise** <br>

<div style="display:flex; justify-content:center; align-items:flex-start; gap:30px; margin-top:8px;">
<div style="text-align:center;">

![signed](./images/tradingvolumes_signed.png){style="height: 205px;"}

</div>

</div>
<div class="fig-cap" style="max-width:360px;">Distribution of normalized volume as a function of queue position. &nbsp;<b>Data</b>: 75 Uniswap v3 pools whose asset is <i>not</i> on Binance: 317,901 trades in 36,692 blocks, 2021–2026.</div>



---

# <span style="font-size:0.56em; font-weight:600;"><span style="opacity:0.45;">① priority fees</span> <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">② volumes</span> <span style="opacity:0.4;">→</span> ③ liquidity <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">④ entry <i>M</i></span></span>

### <u>setup</u>

<div style="float:right; width:300px; margin:4px 18px 6px 24px;">
<svg viewBox="0 0 360 260" style="width:100%; height:auto; display:block;">
  <rect x="0" y="0" width="360" height="260" fill="#ffffff"/>
  <defs>
    <marker id="ndah" markerUnits="userSpaceOnUse" markerWidth="12" markerHeight="12" refX="9" refY="4.5" orient="auto">
      <path d="M0,0 L9,4.5 L0,9 z" fill="#000000"/>
    </marker>
  </defs>
  <line x1="48" y1="69.1" x2="330" y2="69.1" stroke="#000000" stroke-width="1" stroke-dasharray="5 4"/>
  <line x1="48" y1="210" x2="340" y2="210" stroke="#000000" stroke-width="1.4" marker-end="url(#ndah)"/>
  <line x1="48" y1="210" x2="48" y2="34" stroke="#000000" stroke-width="1.4" marker-end="url(#ndah)"/>
  <path d="M 48.0 210.0 L 61.6 194.3 L 75.2 181.8 L 88.8 171.6 L 102.4 163.0 L 116.0 155.8 L 129.6 149.6 L 143.2 144.3 L 156.8 139.6 L 170.4 135.4 L 184.0 131.7 L 197.6 128.4 L 211.2 125.5 L 224.8 122.8 L 238.4 120.4 L 252.0 118.1 L 265.6 116.1 L 279.2 114.2 L 292.8 112.5 L 306.4 110.9 L 320.0 109.4" fill="none" stroke="#000000" stroke-width="2"/>
  <text x="40" y="74" text-anchor="end" style="font-size:16px;" fill="#000000">N</text>
  <text x="334" y="232" text-anchor="middle" style="font-size:16px;" fill="#000000">L</text>
  <text transform="translate(16 132) rotate(-90)" text-anchor="middle" style="font-size:14px;" fill="#000000">noise demand</text>
</svg>
</div>

- price-sensitive zero-mean noise demand, $\text{fee} = 0$
$$
N\,\dfrac{L}{L+\theta}
$$
<v-click>

$\implies$ deeper liquidity $L$ → more revenue 

<v-click>

- adverse selection losses 
$$
L\,A(M)
$$

$\implies$ deeper liquidity $L$  → more adverse selection

<v-click>

-  liquidity provision is competitive
    $$\underbrace{\pi N\,\dfrac{L}{L+\theta}}_{\text{fee revenue from noise demand}}\qquad=\qquad \underbrace{L\,A(M)}_{\text{adverse-selection}}$$
    
</v-click>
</v-click>
</v-click>

---

# <span style="font-size:0.56em; font-weight:600;"><span style="opacity:0.45;">① priority fees</span> <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">② volumes</span> <span style="opacity:0.4;">→</span> ③ liquidity <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">④ entry <i>M</i></span></span>


<br><br>


<br>

<div class="prop-box">


### Equilibrium liquidity

- number of traders $M$ **decreases liquidity** 
<br>
(Holden & Subrahmanyam 1992)

- market viability condition 
<br>(Glosten & Milgrom 1985, Glosten 1989, Leach & Madhavan 1989) 
$$A(M)\ \le\ \dfrac{\pi N}{\theta}$$


</div>

---


# <span style="font-size:0.56em; font-weight:600;"><span style="opacity:0.45;">① priority fees</span> <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">② volumes</span> <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">③ liquidity</span> <span style="opacity:0.4;">→</span> ④ entry <i>M</i></span>

### <u>setup</u>
- trader pays $C$ iff expected ex-ante profit covers it

$$C \le  \underbrace{H(M)}_{\text{ex-ante profit per informed trader}}=L^\star(M)\!\int_{\underline v(M)}^{\overline v}\!\tilde Q(v)^2\,\underbrace{\big[\,1-2(M-1)(1-F(v))\,\big]}_{\text{own profit}\ - \ \text{losses due to competitors}}\,dF(v)$$

<v-click>
<div class="prop-box">

$H(M)$ decreasing in $M$

</div>

<br>

<v-click>

<div class="prop-box">


### Equilibrium number of traders
- $M^\star$ increases in noise $N$ 
- $M^\star$ decreases in information cost $C$

</div>

</v-click>
</v-click>

---

# <span style="font-size:0.56em; font-weight:600;"><span style="opacity:0.45;">① priority fees</span> <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">② volumes</span> <span style="opacity:0.4;">→</span> <span style="opacity:0.45;">③ liquidity</span> <span style="opacity:0.4;">→</span> ④ entry <i>M</i></span>

### The information paradox

$$\underbrace{C\downarrow\ \ }_{\text{cheaper info}}\ \Rightarrow\ \underbrace{M\uparrow}_\text{more traders}\ \Rightarrow\ \underbrace{\underline v(M)\uparrow\ }_\text{higher cutoff} \Rightarrow\ \begin{cases}\text{less information revealed}\\~\\\text{prices more biased}\end{cases}$$

---

# Block time

### Block time: time needed to run **consensus**
- longer blocks $\rightarrow$ **security** and **decentralization**

<br>

<v-click>

### Block time: length of a trading round
- extreme valuations  more likely
- noise trading decraeses

<v-click>

<br>

### A longer block amplifies every friction
- the participation cutoff increases, information is more truncated, prices are more extreme
- less liquidity, market shutdown more likely



<br>

<v-click>

<div class="prop-box">

### Security vs. market efficiency

</div>

</v-click>
</v-click>
</v-click>

---
layout: end
---

**Takeaway:** The features of decentralization undermine blockchains as a venue for **price formation**.

<v-click>

Thank you !

<br>

Capponi, Cartea, and Drissi (2025), *The Viability of Blockchain Markets under Discrete Clearing and Paid Priority*

<br>

These slides: [www.faycaldrissi.com/mempools-talk](https://www.faycaldrissi.com/mempools-talk)

</v-click>
