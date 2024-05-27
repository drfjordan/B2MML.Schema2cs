# Generate B2MML C# classes

Tutorial for generating B2MML V7 .net c# classes

1. Make sure to have `xscgen` available.
   ([GitHub](https://github.com/mganss/XmlSchemaClassGenerator))
2. Copy current release of B2MML V7 into folder `MESAInternational/B2MML-BatchML`.
   ([GitHub](https://github.com/MESAInternational/B2MML-BatchML))
3. Execute `xscgen -nc -nf xscgen/B2MML-V7-AllSchemas.namespaceFile -o src/generated/B2MML-V7  MESAInternational/B2MML-BatchML/Schema/AllSchemas.xsd`

Generated classes should appear in folder `src/generated/B2MML-V7`
