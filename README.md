# 📘 OSCAL Plugfest 2025

This repository contains validated and non-validated OSCAL files across multiple FedRAMP and NIST-supported formats. Validation was performed using the [OSCAL CLI Tool](https://github.com/metaschema-framework/oscal-cli)
, a high-fidelity metaschema-based framework for OSCAL schema validation.

## 📂 Repository Structure
Each top-level directory represents a distinct OSCAL model:
```
📁 SAP/
   ├── 📁 Valid/
   └── 📁 Not_Valid/
📁 SSP/
   ├── 📁 Valid/
   └── 📁 Not_Valid/
📁 POAM/
📁 Component_Definition/
📁 Profile/
```
Each model folder contains:

- Valid/: Files that successfully passed validation via oscal-cli validate
- Not_Valid/: Files that did not pass validation and require attention

## 📄 File Type Overview
| Format                  | Description                                                                 |
|-------------------------|-----------------------------------------------------------------------------|
| SAR (Security Assessment Report)     | Contains results from a completed assessment                                    |
| SSP (System Security Plan)           | Documents implementation of security controls for an information system        |
| POAM (Plan of Action and Milestones) | Lists known security issues, planned fixes, and deadlines                      |
| Component Definition                 | Describes individual system components and associated control implementations  |
| Profile                              | Tailors a catalog to specific requirements (e.g., FedRAMP Moderate Baseline)   |

## ✅ Validation Process
All files in the Valid/ subfolders were tested using the oscal-cli as follows:

🧪 Sample Validation Command:

```oscal-cli validate (File)```

For SSP:

```oscal-cli validate (File) -c (Constraint File 1) -c (Constraint File 2)```

The tool checks against:
- OSCAL metaschema constraints
- Format correctness for JSON/XML/YAML
- Required fields, enumerations, and references

## ❗ Non-Validated Files
Files in the Not_Valid/ directories failed at least one validation check. Common issues include:
- Missing required metadata (e.g., uuid, title)
- Schema mismatches
- Malformed JSON, XML, or YAML
- Unresolved import/include references
  
These files are retained for debugging, completeness, and ongoing improvement.

