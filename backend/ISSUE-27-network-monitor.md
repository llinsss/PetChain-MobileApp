# Issue #27: Create Network Status Monitor

## Description
Build a utility to monitor network connectivity and trigger data sync when the app comes online.

## Requirements
- Create network status listener
- Implement online/offline state management
- Add automatic sync trigger when online
- Create network quality detection
- Handle network state changes gracefully

## File to Create
`src/utils/networkMonitor.ts`

## Acceptance Criteria
- [ ] Network status is accurately detected
- [ ] Online/offline events are handled
- [ ] Sync is triggered automatically when online
- [ ] Network quality is detected (WiFi vs cellular)
- [ ] State changes are handled smoothly

## Tech Stack
- TypeScript
- React Native NetInfo

## Example Functions
- startNetworkMonitoring(): void
- stopNetworkMonitoring(): void
- isOnline(): Promise<boolean>
- getNetworkType(): Promise<NetworkType>
- onNetworkChange(callback: (isOnline: boolean) => void): void
