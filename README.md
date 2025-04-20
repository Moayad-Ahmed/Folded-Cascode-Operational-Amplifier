# Folded Cascode Operational Amplifier
## 📋 Project Overview
This project focuses on the design and simulation of a Folded Cascode Op-Amp using 65nm TSMC technology. The project includes DC, AC, and transient analyses, along with various performance metrics to validate the design.

## 🎯 Project Specifications  
The amplifier was designed to meet the following key specifications:  
- **Supply Voltage (VDD)**: 3.3V  
- **Input Common-Mode Voltage (VinCM)**: 0.5*VDD  
- **DC Gain (ADC)**: > 58dB  
- **Gain Bandwidth (GBW)**: > 150MHz for 1pF load  
- **Slew Rate**: > 100 V/μs  
- **Output Swing**: > 1.5V peak-to-peak  
- **Input Referred Noise Density**: < 30nV/√Hz  
- **Phase Margin (PM)**: > 60°  
- **Gain Margin (GM)**: > 12dB  
- **Minimal power consumption and area** 

## 🛠️ Design Methodology

1. **Current Generation & Distribution**  
   - Used biasing circuit to generate I₁
   - Designed current mirror network to generate I₃ using the relation: `I₃ = ½I₁ + I₂`
   - Ensured proper current scaling
   - Maintained compliance voltage for maximum swing

3. **Biasing Circuits**  
   - Implemented optimum bias generation for:  
     * Vb₁ (Current Source stage bias Voltage)
     * Vb₂ (PMOS Cascode stage bias Voltage)
     * Vb₃ (NMOS Cascode stage bias Voltage)

4. **Transistor Sizing**
   - Optimized for Maximum output swing (±1.5V)
   - Maintained `VDS = Veff + 100mV` for optimal rₒ
   - Balanced gm/ID for noise-performance
   - Balanced gain-bandwidth tradeoff

## 📊 Simulation Tasks Completed

- **DC Analysis with operating points**
- **AC Analysis (gain & phase vs frequency)**
- **Common-Mode Rejection Ratio (CMRR)**
- **Power Supply Rejection Ratio (PSRR)**
- **Stability Analysis using STB and IPROBE**
- **Closed-Loop Frequency Response**
- **Input-Referred Noise Analysis**
- **Slew Rate Verification**
- **Harmonic Distortion Analysis (HD2, HD3, THD)**
- **Step Response Analysis (FGE and settling time)**
