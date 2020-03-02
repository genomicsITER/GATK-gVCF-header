# GATK.gVCF.header
Description of a typical gVCF

##fileformat=VCFv4.2
##ALT=<ID=NON_REF,Description="Represents any possible alternative allele at this location">

##FILTER=<ID=LowQual,Description="Low quality">

##FORMAT section
AD
Allelic depths for the ref and alt alleles in the order listed
Number=R
Type=Integer

DP
Approximate read depth (reads with MQ=255 or with bad mates are filtered)
Number=1
Type=Integer

GQ
Genotype Quality
Number=1
Type=Integer
It corresponds to the difference of the two most probable genotypes (since the most probable is assigned a '0', the lowest, likelihood)

GT
Genotype
Number=1
Type=String

PGT
Physical phasing haplotype information, describing how the alternate alleles are phased in relation to one another
Number=1
Type=String

PID
Physical phasing ID information, where each unique ID within a given sample (but not across samples) connects records 
within a phasing group
Number=1
Type=String

PL
Normalized, Phred-scaled likelihoods for genotypes as defined in the VCF specification
Number=G
Type=Integer

SB,Number=4,Type=Integer,
Description="Per-sample component statistics which comprise the Fisher's Exact Test to detect strand bias.">

##INFO=<ID=BaseQRankSum,Number=1,Type=Float,Description="Z-score from Wilcoxon rank sum test of Alt Vs. Ref base qualities">
##INFO=<ID=ClippingRankSum,Number=1,Type=Float,Description="Z-score From Wilcoxon rank sum test of Alt vs. Ref number of hard clipped bases">
##INFO=<ID=DP,Number=1,Type=Integer,Description="Approximate read depth; some reads may have been filtered">
##INFO=<ID=DS,Number=0,Type=Flag,Description="Were any of the samples downsampled?">
##INFO=<ID=ExcessHet,Number=1,Type=Float,Description="Phred-scaled p-value for exact test of excess heterozygosity">
##INFO=<ID=HaplotypeScore,Number=1,Type=Float,Description="Consistency of the site with at most two segregating haplotypes">
##INFO=<ID=InbreedingCoeff,Number=1,Type=Float,Description="Inbreeding coefficient as estimated from the genotype likelihoods per-sample when compared against the Hardy-Weinberg expectation">
##INFO=<ID=MLEAC,Number=A,Type=Integer,Description="Maximum likelihood expectation (MLE) for the allele counts (not necessarily the same as the AC), for each ALT allele, in the same order as listed">
##INFO=<ID=MLEAF,Number=A,Type=Float,Description="Maximum likelihood expectation (MLE) for the allele frequency (not necessarily the same as the AF), for each ALT allele, in the same order as listed">
##INFO=<ID=MQ,Number=1,Type=Float,Description="RMS Mapping Quality">
##INFO=<ID=MQRankSum,Number=1,Type=Float,Description="Z-score From Wilcoxon rank sum test of Alt vs. Ref read mapping qualities">
##INFO=<ID=RAW_MQ,Number=1,Type=Float,Description="Raw data for RMS Mapping Quality">
##INFO=<ID=ReadPosRankSum,Number=1,Type=Float,Description="Z-score from Wilcoxon rank sum test of Alt vs. Ref read position bias">

