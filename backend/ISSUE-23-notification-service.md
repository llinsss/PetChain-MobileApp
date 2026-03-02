# Issue #23: Create Notification Service

## Description
Build a service to handle push notifications for medication reminders, appointment alerts, and vaccination due dates.

## Requirements
- Create function to schedule medication reminders
- Create function to schedule appointment notifications
- Add vaccination reminder scheduling
- Implement notification permission handling
- Add notification cancellation logic

## File to Create
`src/services/notificationService.ts`

## Acceptance Criteria
- [ ] Medication reminders can be scheduled
- [ ] Appointment notifications work correctly
- [ ] Vaccination reminders are scheduled properly
- [ ] Permission handling is implemented
- [ ] Notifications can be cancelled

## Tech Stack
- TypeScript
- React Native Push Notifications or Expo Notifications

## Example Functions
- scheduleMedicationReminder(medication: Medication): Promise<string>
- scheduleAppointmentNotification(appointment: Appointment): Promise<string>
- scheduleVaccinationReminder(vaccination: Vaccination): Promise<string>
- cancelNotification(notificationId: string): Promise<void>
- requestPermissions(): Promise<boolean>
