# Arunim Shukla

**GTM audits · Upstream fixes · Tools I built**

I audit public claims, reproduce software failures, and turn the evidence into clearer product stories and fixes that others can verify.

## GTM audits

I trace product and customer claims back to the evidence a buyer can check. In my SquadStack review, the canonical facts file gave a customer a 200% reduction in acquisition cost. The case study reported 70%. [Read the finding](https://github.com/arunimshukla/GTM-Teardowns/blob/194837a5a0a30e4f53251d49db45735b1905b173/SquadStack.ai.md#1-the-canonical-facts-file-disagrees-with-the-case-studies) · [Browse GTM Teardowns](https://github.com/arunimshukla/GTM-Teardowns)

<a name="merged-upstream"></a>

## Upstream fixes

In [Sourcify](https://github.com/argotorg/sourcify), repeated requests after a completed no-match similarity verification launched redundant bytecode fetches, searches and jobs. I added a configurable cooldown that rejects immediate retries with HTTP `429` and `Retry-After`, backed by persisted job history and regression tests. The PR reports 38 passing focused tests, including 13 new cases. [Merged PR #3002](https://github.com/argotorg/sourcify/pull/3002).

In BlobKit, direct EIP-7594 blob submissions required a custom signing method that standard ethers wallets lack. I added support for standard ethers wallets, preserved the existing custom signer flow, and added three tests covering both signer types and the error for unsupported signers. [Merged PR #116](https://github.com/ETHCF/blobkit/pull/116).

In Microsoft's [Web Dev for Beginners banking API](https://github.com/microsoft/Web-Dev-For-Beginners/pull/1927), deleting a transaction removed the ledger entry but left the account balance unchanged. I fixed the reconciliation bug, made the Express app importable for testing, and added an HTTP regression test covering the create-delete cycle. [Merged PR #1927](https://github.com/microsoft/Web-Dev-For-Beginners/pull/1927).

In OSS Verify, I found that indirect library inputs could bypass allocation instrumentation and repeated lock files could hide conflicting binary hashes. Maintainers reproduced 16 failing regression cases on the original code and carried my changes into [PR #13](https://github.com/theorem-labs/oss-verify/pull/13). [Read the fix analyses](https://github.com/arunimshukla/open-source-fix-analysis) · [Full upstream record](UPSTREAM.md#merged-upstream)

## Tools I built

The AI Security Job Alert Agent checks first-party ATS boards and remote job feeds every 15 minutes. It filters for eligible roles and deduplicates listings before sending email. The repository includes a reusable configuration and tests for the watcher and dispatcher. [Explore the job alert agent](https://github.com/arunimshukla/ai-security-job-alert-agent)

## Contact

[LinkedIn](https://www.linkedin.com/in/arunimshukla) or
[Twitter (X)](https://x.com/arunim_shukla)
