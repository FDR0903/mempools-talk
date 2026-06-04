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

# Viability of Blockchain Markets

<br>
<br>


### Agostino Capponi, Álvaro Cartea, and Fayçal Drissi

<br>

### 6th Annual CBER Conference, NYU Stern

<br>

#### These slides: [https://www.faycaldrissi.com/mempools-talk](https://www.faycaldrissi.com/mempools-talk)



---
section: Motivation
---

# Blockchains

### Blockchains promise to coordinate economic activity at scale without intermediaries
- **financial markets are central to this promise**: whether the chain can host *viable* markets is a fundamental test
- blockchains replace *institutional trust* with *algorithmic, publicly verifiable rules*

<br>

<v-click>

### Consensus has a price
- requires **time** to secure the chain
  $\implies$ **block time**
- requires economic **incentives** to compensate validators
  - **priority fees**
  - others (gas fees, issuance ..)
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
    <div>priority fee Φ<sub>(1)</sub></div>
  </div>
  <div style="flex: 70; border: 1.5px solid #1e40af; background: #dbeafe; padding: 6px 2px; text-align: center; font-size: 10px; line-height: 1.4; color: #1e3a8a;">
    <div style="font-weight: 700;">txn # 2</div>
    <div>priority fee Φ<sub>(2)</sub></div>
  </div>
  <div style="flex: 70; border: 1.5px solid #1e40af; background: #dbeafe; padding: 6px 2px; text-align: center; font-size: 10px; line-height: 1.4; color: #1e3a8a;">
    <div style="font-weight: 700;">⋯</div>
    <div>⋯</div>
  </div>
  <div style="flex: 70; border: 1.5px solid #1e40af; background: #dbeafe; padding: 6px 2px; text-align: center; font-size: 10px; line-height: 1.4; color: #1e3a8a;">
    <div style="font-weight: 700;">...</div>
    <div>...</div>
  </div>
  <div style="flex: 70; border: 1.5px solid #1e40af; background: #dbeafe; padding: 6px 2px; text-align: center; font-size: 10px; line-height: 1.4; color: #1e3a8a;">
    <div style="font-weight: 700;">txn # <i>N</i></div>
    <div>priority fee Φ<sub>(<i>N</i>)</sub></div>
  </div>
  <div style="flex: 400; border: 1.5px solid #888; background: #f3f4f6; padding: 6px 6px; text-align: center; font-size: 10px; line-height: 1.4; color: #374151;">
    <div>priority fee = 0</div>
  </div>
</div>
</div>

<div style="text-align: center; font-size: 0.85em; color: #555; margin-top: 8px;">higher priority fee &nbsp;⟹&nbsp; earlier execution</div>

<br>

</v-click>
</v-click>

---

# This paper

### Can the blockchain itself be a venue for price formation?

- A model of price formation and liquidity on a blockchain with **discrete clearing** and **paid-priority** ordering 

<br>

<!--
<v-click>

### Findings

1. **Endogenous selection**: only aggressive traders participate $\implies$ prices are biased, less information in markets
2. Cheaper information and benign trading flow **impair** price formation
3. Block time impairs markets

</v-click>
-->

<v-click>

### The model: three stages
<u>**Stage one**</u>: $M$ traders pay an information cost $C$<br>
<u>**Stage two**</u>: liquidity supplier sets liquidity supply $L$ <br>
<u>**Stage three**</u>: informed traders compete for queue position and price-sensitive traders submit transactions

![model1](./images/model1.png){style="transform: translate(43%, 0%); width: 450px"} 
<v-click>


![model2](./images/model2.png){style="transform: translate(43%, -106%); width: 450px"}
<v-click>

![model3](./images/model3.png){style="transform: translate(43%, -211%); width: 450px"}
<v-click>

![model4](./images/model4.png){style="transform: translate(43%, -318%); width: 450px"}

We solve by **backward induction**, starting from stage three and working back to stage one

</v-click>
</v-click>
</v-click>
</v-click>


---
section: Results
---

# Result 1: endogenous selection



<div style="border: 1.5px solid #1e40af; border-radius: 6px; padding: 18px 26px; background: #f8fafc; margin: 34px auto 0; max-width: 840px;">

