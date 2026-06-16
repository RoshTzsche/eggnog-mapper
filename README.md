[![Build Status](https://travis-ci.com/eggnogdb/eggnog-mapper.svg?branch=master)](https://travis-ci.com/eggnogdb/eggnog-mapper)
[![European Galaxy server](https://img.shields.io/badge/usegalaxy-.eu-brightgreen?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAASCAYAAABB7B6eAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAACXBIWXMAAAsTAAALEwEAmpwYAAACC2lUWHRYTUw6Y29tLmFkb2JlLnhtcAAAAAAAPHg6eG1wbWV0YSB4bWxuczp4PSJhZG9iZTpuczptZXRhLyIgeDp4bXB0az0iWE1QIENvcmUgNS40LjAiPgogICA8cmRmOlJERiB4bWxuczpyZGY9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkvMDIvMjItcmRmLXN5bnRheC1ucyMiPgogICAgICA8cmRmOkRlc2NyaXB0aW9uIHJkZjphYm91dD0iIgogICAgICAgICAgICB4bWxuczp0aWZmPSJodHRwOi8vbnMuYWRvYmUuY29tL3RpZmYvMS4wLyI+CiAgICAgICAgIDx0aWZmOlJlc29sdXRpb25Vbml0PjI8L3RpZmY6UmVzb2x1dGlvblVuaXQ+CiAgICAgICAgIDx0aWZmOkNvbXByZXNzaW9uPjE8L3RpZmY6Q29tcHJlc3Npb24+CiAgICAgICAgIDx0aWZmOk9yaWVudGF0aW9uPjE8L3RpZmY6T3JpZW50YXRpb24+CiAgICAgICAgIDx0aWZmOlBob3RvbWV0cmljSW50ZXJwcmV0YXRpb24+MjwvdGlmZjpQaG90b21ldHJpY0ludGVycHJldGF0aW9uPgogICAgICA8L3JkZjpEZXNjcmlwdGlvbj4KICAgPC9yZGY6UkRGPgo8L3g6eG1wbWV0YT4KD0UqkwAAAn9JREFUOBGlVEuLE0EQruqZiftwDz4QYT1IYM8eFkHFw/4HYX+GB3/B4l/YP+CP8OBNTwpCwFMQXAQPKtnsg5nJZpKdni6/6kzHvAYDFtRUT71f3UwAEbkLch9ogQxcBwRKMfAnM1/CBwgrbxkgPAYqlBOy1jfovlaPsEiWPROZmqmZKKzOYCJb/AbdYLso9/9B6GppBRqCrjSYYaquZq20EUKAzVpjo1FzWRDVrNay6C/HDxT92wXrAVCH3ASqq5VqEtv1WZ13Mdwf8LFyyKECNbgHHAObWhScf4Wnj9CbQpPzWYU3UFoX3qkhlG8AY2BTQt5/EA7qaEPQsgGLWied0A8VKrHAsCC1eJ6EFoUd1v6GoPOaRAtDPViUr/wPzkIFV9AaAZGtYB568VyJfijV+ZBzlVZJ3W7XHB2RESGe4opXIGzRTdjcAupOK09RA6kzr1NTrTj7V1ugM4VgPGWEw+e39CxO6JUw5XhhKihmaDacU2GiR0Ohcc4cZ+Kq3AjlEnEeRSazLs6/9b/kh4eTC+hngE3QQD7Yyclxsrf3cpxsPXn+cFdenF9aqlBXMXaDiEyfyfawBz2RqC/O9WF1ysacOpytlUSoqNrtfbS642+4D4CS9V3xb4u8P/ACI4O810efRu6KsC0QnjHJGaq4IOGUjWTo/YDZDB3xSIxcGyNlWcTucb4T3in/3IaueNrZyX0lGOrWndstOr+w21UlVFokILjJLFhPukbVY8OmwNQ3nZgNJNmKDccusSb4UIe+gtkI+9/bSLJDjqn763f5CQ5TLApmICkqwR0QnUPKZFIUnoozWcQuRbC0Km02knj0tPYx63furGs3x/iPnz83zJDVNtdP3QAAAABJRU5ErkJggg==)](https://usegalaxy.eu/root?tool_id=eggnog_mapper)

# EggNOG-mapper

## Overview

**EggNOG-mapper** is a powerful tool designed for fast functional annotation of novel sequences. It leverages precomputed orthologous groups and phylogenies from the eggNOG database (http://eggnog5.embl.de) to transfer functional information exclusively from fine-grained orthologs.

### Key Features

- **Fast Annotation**: Optimized for rapid processing of large datasets
- **High Precision**: Uses orthology predictions instead of traditional homology searches to avoid annotation errors from paralogs
- **Multiple Search Methods**: Supports HMMER, DIAMOND, and MMseqs2 for protein sequence searches
- **Gene Prediction**: Integrated support for Prodigal for prokaryotic gene prediction
- **Flexible Input**: Accepts various input formats including FASTA files with nucleotide or protein sequences

### Common Use Cases

- Functional annotation of novel genomes
- Transcriptome analysis and annotation
- Metagenomic gene catalog annotation
- Orthology assignment across species

## Why Choose EggNOG-mapper?

Traditional homology-based annotation methods (like BLAST) can lead to erroneous functional transfers when close paralogs are involved. Paralogs are duplicate genes that may have undergone functional divergence. EggNOG-mapper addresses this limitation by:

1. Using orthologous groups from the eggNOG database
2. Transferring annotations only from fine-grained orthologs
3. Providing higher precision in functional predictions

For detailed benchmarks comparing different eggNOG-mapper options against BLAST and InterProScan, please visit: [Benchmark Analysis](https://github.com/jhcepas/emapper-benchmark/blob/master/benchmark_analysis.ipynb)

## Online Resource

EggNOG-mapper is also available as a public online resource at: http://eggnog-mapper.embl.de

## Documentation

Comprehensive documentation, installation guides, and usage examples can be found in our wiki:  
https://github.com/jhcepas/eggnog-mapper/wiki

## Installation

### Requirements

- Python 3.x
- Required Python packages (see `requirements.txt`)
- External tools: HMMER, DIAMOND, or MMseqs2 (depending on search method)
- Optional: Prodigal for gene prediction

### Quick Start

```bash
# Clone the repository
git clone https://github.com/jhcepas/eggnog-mapper.git
cd eggnog-mapper

# Install dependencies
pip install -r requirements.txt

# Download and setup databases (requires significant disk space)
python download_eggnog_data.py
```

## Usage

### Basic Annotation

```bash
# Annotate protein sequences using DIAMOND
python emapper.py -i input_proteins.faa -o output_annotation

# Annotate nucleotide sequences (with automatic translation)
python emapper.py -i input_nucleotides.fna -o output_annotation --translate

# Use HMMER for more sensitive searches
python hmm_mapper.py -i input_proteins.faa -o output_annotation
```

### Advanced Options

```bash
# Specify taxonomic scope for better annotations
python emapper.py -i input.faa -o output --tax_scope 9606  # Human

# Use specific eggNOG database version
python emapper.py -i input.faa -o output --data_dir /path/to/data

# Enable gene prediction for nucleotide input
python emapper.py -i genome.fna -o output --genepred prodigal
```

For a complete list of options, run:
```bash
python emapper.py --help
```

## Output Files

EggNOG-mapper generates several output files:

- `.emapper.annotations`: Main annotation file with functional predictions
- `.seed_orthologs`: Identified seed orthologs
- `.log`: Execution log with statistics and warnings

## Database Information

The eggNOG database provides orthologous groups and functional annotations for:
- Over 5000 organisms
- 2500 viruses
- Multiple taxonomic levels from general to species-specific

Database files should be downloaded separately using the provided scripts.

## Configuration and Environment Variables

### Sensitive Configuration

**Important**: If you have any API keys or sensitive configuration data, store them securely:

1. **Environment Variables**: Store sensitive data in environment variables rather than in configuration files
2. **Secure Storage**: Use secure secret management systems for production environments
3. **Access Control**: Restrict access to configuration files containing sensitive information

Example of setting environment variables:
```bash
export EGGNOG_DATA_DIR=/path/to/eggnog/data
export CUSTOM_CONFIG_PATH=/secure/path/config
```

### General Configuration

Configuration options can be set via:
- Command-line arguments (recommended)
- Environment variables
- Configuration files (for advanced users)

## Citation

If you use this software in your research, please cite:

```
[1] eggNOG-mapper v2: functional annotation, orthology assignments, and domain 
    prediction at the metagenomic scale. Carlos P. Cantalapiedra, 
    Ana Hernandez-Plaza, Ivica Letunic, Peer Bork, Jaime Huerta-Cepas. 2021.
    Molecular Biology and Evolution, msab293, https://doi.org/10.1093/molbev/msab293

[2] eggNOG 5.0: a hierarchical, functionally and phylogenetically annotated
    orthology resource based on 5090 organisms and 2502 viruses. Jaime
    Huerta-Cepas, Damian Szklarczyk, Davide Heller, Ana Hernández-Plaza, Sofia
    K Forslund, Helen Cook, Daniel R Mende, Ivica Letunic, Thomas Rattei, Lars
    J Jensen, Christian von Mering, Peer Bork Nucleic Acids Res. 2019 Jan 8;
    47(Database issue): D309–D314. doi: 10.1093/nar/gky1085 
```

Please also cite the underlying algorithms used:

```
[HMMER] Accelerated Profile HMM Searches. 
        Eddy SR. 2011. PLoS Comput. Biol. 7:e1002195.

[DIAMOND] Sensitive protein alignments at tree-of-life scale using DIAMOND.
          Buchfink B, Reuter K, Drost HG. 2021.
          Nature Methods 18, 366–368 (2021). https://doi.org/10.1038/s41592-021-01101-x

[MMSEQS2] MMseqs2 enables sensitive protein sequence searching for the analysis of massive data sets.
          Steinegger M & Söding J. 2017. Nat. Biotech. 35, 1026–1028. https://doi.org/10.1038/nbt.3988

[PRODIGAL] Prodigal: prokaryotic gene recognition and translation initiation site identification.
           Hyatt et al. 2010. BMC Bioinformatics 11, 119. https://doi.org/10.1186/1471-2105-11-119.
```

## Contributing

We welcome contributions from the community! Please check our wiki for guidelines on:
- Reporting bugs
- Suggesting features
- Submitting pull requests
- Code style and testing

## License

This project is licensed under the terms specified in the LICENSE.txt file.

## Support

For questions, issues, or feature requests:
- Check the documentation wiki: https://github.com/jhcepas/eggnog-mapper/wiki
- Open an issue on GitHub
- Contact the development team

## Acknowledgments

EggNOG-mapper is developed and maintained by the European Molecular Biology Laboratory (EMBL) and collaborators. We thank all contributors and users for their feedback and support.