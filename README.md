# Arunim Shukla

![AI](https://img.shields.io/badge/AI-1F3A5F?style=flat-square)
![Security](https://img.shields.io/badge/Security-1F3A5F?style=flat-square)
![Technical PMM](https://img.shields.io/badge/Technical%20PMM-1F3A5F?style=flat-square)
![Open Source](https://img.shields.io/badge/Open%20Source-1F3A5F?style=flat-square&logo=github&logoColor=white)
![Ethereum](https://img.shields.io/badge/Ethereum-1F3A5F?style=flat-square&logo=ethereum&logoColor=white)
![Developer Tooling](https://img.shields.io/badge/Developer%20Tooling-1F3A5F?style=flat-square)
![AI Tooling](https://img.shields.io/badge/AI_Tooling-1F3A5F?style=flat-square)
![GTM Strategy](https://img.shields.io/badge/GTM_Strategy-1F3A5F?style=flat-square)

I work at the intersection of security, open source, Ethereum and AI, with a focus on technical product marketing and developer-facing products.

## Merged upstream

Fixes merged, cherry-picked or otherwise incorporated upstream by project maintainers:

| Project | Impact | Change |
| --- | --- | --- |
| [openai/codex-security #1021](https://github.com/openai/codex-security/pull/1021) | **Medium · security coverage** | Added Solidity `.sol` files to diff scan inventories and rank inputs, with red/green coverage across repository, revision and local-patch modes |
| [openai/codex-security #1020](https://github.com/openai/codex-security/pull/1020) | — | Required verification evidence before `no_change` remediation results are treated as resolved, with a regression proving evidence-free results fail closed |
| [openai/openai-guardrails-js #148](https://github.com/openai/openai-guardrails-js/pull/148) | — | Fixed vector-store uploads for supported documents inside directories whose names contain dots. Three red/green regressions, 882 tests, multi-version CI and CodeQL passed |
| [GoogleChrome/chromium-dashboard #6946](https://github.com/GoogleChrome/chromium-dashboard/pull/6946) | — | Restored the “Draft Intent to Extend Experiment” email action when API-owner gates are active across normal launch, fast-track and deprecation processes. Added a regression covering all three definitions; merged as [`ca80064`](https://github.com/GoogleChrome/chromium-dashboard/commit/ca80064d966c5f58df7c25941ebe8416d7ae9a03) and deployed in [release #6950](https://github.com/GoogleChrome/chromium-dashboard/issues/6950) |
| [promptfoo/promptfoo #11243](https://github.com/promptfoo/promptfoo/pull/11243) | — | Fixed Vertex Claude sampling resolution so explicit `top_p: 0` and `top_k: 0` values are preserved instead of being replaced or omitted. Maintainer verification covered 1,146 Google provider tests, typecheck, CLI build, formatting/lint and all 57 applicable PR checks |
| [promptfoo/modelaudit #1859](https://github.com/promptfoo/modelaudit/pull/1859) | — | Preserved native SafeTensors routing for valid FDICT-shaped headers while retaining fail-closed compression routing for unknown, inconclusive and genuine compressed inputs. Superseded by maintainer PR [#1863](https://github.com/promptfoo/modelaudit/pull/1863), merged as [`2a5185a`](https://github.com/promptfoo/modelaudit/commit/2a5185a32a3993ac6188b20a04fe6cec7cc2eddc) with my commits and co-authorship preserved |
| [ethereum/go-ethereum](https://github.com/ethereum/go-ethereum/pull/35710) | — | Corrected the `eth` RPC endpoint documentation |
| [ethereum/ethereum-org-website #19272](https://github.com/ethereum/ethereum-org-website/pull/19272) | — | Synced the Glamsterdam proposal list, removing EIP-7610 and adding eth/72 (EIP-8070), EIP-8136 and snap/2 (EIP-8189). Maintainers added me as an ethereum.org maintenance contributor in [#19364](https://github.com/ethereum/ethereum-org-website/pull/19364) |
| [google/skill-reach](https://github.com/google/skill-reach/pull/23) | — | Preserved query metadata across CSV and JSONL exchange formats |
| [nasa/delta](https://github.com/nasa/delta/pull/158) | — | Fixed cache eviction for files |
| [Samsung/CredSweeper](https://github.com/Samsung/CredSweeper/pull/951) | **Medium · scanner coverage** | Fixed CRX3 payload extraction, so credentials inside current Chrome extensions are no longer skipped |
| [ethsystems/map](https://github.com/ethsystems/map/pull/200) | — | Clarified the ERC-3643 transfer and admin paths |
| [ethsystems/web #44](https://github.com/ethsystems/web/pull/44) | — | Repaired four broken proof-of-concept and specification links across the private bonds, shielded transfers and cross-chain swap write-ups. Cherry-picked upstream in [commit `82bd4f0`](https://github.com/ethsystems/web/commit/82bd4f01ebe61dc1fec30d0b1c41de0c67ae1019), preserving my authorship |
| [ethsystems/web #45](https://github.com/ethsystems/web/pull/45) | — | Fixed glossary link handling so linked terms and definitions render correctly and root map documents resolve to their GitHub source. Cherry-picked upstream in [commit `63f99bd`](https://github.com/ethsystems/web/commit/63f99bde89cddf512f0304b9912fd25e8917ca81), preserving my authorship; 58/58 tests passed and 218 pages built |
| [Consensys/ask-o11y-plugin](https://github.com/Consensys/ask-o11y-plugin/pull/226) | — | Switched LLM requests from the deprecated `max_tokens` to `max_completion_tokens`, with tests. Shipped in v0.3.18 |
| [NethermindEth/nethermind](https://github.com/NethermindEth/nethermind/pull/13747) | — | Made `engine_newPayloadV3+` reject null or missing `withdrawals`, `blobGasUsed` and `excessBlobGas` with `-32602` instead of marking the payload `INVALID`. My fix and regression test, merged in a maintainer PR that extended the tests |
| [NethermindEth/nethermind #13755](https://github.com/NethermindEth/nethermind/pull/13755) | **Medium · protocol availability** | Fixed the Amsterdam Engine API boundary: `engine_getPayloadV5` now returns `-38005 Unsupported fork` at Amsterdam instead of dropping `slotNumber` and `blockAccessList`. Added a red/green regression and preserved Osaka V5 behaviour; merged upstream and closed [#13713](https://github.com/NethermindEth/nethermind/issues/13713) |
| [DefiLlama/peggedassets-server](https://github.com/DefiLlama/peggedassets-server/pull/927) | — | Corrected the EURR issuer attribution: Bridge Building S.A. issues it, Revolut distributes it |
| [centrifuge/api-v3](https://github.com/centrifuge/api-v3/pull/489) | — | Added the Pharos block explorer URL |
| [solana-foundation/solana-web3.js #3943](https://github.com/solana-foundation/solana-web3.js/pull/3943) | **Medium · release integrity** | Added runtime smoke tests for both IIFE browser bundles. Review surfaced a Rollup substitution bug that made the v3 bundles throw in browsers; the PR merged with the maintainer's fix |

Impact is listed only for findings with demonstrated security, scanner-integrity, protocol-availability or release-integrity consequences; ratings are evidence-based and not upstream-assigned.

Also:

- proposed the fix for a reported Claude Code startup failure in Trail of Bits' `second-opinion` plugin ([#303](https://github.com/trailofbits/skills/pull/303)). The maintainer shipped the same fix in [#306](https://github.com/trailofbits/skills/pull/306).
- EthSystems maintainers accepted and consolidated three validated web fixes ([#46](https://github.com/ethsystems/web/pull/46), [#47](https://github.com/ethsystems/web/pull/47) and [#48](https://github.com/ethsystems/web/pull/48)) in [#49](https://github.com/ethsystems/web/pull/49), preserving my commit authorship. The patches repair sibling RFP routing, restore continuation-line glossary definitions and replace a stale Custom UTXO reference; the combined suite passed 62/62 tests. GitHub records #49 as closed, with the public `main` sync pending.

## Selected work
 
[![Open Source Fix Analysis](https://github-readme-stats.vercel.app/api/pin/?username=arunimshukla&repo=open-source-fix-analysis&theme=transparent&hide_border=true)](https://github.com/arunimshukla/open-source-fix-analysis)

Plain-English case studies of verified open-source fixes, with each problem, change and proof recorded.

- [GTM-Teardowns](https://github.com/arunimshukla/GTM-Teardowns):
  public, audit-first go-to-market teardowns of target companies.
  
- [Web3 Security Library](https://github.com/immunefi-team/Web3-Security-Library)
  ![Stars](https://img.shields.io/github/stars/immunefi-team/Web3-Security-Library?style=flat-square&label=stars&color=1F3A5F):
  Immunefi's library of Web3 security tutorials and tools. Second-largest contributor while at Immunefi
  
  ([commits](https://github.com/immunefi-team/Web3-Security-Library/commits?author=Arunim-Immunefi)).
- [Best-DeFi-Security-Practices](https://github.com/arunimshukla/Best-DeFi-Security-Practices)
  ![Stars](https://img.shields.io/github/stars/arunimshukla/Best-DeFi-Security-Practices?style=flat-square&label=stars&color=1F3A5F):
  a reference list of security practices for DeFi protocols.

## 📊 GitHub Stats

<p>
  <img src="https://github-readme-stats.vercel.app/api?username=arunimshukla&show_icons=true&theme=transparent&hide_border=true&rank_icon=github" height="165" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=arunimshukla&theme=transparent&hide_border=true" height="165" />
</p>

<p>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=arunimshukla&layout=compact&theme=transparent&hide_border=true" height="165" />
</p>

## 🚀 Current Focus

- Open-source contributions across Ethereum, security and developer tooling
- Finding and fixing high-impact technical issues
- Building visible proof of work through code, audits and documentation

## 🛠 Tech

![Python](https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-121011?style=for-the-badge&logo=github&logoColor=white)
![Ethereum](https://img.shields.io/badge/Ethereum-3C3C3D?style=for-the-badge&logo=ethereum&logoColor=white)
![Solidity](https://img.shields.io/badge/Solidity-363636?style=for-the-badge&logo=solidity&logoColor=white)

## Recent validated contributions

Submitted upstream changes backed by reproducible regression evidence and broader checks. These pull requests are open for maintainer review; they are not presented as merged or accepted.

| Project | Change | Status |
| --- | --- | --- |
| [NethermindEth/nethermind #14228](https://github.com/NethermindEth/nethermind/pull/14228) | Fixed acceptance of cached JWTs after explicit `exp`, with expiration-boundary regressions for both parser paths | ![state](https://img.shields.io/github/pulls/detail/state/NethermindEth/nethermind/14228?style=flat-square&label=) Changes requested |
| [promptfoo/mcp-agent-provider #95](https://github.com/promptfoo/mcp-agent-provider/pull/95) | Replaced message-count token estimates and hard-coded cost with measured OpenAI usage aggregated across ReAct iterations; Node 20/22/24 and Biome CI pass | ![state](https://img.shields.io/github/pulls/detail/state/promptfoo/mcp-agent-provider/95?style=flat-square&label=) |
| [promptfoo/mcp-agent-provider #96](https://github.com/promptfoo/mcp-agent-provider/pull/96) | Fixed Streamable HTTP → legacy SSE fallback so compatibility retry happens after connection negotiation, with an end-to-end SSE server regression; Node 20/22/24 and Biome CI pass | ![state](https://img.shields.io/github/pulls/detail/state/promptfoo/mcp-agent-provider/96?style=flat-square&label=) |
| [NethermindEth/pluto #714](https://github.com/NethermindEth/pluto/pull/714) | Kept tracing topic labels visible to metrics at the default `info` log level, with an integration regression | ![state](https://img.shields.io/github/pulls/detail/state/NethermindEth/pluto/714?style=flat-square&label=) |
| [NethermindEth/pluto #715](https://github.com/NethermindEth/pluto/pull/715) | Stopped ignored OTLP header values from leaking into WARN logs; the warning now records only the header count | ![state](https://img.shields.io/github/pulls/detail/state/NethermindEth/pluto/715?style=flat-square&label=) |
| [solana-foundation/solana-com](https://github.com/solana-foundation/solana-com/pull/2150) | Slot-time block requests now accept v1 transactions | ![state](https://img.shields.io/github/pulls/detail/state/solana-foundation/solana-com/2150?style=flat-square&label=) Awaiting review |

<!-- Move an entry to "Merged upstream" only when GitHub records a merge or a maintainer provides a verifiable upstream commit incorporating the change.
Move human-reviewed open work to "In review"; remove entries closed without acceptance. -->

## Numbers behind the work

| Area | Result |
| --- | --- |
| Security research | H1 2026 Digital Asset Security Review: 100+ incidents, $850M in losses |
| Exploit forensics | $287M+ in losses reconstructed |
| Organic reach | 2M+ impressions in 90 days, zero paid spend |
| Community | 2,300+ member security community |
| Disclosures | Acknowledged by the DoD (DARPA, Air Force, Navy), Toyota and Philips |
| Category | Created W3SPM (Web3 Security Posture Management) |

## Contact

[LinkedIn](https://www.linkedin.com/in/arunimshukla) or
[Twitter (X)](https://x.com/arunim_shukla)
