# SDR-Learning-Project
Repository of stuff to learn about and build an SDR

# SDR Radio Research

## Chips
- Mixer: TS3A5017
- Mixer: FST3253
- VFO: Si5351A
- DSP: F-V1
- DSP/Micro: https://docs.ai-thinker.com/en/esp32-a1s
- OpAmp: LMP7715
- OpAmp: LM4562
- OpAmp: THS4304 / LT1818
    - https://www.ti.com/lit/gpn/ths4304
    - 
  
## Basics
### Quadrature Signals
- https://www.ieee.li/pdf/essay/quadrature_signals.pdf
### Phase Locked Loop (PLL): 
Create stable signal reference. Use a stable low freq reference (Crystal) to stabilize a high freq unstable ref (VCO). 
- https://www.youtube.com/watch?v=A9qt0JYdvFU
- https://www.youtube.com/watch?v=P8agoshy3H4
- https://www.youtube.com/watch?v=CM8n3wzNOvc
### Voltage Controlled Oscillator (VCO)
- Usually unstable, and require something like a PLL to stabilize 
### Operational Amplifiers
- https://www.youtube.com/watch?v=7FYHt5XviKc
- Gain is huge
- In open loop configuration, they are just comparators; Add negative feedback to become amplifiers rather than comparators
- If non-inverting input is higher than inverting input, output will be V+
- If non-inverting input is lower than inverting input, output will be V-
- Called "Operational" cause they were designed to perform mathematical "operations."
- Can be used as a buffer in buffer configuration
- Input impedance is high, so won’t draw current or effect anything on the input side
- Output impedance is low, so you can drive a bit of current through it. Tens of milliamps
- Non-Inverting Amp Configuration (Single Ended Amp)
    - Gain = Rf/R1 + 1
- Inverting Amp configuration
    - Gain = Rf/R1
    - Input * Gain * -1
    - With DC supply, it can never go negative. So need to off set and can do that by supply 1/2 Vcc to non-inverting pin
  

## Radio Designs
- https://circuitsalad.com/wp-content/uploads/2020/05/si5351_sdr3.jpg
- NA5Y - https://www.youtube.com/watch?v=prCrbD4T6I4
- NA5Y - https://www.youtube.com/watch?v=redvZ7LcXT0&t=171s

## Filters
### Receive 
- https://qrp-labs.com/images/bpfkit/bpf3.pdf
- 
### Transmit
- 


##M ixing and Switching
- VFO : https://www.youtube.com/watch?v=9Dz9BO6VJIk
- 
https://www.allaboutcircuits.com/technical-articles/how-to-multiply-RF-signals-without-a-multiplier-the-switching-mixer/

### Tayloe Detector/Mixer:
- https://norcalqrp.org/files/Tayloe_mixer_x3a.pdf
- https://www.youtube.com/watch?v=EarY64Lf3ls&t=327s
- https://github.com/thaaraak/Tayloe-Mixer-v3
