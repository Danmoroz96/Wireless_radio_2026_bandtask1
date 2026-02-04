# Wireless_radio_2026_bandtask1
Task 1 is to design appropriate filters to isolate specific frequency components from a composite input signal.

Based on the input signal frequencies (100 Hz, 200 Hz, 300 Hz, and 400 Hz), here is the completed table with the appropriate filter designs.
Logic used for Cutoff Frequencies:
To isolate a frequency (or group of frequencies), the cutoff should ideally be placed halfway between the frequency you want to keep and the nearest frequency you want to reject.
Gap size: The frequencies are spaced 100 Hz apart.
Ideal Cutoff: The midpoint between components (e.g., 150 Hz, 250 Hz, 350 Hz).

Table is presented in xlsx file in this repository.

100 Hz (LPF): You only want the lowest frequency. A Low Pass filter lets everything below the cutoff pass. Setting it at 150 Hz keeps the 100 Hz signal but blocks the 200 Hz signal.
400 Hz (HPF): You only want the highest frequency. A High Pass filter lets everything above the cutoff pass. Setting it at 350 Hz blocks the 300 Hz signal but keeps the 400 Hz.
200 Hz (BPF): You want to isolate a middle frequency. A Band Pass filter creates a window. You need to open the window above 100 Hz (so, 150 Hz) and close it before 300 Hz (so, 250 Hz).
100 Hz and 400 Hz (BSF): You want the extremes but not the middle 200 Hz and 300 Hz. A Band Stop filter (sometimes called a Notch filter, though usually wider) rejects a specific range while passing everything else. Rejecting 150 Hz to 350 Hz removes the middle components.
