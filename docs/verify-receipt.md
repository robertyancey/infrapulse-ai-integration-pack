# Receipt Verification

Every paid InfraPulse response returns a signed receipt.

## Verification steps
1. Read `kid` from the receipt
2. Fetch public keys from `/.well-known/keys`
3. Canonicalize the `payload` (sorted keys, no whitespace)
4. Verify the Ed25519 signature using the public key for that `kid`

## Trust guarantee
A valid signature proves that:
- funds were accepted
- compute executed
- InfraPulse produced the response
