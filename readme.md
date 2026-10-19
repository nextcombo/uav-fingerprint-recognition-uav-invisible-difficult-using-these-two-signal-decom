# UAV Fingerprint Recognition]UAV "Invisible" Difficult! Using these two signal decomposition techniques, Precisely Capture the Trajectory of Black Falcons [with MATLAB + Python Code]

Traditional detection methods have obvious shortcomings:
Doppler radar
Monitoring scope is limited, and the frequency resolution in long-distance detection is insufficient to capture the subtle features of drones.
Regular RF analysis
Depends on short-time Fourier Transform (STFT) and other technologies, but is easily interfered in low Signal-to-Noise Ratio (SNR) environments, and has poor recognition effect for time-varying signals.
This paper proposes an innovative scheme: extract the RF fingerprint of UAV through EMD and EEMD. Implement high-precision detection through machine learning. Experimental evidence, This method can effectively filter out noise. Particularly, the recognition accuracy of time-varying radio frequency signals has been significantly improved.
Core Technology: How EMD and EEMD "Unlock" the Radio Frequency Fingerprints of Drones? 1. The Mystery of Signal Decomposition: Extraction of Effective Features from Chaos. The communication signals between drones and remote controllers (such as 2.4G control signals, 5.8G video signals) contain rich radio frequency features, but these features are often masked by noise. EMD and EEMD solve this problem in the following ways:
EMD  
: Adaptively decompose complex signals into multiple Intrinsic Mode Functions (IMF), each corresponding to different frequency components, and finally retain the non-noise components for analysis.
EEMD  
: Introduction of white noise on the basis of EMD to solve the "modal mixing" problem (i.e., interference between signal components), making the decomposition more accurate.
For example, in 2.4G control signal decomposition:
The 10th EMD decomposition still contains significant noise (Figure 2), preventing the complete extraction of data packet transmission characteristics.
When the EMD decomposition reaches the 5th IMF, the signal characteristics are clearly presented. The subsequent IMFs mainly consist of noise (Figure 3), facilitating the selection of effective components.
2. Time-frequency analysis: STFT makes hidden features "visible" by applying short-time Fourier Transform (STFT) to the filtered IMFs, which can generate a time-frequency energy spectrum and intuitively display the signal's time-frequency distribution.
The single-path control signal exhibits a distinct "linear" transmission characteristic (Figure 5);
The spectrum of two control signals can clearly distinguish two data packets (Figure 6);
Video signals have stronger spectral energy and more continuous distribution due to continuous transmission (Figure 7).
This visualization feature provides a crucial basis for machine learning classification.
Experimental verification: Which method is superior? 1. Experimental setup of signal source
2.4G uplink control signal (1/2 channels), 5.8G downlink video signal, and environmental white noise for drones.
Data Collection
Using GNURadio module, center frequency 2.455G, sampling rate 31.25MHz, record the signal when drone flies along 340 feet track;
Classification model
The 100×1280 time-frequency matrix (combination of 5 IMF features) is trained using machine learning algorithms such as CNN, MLP, decision tree, SVM.
2. Key Result Signal Type
EMD recognition accuracy
EEMD identification accuracy
White noise (without drones)
100%  
100%  
1. Road control signals
Approximately 75%
Approximately 90%
2. Traffic control signals
Approximately 70%
Approximately 95%
1. Road video signal
Approximately 85%
Approximately 75%
EEMD Advantages
Outperforms in multipath control signal identification due to the ability to effectively separate overlapping signal components and reduce noise interference.
EMD Advantages
- More accurate recognition of continuous video signal, indicating its stability in processing continuous signals;
Common highlights
The recognition accuracy of white noise is 100%, which can greatly reduce the false alarm rate.
Conclusion: The two technologies complement each other, establishing a new paradigm for drone detection. This paper confirms that EMD and EEMD can effectively extract unique fingerprints of drones through adaptive decomposition of radio frequency signals, and combined with machine learning, achieve high-precision detection. Specifically:
EEMD is more suitable for recognizing time-varying and multipath control signals, applicable to multi-drone detection in complex environments;
EMD is more stable in continuous video signal recognition, which can serve as a supplementary solution for specific scenarios.
In the future, by combining these two methods and optimizing classification models, it is expected to further improve detection performance in long-distance, low-signal-to-noise ratio scenarios, providing more reliable technical support for airspace security in sensitive areas such as airports and nuclear power plants.
End

## Images

![(UAV Fingerprint Recognition)The "Invisibility" of UAVs Has Been Struggled! Use These Two Signal Decomposition Technologies to Precisely Capture the Footprints of Unauthorized Flights [with MATLAB + Python Code]](01.jpg)
![(UAV Fingerprint Recognition)The "Invisibility" of UAVs Has Been Struggled! Use These Two Signal Decomposition Technologies to Precisely Capture the Footprints of Unauthorized Flights [with MATLAB + Python Code]](02.jpg)
![(UAV Fingerprint Recognition)The "Invisibility" of UAVs Has Been Struggled! Use These Two Signal Decomposition Technologies to Precisely Capture the Footprints of Unauthorized Flights [with MATLAB + Python Code]](03.jpg)
![(UAV Fingerprint Recognition)The "Invisibility" of UAVs Has Been Struggled! Use These Two Signal Decomposition Technologies to Precisely Capture the Footprints of Unauthorized Flights [with MATLAB + Python Code]](04.jpg)
![(UAV Fingerprint Recognition)The "Invisibility" of UAVs Has Been Struggled! Use These Two Signal Decomposition Technologies to Precisely Capture the Footprints of Unauthorized Flights [with MATLAB + Python Code]](05.jpg)
![(UAV Fingerprint Recognition)The "Invisibility" of UAVs Has Been Struggled! Use These Two Signal Decomposition Technologies to Precisely Capture the Footprints of Unauthorized Flights [with MATLAB + Python Code]](06.jpg)
![(UAV Fingerprint Recognition)The "Invisibility" of UAVs Has Been Struggled! Use These Two Signal Decomposition Technologies to Precisely Capture the Footprints of Unauthorized Flights [with MATLAB + Python Code]](07.jpg)
![(UAV Fingerprint Recognition)The "Invisibility" of UAVs Has Been Struggled! Use These Two Signal Decomposition Technologies to Precisely Capture the Footprints of Unauthorized Flights [with MATLAB + Python Code]](08.jpg)
![(UAV Fingerprint Recognition)The "Invisibility" of UAVs Has Been Struggled! Use These Two Signal Decomposition Technologies to Precisely Capture the Footprints of Unauthorized Flights [with MATLAB + Python Code]](09.jpg)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
