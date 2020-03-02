# GATK.gVCF.header
Description of a typical gVCF (fileformat=VCFv4.2).<br>

<br>
## ALT
NON_REF.<br>
Represents any possible alternative allele at this location<br>
<br>
<br>

# FILTER section
LowQual.<br>
Low quality<br>
<br>
<br>

# FORMAT section
## AD
Allelic depths for the ref and alt alleles in the order listed.<br>
Number=R<br>
Type=Integer<br>
<br>
<br>

## DP
Approximate read depth (reads with MQ=255 or with bad mates are filtered).<br>
Number=1<br>
Type=Integer<br>
<br>
<br>

## GQ
Genotype Quality.<br>
It corresponds to the difference of the two most probable genotypes (since the most probable is assigned a '0', the lowest, likelihood).<br>
Number=1<br>
Type=Integer<br>
<br>
<br>

## GT
Genotype.<br>
Number=1<br>
Type=String<br>
<br>
<br>

## MIN_DP
Minimum DP observed within the GVCF block.<br>
Number=1<br>
Type=Integer<br>
<br>
<br>

## PGT
Physical phasing haplotype information, describing how the alternate alleles are phased in relation to one another.<br>
Number=1<br>
Type=String<br>
<br>
<br>

## PID
Physical phasing ID information, where each unique ID within a given sample (but not across samples) connects records 
within a phasing group.<br>
Number=1<br>
Type=String<br>
<br>
<br>

## PL
Normalized, Phred-scaled likelihoods for genotypes as defined in the VCF specification.<br>
Number=G<br>
Type=Integer<br>
<br>
<br>

## RGQ
Unconditional reference genotype confidence, encoded as a phred quality -10*log10 p(genotype call is wrong).<br>
Number=1<br>
Type=Integer<br>
<br>
<br>

## SB
Per-sample component statistics which comprise the Fisher's Exact Test to detect strand bias.<br>
Number=4<br>
Type=Integer<br>
<br>
<br>

# INFO section
## AC
Allele count in genotypes, for each ALT allele, in the same order as listed.<br>
Number=A<br>
Type=Integer<br>
<br>
<br>

## AF
Allele Frequency, for each ALT allele, in the same order as listed.<br>
Number=A<br>
Type=Float<br>
<br>
<br>

## AN
Total number of alleles in called genotypes.<br>
Number=1<br>
Type=Integer<br>
<br>
<br>

## BaseQRankSum
Z-score from Wilcoxon rank sum test of Alt Vs. Ref base qualities.<br>
Number=1<br>
Type=Float<br>
<br>
<br>

## ClippingRankSum
Z-score From Wilcoxon rank sum test of Alt vs. Ref number of hard clipped bases.<br>
Number=1<br>
Type=Float<br>
<br>
<br>

## DP
Approximate read depth; some reads may have been filtered.<br>
Number=1<br>
Type=Integer<br>
<br>
<br>

## DS
Were any of the samples downsampled?
Number=0<br>
Type=Flag<br>
<br>
<br>

## END
Stop position of the interval.<br>
Number=1<br>
Type=Integer<br>
<br>
<br>

## ExcessHet
Phred-scaled p-value for exact test of excess heterozygosity.<br>
Number=1<br>
Type=Float<br>
<br>
<br>

## FS
Phred-scaled p-value using Fisher's exact test to detect strand bias.<br>
Number=1<br>
Type=Float<br>
<br>
<br>

## HaplotypeScore
Consistency of the site with at most two segregating haplotypes.<br>
Number=1<br>
Type=Float<br>
<br>
<br>

## InbreedingCoeff
Inbreeding coefficient as estimated from the genotype likelihoods per-sample when compared against the Hardy-Weinberg expectation.<br>
Number=1<br>
Type=Float<br>
<br>
<br>

## MLEAC
Maximum likelihood expectation (MLE) for the allele counts (not necessarily the same as the AC), for each ALT allele, in the same order as listed.<br>
Number=A<br>
Type=Integer<br>
<br>
<br>

## LEAF
Maximum likelihood expectation (MLE) for the allele frequency (not necessarily the same as the AF), for each ALT allele, in the same order as listed.<br>
Number=A<br>
Type=Float<br>
<br>
<br>

## MQ
RMS Mapping Quality.<br>
Number=1<br>
Type=Float<br>
<br>
<br>

## MQRankSum
Z-score From Wilcoxon rank sum test of Alt vs. Ref read mapping qualities.<br>
Number=1<br>
Type=Float<br>
<br>
<br>

## QD
Variant Confidence/Quality by Depth.<br>
Number=1<br>
Type=Float<br>
<br>
<br>

## RAW_MQ
Raw data for RMS Mapping Quality.<br>
Number=1<br>
Type=Float<br>
<br>
<br>

## ReadPosRankSum
Z-score from Wilcoxon rank sum test of Alt vs. Ref read position bias.<br>
Number=1<br>
Type=Float<br>
<br>
<br>

## SOR
Symmetric Odds Ratio of 2x2 contingency table to detect strand bias.<br>
Number=1<br>
Type=Float<br>
<br>
<br>

