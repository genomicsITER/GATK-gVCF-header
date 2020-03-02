# GATK.gVCF.header
Description of a typical gVCF

##fileformat=VCFv4.2
##ALT=<ID=NON_REF,Description="Represents any possible alternative allele at this location">

# FILTER section
LowQual
Low quality

# FORMAT section
## AD
Allelic depths for the ref and alt alleles in the order listed
Number=R
Type=Integer

## DP
Approximate read depth (reads with MQ=255 or with bad mates are filtered)
Number=1
Type=Integer

## GQ
Genotype Quality
Number=1
Type=Integer
It corresponds to the difference of the two most probable genotypes (since the most probable is assigned a '0', the lowest, likelihood)

## GT
Genotype
Number=1
Type=String

## PGT
Physical phasing haplotype information, describing how the alternate alleles are phased in relation to one another
Number=1
Type=String

## PID
Physical phasing ID information, where each unique ID within a given sample (but not across samples) connects records 
within a phasing group
Number=1
Type=String

## PL
Normalized, Phred-scaled likelihoods for genotypes as defined in the VCF specification
Number=G
Type=Integer

## SB
Per-sample component statistics which comprise the Fisher's Exact Test to detect strand bias
Number=4
Type=Integer

## BaseQRankSum
Z-score from Wilcoxon rank sum test of Alt Vs. Ref base qualities
Number=1
Type=Float

## ClippingRankSum
Number=1
Type=Float
Z-score From Wilcoxon rank sum test of Alt vs. Ref number of hard clipped bases

## DP
Approximate read depth; some reads may have been filtered
Number=1
Type=Integer

## DS
Were any of the samples downsampled?
Number=0
Type=Flag

## ExcessHet
Number=1
Type=Float
Phred-scaled p-value for exact test of excess heterozygosity

## HaplotypeScore
Number=1
Type=Float
Consistency of the site with at most two segregating haplotypes

## InbreedingCoeff
Inbreeding coefficient as estimated from the genotype likelihoods per-sample when compared against the Hardy-Weinberg expectation
Number=1
Type=Float

## MLEAC
Maximum likelihood expectation (MLE) for the allele counts (not necessarily the same as the AC), for each ALT allele, in the same order as listed
Number=A
Type=Integer

## LEAF
Maximum likelihood expectation (MLE) for the allele frequency (not necessarily the same as the AF), for each ALT allele, in the same order as listed
Number=A
Type=Float

## MQ
RMS Mapping Quality
Number=1
Type=Float

## MQRankSum
Z-score From Wilcoxon rank sum test of Alt vs. Ref read mapping qualities
Number=1
Type=Float

## RAW_MQ
Number=1
Type=Float
Raw data for RMS Mapping Quality

## ReadPosRankSum
Number=1
Type=Float
Z-score from Wilcoxon rank sum test of Alt vs. Ref read position bias

