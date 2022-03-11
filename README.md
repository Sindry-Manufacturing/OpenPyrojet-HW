# OpenPyrojet-HW
This is a repository for the hardware components of the OpenPyrojet 3D printer project. 
The current objective of OpenPyrojet, is  to create the first generation Open source/hardware/software thermal spraying 3D printer. 
In short, by using affordable, accessible and readily available parts and materials, we will create a new breed of 3D printer, that enables the heterogenous additive manufacturing of metal, plastic and ceramic monoliths rapidly, precisely, autonomously and at relatively low cost(in terms of time and money) to the user compared to contemporary 3D printing solutions. 

We believe this to be possible, due to the convergence of several co-factors in the present day(2022). In particular, the incredible decline in cost and complexity of autonomous CNC and robotic components, in terms of control and actuation, as well as the wide availability of good quality standard structural elements, the decreasing cost of refractory materials in favorble form factors, the wide availability of energy dense fuel products, and the increasing availability and declining cost of particulate material feedstocks. 
Additionally, the need for low cost, autonomous and widely accessible electronics prototyping and manufacturing processes, that improve on the user experience and the overall dirty dull and dangerous state of the art in electronics manufacturing are highly desirable to many parties beyond just we the developers. Current 3D printing approaches are largely ineffective in terms of cost and time for generating high quality, looks like, feels like, and works like, electronic parts, we believe this represetns a substantial opportunity to create change in electronics manufacturing and prototyping, and eventually in the whole of manufacturing as a concept through the introduction of relatively low cost, autonomous, high speed, high precision 3D printing of metals, plastics and ceramics. 
We also aim to eventually bring totally custom, free open and autonomous, on demand manufacturing, to the consumer desktop, or at least to the community scale, facilitating a return to the flexible and local cottage industries of the past, now cybernetically enhanced with the ability to create with the speed and quality of autonomous mass production assembly lines, and accelerated by the computerization and networked intelligence of the modern internet. 

We believe we can accomplish these lofty goals by hybridizing thermal inkjet printing and thermal spray tehnologies into a compact, self contained, open source 3D printer print head assembly and material feedstock handling system integrable with mass market consumer 3D printer control boards and robotic motion systems such as the Ender 3, the Prusa mk3s and mini, and others. 

The basic system concept is thus:
Fuel and material are held in a reservoir, kept mixed and pumped in and out by a syringe pump. This pump pushes fuel, and suspended material particles to the print head from the back through perfboard(of which the print head is made) holes. The fuel and material mixture circulate over the top of the print head at a constant average velocity to produce a negative pressure and prevent settling of the materials suspended in the fuel.
When the time comes to deposit material on the build plate, a short voltage pulse of controlled amplitude is applied to the captive heater wire, across two adjacent plated through vias in the perfboard.  This causes the wire to rapidly(with in 1-10 milliseconds) heat up, vaporizing the fuel and entraining the suspended material. 
Once an appropriate volume of fuel and material has been vaporized into the nozzle, a second, larger amplitude voltage pulse is applied, raising the temperature in the nozzle to the autoignition temperature of the fuel/air mixture in the nozzle. This ignites the fuel-air mixture, and melts and accelerates the material to deposit it on the build plate. Thusly, can we deposit virtually any material known, heterogenously, autuonomously with nearly complete closed loop control of the mass and energy flows of the process. 
Control is achieved by continuously performing 3 simultaneous measurement techniques, namely, differential scanning calorimetry(DSC), Surface enhanced IR spectroscopy(IRSPEC), and cyclcic voltammetry(CV). 
The first technique(DSC) is done by continuously monitoring the relationship between temperature, and power of the heating element throughout the deposition process. By tracking changes in the power applied to the element to maintain a given temperature across the whole temperature ramp during deposition, we can spot phase changes, ignition, deflagration and combustion, and continuously monitor the health and efficiency of the deposition proces in each nozzle during each discrete deposition event.  
The second technique (IRSPEC) is done by continuously monitoring the short time scale photocurrents induced in the element by the emitted and reflected ir-photons fromthe combustion ofthe fuel, the melting and cooling of the feed stock material and from te various surfaces effected during deposition. This allows us to monitor the chemical composition of the involved surfaces in real time, and to get a handle on the specic bonding events taking place to allow tunig and monitoring of interface growth and quality during deposition.
The third technique(CV) is done by providing a controlled input voltage waveform, and continuously monitoring changes in the response current of the heating element and adjoining electrical contacts. In this way we can detect electrochemical events and manipulate the electrochemistry of the combustion, and gaseous phases in the vicinity of the deposition process, in particular, oxidation events, reduction events, partial combustion, coking, etc.

