# InspectaPro-Moana

# 1. **Business Interpretation**

**~ Ulith ~**

## 1.1 **Business model Interpretation**

InspectaPro is a SaaS platform for companies that do inspections in the field. These companies can work in different areas like maintenance, quality control, security, or audits. The main idea of the system is to help companies organize, assign, and store inspections in a digital way instead of using paper or informal tools.

The system works with a subscription model. Each company pays for a plan to use the platform. If the subscription is active, the company can create users, manage roles, create inspection types, and assign inspections. If the subscription is not active, the company should not be able to create new inspections.

---

## 1.2 **Actors of the system**

*Company*
The company is the organization that uses the system. It represents the client. All users and inspections belong to a company.

*Company Administrator*
This user manages the system inside the company. The administrator can create users, define roles, create inspection types, assign inspections to technicians, and review results.

*Technician*
The technician is the person who goes to the field and performs the inspection. The technician answers the questions, adds notes, and uploads evidence like photos or files.

*System*
The system controls permissions, validates the subscription, saves the data, and manages the inspection status.

---

## 1.3 Data clasification

### Structured data

- Companies
- Users
- Roles
- Subscriptions
- Inspection types
- Inspections

### Dynamic data

- Questions inside an inspection form
- Different types of answers
- Evidence links
- Extra notes

### Critical Data for Audit

- Who created the inspection
- Who was assigned
- Who completed it
- Dates
- Final results
- Status changes

---