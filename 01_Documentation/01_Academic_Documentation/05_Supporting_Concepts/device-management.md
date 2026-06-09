# Device Inventory Management Approaches for SMEs

## Purpose

This document explores practical approaches that Small and Medium-Sized Enterprises (SMEs) can use to maintain an accurate inventory of devices for Cyber Essentials readiness and ongoing cybersecurity management.

Device inventory management is a fundamental requirement for effective cybersecurity because organisations cannot secure assets they do not know exist. The approaches presented here are designed to accommodate organisations with varying levels of technical maturity, resources, and budget.

---

## Background

Cyber Essentials requires organisations to understand which devices are within scope and ensure that those devices are appropriately managed, updated, and protected.

Many SMEs struggle with maintaining accurate inventories due to:

* Limited IT resources.
* Informal device management processes.
* Remote and hybrid working arrangements.
* Employee-owned device usage.
* Lack of dedicated asset management tools.

The following approaches provide scalable solutions suitable for different organisational sizes and levels of complexity.

---

# Method 1 – Manual Spreadsheet Inventory

## Overview

**Best For:** Small businesses (1–15 devices)

**Implementation Effort:** Low

**Cost:** Free

**Cyber Essentials Suitability:** Fully Suitable

### Approach

A shared spreadsheet is used as the central device inventory repository.

Each device that:

* Accesses business data.
* Connects to business systems.
* Uses business email.
* Operates remotely for business purposes.

is recorded within the inventory.

Users update their information when changes occur, and management performs periodic reviews.

### Suggested Data Fields

* Device Name
* Device Type
* Assigned User
* Operating System
* OS Version
* Serial Number
* Antivirus Installed
* Auto Updates Enabled
* Encryption Enabled
* Last Review Date

### Advantages

* Extremely simple to implement.
* No specialist knowledge required.
* No licensing costs.
* Easy to explain during Cyber Essentials assessment.

### Limitations

* Relies heavily on user compliance.
* Prone to manual errors.
* Difficult to scale as device numbers increase.

### Repository Structure

```text
/Device_Inventory/
│
├── device_inventory_template.xlsx
├── METHOD_1_SPREADSHEET.md
└── example_inventory.xlsx
```

---

# Method 2 – Form-Based Inventory Workflow

## Overview

**Best For:** SMEs with 15–50 devices

**Implementation Effort:** Medium

**Cost:** Free

**Cyber Essentials Suitability:** Strong

### Approach

A structured onboarding form is used to collect device information automatically.

When users join the organisation, they complete a form containing:

* Device type.
* Operating system.
* Serial number.
* Antivirus status.
* Update status.
* Encryption status.

Responses automatically populate a central inventory spreadsheet.

Periodic device confirmation forms are then used to validate inventory accuracy.

### Monthly Device Confirmation

Users confirm:

* Device remains in use.
* Updates are installed.
* No major configuration changes occurred.
* Device ownership remains unchanged.

### Advantages

* Reduces manual administration.
* Creates timestamped records.
* Encourages user accountability.
* Produces audit-friendly evidence.

### Limitations

* Depends on users completing forms.
* Still requires management oversight.
* May not identify unmanaged devices automatically.

### Repository Structure

```text
/Device_Inventory/
│
└── Method_2_Form_Workflow/
    │
    ├── onboarding_form_template.md
    ├── monthly_device_check.md
    ├── process_workflow_diagram.png
    └── inventory_process_guide.md
```

---

# Method 3 – Automated Device Management

## Overview

**Best For:** Organisations with more than 50 devices

**Implementation Effort:** Initial setup required

**Cost:** Low to Moderate

**Cyber Essentials Suitability:** Excellent

### Example Solutions

* Microsoft Intune
* JumpCloud
* ManageEngine Endpoint Central
* Kandji
* Mosyle
* Jamf

### Approach

A management agent is deployed to managed devices.

The platform automatically collects information including:

* Device name.
* Operating system.
* Patch status.
* Antivirus status.
* Encryption status.
* Assigned user.
* Device location.
* Compliance status.

Information is continuously updated and centrally managed.

### Advantages

* Real-time inventory visibility.
* Minimal manual effort after deployment.
* Supports compliance monitoring.
* Produces strong assessment evidence.
* Helps satisfy multiple Cyber Essentials requirements simultaneously.

### Limitations

* Requires implementation effort.
* May involve licensing costs.
* Requires administrative expertise.

### Evidence Benefits

Automated platforms can assist with:

* Device inventory maintenance.
* Security update verification.
* Malware protection monitoring.
* Secure configuration oversight.
* Compliance reporting.

These capabilities can significantly simplify Cyber Essentials readiness activities.

---

# Comparative Analysis

| Feature                 | Method 1 | Method 2 | Method 3     |
| ----------------------- | -------- | -------- | ------------ |
| Cost                    | Free     | Free     | Low–Moderate |
| Setup Complexity        | Low      | Medium   | High         |
| Scalability             | Low      | Medium   | High         |
| Automation              | None     | Partial  | Full         |
| Audit Evidence          | Basic    | Good     | Excellent    |
| Suitable Device Count   | 1–15     | 15–50    | 50+          |
| Administrative Overhead | High     | Medium   | Low          |

---

# Recommendation

The most appropriate approach depends on organisational size and maturity.

### Small Organisations

Method 1 provides a simple and cost-effective solution that satisfies Cyber Essentials requirements.

### Growing SMEs

Method 2 introduces structure and automation without additional cost and is likely to provide the best balance between usability and compliance.

### Mature Organisations

Method 3 offers the strongest long-term solution and supports broader cybersecurity governance, compliance monitoring, and operational efficiency.

---

## Future Development

Potential future enhancements include:

* Automated readiness scoring.
* Asset lifecycle tracking.
* Vulnerability management integration.
* Compliance dashboards.
* Cyber Essentials evidence repositories.
* Continuous compliance monitoring.

---

## Status

**Status:** Research Concept / Future Toolkit Component

This document forms part of the Supporting Concepts section and may be incorporated into future versions of the Tanasiom Aegis Cyber Essentials Readiness Toolkit.
