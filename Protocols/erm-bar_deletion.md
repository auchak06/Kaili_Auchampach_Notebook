#### Protocol summarized from Avery's notebook
### Generate US-LL and DS-RL
* Extract parent strain gDNA from 700 ul of overnight culture of "V. fischeri"
  * Incubate strains at 25˚C in 3 mL LBS overnight
  * Extract and purify DNA with DNeasy Blood and Tissue Kit (Qiagen) and quantify
* Generate homology arms
  * Thaw 10 uM of primers F1+R1, F2+R2 for each deletion
  * Set up 3x reactions for 25 uL volume per reaction PCRs for both hology arms of each deletion

Reagent | Volume | 3x Reactions
---------|------- |-------------
Phusion HF Buffer| 5µL | 15µL
NF H20 | 9.5µL | 28.5µL
dNTPs | 0.5µL | 1.5µL
DMSO | 0.75µL | 2.25µL
Phusion Polymerase | 0.25µL | 1µL

* Add 1 uL of 10 uM primers for respective arms -> 3 uL of each primer in pair
  * US-LL: F1+R1
  * DS-RL: F2+R2
* Mix and remove 25 uL for negative control
* Add ~1 uL of 5 ng/uL parent gDNA -> 2 uL of diluted gDNA
* Run PCR using manufacturer's protocol for Phusion DNAP, with annealign temp raised from 60˚C as in original protocol to 70˚C to account for higher Tm of primers being used

Cycle Step | Temp (˚C) | Time | Cycles
---------|------- |----------|--
Initial denaturation|98|30 sec|1
Denaturation|98|5 sec|29
Annealing|70|30 sec|
Extension|72|1 min|
Final extension|72|5 min|1
Hold|<12|Indefinitely|

Running gel:
* Visualize 5 uL of reaction in 1 uL of 6x purple gel loading dye
  * Load 6 uL of mixture in 1% agarose gel electrophoresis
  * Run gel for 35 min at 100 V until separated

 #### Purify homology arm DNA
 * Purify amplified US-LL and DS-RL DNA fragments using QIAquick PCR Purification kit following manufacturer's protocol
 * Determine DNA concentration of samples using Nanodrop (want >10 ng/uL DNA)
 * Store stocks of DNA at -20˚C and make working dilutions of 10 ng/uL of both US-LL and DS-RL DNA fragments and store at -20˚C for SOE-PCR

### Synthesize Mutant DNA via SOE-PCR

Reagent | Volume 
---------|-------
Phusion HF Buffer| 5µL 
NF H20 | 9.25µL
dNTPs | 2µL
DMSO | 1.5µL
Phusion Polymerase | 0.25µL 
erm-bar DNA | 1µL

* Add 1 uL of each LL and RL to PCR tubes, and 2 uL each of F1 primer and R2 primer

Cycle Step | Temp (˚C) | Time | Cycles
---------|------- |----------|--
Initial denaturation|98|30 sec|1
Denaturation|98|5 sec|29
Annealing|65|20 sec|
Extension|72|1 min|
Final extension|72|5 min|1
Hold|<12|Indefinitely|

Running gel:
* Visualize in gel electrophoresis and purify amplified mutant DNA using QIAquick PCR purification
* Determine concentration is at least 10 ng/uL DNA using nanodrop and qubit and store at -20˚C
