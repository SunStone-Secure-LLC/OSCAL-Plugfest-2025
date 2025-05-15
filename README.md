# 📘 OSCAL Plugfest 2025

This repository contains validated and non-validated OSCAL files across multiple FedRAMP and NIST-supported formats. Validation was performed using the [OSCAL CLI Tool](https://github.com/metaschema-framework/oscal-cli)
, a high-fidelity metaschema-based framework for OSCAL schema validation.

## Link Share

[Link to OSCAL Foundation Open Letter to FedRAMP](https://github.com/FedRAMP/rev5-continuous-monitoring-cwg/discussions/35)

## Tool Identification
List out the different files tested. Which ones work and which did not. 
For the ones that did not work, do you know why it failed? 

If Yes, 
What would be the recommended fix. Please Submit a Github Issue OR Add the information in the readme for each folder type.

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
| SAR (Security Assessment Report)     | Describes how the system implements required security controls.                |
| SSP (System Security Plan)           | Documents implementation of security controls for an information system        |
| POAM (Plan of Action and Milestones) | Lists known security issues, planned fixes, and deadlines                      |
| Component Definition                 | Describes individual system components and associated control implementations  |
| Profile                              | Tailors a catalog to specific requirements (e.g., FedRAMP Moderate Baseline)   |

## ✅ Validation Process
All files in the Valid/ subfolders were tested using the oscal-cli as follows:

🧪 Sample Validation Command:

```oscal-cli validate (File)```

For SSP (FedRAMP Contraints in SSP Folder):

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

