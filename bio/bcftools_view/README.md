# Wrapper for samtools sort.

## Example:

```
rule bcf_to_vcf:
    input:
        "{prefix}.bcf"
    output:
        "{prefix}.vcf"
    params:
        ""  # optional parameters for bcftools view (except -o)
    wrapper:
        "master/bio/bcftools_view"
```