# Real-Time Spectrum Analyzer with Streamlit

This is a real-time radio frequency spectrum analyzer built using Python, Streamlit, and matplotlib. It allows users to capture, visualize, and analyze frequency data using inputs from an SDR device, UDP socket, or Red Pitaya.

## Features
- Real-time FFT and spectrogram display
- Supports input from:
  - RTL-SDR (software-defined radio)
  - UDP Socket (Unicast or Broadcast)
  - Red Pitaya
- Manual frequency selection or automated sweep
- Power monitoring and averaged tracking
- Frequency probability distribution
- Option to export data to CSV
- Web interface built with Streamlit

## Technologies Used
- Python
- Streamlit
- matplotlib
- NumPy
- Pandas
- pyrtlsdr for SDR input
- Socket programming

## Input Modes
- SDR: Captures live radio samples using RTL-SDR
- UDP Socket: Receives complex samples over the network
- Red Pitaya: Receives FFT data over UDP from Red Pitaya board

## How to Run
1. Install the required Python packages:
```bash
pip install streamlit matplotlib numpy pandas pyrtlsdr
```
2. Connect your SDR device if needed
3. Run the application:
```bash
streamlit run main.py
```
4. Use the sidebar to select mode, input source, and configuration options

## Output
- Real-time frequency and power plot
- Heatmap of recent FFT data (spectrogram)
- Line graph showing power over time
- Bar graph of frequency distribution
- Option to save captured samples as CSV

## Interface Overview
- Sidebar: Select input source, control sweep/manual mode, enter UDP settings
- Main View:
  - FFT plot
  - Spectrogram
  - Power tracking
  - Frequency distribution

## Authors
Developed by:
- Srikant Ravi Jois
- Chandana Alagod
- Shishir Ravi Jois
- Meenakshi Nair

## License
This project is intended for academic and learning use.

