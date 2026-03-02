# Issue #22: Create Medical Records Service

## Description
Build a service to fetch and manage pet medical records from the PetChain backend API.

## Requirements
- Create functions to fetch medical records by pet ID
- Implement filtering by record type (vaccination, treatment, diagnosis)
- Add function to fetch vaccination history
- Add function to fetch treatment history
- Handle API responses and errors

## File to Create
`src/services/medicalRecordService.ts`

## Acceptance Criteria
- [ ] All fetch functions are implemented
- [ ] Filtering by record type works correctly
- [ ] Proper error handling is in place
- [ ] Functions return typed responses
- [ ] Pagination is supported

## Tech Stack
- TypeScript
- Axios

## Example Functions
- getMedicalRecords(petId: string, filters?: RecordFilters): Promise<MedicalRecord[]>
- getVaccinationHistory(petId: string): Promise<Vaccination[]>
- getTreatmentHistory(petId: string): Promise<Treatment[]>
