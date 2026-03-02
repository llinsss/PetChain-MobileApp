# Issue #25: Create Emergency Contacts Service

## Description
Build a service to manage emergency vet contacts and nearby clinics for quick access during pet emergencies.

## Requirements
- Create function to fetch emergency contacts
- Implement nearby clinics search (by location)
- Add function to save favorite emergency contacts
- Add emergency call/navigation helpers
- Handle location permissions

## File to Create
`src/services/emergencyService.ts`

## Acceptance Criteria
- [ ] Emergency contacts can be fetched
- [ ] Nearby clinics search works with geolocation
- [ ] Favorite contacts can be saved locally
- [ ] Call and navigation helpers are implemented
- [ ] Location permissions are handled

## Tech Stack
- TypeScript
- React Native Geolocation
- AsyncStorage

## Example Functions
- getEmergencyContacts(): Promise<EmergencyContact[]>
- getNearbyVetClinics(latitude: number, longitude: number, radius: number): Promise<VetClinic[]>
- saveFavoriteContact(contact: EmergencyContact): Promise<void>
- callEmergencyContact(phoneNumber: string): void
- navigateToClinic(address: string): void
