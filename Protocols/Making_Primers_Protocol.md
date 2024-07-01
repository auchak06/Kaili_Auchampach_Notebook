### Making Primers

1. Create a new Benchling file with your gene of interest and about 2kB on either side
2. Go approximately 1kB upstream from the beginning of your gene
    * Take into consideration the direction of your gene
3. Find a section that is relatively G-C rich
4. Highlight until the melting temp is around 57-60˚C
5. Go to IDT's OligoAnalyzer tool https://www.idtdna.com/calc/analyzer
6. Copy chosen DNA sequence (forward, not reverse) into IDT and Analyze
    * Under Results section, the melt temp should be about 60˚C (+/- 3˚C)
    * Under the Hairpin section, the hairpin temp should be less than 45˚C
    * Under the Self-Dimer section, the Delta G should be greater than -10 (closer to 0)
7. If all numberes are correct, move on, if not try a different sequence
8. Back in Benchling, click Create -> Primer -> Direction towards gene
      * When chossing Forward or Reverse, remember that the primer should always be facing towards your protein
9. This is you F1 primer
10. Go 500bp away (further from gene) from the primer you just made and repeat steps 3-8
11. This will be your F0 primer
12. Next, go to the start codon of your gene and make another primer, repeating steps 3-8
      * This must only include the start codon, and no more of the gene
      * This primer should be facing away from your gene, towards the F1 primer
      * Once you have your primer, select the Left Linker sequence for the Erm-bar-scar genome and add it to the 5' end of you primer
      * Make sure you select the correct complement (either the actual complement or the reverse), if the primer faces int he reverse direction you will use the reverse complement and vice versa
      * This is your R1 primer
13. At the end of your gene, select the last six amino acids not including the stop codon (or more if needed NOT LESS) and repeat steps 3-8
      * Select the Right Linker sequence of the Erm-bar-scar genome and add it to the 5' end of your primer
      * This is your F2 primer
14. Recheck R1 and F2 primers in IDT with the linking sequences including
      * The melting temp for these will be closer to 65˚C
      * Both R1 and F2 primers will be facing away from the gene
15. Go about 1kB away from the end of you gene, and make one more primer repeating steps 3-8
      * This is your R2 primer
16. Go 500bp away (further from gene) from the primer you just made, repeat steps 3-8       * This is your R0 primer
17. Finally make two more primers (one forward and one reverse) that will make a product of about 500bp in the middle of your gene
      * These are to check that the deletion was successful