**Proposition (endogenous selection).** Only aggressive informed traders participate

$\longleftrightarrow$ 

There is a cutoff valuation $\underline v_M$ below which informed traders do not participate.


<!-- As the number $M$ of informed traders on the blockchain rises:

1. &nbsp; the participation **cutoff rises** $\implies$ fraction of the valuation distribution that generates transactions shrinks
2. &nbsp; aggregate trading volume increases
3. &nbsp; prices becomes systematically biased -->

</div>

---
layout: two-cols-header
---

# Position in the block matters

##  Blockchain round with discriminatory pricing
<div style="margin: 4px 30px 0;">
<svg viewBox="0 0 600 72" preserveAspectRatio="none" style="width: 100%; height: 70px; display: block;">
  <path d="M 0 64 L 35 64 L 35 51 L 105 51 L 105 39 L 175 39 L 175 28 L 245 28 L 245 18 L 600 18" stroke="#1e40af" stroke-width="1.6" fill="none" vector-effect="non-scaling-stroke"/>
  <text x="4" y="12" style="font-size: 8px;" fill="#444">price</text>
</svg>

<div style="position: relative; border: 1.5px solid #4b5563; border-radius: 4px; padding: 7px 0 3px; margin-top: 1px;">
<div style="position: absolute; top: -8px; left: 12px; background: white; padding: 0 6px; font-size: 9px; font-weight: 700; color: #4b5563;">block</div>
<div style="display: flex;">
  <div style="flex: 70; border-right: 1px solid #93c5fd; background: #dbeafe; padding: 3px 1px; text-align: center; font-size: 9px; color: #1e3a8a;">txn 1 · Φ<sub>(1)</sub></div>
  <div style="flex: 70; border-right: 1px solid #93c5fd; background: #dbeafe; padding: 3px 1px; text-align: center; font-size: 9px; color: #1e3a8a;">txn 2 · Φ<sub>(2)</sub></div>
  <div style="flex: 70; border-right: 1px solid #93c5fd; background: #dbeafe; padding: 3px 1px; text-align: center; font-size: 9px; color: #1e3a8a;">⋯</div>
  <div style="flex: 70; border-right: 1px solid #93c5fd; background: #dbeafe; padding: 3px 1px; text-align: center; font-size: 9px; color: #1e3a8a;">txn N · Φ<sub>(N)</sub></div>
  <div style="flex: 320; background: #f3f4f6; padding: 3px 6px; text-align: center; font-size: 9px; color: #374151;">fee = 0</div>
</div>
</div>

</div>

<br>

<v-click>

### $\implies$ blockchain trading round is a single **sealed-bid multi-prize auction**

</v-click>

::left::

<v-click>


<br><br>

## Not an online auction

1. **Private memory pools**: bids are concealed until block creation
<v-click>

2. **Public memory pools**: late bidding is dominant

</v-click>
</v-click>

::right::

<v-click at="3">

![distribPF](./images/distribPF.png){style="transform: translate(25%, 0%); width: 90%;"}

</v-click>


---

# Execution prices in the DEX

#### <u>**Linear price schedule**</u>. Buying a quantity $Q$ executes at

$$\small \underbrace{Q/L}_{\text{slippage}} \;+\; \underbrace{\pi}_{\text{DEX fee}}\quad\text{ per unit}$$
<!--\qquad\implies\qquad\text{cash paid } = Q\,(Q/L + \pi)-->
Deeper $L$ $\implies$ cheaper liquidity

<v-click>

#### <u>**Linear price update rule**</u>. After a buy of size $Q$, the marginal price moves to

$$ \small
2\,Q/L
$$


Deeper $L$ $\implies$ smaller impact

<v-click>

<br>

#### <u>**Why compete ?**</u>

- Trader 1 buys $Q_1$ first, then trader 2 buys $Q_2$ 
<v-click>

- Trader 1 pays $Q_1/L + \pi$ per unit, and the marginal price moves to $2Q_1/L$
<v-click>

