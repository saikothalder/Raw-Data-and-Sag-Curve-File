# DO Sag Curve Workflow:
1. Software
 * Software: Excel Sheet
2. Data Collections & Preparation
* Data Collections > Lab Test > Data analysis > The Model Parameters Were Determined Using the Streeter-Phelps Equations.
 * Parameters: critical time (tc), Initial DO deficit (Do), DOmin, Critical Deficit (Do), Reaeration Co-efficient (Kr), 	De-oxygenation Co-efficient (Kd), Ultimate BOD (Lo), Natural exponential base (e=2.718), DO saturations	
Equations: 
1. Calculate Reaeration Co-efficient (per day): Kr=K20° (θ)^T-20°
    Where,	θ=1.024			
	             K20° =0.35-0.46 (Large Stream of Normal Velocity)	
2. Calculate De-oxygenation Co-efficient (per Day): Kd=k20°(θ)^T-20°
    Where,	θ= 1.047			
	             K20°= 0.12-0.23 (Sewage or Polluted River Water)
3. Ultimate Biochemical Oxygen Demand, L0 (mg/L): L0= BOD5/(1-e^-kdt)
4. Dissolved Oxygen Saturation Concentration, DOsat (mg/L): DOsat= 14.62-0.394T+0.007714T^2-0.0000646T^3
     Where,	T= Temperature		
5. Initial DO Deficit, D0 (mg/L)	: D0= Dosat-DOi
6. Critical Time, tc (Day): tc= {1/(Kr-Kd)} *ln[(Kr/Kd) *{1-(D0*(Kr-Kd)/(Kd*L0))}]
7. Critical Deficit, Dc (mg/L): Dc= {(Kd/Kr) *(L0*e^(-kd*tc))}
8. Minimum Dissolved Oxygen, DOmin (mg/L): DOmin= DOsat-DC
*Note: The required data is attached with the file and the sag curve trail equation is given in a box at the top of the file. How I implemented this: 
The method followed for designing the sag curve is attached as a PDF file. Please review it.
