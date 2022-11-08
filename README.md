# Snakemake workflow: rna-seq-star-deseq2

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4737358.svg)](https://doi.org/10.5281/zenodo.4737358)
[![Snakemake](https://img.shields.io/badge/snakemake-≥6.1.0-brightgreen.svg)](https://snakemake.github.io)
[![GitHub actions status](https://github.com/snakemake-workflows/rna-seq-star-deseq2/workflows/Tests/badge.svg?branch=master)](https://github.com/snakemake-workflows/rna-seq-star-deseq2/actions?query=branch%3Amaster+workflow%3ATests)

This workflow performs a differential gene expression analysis with STAR and Deseq2.

## Personally modified version to apply for custom genomes 

Tips:
1 Fix some bugs and add some tips in the configs and workflows.
2 Disable some steps, because custom genome may not have uniform Gene Symbol.
3 The custom genome and annotation should be put in `resources/genemone.fasta` and `resources/genemone.gtf` in advance.
4 If you can't get access to the wrappers from github like me, you can download the wappers(versions:0.77.0 and 0.75.0) and put them in the homedir and rewrite the wrappers in the workflows as `file://wrapper/0.77.0/bio/star/align`.

## Usage

The usage of this workflow is described in the [Snakemake Workflow Catalog](https://snakemake.github.io/snakemake-workflow-catalog/?usage=snakemake-workflows%2Frna-seq-star-deseq2).

If you use this workflow in a paper, don't forget to give credits to the authors by citing the URL of this (original) repository and its DOI (see above).
