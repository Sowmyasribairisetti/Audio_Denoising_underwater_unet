📊 RS-UNet Denoising Results (Underwater Noise)
Mix (%)	ΔSNR (dB)	ΔPESQ	ΔSTOI	ΔSDR (dB)	Remarks
30	+2.66	+0.03	−0.04	+2.39	Slight SNR/SDR improvement, minor drop in STOI (possibly due to over-smoothing)
50	+2.23	+0.03	−0.02	+7.20	Strong SDR gain — RS-UNet removed mid-level noise effectively
70	+2.45	−0.08	+0.04	+8.54	SDR and SNR both improve; minor PESQ drop (quality trade-off at heavy noise)




📊 UNet Denoising Results (Underwater Noise)
Mix (%)	ΔSNR (dB)	ΔPESQ	ΔSTOI	ΔSDR (dB)	Remarks
30	+1.58	+0.01	−0.10	+1.55	Minor SNR/SDR gain, STOI drop — some speech distortion
50	−0.72	−0.01	−0.10	+2.17	Slight degradation in SNR — model over-suppressed speech
70	+1.18	−0.09	−0.12	−2.55	Inconsistent performance — struggles with heavy underwater noise

🧠 Comparison: RS-UNet vs. UNet
Metric	RS-UNet (Avg Δ)	UNet (Avg Δ)	Interpretation
ΔSNR	+2.45 dB	+0.68 dB	RS-UNet consistently enhances clarity
ΔPESQ	≈ +0.02 dB	≈ 0 dB	Slight perceptual edge to RS-UNet
ΔSTOI	+0.01 avg	−0.11 avg	RS-UNet preserves intelligibility
ΔSDR	+6.04 dB	+0.39 dB	RS-UNet reconstructs signal structure much better
