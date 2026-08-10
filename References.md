# GATk.GRCh38 used by nfcore sarek
## First download the awscli
```bash
aws s3 --no-sign-request --region eu-west-1 sync s3://ngi-igenomes/igenomes/Homo_sapiens/GATK/GRCh38/ ./GATK_GRCh38/
```
What is included in this download?The command pulls down approximately 50 GB to 100 GB of data, spanning three major components:
1. Sequence/WholeGenomeFasta/: The complete reference genome (.fasta), index (.fai), and sequence dictionary (.dict).
2. Sequence/BWAIndex/: Pre-built alignment indexes (including the .alt file for alt-aware mapping with BWA-MEM).
3. Annotation/GATKBundle/: Known variant structural files required for GATK Base Quality Score Recalibration (BQSR). These include files like dbsnp_146.hg38.vcf.gz and Mills_and_1000G_gold_standard.indels.hg38.vcf.gz

