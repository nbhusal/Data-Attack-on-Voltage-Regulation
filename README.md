All the system data for the 240-node real distribution system are taken from [1]. 

[1] F. Bu, Y. Yuan, Z. Wang, K. Dehghanpour, and A. Kimber, “A time-series distribution test system based on real utility data,” in 2019 North AmericanPower Symposium (NAPS), Wichita, KS, USA, USA, 2019, pp. 1–6


The MATLAB and OpedDSS integration of the system are are available in 
http://wzy.ece.iastate.edu/Testsystem.html

Iowa Distribution Test Systems
A Real 240-Node Distribution System with One-Year Smart Meter Data
Summary
System description
One year smart meter data
OpenDSS model
Quasi-static time-series analysis
Update history

In these given data we have added PV systems at various nodes and the voltage measurements are taken from these nodes to use them for the proposed work. 

The description of the python file are as follows.
For 240 node system 
Matlab_OpenDSS_interface.m: This is the main program that integrates MATLAB and OpenDSS, this contains the PV system addition on the various nodes. This program will require the following files. 
FeederA_P.mat
FeederA_P_W_Header.mat
FeederA_Q.mat
FeederB_P.mat
FeederB_P_W_Header.mat
FeederB_Q.mat
FeederC_P.mat
FeederC_P_W_Header.mat
FeederC_Q.mat
irradiance.csv
temperature.csv
Capacitor.dss
CircuitBreaker.dss
DistriTransformer.dss
Lines.dss
Linecode.dss
Load.dss
Master.dss
pvdata.dss
RegControl.dss
SubTransformer.dss
Vsources.dss

The .dss (except pvdata.dss) and .mat files were obtained from the link provided above. Two excel files are solar   irradiance and the temperature data. 
For IEEE 123-node system 
The integrated .dss data obtained for this case were obtained from EPRI https://sourceforge.net/projects/electricdss/
We integrated the OpenDSS with the MATLAB to run the quasi-time series simulation.  All the data are provided inside the folder. 

All the source code and the program is available in this link 
https://drive.google.com/drive/u/1/folders/1AMr7XEDzXxuwL5ObIR0QVis1shWaMfU6
