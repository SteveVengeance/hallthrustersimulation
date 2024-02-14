# hallthrustersimulation
This is a code for Hall Thruster simulation using HallThruster.jl package. I have also added the code as a separate Julia file.

Simulations of Hall Thruster (called Red - renamed from Honest John) Operating Parameters 
One last thing I would like to achieve as well is to simulate what are the operational parameters of my Hall Thruster should it be ever brought to an orbit. I have used one of the packages available as an open-source solution for Hall Thruster simulation called HallThruster.jl [12].

I have used basic tutorial (obviously, I have modified parameters of the Thruster) and modified few aspects of the code to match my needs (added Thrust mean as well as Plot for Thrust simulations). You can find the code in Appendix A. One important aspect to know is that due to the lack of time I couldn’t add custom propellant thus I used Krypton as a main propellant for simulations.

I have also performed few simulations with different voltage. Starting with 500 V (as an approximation from my previous discharge experiment) and ending up with 200 V as some of the minimum discharge voltage.

Simulation 400 V – 
Mean Thrust (250 mN)	Simulation 300 V – 
Mean Thrust (213 mN)
 	 
Oscillations of Discharge current, Electron current and Ion current continue after 10 ms. I was not able to achieve stable state for this combination of voltage and engine.	Engine stabilises after 5 ms and produces stable thrust around 213 mN.
	
Simulation 200 V – 
Mean Thrust (173 mN)	Simulation 500 V – 
Mean Thrust (185 mN)
 	 
Smaller oscillations continue and this combination yields lower thrust.	Strange deviation in calculation. It potentially require some other model or parameters finetuning.

Based on these simulations, it appeared that 300 V is the optimal voltage (at least for Krypton) as oscillations disappear in 5 ms and stable thrust of approximately 213 mN should be achieved.
![image](https://github.com/SteveVengeance/hallthrustersimulation/assets/120807669/ab35c8d7-d843-40dd-ac5b-85ed2635a609)
