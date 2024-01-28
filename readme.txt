Version 3.1:

About:

This Program uses ordinary differential equations (ODEs) to simulate the evolution of Saturn's rings under the influence of the Saturnian moon Mimas, with modifiable values to demonstrate the impacts of different qualities (eg. setting Mimas to a higher mass). The intention of this program is to model the formation of the Cassini Division, a low-density region between Saturn's A and B rings believed to be formed from orbital resonance effects from Mimas. To observe this effect, the runtime of the program must be increased from the default value (I also strongly recommend raising the timestep to reduce runtime). 

-The function "MimasODE" defines an ODE calculating a new position and velocity for Mimas using Newton's Law of Universal Gravitation. 

-The function "ParticlesODE" defines an ODE calculating new positions and velocities for all particles in the ring system based on the net gravitational attraction between Mimas and Saturn. 

The program initializes the system with nParticles number of ring particles randomly placed within a ring surrounding Saturn. The radius of the ring is defined by the innermost bounds of the B ring and the outermost bounds of the A ring. Mimas is positioned outside of the ring system.

Links: 
-Youtube videos of my original animations (from Version 1.0) can be found on the "COSIPS: Computer Simulations in Planetary Science" YouTube channel. 
  > youtube.com/watch?v=pNShC5iLG18
  > youtube.com/watch?v=an6R5dO6Xmg
  > youtube.com/watch?v=6yPayqetpvU

Changes:
-Added a new cell that animates a bar plot of density by ring region (A ring, B ring, and the Cassini Division), providing a quantitative measure of change over time.

Known Issues:
-If ring radii are changed from default, real world values, the bar plot will not display the resultant gap's density, and will instead just display the density in the region of the real world division. Must manually adjust values to find where orbital resonance will create a gap. 

Acknowledgements:
-I want to thank Jizhou Wu, who's assistance was invaluable throughout the process of debugging and optimizing this project. 
-I also wish to thank Professor Militzer, who taught EPS 109.  
