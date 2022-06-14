Lab session:  1 (b)


Title: Representation of pole zero and transfer function of control system


Objective

To obtain

i. Pole, zero, gain from a given transfer function.

ii. Construct Transfer function from pole, zero, gain values.

iii. Plot Pole, zero plot of a transfer function and understand about stability.


Theory

A transfer function is also known as the network function is a mathematical representation, in terms of spatial or temporal frequency, of the relation between the input and output of a (linear time invariant) system. The transfer function is the ratio of Laplace Transform of Output to the Laplace Transform of input , assuming zero initial conditions. Many important characteristics of dynamic or control systems can be determined from the transfer function. The transfer function is commonly used in the analysis of single-input single-output electronic system. It has various applications such as control theory, communication, signal system. If input signal x(t) is applied to a system which gives output y(t), the transfer function can be represented as,

Gs=L{yt}L{xt}=Y(s)X(s)

Roots of the numerator gives zeroes of transfer function, i.e. zeros are the value(s) ofsfor which the transfer function becomes zero. Roots of the denominator gives poles of transfer function, i.e. Poles are the value(s) ofsfor which the denominator of the transfer function becomes zero, i.e. the transfer function becomes infinite. 

The transfer function provides a basis for determining important system response characteristics without solving the complicated differential equation. 

It is defined as ratios of two polynomials in the numerator and the denominator, 

Gs=N(s)D(s)=a0+a1s+a2s2+a3s3+…ansnb0+b1s+b2s2+b3s3+…bnsm

It is often convenient to factor the polynomials in the numerator and the denominator, and to write the transfer function in terms of those factors:

Gs=N(s)D(s)=ks-z1s-z2s-z3s-z4………….s-zns-p1s-p2s-p3s-p4………..(s-pm)

Where,s= σ+jω, denotes the real part and jω denotes imaginary part of complex frequency s.

z1, z2,z3,…………. zn  are zeroes of transfer function and p1, p2,p3,…………. pn  are poles of transfer function.



Problem statement:

Q1. Find Pole, Zero and Gain of the transfer function G(s) = s2+3s+2(s+4)(s2+4s+7) and plot pole zero diagram.


Q2. Find Pole, Zero and Gain of the transfer function G(s) = s2+9s2(s-3)(s+4)(s2+4s+13)and plot pole zero diagram.


Q3. Find Pole, Zero and Gain of the transfer function G(s) = 2s2+18s+36s(s-2)(s+4)(s2+2s+1)and plot pole zero diagram.


Q4. Write Matlab code to obtain transfer function of a system from its pole ,zero, gain values. Assume pole locations are -3, 2, zero at -1 and gain is 7



Lab Lesson: 02
Title: Determination of transfer function of a given system from its state model 
Objective
i. To identify different connection between blocks.
ii. to determine Overall transfer function of a control system
Theory
A block diagram is used to represent a control system in diagram form. It is not convenient to derive complete transfer function for a complex control system, therefore, the transfer function of each element of control system is mentioned in the block diagram represented by block diagram and concerned symbol mentioned in the block represents the transfer function of the element. Block diagrams of complex control systems with complicated configurations can be simplified into simple open loop forms. In order to obtain the overall transfer function, a procedure called block diagram reduction technique is followed.


Lab Lesson: 03
Title: Determination of Step and Impulse response for a first order and second order unity feedback system

Objective:
To determine 
i. Impulse response of 1st  and 2nd order system
ii. . Step response of 1st  and 2nd order system.

Theory:
The time response is analysis is very important to design and analysis of transfer function in time domain at the presence of input. The variation of output with respect to time can be studied in time domain analysis. From time response analysis and corresponding results, the stability of system, accuracy of system and complete evaluation can be studied also. The response of the system is function of time at the presence of excitation or input. There are two parts of response of any system: Transient response and Steady-state response. Transient response are  part of the time response which goes to zero after large duration of time. Steady state responses are part of time response after the transients have died out. The total response of a system is sum of transient response and steady state response. C(t)=Ctr(t)+Css(t)

Lab Lesson: 04
Title: Determination of Root Locus from transfer function and evaluation of system parameters
Objective
To determine Root Locus plot from transfer function .
Theory
The Root Locus is a plot of the roots of the characteristics equation of that is obtained from the closed loop system as a function of gain (K) of the open-loop-transfer function. This is a graphical approach gives the closed-loop roots trajectories as gain (K) is varied from zero to infinity. The closed loops transfer function  CsRs=G(s)1+GsH(S)  are related to the zeros and poles of the open loop transfer function G(s)H(s) and also depends on gain. It also gives idea how system performance changes with addition of pole and zero.

