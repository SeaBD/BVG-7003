# BVG-7003
Analysis of genomic information: from genome to phenome

This project is a classroom project for the “BVG-7003: Analysis of genomic information: from genome to phenome” course.
The PyCharm Community version 2022.2.3 was used for editing the codes and the python version 3.10.5 was use to run them.

Summary of the file formats:
•	.gbk: is a GenBank format for storing genomic information
•	.fasta: is a text-based file format which regularly use single-letter codes for representing either nucleotide or protein sequences.
•	.faa: is similar to fasta and use for amino acid sequence.

Description of the data files used as input files for the codes:
•	The NC_000913.gbk file consists of the complete genome of the Escherichia coli str. K-12 substring MG1655.
•	NC_000913.faa file represents the protein sequences of the Escherichia coli str. K-12 substring MG1655.
•	PGSC_DM_v3.4_pep_representative.fasta file includes potato protein sequences of doubled monoploid S. tuberosum Group Phureja clone DM1-3.
•	PGSC_DM_v3.4_pep_rep_no_stars.fasta file is identical with the PGSC_DM_v3.4_pep_representative file except for not having asterisk sign (*) at the end of each record.

The python source codes are:
•	Total_gene_lengths.py: calculates the total length of all genes of E.coli using the input file, NC_000913.gbk, and prints it.
•	Check_start_met.py: accepts the protein sequence as an input file, PGSC_DM_v3.4_pep_representative.fasta, calculates the number of proteins that do not start with Methionine, prints the records and their first residue.
•	Convert.py: simply converts a GenBank format (NC_000913.gbk) into a fasta format (NC_000913_converted.fasta) and prints the number of converted files.
•	Count_fasta.py: calculates the number of E.coli proteins using the input file, NC_000913.faa, and prints it.
•	Count_record.py: prints each protein records and its length for the input file, NC_000913.faa.
•	Edit.py: accepts the PGSC_DM_v3.4_pep_representative.fasta file as its input and removes the asterisk sign (*) at the end of each record then saves the edited file as PGSC_DM_v3.4_pep_rep_no_stars.fasta.
•	Filter1.1.py: accepts the NC_000913.faa as an input file, calculates and selects (filter) the proteins with the length of equal and greater than 100 and saves only the first one under the file name of NC_000913_long_only.faa.
•	Filter1.2.py: accepts the NC_000913.faa as an input file, calculates and selects (filter) the proteins with the length of equal and greater than 100 and saves all of them under the file name of NC_000913_long_only.faa.
•	Filter.py: accepts NC_000913.gbk as an input file calculates the number of cds sequences, extracts and save all of them without line wrapping (each cds in a single line) under the file name of NC_000913_cds.fasta.
