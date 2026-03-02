# Issue #26: Create Offline Cache Manager

## Description
Build a cache manager to handle offline data storage and retrieval for pet records, ensuring the app works without internet.

## Requirements
- Create cache storage functions for pet data
- Implement cache expiration logic
- Add cache invalidation on data updates
- Create cache size management
- Handle cache conflicts during sync

## File to Create
`src/services/cacheManager.ts`

## Acceptance Criteria
- [ ] Pet data can be cached locally
- [ ] Cache expiration works correctly
- [ ] Cache is invalidated on updates
- [ ] Cache size is managed (prevent overflow)
- [ ] Conflicts are resolved during sync

## Tech Stack
- TypeScript
- AsyncStorage or SQLite

## Example Functions
- cacheData<T>(key: string, data: T, ttl?: number): Promise<void>
- getCachedData<T>(key: string): Promise<T | null>
- invalidateCache(key: string): Promise<void>
- clearExpiredCache(): Promise<void>
- getCacheSize(): Promise<number>
