# BAE 305 Lab 4
# Go Big: Operational Amplifiers
Group Members: Heath Shewmaker and Terence Redford

Submitted: 2/24/25

# Introduction: 
This lab centered around the subset of devices known as Operational amplifiers (“Op-Amps”). We used the LM741 Op-Amp in six different circuits, each wired in such a way that they could electronically perform a certain abstract task. These tasks include voltage inversion, signal replication and even signal integration or differentiation. The aim of this lab was to demonstrate how the principles of an ideal Op-Amp can be applied to real devices and used in specialized circuits to perform complex and abstract functions automatically.
# Methods: 
Step 1) As always, the initial step involved collecting all the circuit elements we will need and verifying that they have the expected values.

 ![image](https://github.com/user-attachments/assets/13da3516-15c8-4012-abe9-bc61caeb0b2e)

Table 1: Actual resistance and capacitance vs. Expected resistance and capacitance

Step 2) In this step we wired a circuit called a “Unity gain Inverting amplifier”. The diagram below summarizes the intended wiring of the circuit:

 ![image](https://github.com/user-attachments/assets/200271ed-77c9-4b69-91b0-1ef09fc3eb6d)
 
Figure 1: Unity Gain Inverting Amplifier circuit

We used two DCPS units to supply the voltage differences reflected above. It should be noted that one DCPS acts as the source of -15 V, and the other as the source of the +15 V. Another important facet of this circuit is that Op-Amps need to be supplied with a potential difference, connected to the V+ and V-, in order to perform the way we expect. The important part of this is that this potential difference is not the input signal. Because of this, the potential difference reflected across the Op-Amp in the above circuit will remain constant across the rest of the circuits.
Included in this circuit was also a potentiometer which allowed us to vary the voltage input into the circuit by changing the percentage of the 1000 Ohm resistance. This was connected to a resistor measuring 68k Ohms, which was wired into the inverting input of the Op-Amp. Finally, another 68k Ohm resistor was connected to the inverting input and output terminals of the Op-Amp. Measurements of both the input and output voltage with respect to ground were taken using a DMM and tabulated in the results section.

Step 3) In this step we wired an “inverting moderate gain amplifier”, shown in the figure below:

 ![image](https://github.com/user-attachments/assets/2ead5c81-0a0d-4129-a3f7-e1c97c25fb14)

Figure 2: Inverting Moderate Gain Amplifier circuit

Much of this circuit remains the same as the first circuit, with the critical differences being the changing of the resistors, and the replacement of the DCPS and Potentiometer with a function generator as the means of delivering voltage input. By replacing the voltage input with the function generator, we traded the ability to manually modify the exact value of the input voltage for the ability to send time varying signals into the Op-Amp. We also changed the input resistor to 8.2k Ohms and the resistor connecting the inverting input and output terminals of the Op-Amp was replaced with a 330k Ohm resistor.  We then set the function generator to supply a 100 millivolt 2 kHz sine wave and made use of an oscilloscope to observe and compare the input and output voltage signals to estimate the gain. 
	*** Note: Make sure to have your multiplier function on the oscilloscope set to “1X”, or your gain will be misleading. 
Step 4) In this step we wired an “Inverting High gain amplifier”. This has the same circuit design as step 3, with the only difference being the resistors. The resistor between the voltage input and the inverting input terminal was exchanged for a 1k Ohm resistor, and the resistor connecting the inverting input and output terminals of the Op-Amp was exchanged for a 1.5M Ohm resistor.
The function generator was set to supply a 10 milliVolt 2 kHz sine wave, and the Oscilloscope was used to compare the voltage input and output to estimate the gain.
Step 5) This step involved wiring a “Voltage follower” circuit, shown schematically below

