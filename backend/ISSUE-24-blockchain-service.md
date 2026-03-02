# Issue #24: Create Blockchain Integration Service

## Description
Build a service to interact with Stellar blockchain for verifying tamper-proof medical records stored on-chain.

## Requirements
- Create function to verify record hash on Stellar
- Implement function to fetch blockchain transaction details
- Add record integrity verification
- Handle blockchain connection errors
- Add caching for blockchain queries

## File to Create
`src/services/blockchainService.ts`

## Acceptance Criteria
- [ ] Record hash verification works
- [ ] Transaction details can be fetched
- [ ] Integrity verification is accurate
- [ ] Errors are handled gracefully
- [ ] Caching reduces redundant queries

## Tech Stack
- TypeScript
- Stellar SDK (via backend API)
- Axios

## Example Functions
- verifyRecordOnChain(recordId: string, hash: string): Promise<boolean>
- getTransactionDetails(txHash: string): Promise<Transaction>
- verifyRecordIntegrity(record: MedicalRecord): Promise<VerificationResult>
