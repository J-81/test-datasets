# test-datasets


- NOTE TO SELF: Grabbing these files requires replacing "blob" with "raw" in the path on github.

- raw_subsampled
  - 6 samples with paired end reads file, sampled with only 50,000 sequences
    - > seqtk sample -s777 $file 50000 | gzip > `basename $file`


- ensembl
  - genomes
    - mouse
      - subsampled_Mus_musculus.GRCm38.101.gtf 
        - > grep -E "^(#|1[9])" Mus_musculus.GRCm38.101.gtf > subsampled_Mus_musculus.GRCm38.101.gtf
      - subsampled_Mus_musculus.GRCm38.dna.toplevel.fa
        - > samtools faidx Mus_musculus.GRCm38.dna.toplevel.fa 19 > subsampled_Mus_musculus.GRCm38.dna.toplevel.fa
