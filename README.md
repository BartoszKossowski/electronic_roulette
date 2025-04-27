# electronic_roulette
### Short description
Electronic roulette based on analog integrated circuits NE555 and CD4017.

The idea of ​​implementing an electronic roulette was born from a ready-made project of a circuit presented at: https://www.555-timer-circuits.com/roulette.html

### To~Do List

- [x] create a board measuring 200 mm x 200 m with the option to accommodate 38 mm glasses.
- [x] print the board
- [x] Create a prototype of an electronic roulette wheel on a breadboard [Malfunction](#no-filtration-no-peace)
- [ ] Design PCB
- [ ] Produce PCB
- [ ] Solder the PCB and check its operation
- [ ] Create a PCB case and print it
- [ ] Testing ;_;
- [ ] Done


# Model

At first I planned what the main 'scene' of roulette should look like. Of course, this is not an ordinary roulette, it is intended for predicting which glass to drink from.
It was easy to determine for 10 glasses: 360°/10 = 36° for each glass. Then just centering a circle slightly wider than the diameter of the glass.

 ![Fusion360](pic/fusionview.png)

I printed the board for the glasses using Prusament PETG Clear filament. This allowed the light from the rouette to better illuminate the drawn glass.

![Prusa](pic/processprint.png)


# First tests

First test attempt at mounting the LED diode and lighting it up from a working roulette wheel. It looks great, and the roulette wheel just happened to land on the LED diode I placed in the board.

![FR](pic/prerulette.jpg)

Unfortunately, I miscounted the holes for the LEDs and they will need to be drilled out a bit depending on the diameter of the LED that will be used (mine were 5.5 mm and 6.0 mm).

I am making the .stl model of this shot glass roulette board available under the Creative Commons 4.0 BY license.

You can find the model in the prusa3D folder, file named "roulette v5.stl" or just click the [link](prusa3D/ruletka%20v5.stl)



## No filtration, no peace

During the assembly of the entire electronic circuit, various errors occurred: from no operation, to operation at a lower voltage and even every other LED (only 5 out of ten) lighting up, interestingly every other one was perfect.

I added a 100nF ceramic capacitor to each integrated circuit near the power supply pins and the problem was solved.