Lab Lesson: 05
Title:Study of Nyquist plot and Bode plot from transfer function of a control system and estimation of relative system parameters .
Objective
i. To obtainNyquist plot of a system and understand stability of the system.
ii. To obtainBode plot of a system and understand stability of the system.

Theory
Nyquist criterion is used to identify the presence of roots of a characteristic equation of a control system in a entire right hand side beyond the imaginary axis of complex of s plane. For the analysis of stability mapping is done from ‘s’ plane to G(s)H(s) plane. Zeros are calculated from number of the roots of the characteristic equation of 1+G(s)H(s) = 0. As the s-plane region wherein only poles and zeroes of 1+G(s)H(s)=0 with positive real part is under investigation, the expression relating the number of poles and zeroes present in the R.H.S. of s-plane is written as,
∆Aug GsHs=2π(P+-Z+)
(origin at -1+j0)
∆AugGsHs2π=(P+-Z+)
N=(P+-Z+)
N=Number of encirclement of the point-1+j0by GsHsplot. The anti clockwise direction of encirclement is considered positive. 
P+=Number of poles of  GsHs  with positive real part.
Z+=Number of zeros of  1+GsHs=0  with positive real part.
For a stable control system Z+=0. There fore for a stable control system
N=(P+-0)
i.e.  N=P+


    The Bode plot method gives a graphical procedure for determining the stability of a control system based on sinusoidal frequency response. The transfer function of a system for sinusoidal input response can be obtained by substituting‘jω’ in place of Laplace operator “s”. Open loop transfer function GjωH(jω) can be expressed from magnitude and phase angle. Magnitude of GjωH(jω) is expressed ion decibel, i.e. 20log GjωHjω vs.   . Phase angle is expressed as ∠ GjωH(jω)vs.   . Gain crossover point on the frequency domain plot GjωHjω,is the point at which  GjωHjωdB=0 dBand denoted by cg . Phase crossover point on the frequency domain plot GjωHjω, is the point at which  ∠GjωHjω =-180 °  and denoted by cp . 
GM=-20logGjωHjωdB     , at  ω =cp
PM=180°+∠ GjωH(jω)     , at  ω =cg

For Positive gain margin and phase margin, the system is stable and gain crossover frequency is less than phase crossover frequency. If gain crossover frequency is greater than phase crossover frequency, gain margin and phase margin will be negative and system will be unstable. If gain crossover frequency is equal to phase crossover frequency, system is marginally stable. 

Lab Lesson: 06
Title: Design PI, PD and PID controller for specified system requirements.

Objective
To determine
i. Effect of PI controller on system performance 
ii. Effect of PD controller on system performance
iii. Effect of PID controller on system performance

Theory




Fig: Block Diagram representation of a second order closed loop system with proportional plus derivative plus integral control action


Controllers are components which basically have an input of the error signal and output of a signal to modify the system output and give the required characteristics.
There are three basic modes of control actions as follows:
Proportional (P) : The controller produces a control action that is proportional to the error (e), i,e. controller output = Kpe or (KpE(s)), with Kp being proportional gain.
Derivative (D) : The controller produces a control action that is proportional to the rate at which the error ( e) is changing dedt, i,e controller output = Kddedtor (sKDE(s)), with Kd being derivative gain.
Integral (I) : The controller produces a control action that is proportional to the integral of the error with time, i,e. controller output = KIe dt  or KIsEs , with KI being integral gain.
In practical system combinations of  PI , PD and PID controller are very often used. 
P Controller: Proportional controller can stabilize only 1st order unstable process. Steady state error is minimized and system becomes faster (rise time decreases) in Proportional controller, but overshoot is also increased.
PD Controller: With PD control the output rises more rapidly towards the steady state value and the overshoot is reduced. Because the derivative mode reduces the oscillations, we can increase proportional gain element to the higher values than would be feasible with just with the proportional mode without oscillation. Derivative control is not effective in steady state response.
PI Controller : Integral mode  gives a controlling response which is proportional to the area under the error time graph upto the current point and so can give a controller output even when the error has become zero.Here system typeand order is increased.
PID controller: PID controller is used where rapid and large disturbances may occur, the derivative mode taking care of the rapid changes and the integral mode the large offset resulting from the large disturbance.
For PID control the actuating signal consists of proportional error signal added with derivative and integral of the error signal. Therefore the actuating signal for PID control is,
eat=Kpet+Kdde(t)dt+KIetdt
The Laplace transform of the actuating signal of PID Control is,
Eas=KpE(s)+KdsE(s)+KIsE(s)

This can be expressed as,
CsRs=Kp+Tds+KIsn2s2+2ξns1+Kp+Kds+KIsn2s2+2ξns



