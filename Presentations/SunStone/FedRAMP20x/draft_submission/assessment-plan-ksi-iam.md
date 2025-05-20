{
  "assessment-plan": {
    "uuid": "1a2b3c4d-5e6f-7a8b-9c0d-1e2f3a4b5c6d",
    "metadata": {
      "title": "Assessment Plan for KSI-IAM Metrics and Related Cloud Native IAM Characteristics",
      "last-modified": "2025-05-19T23:30:00.000Z",
      "version": "1.0.0",
      "oscal-version": "1.1.3",
      "remarks": "This assessment plan details the scope and methodology for assessing Key Security Indicator (KSI) metrics for Identity and Access Management (IAM) effectiveness, focusing on phishing-resistant MFA, strong passwords, secure API authentication, and least privilege principles. It also considers related FedRAMP Rev 5 Low baseline controls.",
      "roles": [
        {
          "id": "assessor",
          "title": "Assessment Team Lead"
        },
        {
          "id": "csp-contact",
          "title": "Cloud Service Provider Primary Contact"
        }
      ],
      "parties": [
        {
          "uuid": "party-assessor-org-uuid",
          "type": "organization",
          "name": "Independent Assessor Organization",
          "short-name": "IAO"
        },
        {
          "uuid": "party-csp-org-uuid",
          "type": "organization",
          "name": "Example Cloud Service Provider Inc.",
          "short-name": "ExampleCSP"
        }
      ],
      "responsible-parties": [
        {
          "role-id": "assessor",
          "party-uuids": [
            "party-assessor-org-uuid"
          ]
        },
        {
          "role-id": "csp-contact",
          "party-uuids": [
            "party-csp-org-uuid"
          ]
        }
      ]
    },
    "import-ssp": {
      "href": "./ssp-example.json",
      "remarks": "System Security Plan for the target Cloud Service Offering (CSO) being assessed."
    },
    "reviewed-controls": {
      "description": "This assessment will review the specified KSI-IAM metrics and related FedRAMP Rev5 Low baseline controls.",
      "control-selections": [
        {
          "description": "KSI-IAM Metrics from the KSI Metrics Catalog.",
          "source": "urn:uuid:aadc2898-59A9-4C00-A09A-946C0D4A78F5",
          "include-controls": [
            {
              "control-id": "ksi-iam"
            },
            {
              "control-id": "ksi-iam-metric-01-mfa-enforcement"
            },
            {
              "control-id": "ksi-iam-metric-02-strong-passwords"
            },
            {
              "control-id": "ksi-iam-metric-03-secure-api-auth"
            },
            {
              "control-id": "ksi-iam-metric-04-least-privilege-rbac-jit"
            }
          ]
        },
        {
          "description": "Related FedRAMP Rev5 Low Baseline Controls.",
          "source": "urn:uuid:97bf2d6d-1907-4e51-8c5e-2a8776c39820",
          "include-controls": [
            {
              "control-id": "ac-2"
            },
            {
              "control-id": "ac-3"
            },
            {
              "control-id": "ac-14"
            },
            {
              "control-id": "ia-2"
            },
            {
              "control-id": "ia-2.1"
            },
            {
              "control-id": "ia-2.2"
            },
            {
              "control-id": "ia-2.8"
            },
            {
              "control-id": "ia-2.12"
            },
            {
              "control-id": "ia-4"
            },
            {
              "control-id": "ia-5"
            },
            {
              "control-id": "ia-5.1"
            },
            {
              "control-id": "ia-6"
            },
            {
              "control-id": "ia-8"
            },
            {
              "control-id": "ia-8.1"
            },
            {
              "control-id": "ia-8.2"
            },
            {
              "control-id": "ia-8.4"
            },
            {
              "control-id": "ia-11"
            },
            {
              "control-id": "ps-2"
            },
            {
              "control-id": "ps-3"
            },
            {
              "control-id": "ps-4"
            },
            {
              "control-id": "ps-5"
            },
            {
              "control-id": "ps-7"
            },
            {
              "control-id": "ps-9"
            },
            {
              "control-id": "au-9"
            }
          ]
        }
      ],
      "control-objective-selections": [
        {
          "description": "Assessment objectives for KSI-IAM metrics derived from the KSI Metrics Catalog.",
          "source": "urn:uuid:aadc2898-59A9-4C00-A09A-946C0D4A78F5",
          "include-objectives": [
            {
              "objective-id": "ksi-iam-objective"
            },
            {
              "objective-id": "ksi-iam-metric-01-main-objective"
            },
            {
              "objective-id": "ksi-iam-metric-01-obj-priv-mfa"
            },
            {
              "objective-id": "ksi-iam-metric-01-obj-nonpriv-mfa"
            },
            {
              "objective-id": "ksi-iam-metric-01-obj-api-mfa"
            },
            {
              "objective-id": "ksi-iam-metric-01-obj-replay-resistance"
            },
            {
              "objective-id": "ksi-iam-metric-01-obj-piv-acceptance"
            },
            {
              "objective-id": "ksi-iam-metric-02-main-objective"
            },
            {
              "objective-id": "ksi-iam-metric-02-obj-strength-init"
            },
            {
              "objective-id": "ksi-iam-metric-02-obj-compromised-check"
            },
            {
              "objective-id": "ksi-iam-metric-02-obj-secure-storage-transmit"
            },
            {
              "objective-id": "ksi-iam-metric-02-obj-composition-complexity"
            },
            {
              "objective-id": "ksi-iam-metric-03-main-objective"
            },
            {
              "objective-id": "ksi-iam-metric-03-obj-protocol-use"
            },
            {
              "objective-id": "ksi-iam-metric-03-obj-token-security"
            },
            {
              "objective-id": "ksi-iam-metric-03-obj-authorization"
            },
            {
              "objective-id": "ksi-iam-metric-03-obj-tls-encryption"
            },
            {
              "objective-id": "ksi-iam-metric-04-main-objective"
            },
            {
              "objective-id": "ksi-iam-metric-04-obj-rbac-coverage"
            },
            {
              "objective-id": "ksi-iam-metric-04-obj-least-privilege"
            },
            {
              "objective-id": "ksi-iam-metric-04-obj-jit-adoption"
            }
          ]
        }
      ]
    },
    "assessment-subjects": [
      {
        "type": "component",
        "description": "The primary Identity and Access Management system of the Cloud Service Offering.",
        "include-subjects": [
          {
            "subject-uuid": "subject-uuid-iam-platform",
            "type": "component",
            "title": "CSO IAM Platform"
          }
        ]
      },
      {
        "type": "component",
        "description": "API Gateways and related components responsible for API authentication and authorization.",
        "include-subjects": [
          {
            "subject-uuid": "subject-uuid-api-gateway-main",
            "type": "component",
            "title": "Main API Gateway"
          }
        ]
      },
      {
        "type": "component",
        "description": "User account repositories and directories.",
        "include-subjects": [
          {
            "subject-uuid": "subject-uuid-user-directory",
            "type": "component",
            "title": "Primary User Directory"
          }
        ]
      }
    ],
    "assessment-assets": {
      "components": [
        {
          "uuid": "asset-component-uuid-log-analyzer",
          "type": "software",
          "title": "Automated Log Analysis Tool",
          "description": "Tool used for automated analysis of authentication and audit logs.",
          "status": {
            "state": "operational"
          }
        },
        {
          "uuid": "asset-component-uuid-config-scanner",
          "type": "software",
          "title": "Configuration Compliance Scanner",
          "description": "Tool used to scan and verify system configurations against defined baselines.",
          "status": {
            "state": "operational"
          }
        }
      ],
      "assessment-platforms": [
        {
          "uuid": "platform-uuid-main-assessment-suite",
          "title": "KSI Metric Assessment Suite",
          "uses-components": [
            {
              "component-uuid": "asset-component-uuid-log-analyzer"
            },
            {
              "component-uuid": "asset-component-uuid-config-scanner"
            }
          ]
        }
      ]
    },
    "tasks": [
      {
        "uuid": "task-uuid-assess-ksi-iam-overall",
        "type": "action",
        "title": "Assess KSI-IAM Overall Metric Calculation and Reporting",
        "description": "Verify the calculation and reporting of the overall KSI-IAM metric based on its constituent sub-metrics.",
        "associated-activities": [
          {
            "activity-uuid": "activity-uuid-review-ksi-iam-aggregation",
            "subjects": [
              {
                "subject-uuid": "subject-uuid-iam-platform",
                "type": "component"
              }
            ]
          }
        ]
      },
      {
        "uuid": "task-uuid-assess-mfa-metric",
        "type": "action",
        "title": "Assess Phishing-Resistant MFA Enforcement Metric (ksi-iam-metric-01)",
        "description": "Verify the CSP's measurement process and results for the Phishing-Resistant MFA Enforcement metric.",
        "associated-activities": [
          {
            "activity-uuid": "activity-uuid-verify-mfa-measurement",
            "subjects": [
              {
                "subject-uuid": "subject-uuid-iam-platform",
                "type": "component"
              },
              {
                "subject-uuid": "subject-uuid-api-gateway-main",
                "type": "component"
              }
            ]
          }
        ]
      },
      {
        "uuid": "task-uuid-assess-password-metric",
        "type": "action",
        "title": "Assess Strong Password Policy Enforcement Metric (ksi-iam-metric-02)",
        "description": "Verify the CSP's measurement process and results for the Strong Password Policy Enforcement metric.",
        "associated-activities": [
          {
            "activity-uuid": "activity-uuid-verify-password-measurement",
            "subjects": [
              {
                "subject-uuid": "subject-uuid-iam-platform",
                "type": "component"
              },
              {
                "subject-uuid": "subject-uuid-user-directory",
                "type": "component"
              }
            ]
          }
        ]
      },
      {
        "uuid": "task-uuid-assess-api-auth-metric",
        "type": "action",
        "title": "Assess Secure API Authentication Metric (ksi-iam-metric-03)",
        "description": "Verify the CSP's measurement process and results for the Secure API Authentication and Authorization Standards metric.",
        "associated-activities": [
          {
            "activity-uuid": "activity-uuid-verify-api-auth-measurement",
            "subjects": [
              {
                "subject-uuid": "subject-uuid-api-gateway-main",
                "type": "component"
              }
            ]
          }
        ]
      },
      {
        "uuid": "task-uuid-assess-least-priv-metric",
        "type": "action",
        "title": "Assess Least Privilege, RBAC, and JIT Metric (ksi-iam-metric-04)",
        "description": "Verify the CSP's measurement process and results for the Implementation of Least Privilege, RBAC, and Just-in-Time (JIT) Access metric.",
        "associated-activities": [
          {
            "activity-uuid": "activity-uuid-verify-least-priv-measurement",
            "subjects": [
              {
                "subject-uuid": "subject-uuid-iam-platform",
                "type": "component"
              }
            ]
          }
        ]
      }
    ],
    "local-definitions": {
      "activities": [
        {
          "uuid": "activity-uuid-review-ksi-iam-aggregation",
          "title": "Review KSI-IAM Overall Metric Aggregation",
          "description": "Validate the aggregation method and calculation for the overall KSI-IAM metric as defined in the KSI Metrics Catalog. This involves confirming how scores from sub-metrics (ksi-iam-metric-01 through ksi-iam-metric-04) are combined.",
          "steps": [
            {
              "uuid": "step-uuid-ksi-iam-agg-1",
              "description": "Examine the documented aggregation formula for 'ksi-iam' (KSI Metrics Catalog, prop: metric-aggregation-method)."
            },
            {
              "uuid": "step-uuid-ksi-iam-agg-2",
              "description": "Verify that the reported scores from constituent sub-metrics (ksi-iam-metric-01, ksi-iam-metric-02, ksi-iam-metric-03, ksi-iam-metric-04) are accurately used as inputs to the KSI-IAM calculation."
            },
            {
              "uuid": "step-uuid-ksi-iam-agg-3",
              "description": "Recalculate a sample of KSI-IAM scores based on provided sub-metric data to validate the CSP's calculation process."
            },
            {
              "uuid": "step-uuid-ksi-iam-agg-4",
              "description": "Assess evidence of adherence to the KSI-IAM SLO recommendations."
            }
          ],
          "related-controls": {
            "description": "KSI-IAM Overall Metric and its assessment objective.",
            "control-selections": [
              {
                "include-controls": [
                  {
                    "control-id": "ksi-iam"
                  }
                ]
              }
            ],
            "control-objective-selections": [
              {
                "include-objectives": [
                  {
                    "objective-id": "ksi-iam-objective"
                  }
                ]
              }
            ]
          }
        },
        {
          "uuid": "activity-uuid-verify-mfa-measurement",
          "title": "Verify Measurement of Phishing-Resistant MFA Enforcement (ksi-iam-metric-01)",
          "description": "Assess the CSP's methodology, data sources, and calculations for measuring the 'Effectiveness of Phishing-Resistant MFA Enforcement' metric (ksi-iam-metric-01) as defined in the KSI Metrics Catalog. Correlate with relevant FedRAMP controls.",
          "steps": [
            {
              "uuid": "step-uuid-mfa-1",
              "description": "Review the CSP's documented procedures for collecting data for A_priv, B_priv, A_nonpriv, B_nonpriv, A_api, B_api, as per the 'metric-rules' for ksi-iam-metric-01."
            },
            {
              "uuid": "step-uuid-mfa-2",
              "description": "Examine samples of data sources (e.g., IAM configurations, authentication logs, API gateway settings, account inventories) to verify the accuracy of reported figures for A_priv, B_priv, etc.."
            },
            {
              "uuid": "step-uuid-mfa-3",
              "description": "Validate the CSP's calculation of the 'Overall Percentage' for MFA enforcement using the 'metric-expression'."
            },
            {
              "uuid": "step-uuid-mfa-4",
              "description": "Verify that 'approved phishing-resistant MFA methods' align with NIST SP 800-63B AAL3 capabilities as stated in the metric rules."
            },
            {
              "uuid": "step-uuid-mfa-5",
              "description": "Assess reported adherence to the SLO recommendations for privileged, non-privileged, and API access."
            },
            {
              "uuid": "step-uuid-mfa-6",
              "description": "Correlate findings with the implementation status and effectiveness of related FedRAMP controls: IA-2, IA-2(1), IA-2(2), IA-2(8), IA-2(12)."
            }
          ],
          "related-controls": {
            "description": "KSI Metric for MFA Enforcement and related FedRAMP controls.",
            "control-selections": [
              {
                "include-controls": [
                  {
                    "control-id": "ksi-iam-metric-01-mfa-enforcement"
                  }
                ]
              },
              {
                "include-controls": [
                  {
                    "control-id": "ia-2"
                  },
                  {
                    "control-id": "ia-2.1"
                  },
                  {
                    "control-id": "ia-2.2"
                  },
                  {
                    "control-id": "ia-2.8"
                  },
                  {
                    "control-id": "ia-2.12"
                  }
                ]
              }
            ],
            "control-objective-selections": [
              {
                "include-objectives": [
                  {
                    "objective-id": "ksi-iam-metric-01-main-objective"
                  },
                  {
                    "objective-id": "ksi-iam-metric-01-obj-priv-mfa"
                  },
                  {
                    "objective-id": "ksi-iam-metric-01-obj-nonpriv-mfa"
                  },
                  {
                    "objective-id": "ksi-iam-metric-01-obj-api-mfa"
                  },
                  {
                    "objective-id": "ksi-iam-metric-01-obj-replay-resistance"
                  },
                  {
                    "objective-id": "ksi-iam-metric-01-obj-piv-acceptance"
                  }
                ]
              }
            ]
          }
        },
        {
          "uuid": "activity-uuid-verify-password-measurement",
          "title": "Verify Measurement of Strong Password Policy Enforcement (ksi-iam-metric-02)",
          "description": "Assess the CSP's methodology, data sources, and calculations for measuring the 'Effectiveness of Strong Password Policy Enforcement' metric (ksi-iam-metric-02) as defined in the KSI Metrics Catalog. Correlate with relevant FedRAMP controls.",
          "steps": [
            {
              "uuid": "step-uuid-pwd-1",
              "description": "Review the CSP's documented procedures for identifying systems/applications (B) and those enforcing compliant password policies (A), according to 'metric-rules' for ksi-iam-metric-02."
            },
            {
              "uuid": "step-uuid-pwd-2",
              "description": "Examine password policy configurations and system documentation to verify alignment with NIST SP 800-63B requirements (minimum length, breached password checks, secure storage)."
            },
            {
              "uuid": "step-uuid-pwd-3",
              "description": "Validate the CSP's calculation of the 'Percentage' using the 'metric-expression'."
            },
            {
              "uuid": "step-uuid-pwd-4",
              "description": "Assess reported adherence to the SLO recommendations."
            },
            {
              "uuid": "step-uuid-pwd-5",
              "description": "Correlate findings with the implementation status and effectiveness of related FedRAMP controls: IA-5, IA-5(1)."
            }
          ],
          "related-controls": {
            "description": "KSI Metric for Strong Passwords and related FedRAMP controls.",
            "control-selections": [
              {
                "include-controls": [
                  {
                    "control-id": "ksi-iam-metric-02-strong-passwords"
                  }
                ]
              },
              {
                "include-controls": [
                  {
                    "control-id": "ia-5"
                  },
                  {
                    "control-id": "ia-5.1"
                  }
                ]
              }
            ],
            "control-objective-selections": [
              {
                "include-objectives": [
                  {
                    "objective-id": "ksi-iam-metric-02-main-objective"
                  },
                  {
                    "objective-id": "ksi-iam-metric-02-obj-strength-init"
                  },
                  {
                    "objective-id": "ksi-iam-metric-02-obj-compromised-check"
                  },
                  {
                    "objective-id": "ksi-iam-metric-02-obj-secure-storage-transmit"
                  },
                  {
                    "objective-id": "ksi-iam-metric-02-obj-composition-complexity"
                  }
                ]
              }
            ]
          }
        },
        {
          "uuid": "activity-uuid-verify-api-auth-measurement",
          "title": "Verify Measurement of Secure API Authentication (ksi-iam-metric-03)",
          "description": "Assess the CSP's methodology, data sources, and calculations for measuring 'Adherence to Secure API Authentication and Authorization Standards' metric (ksi-iam-metric-03) as defined in the KSI Metrics Catalog. Correlate with relevant FedRAMP controls.",
          "steps": [
            {
              "uuid": "step-uuid-api-1",
              "description": "Review the CSP's API inventory (B) and methods for confirming secure authentication, authorization, and transit encryption (A) as per 'metric-rules' for ksi-iam-metric-03."
            },
            {
              "uuid": "step-uuid-api-2",
              "description": "Examine API gateway configurations, OAuth/OIDC server settings, and API documentation to verify use of approved protocols and best practices for token management and validation."
            },
            {
              "uuid": "step-uuid-api-3",
              "description": "Validate the CSP's calculation of the 'Percentage' using the 'metric-expression'."
            },
            {
              "uuid": "step-uuid-api-4",
              "description": "Assess reported adherence to the SLO recommendations for external and internal APIs."
            },
            {
              "uuid": "step-uuid-api-5",
              "description": "Correlate findings with the implementation status and effectiveness of related FedRAMP controls: IA-2, IA-8, AC-3, SC-8, SC-13."
            }
          ],
          "related-controls": {
            "description": "KSI Metric for Secure API Authentication and related FedRAMP controls.",
            "control-selections": [
              {
                "include-controls": [
                  {
                    "control-id": "ksi-iam-metric-03-secure-api-auth"
                  }
                ]
              },
              {
                "include-controls": [
                  {
                    "control-id": "ia-2"
                  },
                  {
                    "control-id": "ia-8"
                  },
                  {
                    "control-id": "ac-3"
                  },
                  {
                    "control-id": "sc-8"
                  },
                  {
                    "control-id": "sc-13"
                  }
                ]
              }
            ],
            "control-objective-selections": [
              {
                "include-objectives": [
                  {
                    "objective-id": "ksi-iam-metric-03-main-objective"
                  },
                  {
                    "objective-id": "ksi-iam-metric-03-obj-protocol-use"
                  },
                  {
                    "objective-id": "ksi-iam-metric-03-obj-token-security"
                  },
                  {
                    "objective-id": "ksi-iam-metric-03-obj-authorization"
                  },
                  {
                    "objective-id": "ksi-iam-metric-03-obj-tls-encryption"
                  }
                ]
              }
            ]
          }
        },
        {
          "uuid": "activity-uuid-verify-least-priv-measurement",
          "title": "Verify Measurement of Least Privilege, RBAC, and JIT (ksi-iam-metric-04)",
          "description": "Assess the CSP's methodology, data sources, and calculations for measuring the 'Implementation of Least Privilege, RBAC, and Just-in-Time (JIT) Access' metric (ksi-iam-metric-04) as defined in the KSI Metrics Catalog. Correlate with relevant FedRAMP controls.",
          "steps": [
            {
              "uuid": "step-uuid-lp-1",
              "description": "Review CSP's procedures for calculating Aspect1_RBAC_Coverage (A/B), Aspect2_LeastPrivilege_Review_Compliance (C/D), and Aspect3_JIT_Adoption_for_Privileged_Ops (E/F) based on 'metric-rules' for ksi-iam-metric-04."
            },
            {
              "uuid": "step-uuid-lp-2",
              "description": "Examine IAM system data, role definitions, access review reports, and JIT system configurations/logs to verify the accuracy of numerators and denominators for each aspect."
            },
            {
              "uuid": "step-uuid-lp-3",
              "description": "Validate the CSP's calculation of each aspect's percentage."
            },
            {
              "uuid": "step-uuid-lp-4",
              "description": "Assess reported adherence to the SLO recommendations for each aspect."
            },
            {
              "uuid": "step-uuid-lp-5",
              "description": "Correlate findings with the implementation status and effectiveness of related FedRAMP controls: AC-2, AC-3, PS-2, PS-7."
            }
          ],
          "related-controls": {
            "description": "KSI Metric for Least Privilege/RBAC/JIT and related FedRAMP controls.",
            "control-selections": [
              {
                "include-controls": [
                  {
                    "control-id": "ksi-iam-metric-04-least-privilege-rbac-jit"
                  }
                ]
              },
              {
                "include-controls": [
                  {
                    "control-id": "ac-2"
                  },
                  {
                    "control-id": "ac-3"
                  },
                  {
                    "control-id": "ps-2"
                  },
                  {
                    "control-id": "ps-7"
                  }
                ]
              }
            ],
            "control-objective-selections": [
              {
                "include-objectives": [
                  {
                    "objective-id": "ksi-iam-metric-04-main-objective"
                  },
                  {
                    "objective-id": "ksi-iam-metric-04-obj-rbac-coverage"
                  },
                  {
                    "objective-id": "ksi-iam-metric-04-obj-least-privilege"
                  },
                  {
                    "objective-id": "ksi-iam-metric-04-obj-jit-adoption"
                  }
                ]
              }
            ]
          }
        }
      ],
      "remarks": "Local activity definitions focus on verifying the CSP's measurement and reporting of defined KSI metrics."
    },
    "back-matter": {
      "resources": [
        {
          "uuid": "resource-ksi-catalog-uuid",
          "title": "OSCAL Catalog for KSI-IAM Metrics",
          "description": "The source catalog defining the KSI-IAM metrics being assessed.",
          "rlinks": [
            {
              "href": "urn:uuid:aadc2898-59A9-4C00-A09A-946C0D4A78F5"
            }
          ]
        },
        {
          "uuid": "resource-fedramp-low-catalog-uuid",
          "title": "FedRAMP Rev 5 Low Baseline Resolved Catalog",
          "description": "The source catalog for FedRAMP Rev 5 Low baseline controls.",
          "rlinks": [
            {
              "href": "urn:uuid:97bf2d6d-1907-4e51-8c5e-2a8776c39820"
            }
          ]
        }
      ]
    }
  }
}
