# CMOS Inverter Voltage Transfer Characteristics (VTC) Analysis

## 1. Introduction
The Voltage Transfer Characteristics (VTC) of a CMOS inverter define the relationship between the input voltage (Vin) and the output voltage (Vout). VTC analysis is crucial for understanding the behavior of the inverter in different operating regions and determining key performance metrics like noise margins and switching threshold.

---

## 2. VTC Curve Description
The VTC curve can be divided into three regions:
- **Region 1 (Vin < Vth,n)**: NMOS is OFF, and PMOS is ON, resulting in a high output voltage (Vout ≈ Vdd).
- **Region 2 (Vth,n < Vin < Vdd - Vth,p)**: Both NMOS and PMOS are partially ON, leading to the transition region.
- **Region 3 (Vin > Vdd - Vth,p)**: NMOS is ON, and PMOS is OFF, resulting in a low output voltage (Vout ≈ 0).

---

## 3. Key Metrics from VTC Analysis

### 3.1 Switching Threshold (Vm)
- The input voltage (Vin) at which the output voltage (Vout) equals Vin.
- Observed Vm: `X.X V`

### 3.2 Noise Margins
- **Noise Margin High (NMH):** `NMH = VOH - VIH`
- **Noise Margin Low (NML):** `NML = VIL - VOL`
- Observed NMH: `X.X V`
- Observed NML: `X.X V`

### 3.3 Gain (|dVout/dVin|)
- The maximum slope of the VTC curve in the transition region.
- Observed Gain: `X.X`

---

## 4. Plots
### 4.1 VTC Curve
![VTC Curve](plots/VTC_Curve.png)

### 4.2 Noise Margins
![Noise Margins](plots/Noise_Margins.png)

### 4.3 Gain Plot
![Gain Plot](plots/Gain_Plot.png)

---

## 5. Observations and Conclusion
- The VTC curve demonstrates a clear and sharp transition between the logic levels.
- The calculated noise margins indicate good noise immunity.
- The gain in the transition region is high, ensuring robust signal amplification.

---

### Future Work
- Analyze the effect of process variation and temperature on VTC.
- Extend the study to include dynamic characteristics of the CMOS inverter (e.g., rise/fall times, propagation delay).