![image](https://github.com/user-attachments/assets/ee753d41-355e-401e-84a2-4e55cb43263b)

Figure 3: Voltage Follower circuit

This involved only a 64k Ohm resistor wired between the voltage input of the function generator and the non-inverting input of the Op-Amp, and a single wire directly connecting the inverting input and output terminals of the Op-Amp. We set the function generator to supply a 1V 2 kHz sine wave, and then used the oscilloscope to compare the input and output voltage and estimate the gain. We then attempted to vary the frequency of the wave and find if there was a frequency limit for the 741 Op-Amp.
Step 6) In this step we constructed an “Integrating amplifier”, shown in the diagram below:

 ![image](https://github.com/user-attachments/assets/b24b4904-aa11-4a91-9b00-4f58e5d7c215)

Figure 4: Integrating Amplifier circuit

This circuit is similar to the circuit in step 3, with a few significant modifications. The most notable change is the inclusion of a 1nanoFarad capacitor in parallel with the resistor, which was exchanged for a 220k Ohm resistor in this circuit, connecting the inverting input and output terminals. Secondly, the resistor between the voltage input and inverting input of the Op-Amp was changed to a 22k Ohm resistor.
With this circuit we set the function generator to supply a 1V (peak to peak) 4 kHz signal, and changed the signal type from sine to square and finally triangle waves. By using the Oscilloscope to compare the input and output voltage signals, we were able to observe how this circuit conditions the signals.
Step 7) This step involved wiring a “differentiating amplifier” which can be seen below:

 ![image](https://github.com/user-attachments/assets/d95123b4-f2a5-4dd3-ae71-195d8412037c)

Figure 5: Differentiating Amplifier circuit

The circuit once again shares similarities with step 3, except in this case the resistor between the input voltage and the inverting input pin has been replaced with a 100 nanoFarad capacitor, and the resistor connecting the inverting input and output terminals of the Op-Amp is now a 4.7k Ohm resistor. For this circuit, we set the function generator to supply a 2V (peak to peak) 1 kHz signal and changed the signal type from sine to square and finally triangle waves. By using the Oscilloscope to compare the input and output voltage signals, we were able to observe how this circuit conditions the signals.
# Results: 

Step 2:  for this circuit we noted that the voltage at the output was almost exactly the same as the input, except that it was negative. We did notice some differences in the magnitude of the voltage, which we believe came from a combination of the ratio of the resistances not being exactly 1, and the OP-Amp possibly not functioning like an ideal amplifier.
 
 ![image](https://github.com/user-attachments/assets/ac39e56a-f007-4df0-af5c-be78cfa4e560)

Table 2: Input and output voltages of the Unity Gain Inverting Amplifier

 ![image](https://github.com/user-attachments/assets/18001648-2b82-4781-b2f1-f29f6fcbf79b)

Figure 6: Expected gain vs. actual gain of the Unity Gain Inverting Amplifier

Steps 3 and 4: 

We estimated the gain of both the moderate gain and high gain operational amplifiers by using the ratio of the resistances. The moderate gain amplifier provided almost exactly the expected gain we calculated, whereas the high gain amplifier seemed to have some issues replicating the gain we expected. We assumed that this was due to physical limitations of the LM741 Op-Amp, and possible due to the large differences of the resistances, small variations in the resistance could result in large effects on the resistance ratio.

 ![image](https://github.com/user-attachments/assets/a7fbc225-8eb9-42c6-a265-27a9a1bfe06b)

Table 3: Actual gain vs. expected gain for each circuit

Step 5: 
The function of the voltage follower circuit was to take an input voltage and exactly replicate it. The input voltage was a 1 V sine wave, and using the oscilloscope we checked the peak to peak voltage of the output voltage, and it was exactly 1 V. This means that the circuit functioned as expected, simply replicating the input voltage.

 ![image](https://github.com/user-attachments/assets/2787285a-f4c4-4fa7-a063-96e87d711967)

Table 4: Input voltage, output voltage, and gain for the respective circuit

Step 6:   The integrating circuit we built was intended to compute the integral of any signal passed through the input. To test this, we set the oscilloscope to deliver various waveforms and viewed the output to ensure that it was integrated correctly.

  ![image](https://github.com/user-attachments/assets/59bf43bb-28ba-42c5-9219-2c051f76df5a)

	Figure 7: Sine wave vs integrated sine wave (cosine)

  ![image](https://github.com/user-attachments/assets/ba74470f-886a-4170-a70f-30bacb14fb86)

	Figure 8: Square wave vs. integrated square wave (triangular)

 ![image](https://github.com/user-attachments/assets/d394cc62-aa3d-43ac-94e2-7018126aa088)

	Figure 9: Triangle wave vs. integrated triangle wave (approximation of sine wave)

With these integrated waves, voltage changes influenced the amplitudes of the waves, while frequency changes influenced the period of the waves. 
Step 7: 
The differentiating circuit was designed to perform differentiation. Once again, we supplied the circuit with a variety of signals, and compared the output signal to what we expected the derivative of the signal to be. 

 ![image](https://github.com/user-attachments/assets/c5e248b1-84bc-42ea-a7db-1fa8eb922d12)

Figure 10: Sine wave vs. differentiated sine wave (cosine)

 ![image](https://github.com/user-attachments/assets/055dfed0-db1c-494e-a1ec-a57494a54cba)

Figure 11: Triangle wave vs. differentiated triangle wave (square)

 ![image](https://github.com/user-attachments/assets/217f6cff-0251-4ff8-9f83-4de73a9f788a)

Figure 12: Square wave vs. differentiated square wave 

These waves behaved relatively close to as expected. However, the shapes of the square and triangle waves are not as prominent as expected, and the difference between the sine and cosine waves are a little greater than expected. 
# Discussion: 
Compare the performance of circuits 1,2 and 3 with their expected theoretical gains:

 ![image](https://github.com/user-attachments/assets/e655a8e6-2f11-431d-afd5-3d20fdaa3ab0)

Table 5: Each circuit vs. its performance compared to expected theoretical gains

-	Circuit 2, the inverting moderate gain amplifier, performed the best compared to its expected theoretical gain, with just a 1% difference. The unity gain inverting amplifier and the inverting gain high amplifier circuits both had about a 10% difference from their respective expected gains. 

Comment on the limits of Op-Amp circuits with respect to maximum output voltage.
-	The Op-Amp circuit maxed out quicker when the output voltage was negative. Both input voltages of 14V and 15V gave an output of -13.65 V, which leads me to believe that this is the negative output limit for this circuit. However, the circuit allowed positive output voltages over this limit, at 13.9V and 14.25V. 

Are the LM741 Op-Amps symmetric? (Does positive voltage performance equal negative voltage performance?)
-	As mentioned above, the limits of positive and negative voltage outputs appear to be different. Therefore, the LM741 Op-Amps must not be symmetric. 

Did the integrating and differentiating circuits perform the mathematical operations as expected?
-	The integrating circuit performed as expected, displaying an accurate picture of what should be happening on the oscilloscope. However, as mentioned in the results section, the differentiating circuit behaved slightly irregularly compared to what was expected. 
# Conclusion: 
This lab provided a hands-on demonstration of how operational amplifiers can be utilized in a variety of circuit configurations to perform mathematical and signal-processing functions. By constructing and analyzing six different circuits, we were able to observe the real-world behavior of the LM741 Op-Amp and compare its performance to theoretical expectations.
While the inverting amplifier circuits produced relatively expected gains, small discrepancies were observed due to non-ideal component values and limitations of the Op-Amp. The voltage follower effectively demonstrated the ability of an Op-Amp to provide unity gain while isolating circuits. The integrating and differentiating circuits met expectations for the most part, but small deviations in the differentiating circuit suggested practical limitations in the signal processing.
We also noticed asymmetry in the Op-Amp’s voltage limits, with the negative output voltage reaching its maximum sooner than the positive. This reinforces the importance of understanding real-world Op-Amp behavior when designing circuits. Overall, this lab emphasized the practical applications of Op-Amps and highlighted both their versatility and their limitations in real-world conditions.


