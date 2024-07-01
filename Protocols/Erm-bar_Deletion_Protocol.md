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

### *tfoX*-induced transformation of Mut DNA into *V. fischeri* to generage gene::erm-bar strain
* Inoculate 3 mL of liquid LBS-Cam2.5 with *V. fischeri* host strains carrying pLostfox overnight at 25˚C
* Dilute 30 uL of LBS-Cam2.5 overnight culture into 3 mL of Tris Minimal Media-Cam2.5 and grow at 25˚C
  * Note: inoculations should go 12-16 hours. Over 16 hours causes issues
* Subculture 150 uL fro the previous overnight into 3 mL of the same, fresh media and grow at 25˚C until OD600 reaches 0.2-0.3
  * Transfer 500 uL of culture into 1.7 mL tube
  * Add ~100 ng of Mut DNA
  * Incubate statically at room temp for 30 min to 1 hour
  * Add 1 mL of LBS, then transfer whole volume to culture tube
  * Grow overnight at 25˚C with aeration
* Plate 100 uL of undiluted and 10^-1 dilutions of transformation reactions onto LBS-ERM5 plates and incubate overnight at 25˚C
* Streak out 4 candidates onto LBS-ERM5 plates and incubate overnight at 25˚C
* Pick a single colony from each candidate and patch (in order) onto LBS-ERM5, LBS-CAM2.5, and LBS, and inoculate 3 mL of LBS-Erm5 and incubate overnight at 25˚C
  * This tests antibiotic resistance: all should be ERM-R but CAM-S, all should grow in LBS
* Patch candidat3es (max of 3) with desired phenotype (ERM-R and CAM-S)
  * Freeze temp glycerol stocks of deired candidates: transfer 1.2 mL of LBS-ERM5 culture into sterile red-cap cryovial containing 600 uL of 50% glycerol and freeze at -80˚C
* Harvest 1:10 dilutions of LBS-ERM5 cultures by transferring 2 uL of culture into PCR striptubes with 18 uL of water at -20˚C
  * Use these 1:10 dilutions as template for screen PCR