- Trader 2  pays $\qquad \qquad \qquad \qquad \qquad \qquad \small \underbrace{2Q_1/L}_{\text{impact from trader 1}} \,+\, \underbrace{Q_2/L}_{\text{own slippage}} \,+\, \pi \quad\text{per unit}$

</v-click>
</v-click>
</v-click>
</v-click>


---

# The trading round

**<u>Setup</u>**: $M\,$ buying traders<br> $\qquad\ \,$ Each trader has valuation $\,v \in [0, \overline v] \sim F\,$ chooses a volume $\, Q_i\,$ and a priority fee $\, \Phi_i$

<div style="margin: 4px 30px 0;">

<svg viewBox="0 0 600 54" preserveAspectRatio="none" style="width: 100%; height: 52px; display: block;">
  <path d="M 0 48 L 35 48 L 35 38 L 105 38 L 105 30 L 175 30 L 175 23 L 245 23 L 245 18 L 600 18" stroke="#1e40af" stroke-width="1.6" fill="none" vector-effect="non-scaling-stroke"/>
  <line x1="0" y1="26" x2="600" y2="26" stroke="#dc2626" stroke-width="1" stroke-dasharray="6,4" vector-effect="non-scaling-stroke"/>
  <circle cx="175" cy="26" r="3.5" fill="#dc2626"/>
  <text x="596" y="35" text-anchor="end" style="font-size: 9px; font-style: italic;" fill="#dc2626">trader i's valuation</text>
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

$$\footnotesize
\text{expected wealth of trader } i= \underbrace{-\Phi_i}_{\text{priority fee}} + \underbrace{Q_i\big(v_i-\pi-\dfrac{Q_i}{L}\big)}_{\text{trading profit, net of slippage}} - \underbrace{C}_{\text{information cost}} - \underbrace{\dfrac{2Q_i}{L}\sum_{j=0}^{M-1}\mathbb E_i\big[\mathbf 1_{\Phi_{(j)}<\Phi_i<\Phi_{(j+1)}}\,\Delta_{(j+1:M-1)}\big]}_{\text{adverse impact of competitors}}
$$

<div style="border: 1.5px solid #1e40af; border-radius: 6px; padding: 0px 20px; background: #f8fafc; margin: -5px auto 0; max-width: 920px;">

<div v-click>

**Proposition.** For sufficiently low valuations $v_i < \underline v_M$: $\qquad\qquad\qquad\qquad\qquad\footnotesize
\boxed{\text{volume }=\text{ priority fee }=0\qquad \forall v_i<\underline v_M}$

</div>
<div v-click>

For all $v_i \ge \underline v_M$, the equilibrium priority fee and trading volume **increase in $v_i$**
$$\footnotesize
\underbrace{\Phi^*\left(v_{i}\right)=2L(M-1)\int_{\underline{v}_M}^{v_{i}}\tilde{Q}^*\left(x\right)^{2}dF\left(x\right)}_{\text{priority fee}} 
\qquad 
\text{payoff}=\text{reservation fee}-\Phi^*(v_i)\ge0\qquad 
\underbrace{Q^*(v_i)=L\tilde Q^*(v_i)=L\dfrac{\overline v-\pi}{2(M-1)}\big(e^{(M-1)(v_i-\underline v_M)/(\overline v-\pi)}-1\big)}_{\text{trading volume}}
$$
</div>
</div>

---
layout: two-cols-header
---

# More competition raises the cutoff

::left::

<div style="border: 1.5px solid #1e40af; border-radius: 6px; padding: -8px 22px 2px; background: #f8fafc; margin: 6px auto 0; max-width: 940px;">

**Propositions.** As $M$ rises

- the **cutoff** increases and $\quad \underline v_M \xrightarrow[M\to\infty]{}\;\overline v.$

<div v-click>

- the end-of-block price and aggregate informed volume  **increase**
$$\small
\underbrace{\frac{M(\underline v_M-\pi)}{M-1}}_{\text{end-of-block price}}\;\xrightarrow[M\to\infty]{}\;\overline v-\pi 
\qquad\qquad
\underbrace{L\times\frac{M(\underline v_M-\pi)}{2(M-1)}}_{\text{aggregate informed volume}}\;\xrightarrow[M\to\infty]{}\;L\,\frac{\overline v-\pi}{2}
$$
</div>

