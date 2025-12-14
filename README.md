# 🎤 Audio Recording and FIR Filtering Web Application

This project is a **browser-based audio recording and digital signal processing (DSP) application**. It allows users to **record voice using a microphone**, apply various **FIR (Finite Impulse Response) filters**, and **analyze results visually and audibly** using waveform and frequency spectrum charts.

The application is implemented as a **single HTML file** using **pure JavaScript**, **Web Audio API**, and **Chart.js**, and works directly in modern browsers without any backend.

---

## What this application does

* Records audio from the microphone
* Plays back the recorded audio
* Designs FIR filters with different configurations
* Applies FIR filtering to the recorded signal
* Compares original and filtered signals
* Displays waveform (time-domain) graphs
* Displays frequency spectrum (frequency-domain) graphs
* Allows listening to both original and filtered audio

---

## Application workflow

```text
Microphone Input
      ↓
Audio Recording (MediaRecorder)
      ↓
Audio Buffer (Web Audio API)
      ↓
FIR Filter Design
      ↓
Convolution Filtering
      ↓
Waveform Visualization
      ↓
Frequency Spectrum Visualization
```

---

## FIR filter features

### Supported filter types

* Low-pass filter
* High-pass filter
* Band-pass filter
* Band-stop (Notch) filter

### FIR design methods

* Frequency Sampling
* Least Squares
* Parks–McClellan (Remez Exchange)
* Constrained Least Squares
* Arbitrary Frequency Response
* Raised Cosine window

### Filter parameters

* Filter order (odd values)
* Cutoff frequency (Hz)
* Second cutoff frequency for band filters
* Sampling rate derived automatically from audio

---

## Signal processing details

* Audio is processed in **mono**
* FIR filter coefficients are generated mathematically
* Filtering is done using **time-domain convolution**
* Spectral analysis is performed using a simplified FFT implementation
* Frequency magnitude is displayed in **decibels (dB)**

---

## Visual output

### Time-domain visualization

* Original signal waveform
* Filtered signal waveform
* Time axis in seconds
* Amplitude comparison

### Frequency-domain visualization

* Original signal spectrum
* Filtered signal spectrum
* Frequency axis in Hertz (Hz)
* Magnitude in decibels (dB)

---

## Project structure

```text
.
├── index.html   # Complete application (HTML + CSS + JavaScript)
└── README.md    # Project documentation
```

---

## How to use

1. Open `index.html` in a modern browser (Chrome, Edge, Firefox)
2. Allow microphone access
3. Click **Start Recording** and speak
4. Click **Stop** when finished
5. Choose FIR filter type and parameters
6. Apply the filter
7. View graphs and listen to results

---

## Technologies used

* HTML5
* CSS3
* JavaScript (ES6)
* Web Audio API
* MediaRecorder API
* Chart.js

---

## Browser requirements

* Google Chrome (recommended)
* Microsoft Edge
* Mozilla Firefox

Mobile browsers may have limited support.

---

## Purpose of the project

This project is suitable for:

* Digital Signal Processing (DSP) education
* FIR filter experimentation
* Audio signal analysis
* Engineering and university projects
* Demonstrating browser-based DSP

---

## Limitations

* Designed for educational use
* Not optimized for real-time streaming filters
* FFT implementation is simplified for visualization

---

## License

This project is provided for **educational and experimental purposes only**.
