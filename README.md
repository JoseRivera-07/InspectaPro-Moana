# InspectaPro-Moana
# 6. Architecture Justification

**Responsible:** Jose  

---

## 6.1 Data in SQL

### Data Stored in SQL and Why

The relational database stores **structured and stable business data**, including:

- Companies  
- Users  
- Roles  
- Inspection types  
- Inspections  
- Subscriptions  

These entities require:

- Strong consistency  
- Integrity constraints  
- Clear relationships  

These are core strengths of **relational databases**.

---

## 6.2 Data in NoSQL

### Data Stored in NoSQL and Why

The NoSQL database stores **dynamic inspection response data** because:

- Forms may change over time  
- Questions vary between inspection types  
- Responses can have multiple formats  
- Flexibility is required to add new fields without schema changes  

This model allows high adaptability without modifying the database schema.

---

## 6.3 Risks of a Fully Relational Model

Using only a relational database would introduce:

- Frequent schema modifications  
- High maintenance complexity  
- Difficulty handling variable forms  
- Limited adaptability to evolving business requirements  
- Challenges in preserving historical form versions  

---

## 6.4 Risks of a Fully Document-Based Model

Using only a document database would introduce:

- Lack of strict referential integrity  
- Difficulty managing structured business relationships  
- Potential data duplication  
- More complex transactional consistency  

---

## 6.5 Integration Between SQL and NoSQL

Both databases are connected through the inspection identifier:

`inspection_id`

This identifier links:

- Structured inspection records stored in **SQL**
- Dynamic inspection responses stored in **NoSQL**

### Hybrid Architecture Model

- **Relational database →** Manages core business structure  
- **Document database →** Manages flexible inspection content  