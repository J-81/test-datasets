# test-datasets


- NOTE TO SELF: Grabbing these files requires replacing "blob" with "raw" in the path on github.

- rcsb_fasta
  - 2_seq-mass_dl_rcsb-reformat.fasta
    - 2 pdb sequences downloaded from the rcsb website
    - The titles have been reformated to
      - >xxxx_Y where x is the 4 letter pdb ID and the Y is the 1 letter chain ID

- ensembl
  - genomes
    - mouse
      - subsampled_Mus_musculus.GRCm38.101.gtf 
        - > grep -E "^(#|1[9])" Mus_musculus.GRCm38.101.gtf > subsampled_Mus_musculus.GRCm38.101.gtf
      - subsampled_Mus_musculus.GRCm38.dna.toplevel.fa
        - > samtools faidx Mus_musculus.GRCm38.dna.toplevel.fa 19 > subsampled_Mus_musculus.GRCm38.dna.toplevel.fa
