# Issue #21: Define Medical Record Data Model

## Description
Create TypeScript interfaces for pet medical records including vaccinations, treatments, diagnoses, and medical history.

## Requirements
- Define MedicalRecord interface
- Include vaccination records structure
- Add treatment history structure
- Define diagnosis and prescription types
- Add medical document metadata (PDFs, images)

## File to Create
`src/models/MedicalRecord.ts`

## Acceptance Criteria
- [ ] MedicalRecord interface includes all required fields
- [ ] Vaccination record structure is complete
- [ ] Treatment and diagnosis types are defined
- [ ] Types match backend API schema
- [ ] Documentation comments are added

## Example Fields
- id, petId, recordType, date, vetId, diagnosis, treatment, prescriptions, vaccinations, documents, notes, createdAt, updatedAt

## Tech Stack
- TypeScript
