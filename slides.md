---
layout: cover
class: text-center
title: The Viability of Blockchain Markets
#theme: academic
titleTemplate: '%s'
favicon: ./images/defiicon.png
author: Fayçal Drissi
themeConfig:
  paginationX: disabled
  paginationY: disabled
  paginationPagesDisabled: [1]
fonts:
  local: Montserrat, Roboto Mono, Roboto Slab # local fonts are used for legal reasons for deployment to https://slidev-theme-academic.alexeble.de and only set up for the example project, remove this line for your project to automatically have fonts imported from Google

theme: frankfurt
infoLine: true # on by default, can be turned off
#author: 'Your name here' # shows in infoLine
#title: 'Title' # shows in infoLine
date: '04/06/2026' # shows in infoLine, defaults to the current date

mdc: true
---

## The Viability of Blockchain Markets

Fayçal Drissi (University of Oxford)

<br>


Capponi, Cartea, and Drissi (2025), *The Viability of Blockchain Markets under Discrete Clearing and Paid Priority*

<br>

6th Annual CBER Conference, NYU Stern

<br>

These slides: [https://www.faycaldrissi.com/mempools-talk](https://www.faycaldrissi.com/mempools-talk)



---
section: Motivation
---

# Blockchains

### Blockchains coordinate economic activity without trusted intermediaries
- consensus replaces institutional trust with algorithmic, publicly verifiable rules
- **financial markets are central to this promise** — whether the chain can host *viable* markets is a fundamental test of it

<br>

<v-click>

### Consensus has a price
- consensus requires **time** to secure the chain
  - **block time**
- consensus requires **incentives** to compensate blockchain participants
  - **priority fees**
  - others (gas fees, issuance)
<br><br>

<v-click>

### This talk
- what does the **price of consensus** imply for the markets that live on the chain?

</v-click>

</v-click>

---

# Consensus shapes microstructure
### <u>Traditional markets</u>: continuous trading, cleared over multiple short rounds

<div style="margin-top: 22px; padding: 0 30px;">

<div style="position: relative; height: 60px;">
  <div style="position: absolute; top: 38px; left: 0; right: 0; height: 2px; background: #333;"></div>
  <div style="position: absolute; top: 6px; left: 0%; transform: translateX(-50%); font-size: 0.62em; color: #444; white-space: nowrap;">MM ↔ IT/NT</div>
  <div style="position: absolute; top: 18px; left: 0%; width: 7px; height: 7px; border-radius: 50%; background: #333; transform: translate(-50%, 0);"></div>
  <div style="position: absolute; top: 30px; left: 0%; width: 2px; height: 18px; background: #333;"></div>
  <div style="position: absolute; top: 6px; left: 14.29%; transform: translateX(-50%); font-size: 0.62em; color: #444; white-space: nowrap;">MM ↔ IT/NT</div>
  <div style="position: absolute; top: 18px; left: 14.29%; width: 7px; height: 7px; border-radius: 50%; background: #333; transform: translate(-50%, 0);"></div>
  <div style="position: absolute; top: 30px; left: 14.29%; width: 2px; height: 18px; background: #333;"></div>
  <div style="position: absolute; top: 6px; left: 28.57%; transform: translateX(-50%); font-size: 0.62em; color: #444; white-space: nowrap;">MM ↔ IT/NT</div>
  <div style="position: absolute; top: 18px; left: 28.57%; width: 7px; height: 7px; border-radius: 50%; background: #333; transform: translate(-50%, 0);"></div>
  <div style="position: absolute; top: 30px; left: 28.57%; width: 2px; height: 18px; background: #333;"></div>
  <div style="position: absolute; top: 6px; left: 42.86%; transform: translateX(-50%); font-size: 0.62em; color: #444; white-space: nowrap;">MM ↔ IT/NT</div>
  <div style="position: absolute; top: 18px; left: 42.86%; width: 7px; height: 7px; border-radius: 50%; background: #333; transform: translate(-50%, 0);"></div>
  <div style="position: absolute; top: 30px; left: 42.86%; width: 2px; height: 18px; background: #333;"></div>
  <div style="position: absolute; top: 6px; left: 57.14%; transform: translateX(-50%); font-size: 0.62em; color: #444; white-space: nowrap;">MM ↔ IT/NT</div>
  <div style="position: absolute; top: 18px; left: 57.14%; width: 7px; height: 7px; border-radius: 50%; background: #333; transform: translate(-50%, 0);"></div>
  <div style="position: absolute; top: 30px; left: 57.14%; width: 2px; height: 18px; background: #333;"></div>
  <div style="position: absolute; top: 6px; left: 71.43%; transform: translateX(-50%); font-size: 0.62em; color: #444; white-space: nowrap;">MM ↔ IT/NT</div>
  <div style="position: absolute; top: 18px; left: 71.43%; width: 7px; height: 7px; border-radius: 50%; background: #333; transform: translate(-50%, 0);"></div>
  <div style="position: absolute; top: 30px; left: 71.43%; width: 2px; height: 18px; background: #333;"></div>
  <div style="position: absolute; top: 6px; left: 85.71%; transform: translateX(-50%); font-size: 0.62em; color: #444; white-space: nowrap;">MM ↔ IT/NT</div>
  <div style="position: absolute; top: 18px; left: 85.71%; width: 7px; height: 7px; border-radius: 50%; background: #333; transform: translate(-50%, 0);"></div>
  <div style="position: absolute; top: 30px; left: 85.71%; width: 2px; height: 18px; background: #333;"></div>
  <div style="position: absolute; top: 6px; left: 100%; transform: translateX(-50%); font-size: 0.62em; color: #444; white-space: nowrap;">MM ↔ IT/NT</div>
  <div style="position: absolute; top: 18px; left: 100%; width: 7px; height: 7px; border-radius: 50%; background: #333; transform: translate(-50%, 0);"></div>
  <div style="position: absolute; top: 30px; left: 100%; width: 2px; height: 18px; background: #333;"></div>
</div>
</div>

<br> <br> 

<v-click>

### <u>Blockchain markets</u>: discrete clearing, orders are sequenced by priority fee

<div style="margin-top: -3px; padding: 0 30px;">
<div style="position: relative; height: 50px;">
  <div style="position: absolute; top: 38px; left: 0; right: 0; height: 2px; background: #333;"></div>
  <div style="position: absolute; top: 20px; left: 0; width: 9px; height: 9px; border-radius: 50%; background: #333; transform: translate(-2px, 0);"></div>
  <div style="position: absolute; top: 28px; left: 0; width: 3px; height: 22px; background: #333;"></div>
  <div style="position: absolute; top: 6px; right: 0; font-size: 0.62em; color: #444;">MM ↔ IT/NT</div>
  <div style="position: absolute; top: 20px; right: 0; width: 9px; height: 9px; border-radius: 50%; background: #333; transform: translate(2px, 0);"></div>
  <div style="position: absolute; top: 28px; right: 0; width: 3px; height: 22px; background: #333;"></div>
</div>
<div style="display: flex; justify-content: space-between; font-size: 0.8em; margin-top: 2px;">
  <span>   </span>
  <span style="font-style: italic;">block time T</span>
  <span>block creation</span>
</div>
</div>

<v-click>

<div style="position: relative; border: 1.5px solid #4b5563; border-radius: 4px; padding: 10px 4px 4px 4px; margin: 30px 30px 0;">
<div style="position: absolute; top: -8px; left: 12px; background: white; padding: 0 6px; font-size: 10px; font-weight: 700; color: #4b5563; letter-spacing: 0.5px;">block</div>
<div style="display: flex; gap: 2px;">
  <div style="flex: 70; border: 1.5px solid #1e40af; background: #dbeafe; padding: 6px 2px; text-align: center; font-size: 10px; line-height: 1.4; color: #1e3a8a;">
    <div style="font-weight: 700;">txn # 1</div>
    <div>fee Φ<sub>(1)</sub></div>
  </div>
  <div style="flex: 70; border: 1.5px solid #1e40af; background: #dbeafe; padding: 6px 2px; text-align: center; font-size: 10px; line-height: 1.4; color: #1e3a8a;">
    <div style="font-weight: 700;">txn # 2</div>
    <div>fee Φ<sub>(2)</sub></div>
  </div>
  <div style="flex: 70; border: 1.5px solid #1e40af; background: #dbeafe; padding: 6px 2px; text-align: center; font-size: 10px; line-height: 1.4; color: #1e3a8a;">
    <div style="font-weight: 700;">⋯</div>
    <div>⋯</div>
  </div>
  <div style="flex: 70; border: 1.5px solid #1e40af; background: #dbeafe; padding: 6px 2px; text-align: center; font-size: 10px; line-height: 1.4; color: #1e3a8a;">
    <div style="font-weight: 700;">txn # <i>N</i>−1</div>
    <div>fee Φ<sub>(<i>N</i>−1)</sub></div>
  </div>
  <div style="flex: 70; border: 1.5px solid #1e40af; background: #dbeafe; padding: 6px 2px; text-align: center; font-size: 10px; line-height: 1.4; color: #1e3a8a;">
    <div style="font-weight: 700;">txn # <i>N</i></div>
    <div>fee Φ<sub>(<i>N</i>)</sub></div>
  </div>
  <div style="flex: 400; border: 1.5px solid #888; background: #f3f4f6; padding: 6px 6px; text-align: center; font-size: 10px; line-height: 1.4; color: #374151;">
    <div style="margin-top: 2px;">uninformed demand</div>
    <div>priority fee = 0</div>
  </div>
</div>
</div>

<div style="text-align: center; font-size: 0.85em; color: #555; margin-top: 8px;">higher priority fee &nbsp;⟹&nbsp; earlier execution &nbsp;⟹&nbsp;  priority gas auction</div>

<br>

</v-click>
</v-click>

---
layout: two-cols-header
---

# Consensus shapes microstructure

###  Priority gas auction: **sealed-bid multi-prize auction** [Incorporate picture of prices moving]
**The prize.** A better queue position avoids the adverse price impact of the orders ahead — jumping one order saves its impact $2Q/L$. The contest is **all-pay** (every order executes and pays its fee) with **endogenous, valuation-dependent prizes**.

### Two types of memory pools, late bidding in both

::left::

<v-clicks>

* **Private memory pools**: bids are concealed until block creation $\implies$ traders submit at the last moment <br>

* **Public memory pools.** Late bidding is the dominant strategy because (i) early bids leak information, (ii) revisions increase the priority fee,  (iii) waiting incorporates recent information
  * *pure-noise hypothesis* of Biais, Hillion, and Spatt (1999)

</v-clicks>

::right::

<v-click at="3">


![distribPF](./images/distribPF.png){style="transform: translate(0%, -25%); width: 100%;"}


</v-click>


---

# This paper

### Can the blockchain itself be a venue for price formation?

A model of price formation and liquidity on a blockchain with **discrete clearing** and **paid-priority** ordering. We endogenise information acquisition, liquidity supply, participation, trading volumes, and priority fees.

**Three findings:**

<v-clicks>

1. **Endogenous selection** — paid priority creates a participation cutoff: only aggressive traders trade $\implies$ prices biased, less information revealed

2. **Competition reduces liquidity** — discrete clearing makes the LP absorb all adverse selection in one decision $\implies$ more competition, less depth

3. **Block time amplifies both** — it widens valuations and shrinks uninformed demand $\implies$ beyond a critical $T$, markets shut down

</v-clicks>


---

# The model: three stages

- <u>**Stage one**</u>: $M$ traders pay an information cost $C$ to enter the blockchain
- <u>**Stage two**</u>: liquidity supplier sets DEX depth $L$
- <u>**Stage three**</u>: informed traders compete in the priority gas auction (PGA)
![model1](./images/model1.png){style="transform: translate(10%, 9%); width: 600px"} 
<v-click>

![model2](./images/model2.png){style="transform: translate(13%, -95%); width: 600px"}
<v-click>

![model3](./images/model3.png){style="transform: translate(13%, -200%); width: 600px"}
<v-click>

![model4](./images/model4.png){style="transform: translate(13%, -305%); width: 600px"}

We solve by **backward induction**, starting from stage three and working back to stage one

</v-click>
</v-click>
</v-click>


---
section: Selection
---

# Endogenous selection

<div style="border: 1.5px solid #1e40af; border-radius: 6px; padding: 18px 26px; background: #f8fafc; margin: 34px auto 0; max-width: 840px;">

**Proposition (endogenous selection).** There is a cutoff valuation below which informed traders do not participate.

As the number of informed traders on the blockchain rises:

1. &nbsp; the participation **cutoff rises**,
2. &nbsp; **less information** is revealed to the market,
3. &nbsp; the **price at the end of the block increases**.

</div>


---

# Execution prices in the DEX

#### <u>**Linear price schedule**</u>. Buying a quantity $Q$ executes at

$$\underbrace{Q/L}_{\text{slippage}} \;+\; \underbrace{\pi}_{\text{DEX fee}}\quad\text{ per unit}\qquad\implies\qquad\text{cash paid } = Q\,(Q/L + \pi)$$

<v-click>

#### <u>**Linear price update rule**</u>. After a buy of size $Q$, the marginal price moves to

$$
2\,Q/L
$$


Deeper $L$ $\implies$ cheaper liquidity and smaller impact

<v-click>

<br>

### Why compete: example

- Trader 1 buys $Q_1$ first, then trader 2 buys $Q_2$
- Trader 1 pays $Q_1/L + \pi$ per unit
- The marginal price moves to $2Q_1/L$
- Trader 2 starts from $2Q_1/L$ and pays $\underbrace{2Q_1/L}_{\text{impact from trader 1}} \,+\, \underbrace{Q_2/L}_{\text{own slippage}} \,+\, \pi \quad\text{per unit}$ $\implies$ competition


</v-click>


</v-click>


---

# The priority gas auction

Trader $i$ ($v_i\sim F$ on $[0,\overline v]$) chooses a volume $Q_i$ and a priority fee $\Phi_i$; the builder orders the block by $\Phi$ — **multi-prize, all-pay, sealed-bid**.

<div style="margin: 4px 30px 0;">

<svg viewBox="0 0 600 54" preserveAspectRatio="none" style="width: 100%; height: 52px; display: block;">
  <path d="M 0 48 L 35 48 L 35 38 L 105 38 L 105 30 L 175 30 L 175 23 L 245 23 L 245 18 L 600 18" stroke="#1e40af" stroke-width="1.6" fill="none" vector-effect="non-scaling-stroke"/>
  <line x1="0" y1="26" x2="600" y2="26" stroke="#dc2626" stroke-width="1" stroke-dasharray="6,4" vector-effect="non-scaling-stroke"/>
  <circle cx="175" cy="26" r="3.5" fill="#dc2626"/>
  <text x="596" y="22" text-anchor="end" style="font-size: 9px; font-style: italic;" fill="#dc2626">trader i's valuation</text>
  <text x="4" y="11" style="font-size: 9px;" fill="#444">price</text>
</svg>

<div style="position: relative; border: 1.5px solid #4b5563; border-radius: 4px; padding: 7px 0 3px; margin-top: 1px;">
<div style="position: absolute; top: -8px; left: 12px; background: white; padding: 0 6px; font-size: 9px; font-weight: 700; color: #4b5563;">block</div>
<div style="display: flex;">
  <div style="flex: 70; border-right: 1px solid #93c5fd; background: #dbeafe; padding: 3px 1px; text-align: center; font-size: 9px; color: #1e3a8a;">txn 1 · Φ<sub>(1)</sub></div>
  <div style="flex: 70; border-right: 1px solid #93c5fd; background: #dbeafe; padding: 3px 1px; text-align: center; font-size: 9px; color: #1e3a8a;">txn 2 · Φ<sub>(2)</sub></div>
  <div style="flex: 70; border-right: 1px solid #93c5fd; background: #dbeafe; padding: 3px 1px; text-align: center; font-size: 9px; color: #1e3a8a;">⋯</div>
  <div style="flex: 70; border-right: 1px solid #93c5fd; background: #dbeafe; padding: 3px 1px; text-align: center; font-size: 9px; color: #1e3a8a;">txn N · Φ<sub>(N)</sub></div>
  <div style="flex: 320; background: #f3f4f6; padding: 3px 6px; text-align: center; font-size: 9px; color: #374151;">uninformed demand · fee = 0</div>
</div>
</div>

</div>

$$\scriptsize
\mathbb E_i[W_i] = J(v_i,Q_i)= \underbrace{-\Phi_i}_{\text{priority fee}} + \underbrace{Q_i\big(v_i-\pi-\dfrac{Q_i}{L}\big)}_{\text{trading profit, net of slippage}} - C - \underbrace{\dfrac{2Q_i}{L}\sum_{j=0}^{M-1}\mathbb E_i\big[\mathbf 1_{\Phi_{(j)}<\Phi_i<\Phi_{(j+1)}}\,\Delta_{(j+1:M-1)}\big]}_{\text{adverse impact from rivals ahead}}
$$

<v-click>

<div style="border: 1.5px solid #1e40af; border-radius: 6px; padding: 6px 20px; background: #f8fafc; margin: 4px auto 0; max-width: 920px;">

**Proposition.** The equilibrium priority fee and trading volume both **increase in $v_i$**; traders with $v_i<\underline v_M$ abstain.

</div>

$$\footnotesize
\underbrace{\Phi(Q_i)=\dfrac{2}{L}(M\!-\!1)\!\int_0^{Q_i}\!x^2\,dG(x)}_{\text{priority fee}}, \qquad \text{payoff}=\underbrace{\dfrac{2Q_i}{L}(M\!-\!1)\!\int_0^{Q_i}\!x\,dG}_{\text{reservation fee}}-\Phi(Q_i)\;\ge\;0
$$

$$\footnotesize
\underbrace{Q(v_i)=\dfrac{L(\overline v-\pi)}{2(M-1)}\Big(e^{(M-1)(v_i-\underline v_M)/(\overline v-\pi)}-1\Big)}_{\text{trading volume (uniform $F$)}}, \quad Q(v_i)=0\ \text{ for } v_i<\underline v_M
$$

</v-click>


---

# More competition raises the cutoff

<div style="margin: 6px auto 0; max-width: 600px;">

<svg viewBox="0 0 800 200" preserveAspectRatio="xMidYMid meet" style="width: 100%; height: auto; display: block;">
  <defs><marker id="arrM" markerWidth="7" markerHeight="7" refX="5" refY="2.5" orient="auto"><path d="M0,0 L5,2.5 L0,5 z" fill="#dc2626"/></marker></defs>
  <line x1="70" y1="170" x2="745" y2="170" stroke="#444" stroke-width="1"/>
  <line x1="70" y1="22" x2="70" y2="170" stroke="#444" stroke-width="1"/>
  <text x="64" y="30" text-anchor="end" style="font-size: 9px;" fill="#444">density</text>
  <text x="742" y="186" text-anchor="end" style="font-size: 9px;" fill="#444">valuation</text>
  <text x="70" y="186" text-anchor="middle" style="font-size: 9px;" fill="#444">0</text>
  <text x="730" y="186" text-anchor="middle" style="font-size: 9px;" fill="#444">v̄</text>
  <path d="M 466 170 L 466 44 L 532 60 L 598 86 L 664 123 L 730 170 Z" fill="#1e40af" fill-opacity="0.16"/>
  <path d="M 70 170 L 136 123 L 202 86 L 268 60 L 334 44 L 400 38 L 466 44 L 532 60 L 598 86 L 664 123 L 730 170" stroke="#1e40af" stroke-width="2" fill="none"/>
  <line x1="466" y1="44" x2="466" y2="170" stroke="#dc2626" stroke-width="1.5"/>
  <text x="466" y="186" text-anchor="middle" style="font-size: 9px;" fill="#dc2626">v<tspan baseline-shift="sub" style="font-size: 7px;">M</tspan></text>
  <line x1="598" y1="86" x2="598" y2="170" stroke="#dc2626" stroke-width="1.2" stroke-dasharray="4,3"/>
  <line x1="474" y1="152" x2="590" y2="152" stroke="#dc2626" stroke-width="1.5" marker-end="url(#arrM)"/>
  <text x="531" y="146" text-anchor="middle" style="font-size: 9.5px; font-style: italic;" fill="#dc2626">M ↑</text>
  <text x="600" y="112" text-anchor="middle" style="font-size: 9px;" fill="#1e40af">active traders</text>
</svg>

</div>

**Cutoff** (uniform valuations): $\quad \underline v_M = \overline v - (\overline v-\pi)\,\dfrac{\log M}{M-1}\,$ — increasing in $M$, with $\underline v_M\to\overline v$.

<v-click>

<div style="border: 1.5px solid #1e40af; border-radius: 6px; padding: 8px 22px 2px; background: #f8fafc; margin: 6px auto 0; max-width: 940px;">

**Proposition.** As $M$ rises, the end-of-block price and aggregate informed volume both **increase in $M$**:

$$\small
\underbrace{\frac{M(\underline v_M-\pi)}{M-1}}_{\text{end-of-block price}}\;\xrightarrow[M\to\infty]{}\;\overline v-\pi, \qquad\qquad
\underbrace{\frac{L\,M(\underline v_M-\pi)}{2(M-1)}}_{\text{aggregate informed volume}}\;\xrightarrow[M\to\infty]{}\;L\,\frac{\overline v-\pi}{2}.
$$

</div>

$\implies$ more competition reveals **less** information and biases the price to the extreme.

</v-click>




---

# Empirical validation

- only high-valuation traders participate: per-transaction size $\approx$ \$70k on Uniswap v3 vs $\approx$ \$1.2k on Binance (same pair)
- higher valuations $\to$ larger volumes, higher fees, and better queue positions:

![PF1](./images/tradingvolumes.png){style="width: 50%; display: block; margin: 6px auto 0;"}
<div style="text-align:center;"><font size="2">Average absolute trading volume vs queue position (Uniswap v3): volume falls with position, as predicted</font></div>


---
section: Liquidity
---

# Competition reduces liquidity

### More informed competition $\implies$ less depth — beyond a threshold, the market shuts down

<div style="margin: 4px auto 0; max-width: 720px;">

<svg viewBox="0 0 800 195" preserveAspectRatio="xMidYMid meet" style="width: 100%; height: auto; display: block;">
  <!-- Rounds timeline -->
  <line x1="40" y1="50" x2="790" y2="50" stroke="#333" stroke-width="2"/>

  <text x="48" y="22" text-anchor="middle" style="font-size: 9px;" fill="#444">MM ↔ IT/NT</text>
  <circle cx="48" cy="36" r="3.5" fill="#333"/>
  <line x1="48" y1="40" x2="48" y2="50" stroke="#333" stroke-width="1.5"/>

  <text x="152" y="22" text-anchor="middle" style="font-size: 9px;" fill="#444">MM ↔ IT/NT</text>
  <circle cx="152" cy="36" r="3.5" fill="#333"/>
  <line x1="152" y1="40" x2="152" y2="50" stroke="#333" stroke-width="1.5"/>

  <text x="256" y="22" text-anchor="middle" style="font-size: 9px;" fill="#444">MM ↔ IT/NT</text>
  <circle cx="256" cy="36" r="3.5" fill="#333"/>
  <line x1="256" y1="40" x2="256" y2="50" stroke="#333" stroke-width="1.5"/>

  <text x="360" y="22" text-anchor="middle" style="font-size: 9px;" fill="#444">MM ↔ IT/NT</text>
  <circle cx="360" cy="36" r="3.5" fill="#333"/>
  <line x1="360" y1="40" x2="360" y2="50" stroke="#333" stroke-width="1.5"/>

  <text x="464" y="22" text-anchor="middle" style="font-size: 9px;" fill="#444">MM ↔ IT/NT</text>
  <circle cx="464" cy="36" r="3.5" fill="#333"/>
  <line x1="464" y1="40" x2="464" y2="50" stroke="#333" stroke-width="1.5"/>

  <text x="568" y="22" text-anchor="middle" style="font-size: 9px;" fill="#444">MM ↔ IT/NT</text>
  <circle cx="568" cy="36" r="3.5" fill="#333"/>
  <line x1="568" y1="40" x2="568" y2="50" stroke="#333" stroke-width="1.5"/>

  <text x="672" y="22" text-anchor="middle" style="font-size: 9px;" fill="#444">MM ↔ IT/NT</text>
  <circle cx="672" cy="36" r="3.5" fill="#333"/>
  <line x1="672" y1="40" x2="672" y2="50" stroke="#333" stroke-width="1.5"/>

  <text x="776" y="22" text-anchor="middle" style="font-size: 9px;" fill="#444">MM ↔ IT/NT</text>
  <circle cx="776" cy="36" r="3.5" fill="#333"/>
  <line x1="776" y1="40" x2="776" y2="50" stroke="#333" stroke-width="1.5"/>

  <!-- Liquidity axes -->
  <line x1="40" y1="70" x2="40" y2="180" stroke="#444" stroke-width="1"/>
  <line x1="40" y1="180" x2="790" y2="180" stroke="#444" stroke-width="1"/>
  <text x="6" y="76" style="font-size: 9px;" fill="#444">liquidity</text>
  <text x="40" y="192" text-anchor="start" style="font-size: 9px;" fill="#444">t = 0</text>
  <text x="790" y="192" text-anchor="end" style="font-size: 9px;" fill="#444">t = T</text>

  <!-- Liquidity step function: 8 transitions aligned to the 8 rounds above -->
  <path d="M 40 165 L 48 165 L 48 155 L 152 155 L 152 145 L 256 145 L 256 135 L 360 135 L 360 125 L 464 125 L 464 115 L 568 115 L 568 105 L 672 105 L 672 95 L 776 95 L 776 85 L 790 85"
        stroke="#1e40af" stroke-width="2" fill="none"/>
  <text x="500" y="80" text-anchor="start" style="font-size: 10px;" fill="#1e40af">traditional market: multiple rounds, depth improves</text>

  <!-- Blockchain reference, flat from t = 0 -->
  <line x1="40" y1="172" x2="790" y2="172" stroke="#dc2626" stroke-width="2" stroke-dasharray="5,3"/>
  <text x="785" y="168" text-anchor="end" style="font-size: 10px;" fill="#dc2626">blockchain: single round, depth flat from t = 0</text>
</svg>

</div>

<v-click>

- **discrete clearing**: the LP makes a **single** liquidity decision and absorbs all informed flow at once — no improvement across rounds (vs Holden-Subrahmanyam)

</v-click>

<v-click>

**Free entry $\implies$ zero profit**: fee revenue from noise traders $=$ losses to informed. For uniform valuations,
$$\small
L^\star(M) = \frac{8\,\pi N\,(M-1)^3}{M(\overline v-\pi)^2\big[(M-1)(3M-5)-2(2M-3)\log M+2(\log M)^2\big]} - \theta
$$
**decreasing in $M$** — beyond a critical $M$, $\;L^\star(M)\le 0\;$ and the **market shuts down** (Glosten-Milgrom freeze).

</v-click>


---

# The information paradox

### Cheaper information or more uninformed demand $\implies$ *less* price discovery

<v-click>

**Proposition.** The equilibrium number of informed traders is the largest $M$ such that
$$\small
C\;\le\;\underbrace{L^\star(M)\!\int_{\underline v_M}^{\overline v}\!\tilde Q(v)^2\big[\,1-2(M-1)(1-F(v))\,\big]\,dF(v)}_{\text{ex-ante payoff per informed trader}}
$$

</v-click>

<v-click>

- **more noise trading** ($N\uparrow$) and **cheaper information** ($C\downarrow$) raise the equilibrium $M^\star$
- a higher $M^\star$ $\implies$ **less information** revealed and **less liquidity** in the market

</v-click>


---
section: Block time
---

# Block time: security vs efficiency

### Longer block time secures consensus but degrades markets — beyond a critical $T$, the market collapses

<v-click>

**How.** Block time $T$ shapes the primitives: longer blocks **widen valuations** ($\overline v(T)\uparrow$, in the FOSD sense) and **shrink uninformed demand** ($N(T)\downarrow$).

</v-click>

<v-click>

- the cutoff $\underline v_M(T)$ and the end-of-block price $\overline v(T)-\pi$ both rise $\implies$ prices drift further from fundamentals
- sustainable liquidity $\;L^\infty(T) = \dfrac{8\,\pi\,N(T)}{3\,(\overline v(T)-\pi)^2} - \theta\;$ is **decreasing in $T$** — beyond a critical $T$, the **market collapses**

</v-click>

<v-click>

**Takeaway.** The features that secure decentralization — **block time** and **paid priority** — undermine the blockchain as a venue for **price formation**. Under current design, blockchains are not viable as the sole venue for price discovery; protocols must rethink **how transactions are organized within a block**.

</v-click>

---
layout: end
---
Thank you !

[faycaldrissi.com](https://www.faycaldrissi.com/)
