# Laboratory work
Analysis of analog and digital signals and modulation methods in telecommunication systems

Purpose of the work  
To study the basic characteristics of analog and digital signals, master the principles of amplitude (AM), frequency (FM) and phase (PM) modulation, as well as digital modulation methods - ASK, FSK, PSK. To conduct a comparative analysis of the resistance of different types of modulation to noise and distortion using software modeling.


Theoretical background

1. Analog signal - continuous in time and amplitude. Example: sound, radio waves
2.
3. .[4.txt](https://github.com/user-attachments/files/23289957/4.txt)
4. [1.txt](https://github.com/user-attachments/files/23289958/1.txt)
5. [3.txt](https://github.com/user-attachments/files/23289960/3.txt)
[2.txt](https://github.com/user-attachments/files/23289959/2.txt)


6. Digital signal - discrete in time and amplitude. Represented by a sequence of bits.
7. Modulation - the process of changing the parameters of the carrier signal (amplitude, frequency, phase) in accordance with the information signal.
   - AM (Amplitude Modulation) - change in the amplitude of the carrier.
   - FM (Frequency Modulation) — changing the frequency of the carrier.
   - PM (Phase Modulation) — changing the phase of the carrier.
   - ASK (Amplitude Shift Keying) — a digital equivalent of AM.
   - FSK (Frequency Shift Keying) is a digital equivalent of FM.
   - PSK (Phase Shift Keying) is a digital equivalent of PM.

8. Noise immunity is the ability of a system to maintain the integrity of transmitted information in the presence of noise. PSK and FSK are generally more resistant to noise than ASK.

9. Hardware and Software

- Personal computer running Windows  
- Python 3.x with libraries:  
  - `numpy` - for numerical calculations  
  - `matplotlib` - for signal visualization  
  - `scipy` - for noise generation and filtering (optional)  
> Note: If Python is not installed, you can use an online platform (for example, Google Colab), but the task assumes local launch. For students without administrator rights, it is recommended to use a portable version of Anaconda or WinPython.

Work progress

Task 1. Generation and visualization of analog and digital signals

1. Write a Python script that generates:
   - An analog sinusoidal signal with a frequency of 5 Hz.
   - A digital signal (a sequence of bits: `[1, 0, 1, 1, 0, 0, 1]`), represented as rectangular pulses.

2. Plot the graphs of both signals on the same image (different subplots).

Task 2. Simulation of analog modulation (AM and FM)

1. Create a carrier signal (frequency 50 Hz) and a modulating signal (frequency 5 Hz).
2. Implement:
   - AM: `s_AM(t) = (1 + m * cos(2πf_m t)) * cos(2πf_c t)`, where `m = 0.8` is the modulation coefficient.
   - FM: `s_FM(t) = cos(2πf_c t + β * sin(2πf_m t))`, where `β = 2` is the modulation index.
3. Plot the graphs of the original signal, the carrier, and the modulated signals.

Task 3. Digital Modulation Simulation (ASK, FSK, PSK)

1. Use the same bit sequence from Task 1.
2. Implement:
   - ASK: amplitude = 1 for bit "1", 0 for "0".
   - FSK: frequency = 30 Hz for "1", 10 Hz for "0".
   - PSK: phase = 0 for "1", π for "0".
3. Plot the graphs of all three modulated signals.

Task 4. Noise immunity analysis

1. Add additive white Gaussian noise (AWGN) with signal-to-noise ratio (SNR) = 10 dB to each modulated signal (from Tasks 2 and 3).
2. Compare the distortion visually.
3. Answer the following questions:
   - Which type of modulation is the most noise-resistant?
   - Why are PSK and FSK preferred over ASK in secure communication systems?
Conclusions: Which modulation methods are appropriate for secure telecommunication systems and why.
