The empty operator skip_core_consistency has been created to avoid the dag stopping at the core consistency check
this is because the core consistency is hard to fix at source and it can be easily fixed with a delete statement after loading
the data to the target table IA.PUBLIC_REPORTS.PBIREP_ASSURANCE_LEVEL_CORE_FACT_TABLE.
The issue is created by the field guideline.description_text that has duplicates.
At source the duplication at guideline.name level was avoided with the uniqueness of the IA.AUDIMEX_SOURCE.TBL_AUDMX_AUDIT_MANUAL_TREE
created for the purpose.
We could run a similar procedure for guideline.description_text, but it would be very long