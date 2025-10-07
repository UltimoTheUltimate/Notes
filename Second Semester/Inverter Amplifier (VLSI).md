## Inverter Amplifier

The inverter amplifier consists of:
- A driving transistor **M1** (the transistor where the input signal to be amplified, $v_{in}$, is applied)
- An MOS transistor in pinchoff **M2** (serving as a "current-source" load)

---

### DC Operation

Consider $V_{in}$ as it increases from 0V to $V_{DD}$ (typically $V_{D0} \approx 3V$ or $5V$).



- Note that $V_{GS1} = V_{in}$
- $V_{out} = V_{DD} - V_{SD2}$  
    or  
    $V_{out} = V_{DS1}$

#### When $V_{in} < V_T$ ($V_{GS1} < V_T$)
- M1 is **OFF** $\rightarrow$ $I = 0$
- Therefore, $V_{out} = V_{DD}$
- Since $V_{SD2}$ is the "$I_{DR}$" drop across M2 and $I_D = 0$, $V_{SD2} = 0V$

#### When $V_{in} = V_T^+$
- $V_{GS1} = V_T^+$
- M1 switches **ON** and enters pinchoff  
    (since $V_{DS1} \equiv V_{out} \equiv V_{DD}$)
- Current $I_D$ starts to flow

#### As $V_{in}$ increases:
- $V_{GS1}$ increases $\rightarrow$ $I_D$ increases
- Therefore, "$I_D R$" drop across M2 increases
- $\therefore V_{out} = V_{DD} - V_{SD}$  
    $= V_{DD} -$ ("$I_D R$" drop decreases)

- Both M1 and M2 are in pinchoff

#### As $V_{in} \rightarrow V_{DD}$:
- $V_{out} \rightarrow$ a few mV
- M1 enters the ohmic region