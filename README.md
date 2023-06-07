# Tafs.ElectronicDataInterchange

Tafs.EDI is an open source, [Remora-powered](https://github.com/Remora/Remora.Sdk), [LGPL-licensed](./LICENSE) framework for serializing and deserializing EDI X12, X12 HIPAA, and EDIFACT documents.

This project was originally inspired by [EdiWeave](https://ediweave.net/) but is designed to be a ground-up reinvisioning of the project with full documentation.

Supported frameworks:
- netstandard2.1
- net6.0
- net7.0

## Libraries

### Tafs.EDI.Core

This library provides base types for implementing non-version-specific libraries. Some version control is still provided, however we endeavor to clearly mark when a particular element is and is no longer available.

```
Install-Package Tafs.EDI.Core
```

### Tafs.EDI.TransactionSets

This is a meta library which automatically installs all transaction sets. Current transaction sets include:


|             Industry              |   Supported Transaction Sets    |               Package Name                |
|-----------------------------------|---------------------------------|-------------------------------------------|
| X12C - Communication and Controls | Nothing here yet!               |                                           |
| X12F - Finance                    | Nothing here yet!               |                                           |
| X12I - Transportation             | 204 (Motor Carrier Load Tender) | `Tafs.EDI.TransactionSets.Transportation` |
| X12M - Supply Chain               | Nothing here yet!               |                                           |
| X12N - Insurance                  | Nothing here yet!               |                                           |

