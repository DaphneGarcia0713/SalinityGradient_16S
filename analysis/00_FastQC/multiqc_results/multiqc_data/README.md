 fastqc /workdir/dsg252/SalinityGradient_16S/data/01_DADA2/01_raw_gzipped_fastq/*.fastq.gz \ --threads 5 -o /workdir/dsg252/Salinity_Gradient16S/analysis/00_FastQC/fastqc_reports
  336   fastqc /workdir/dsg252/SalinityGradient_16S/data/01_DADA2/01_raw_gzipped_fastq/*.fastq.gz \ --threads 5 -o /workdir/dsg252/SalinityGradient_16S/analysis/00_FastQC/fastqc_reports/
  337  git config --global init.defaultBranch main
  338  git status
  339  git add *.zip
  340  git add *.html
  341  git commit -m "adding .gzip and .html"
  342  git push --set-upstream origin main
  343  cd ../
  344  cd analysis/00_FastQC/
  345  multiqc fastqc_reports/ -o multiqc_results/
  346  ls
  347  cd multiqc_results/
  348  ls
  349  cd multiqc_data/
  350  ls
  351  pwd
  352  history
[dsg252@cbsulm35 multiqc_data]




#code to execute fastqc


fastqc /workdir/dsg252/SalinityGradient_16S/data/01_DADA2/01_raw_gzipped_fastq/*.fastq.gz \ --threads 5 -o /workdir/dsg252/SalinityGrad>



#MultiQC

##LOAD MULTI QC
export PYTHONPATH=/programs/multiqc-1.15/lib64/python3.9/site-packages:/programs/multiqc-1.15/lib/python3.9/site-packages
export PATH=/programs/multiqc-1.15/bin:$PAT

# LOAD FASTQC
# Full path: /programs/FastQC-0.12.1/fastqc 
export PATH=/programs/FastQC-0.12.1:$PATH

etc
