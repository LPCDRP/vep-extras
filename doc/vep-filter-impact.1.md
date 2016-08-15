% VEP-FILTER-IMPACT(1)
%
%

# NAME

vep-filter-impact - position-based filter for VEP variant annotations

# SYNOPSIS

**vep-filter-impact** [**--strict**] *infile*

# DESCRIPTION

**vep-filter-impact** operates on annotated VCF files produced by **variant_effect_predictor.pl**.
In its default mode, it preserves annotations corresponding to the gene containing the variant, if it is in a coding sequence, as well as the nearest gene downstream of the variant.
If the second-nearest downstream gene is on the opposite strand, the annotation for this is also kept.
When running with **--strict**, no annotations for adjacent genes are kept if the variant is in a coding sequence.

Currently *input* must be in VEP's annotated VCF format.
The native VEP format is not yet supported.

# OPTIONS

**--strict**
:	Enable strict mode. See **DESCRIPTION** for details about this mode.

# SEE ALSO

**vep-extras**(1)
