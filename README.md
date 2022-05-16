# Space Explorer
Repo for Space Explorer, a space game where user can explore procedurally-generated planets. 

The basic outline for my research project on procedural generation:
- make an explorable world in Unity where there is a n-planet n-star system, and all the planets and stars are procedurally generated

The only parameters that should be given at the start of the program are:
   - the number of planets to generate
   - number of stars to generate
   - random seed to control all generation aspects

Stars will simply be of different masses, volumes, and densities. If multiple solar systems will be generated, then we can add some 
variety by maybe introducing a black hole, such as for galaxies. Different kinds of stars:
   - T Tauri stars
   - Main Sequence stars
   - Red Giants
   - White Dwarf stars
   - Red Dwarf stars
   - Neutron stars 
   - Supergiant stars
(link: https://cosmonova.org/different-types-stars-stellar-evolution/)

Planets will be spheres with densely populated points to act as vertices. To generate land, we can try a couple different noise 
algorithms applied to those vertices:
   - Voronoi noise
   - Perlin noise (classic gradient noise)
   - Simplex noise (improvement upon Perlin) 
   - Value noise 

Planets will be populated with trees, shrubs, water, mountains, valleys, deserts, tundras, etc. This will not go as far as to create
peoples/cultures on different types of planets. 
If planets have water, simple aquatic creatures like fish can be generated. Fish movement will be goverened by 3 simple rules:
   - avoid collision with other fish
   - follow dense population
   - avoid collision with other obstacles
Will try to implement something similar for air creatures (time permitting).

Will try to implement Lindenmayer system (L-system) for procedural generation of things like certain geographic features. A good place
to start with all this is with Nested, by Orteil. This is a L-system-based text-generation of a universe with multiple superclusters that 
have galaxies, and it goes on. 

List of different kinds of procedural generation models/algorithms: http://pcg.wikidot.com/category-pcg-algorithms

Potential use cases:
   - Study the universe with these generated models?