<div v-click>

- equilibrium liquidity $L^\star(M)$ is decreasing in $M$
  
  $$L^\star(M)  \xrightarrow[M\to\infty]{} \quad \underbrace{\frac{8\,\pi\,N}{3\,(\overline{v}-\pi)^2}}_\text{ratio of revenue to adverse selection}-\underbrace{\theta}_\text{price sensitivity}$$

</div>
<div v-click>

$\implies$ more competition $\to$ less information + price bias $\to$ less liquidity

</div>
</div>
<br>
<br>

::right::

<div style="margin: 6px auto 0; max-width: 100%;">

<svg viewBox="0 0 600 480" preserveAspectRatio="xMidYMid meet" style="width: 100%; height: auto; display: block;">
  <defs><marker id="arrM" markerWidth="7" markerHeight="7" refX="5" refY="2.5" orient="auto"><path d="M0,0 L5,2.5 L0,5 z" fill="#dc2626"/></marker></defs>
  <line x1="75" y1="410" x2="585" y2="410" stroke="#444" stroke-width="1.2"/>
  <line x1="75" y1="30" x2="75" y2="410" stroke="#444" stroke-width="1.2"/>
  <text x="82" y="26" text-anchor="start" style="font-size: 21px;" fill="#444">density</text>
  <text x="330" y="467" text-anchor="middle" style="font-size: 21px;" fill="#444">valuation</text>
  <text x="75" y="435" text-anchor="middle" style="font-size: 21px;" fill="#444">0</text>
  <text x="575" y="435" text-anchor="middle" style="font-size: 21px;" fill="#444">v̄</text>
  <path d="M 325 410 L 325 318 L 375 351 L 425 377 L 475 395 L 525 406 L 575 410 Z" fill="#1e40af" fill-opacity="0.16"/>
  <path d="M 75 40 L 125 110 L 175 173 L 225 229 L 275 277 L 325 318 L 375 351 L 425 377 L 475 395 L 525 406 L 575 410" stroke="#1e40af" stroke-width="2.5" fill="none"/>
  <line x1="325" y1="318" x2="325" y2="410" stroke="#dc2626" stroke-width="2"/>
  <text x="325" y="435" text-anchor="middle" style="font-size: 21px;" fill="#dc2626">v<tspan baseline-shift="sub" style="font-size: 14px;">M</tspan></text>
  <line x1="405" y1="367" x2="405" y2="410" stroke="#dc2626" stroke-width="1.5" stroke-dasharray="5,4"/>
  <line x1="333" y1="392" x2="397" y2="392" stroke="#dc2626" stroke-width="2" marker-end="url(#arrM)"/>
  <text x="365" y="380" text-anchor="middle" style="font-size: 23px; font-style: italic;" fill="#dc2626">M ↑</text>
  <text x="455" y="288" text-anchor="middle" style="font-size: 21px;" fill="#1e40af">active traders</text>
</svg>

</div>

---

# Result 2: information paradox

<div style="border: 1.5px solid #1e40af; border-radius: 6px; padding: -12px 22px 2px; background: #f8fafc; margin: 6px auto 0; max-width: 940px;">

**Proposition.** The equilibrium number of informed traders is the largest $M$ such that
$$\small
\underbrace{C}_\text{information cost}\;\le\;\underbrace{L^\star(M^\star)\!\int_{\underline v_M}^{\overline v}\!\tilde Q^*(v)^2\big[\,1-2(M^\star-1)(1-F(v))\,\big]\,dF(v)}_{\text{ex-ante payoff per informed trader}}
$$

</div>

<br><br>

-  **more noise trading** ($N\uparrow$) and **cheaper information** ($C\downarrow$) raise the equilibrium $M^\star$

- paid-priority
discriminatory pricing  $\implies$  **less information** revealed and biased prices



---

# Result 3: block time impairs efficiency



<div style="border: 1.5px solid #1e40af; border-radius: 6px; padding: 8px 22px; background: #f8fafc; margin: 6px auto 0; max-width: 940px;">

