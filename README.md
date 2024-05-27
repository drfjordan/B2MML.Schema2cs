# Generate B2MML C# classes

Tutorial for generating B2MML V7 .net c# classes

1. Make sure to have `xscgen` available.
   ([GitHub](https://github.com/mganss/XmlSchemaClassGenerator))
   
   .NET Core CLI tool available in the [dotnet-xscgen NuGet package](https://www.nuget.org/packages/dotnet-xscgen/)

   Install via `dotnet tool install --global dotnet-xscgen --version 2.1.1142`

2. Copy current release of B2MML V7 into folder `MESAInternational/B2MML-BatchML`.
   ([GitHub](https://github.com/MESAInternational/B2MML-BatchML))

   `cd MESAInternational`

   `git clone https://github.com/MESAInternational/B2MML-BatchML.git`
   
3. Execute `xscgen -nc -nf xscgen/B2MML-V7-AllSchemas.namespaceFile -o src/generated/B2MML-V7  MESAInternational/B2MML-BatchML/Schema/AllSchemas.xsd`

Generated classes should appear in folder `src/generated/B2MML-V7`
