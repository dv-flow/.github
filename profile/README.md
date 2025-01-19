## DV-Flow - Flow Automation for Silicon Design


```mermaid

    flowchart TD
      A[IP Fileset] --> B[Testbench]
      C[VIP Fileset] --> D[Precompile]
      D --> B
      B --> E[SimImage]
      E --> F[Test1]
      E --> G[Test2]
      E --> H[Test3]
```

DV Flow is a set of tools focused on automating design and verification
activities for silicon design. Three categories of material are provided:

- **Specification** - Flows are specified using a YAML schema. Flows consist 
  of tasks related by dataflow.
- **Libraries** - Libraries provide pre-defined tasks that implement common
  operations, such as building a simulator image.
- **Technology** - Tools for developing and executing flow specifications