**Assumption.** Longer block time $T$<br>
(i) widens the valuation distribution (FOSD sense) <br> 
(ii) shrinks price-sensitive uninformed demand

</div>
<br>

<v-click>

- the cutoff $\underline v_M(T)$ increases <br><br>
- the end-of-block price $\overline v(T)-\pi$ increases<br><br>
- sustainable liquidity $\;L^\infty(T) = \dfrac{8\,\pi\,N(T)}{3\,(\overline v(T)-\pi)^2} - \theta\;$ is **decreasing in $T$**
<br>
<br>

- beyond a critical block time $T$, the **market collapses**

</v-click>


---

# Some empirics

- only high-valuation traders participate

 per-transaction size $\approx$ \$70k on Uniswap v3 vs $\approx$ \$1.2k on Binance (same pair)

<v-click>

- higher valuations $\to$ larger volumes and higher fees $\to$ better queue positions:

![PF1](./images/tradingvolumes.png){style="width: 70%; display: block; margin: 6px auto 0;"}
<div style="text-align:center;"><font size="2">Average absolute trading volume vs queue position (Uniswap v3)</font></div>

</v-click>



<!--

# Result 2: competition reduces liquidity



<div style="border: 1.5px solid #1e40af; border-radius: 6px; padding: -12px 22px 2px; background: #f8fafc; margin: 6px auto 0; max-width: 940px;">

**Proposition.**  equilibrium liquidity $L^\star(M)$ is decreasing in $M$, increasing in noise  volume $\pi\,N$, decreasing in price sensitivity $\theta$
$$\small
L^\star(M)  \xrightarrow[M\to\infty]{} \quad \underbrace{\frac{8\,\pi\,N}{3\,(\overline{v}-\pi)^2}}_\text{ratio of revenue to adverse selection}-\underbrace{\theta}_\text{price sensitivity}
$$

Condition for markets to operate: $\qquad\qquad \text{adverse selection from }M\text{ traders} < \pi \, N / \theta$

</div>

<v-click>

### <u>Traditional markets</u>: liquidity improves after early rounds
### <u>Blockchain markets</u>: liquidity supply single decision


<div style="margin: 4px auto 0; max-width: 720px;">

<svg viewBox="0 0 800 195" preserveAspectRatio="xMidYMid meet" style="width: 100%; height: auto; display: block;">

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

  <line x1="40" y1="70" x2="40" y2="180" stroke="#444" stroke-width="1"/>
  <line x1="40" y1="180" x2="790" y2="180" stroke="#444" stroke-width="1"/>
  <text x="6" y="76" style="font-size: 9px;" fill="#444">liquidity</text>
  <text x="40" y="192" text-anchor="start" style="font-size: 9px;" fill="#444">t = 0</text>
  <text x="790" y="192" text-anchor="end" style="font-size: 9px;" fill="#444">t = T</text>

  <path d="M 40 165 L 48 165 L 48 155 L 152 155 L 152 145 L 256 145 L 256 135 L 360 135 L 360 125 L 464 125 L 464 115 L 568 115 L 568 105 L 672 105 L 672 95 L 776 95 L 776 85 L 790 85"
        stroke="#1e40af" stroke-width="2" fill="none"/>
  <text x="500" y="80" text-anchor="start" style="font-size: 10px;" fill="#1e40af">traditional market: multiple rounds, depth improves</text>

  <line x1="40" y1="172" x2="790" y2="172" stroke="#dc2626" stroke-width="2" stroke-dasharray="5,3"/>
  <text x="785" y="168" text-anchor="end" style="font-size: 10px;" fill="#dc2626">blockchain: single round, depth flat from t = 0</text>
</svg>

</div>
</v-click>
-->

---
section: conclusion
layout: end
---

**Takeaway:** The features that secure decentralization (**block time** and **paid priority**) undermine the blockchain as a venue for **price formation**.

<v-click>

Thank you !

<br>

Capponi, Cartea, and Drissi (2025), *The Viability of Blockchain Markets under Discrete Clearing and Paid Priority*

<br>

These slides: [www.faycaldrissi.com/mempools-talk](https://www.faycaldrissi.com/mempools-talk)

</v-click>
