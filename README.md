# PairEdit-PPI

AF3 wild-type protein-complex inputs for the PPI mutation-effect benchmark.

## Download

[AF3 input package](af3_wt_le1022_v1.zip) (approximately 14 MB).

- 3,552 unique WT complexes; 3,488 unique protein sequences.
- Each chain is at most 1,022 amino acids; sequences are not truncated.
- Sources: disease, population and SNOOPPI datasets. SNOOPPI includes single and multiple substitutions on one chain.
- Same WT sequence pair is predicted once, irrespective of chain order or mutation count.

The archive includes local AF3 JSON inputs, alternative AlphaFold Server JSON batches, FASTA sequences, a complex manifest, sample-to-structure mappings, provenance, checksums and an export script.

Use either the local JSON files or the server batches, not both. Local inputs require the AF3 data pipeline to generate MSAs/templates before inference. Keep complex IDs, output mmCIF files and confidence/PAE JSON files for downstream mapping.

These are sequence-based WT input preparations, not predictions or a claim of experimentally resolved structures. The package README documents limitations and mapping conventions. Existing benchmark results used an earlier single-substitution, <=900-aa cohort and do not apply directly to this expanded input set.
