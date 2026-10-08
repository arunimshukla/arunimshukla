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
| [blackrock/HOLA #69](https://github.com/blackrock/HOLA/pull/69) | — | Corrected the documented Forrester benchmark so the README and getting-started examples match the repository implementation and reproduce the stated minimum. Added a regression comparing both documented objectives against the benchmark at five inputs; all 10 numerical comparisons fail before the fix and pass within `1e-12` after. Merged upstream as [`55647c9`](https://github.com/blackrock/HOLA/commit/55647c9350fc235a39663820a3c9e12027246dfe) |
| [openai/codex-security #1306](https://github.com/openai/codex-security/pull/1306) | **Medium · security coverage** | Added Vyper `.vy` sources to scan inventories and ranking paths so Vyper-only changes are not omitted before review-item generation. OpenAI maintainer independently verified all five new inventory/ranking regressions fail on the parent and pass with the fix; 295 affected-module tests passed with no blocking behaviour issues. Merged upstream as [`d327164`](https://github.com/openai/codex-security/commit/d32716411f3d7b87085b36f9de55f0ac40454c42) |
| [openai/codex-security #1021](https://github.com/openai/codex-security/pull/1021) | **Medium · security coverage** | Added Solidity `.sol` files to diff scan inventories and rank inputs, with red/green coverage across repository, revision and local-patch modes |
| [openai/codex-security #1020](https://github.com/openai/codex-security/pull/1020) | — | Required verification evidence before `no_change` remediation results are treated as resolved, with a regression proving evidence-free results fail closed |
| [openai/openai-guardrails-js #148](https://github.com/openai/openai-guardrails-js/pull/148) | — | Fixed vector-store uploads for supported documents inside directories whose names contain dots. Three red/green regressions, 882 tests, multi-version CI and CodeQL passed |
| [GoogleChrome/chromium-dashboard #6946](https://github.com/GoogleChrome/chromium-dashboard/pull/6946) | — | Restored the “Draft Intent to Extend Experiment” email action when API-owner gates are active across normal launch, fast-track and deprecation processes. Added a regression covering all three definitions; merged as [`ca80064`](https://github.com/GoogleChrome/chromium-dashboard/commit/ca80064d966c5f58df7c25941ebe8416d7ae9a03) and deployed in [release #6950](https://github.com/GoogleChrome/chromium-dashboard/issues/6950) |
| [promptfoo/mcp-agent-provider #95](https://github.com/promptfoo/mcp-agent-provider/pull/95) | — | Replaced message-count token estimates with measured OpenAI usage aggregated across ReAct iterations, omitted incomplete usage totals and removed fabricated cost estimates. Maintainer-approved with real-SDK loopback regressions for measured, zero and missing usage; 31 tests, lint and Node 20/22/24 CI passed. Merged upstream as [`6478386`](https://github.com/promptfoo/mcp-agent-provider/commit/6478386ffb7207ab832d0e0849695213e09bef71) |
| [promptfoo/promptfoo #11243](https://github.com/promptfoo/promptfoo/pull/11243) | — | Fixed Vertex Claude sampling resolution so explicit `top_p: 0` and `top_k: 0` values are preserved instead of being replaced or omitted. Maintainer verification covered 1,146 Google provider tests, typecheck, CLI build, formatting/lint and all 57 applicable PR checks |
| [promptfoo/modelaudit #1859](https://github.com/promptfoo/modelaudit/pull/1859) | — | Preserved native SafeTensors routing for valid FDICT-shaped headers while retaining fail-closed compression routing for unknown, inconclusive and genuine compressed inputs. Superseded by maintainer PR [#1863](https://github.com/promptfoo/modelaudit/pull/1863), merged as [`2a5185a`](https://github.com/promptfoo/modelaudit/commit/2a5185a32a3993ac6188b20a04fe6cec7cc2eddc) with my commits and co-authorship preserved |
| [ethereum/go-ethereum](https://github.com/ethereum/go-ethereum/pull/35710) | — | Corrected the `eth` RPC endpoint documentation |
| [ethereum/ethereum-org-website #19272](https://github.com/ethereum/ethereum-org-website/pull/19272) | — | Synced the Glamsterdam proposal list, removing EIP-7610 and adding eth/72 (EIP-8070), EIP-8136 and snap/2 (EIP-8189). Shipped to production in [ethereum.org v11.29.0 / #19406](https://github.com/ethereum/ethereum-org-website/pull/19406), where I was credited in the release contributors list. Maintainers also added me as an ethereum.org maintenance contributor in [#19364](https://github.com/ethereum/ethereum-org-website/pull/19364) |
| [ethereum/ethereum-org-website #19368](https://github.com/ethereum/ethereum-org-website/pull/19368) | — | Repaired contributor onboarding in the repository README: replaced two dead links, corrected build-locale setup to use `.env.local`, added the missing staging step before commit, and fixed first-push instructions with `git push -u origin HEAD`. Reproduced each failure path before the fix; approved by a maintainer and merged upstream as [`efb29af`](https://github.com/ethereum/ethereum-org-website/commit/efb29af97f47ab076c52bcb3771dd5facafdc377) |
| [ethereum/ethereum-org-website #19409](https://github.com/ethereum/ethereum-org-website/pull/19409) | **Medium · data availability** | Prevented a transient failure in one Google Sheets app category from overwriting the last good cached catalog with an empty category. Added a regression that returns `503 Service Unavailable` for one category and proves the fetch fails closed instead of persisting partial data; upstream CI passed |
| [google/skill-reach](https://github.com/google/skill-reach/pull/23) | — | Preserved query metadata across CSV and JSONL exchange formats |
| [nasa/delta](https://github.com/nasa/delta/pull/158) | — | Fixed cache eviction for files |
| [Samsung/CredSweeper](https://github.com/Samsung/CredSweeper/pull/951) | **Medium · scanner coverage** | Fixed CRX3 payload extraction, so credentials inside current Chrome extensions are no longer skipped |
| [ethsystems/map](https://github.com/ethsystems/map/pull/200) | — | Clarified the ERC-3643 transfer and admin paths |
| [ethsystems/web #44](https://github.com/ethsystems/web/pull/44) | — | Repaired four broken proof-of-concept and specification links across the private bonds, shielded transfers and cross-chain swap write-ups. Cherry-picked upstream in [commit `82bd4f0`](https://github.com/ethsystems/web/commit/82bd4f01ebe61dc1fec30d0b1c41de0c67ae1019), preserving my authorship |
| [ethsystems/web #45](https://github.com/ethsystems/web/pull/45) | — | Fixed glossary link handling so linked terms and definitions render correctly and root map documents resolve to their GitHub source. Cherry-picked upstream in [commit `63f99bd`](https://github.com/ethsystems/web/commit/63f99bde89cddf512f0304b9912fd25e8917ca81), preserving my authorship; 58/58 tests passed and 218 pages built |
| [ethsystems/web #46](https://github.com/ethsystems/web/pull/46) | — | Fixed sibling RFP link routing so bare RFP Markdown links resolve to `/rfps/...` routes instead of unrelated graph routes. Incorporated upstream in [commit `3330621`](https://github.com/ethsystems/web/commit/3330621002207df1135787d66eb93c25792c773b), with my contribution and authorship explicitly credited |
| [ethsystems/web #47](https://github.com/ethsystems/web/pull/47) | — | Restored glossary definitions written on continuation lines without swallowing the next term or category, with regression coverage. Incorporated upstream in [commit `3330621`](https://github.com/ethsystems/web/commit/3330621002207df1135787d66eb93c25792c773b), with my contribution and authorship explicitly credited |
| [ethsystems/web #48](https://github.com/ethsystems/web/pull/48) | — | Replaced the retired Custom UTXO reference in Private Bonds Part 3 with the maintained Shielding pattern and added the corresponding map reference. Incorporated upstream in [commit `3330621`](https://github.com/ethsystems/web/commit/3330621002207df1135787d66eb93c25792c773b), with my contribution and authorship explicitly credited; combined suite passed 62/62 tests |
| [Consensys/ask-o11y-plugin](https://github.com/Consensys/ask-o11y-plugin/pull/226) | — | Switched LLM requests from the deprecated `max_tokens` to `max_completion_tokens`, with tests. Shipped in v0.3.18 |
| [NethermindEth/nethermind](https://github.com/NethermindEth/nethermind/pull/13747) | — | Made `engine_newPayloadV3+` reject null or missing `withdrawals`, `blobGasUsed` and `excessBlobGas` with `-32602` instead of marking the payload `INVALID`. My fix and regression test, merged in a maintainer PR that extended the tests |
| [NethermindEth/nethermind #13755](https://github.com/NethermindEth/nethermind/pull/13755) | **Medium · protocol availability** | Fixed the Amsterdam Engine API boundary: `engine_getPayloadV5` now returns `-38005 Unsupported fork` at Amsterdam instead of dropping `slotNumber` and `blockAccessList`. Added a red/green regression and preserved Osaka V5 behaviour; merged upstream and closed [#13713](https://github.com/NethermindEth/nethermind/issues/13713) |
| [NethermindEth/nethermind #14228](https://github.com/NethermindEth/nethermind/pull/14228) | **Medium · authentication integrity** | Fixed JWT cache reuse accepting correctly signed tokens after their explicit `exp`. Cached authentication now enforces the same expiration boundary as fresh validation while preserving the fast path, with regressions across both validation paths; merged upstream as [`eeca264`](https://github.com/NethermindEth/nethermind/commit/eeca26403bef8420a980ebde700c9e338caa75e8) |
| [NethermindEth/nethermind #14338](https://github.com/NethermindEth/nethermind/pull/14338) | — | Corrected published Docker image metadata so Nethermind advertises P2P discovery on `30303/udp` as well as `30303/tcp`. Extended the image metadata regression check; the validation build confirmed both standard and chiseled images expose both protocols |
| [NethermindEth/dotnet-riscv #18](https://github.com/NethermindEth/dotnet-riscv/pull/18) | — | Repaired the README's Stateless Executor reference after the old feature branch was deleted, pointing the RISC-V build pipeline to the current `Nethermind.Stateless.Executor` location on `master`. Validated that the old URL returned 404 and the replacement resolves; approved and merged upstream as [`41038a0`](https://github.com/NethermindEth/dotnet-riscv/commit/41038a063eecd9c6998917c7be0b1170c08d829d) |
| [DefiLlama/peggedassets-server](https://github.com/DefiLlama/peggedassets-server/pull/927) | — | Corrected the EURR issuer attribution: Bridge Building S.A. issues it, Revolut distributes it |
| [centrifuge/api-v3](https://github.com/centrifuge/api-v3/pull/489) | — | Added the Pharos block explorer URL |
| [0xPolygon/polygon-agent-cli #142](https://github.com/0xPolygon/polygon-agent-cli/pull/142) | **Medium · transaction safety** | Fixed `x402-pay` bypassing the CLI's dry-run mode and unconditionally broadcasting funding transactions. Integrated shared `--broadcast` / `--dry-run` flags and persisted transaction mode, added structured payment previews, and covered both standard x402 and Bazaar flows with regressions proving no funds are sent during dry runs. Fixes [#130](https://github.com/0xPolygon/polygon-agent-cli/issues/130); merged upstream as [`b3e81d0`](https://github.com/0xPolygon/polygon-agent-cli/commit/b3e81d0fa64b95a5c83f0a1073ee9ea30ec2b6d8) |
| [solana-foundation/solana-web3.js #3943](https://github.com/solana-foundation/solana-web3.js/pull/3943) | **Medium · release integrity** | Added runtime smoke tests for both IIFE browser bundles. Review surfaced a Rollup substitution bug that made the v3 bundles throw in browsers; the PR merged with the maintainer's fix |
| [solana-foundation/solana-com #2150](https://github.com/solana-foundation/solana-com/pull/2150) | **Medium · data freshness** | Fixed slot-time block requests rejecting newer blocks containing Solana v1 transactions, which could leave the endpoint serving cached blocks minutes old despite a four-second refresh target ([#2141](https://github.com/solana-foundation/solana-com/issues/2141)). Raised `maxSupportedTransactionVersion` to `1`, with regression tests for the exact JSON-RPC request and program ID resolution using static and loaded address-table keys. Approved and merged upstream as [`a233795`](https://github.com/solana-foundation/solana-com/commit/a233795827fb9ff3581a3f915c7ccc518c1a7b88) |

Impact is listed only for findings with demonstrated security, scanner-integrity, protocol-availability, data-availability or release-integrity consequences; ratings are evidence-based and not upstream-assigned.

Also:

- proposed the fix for a reported Claude Code startup failure in Trail of Bits' `second-opinion` plugin ([#303](https://github.com/trailofbits/skills/pull/303)). The maintainer shipped the same fix in [#306](https://github.com/trailofbits/skills/pull/306).

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

Submitted upstream changes backed by reproducible regression evidence and broader checks. Entries stay here until merged; maintainer-approved work is labelled explicitly and is not presented as merged.

| Project | Change | Status |
| --- | --- | --- |
| [NethermindEth/nethermind #14372](https://github.com/NethermindEth/nethermind/pull/14372) | Normalised malformed receipt post-state lengths to `RlpException` instead of a generic `ArgumentException`, keeping invalid peer input on the standard RLP deserialisation path. Locally reproduced; regressions cover 5, 31, 33 and 34-byte first items across both receipt decoder variants | ![state](https://img.shields.io/github/pulls/detail/state/NethermindEth/nethermind/14372?style=flat-square&label=) |
| [promptfoo/mcp-agent-provider #96](https://github.com/promptfoo/mcp-agent-provider/pull/96) | Fixed Streamable HTTP → legacy SSE fallback so compatibility retry happens after connection negotiation, with an end-to-end SSE server regression; Node 20/22/24 and Biome CI pass | ![state](https://img.shields.io/github/pulls/detail/state/promptfoo/mcp-agent-provider/96?style=flat-square&label=) |
| [NethermindEth/pluto #714](https://github.com/NethermindEth/pluto/pull/714) | Kept tracing topic labels visible to metrics at the default `info` log level, with an integration regression | ![state](https://img.shields.io/github/pulls/detail/state/NethermindEth/pluto/714?style=flat-square&label=) |
| [NethermindEth/pluto #715](https://github.com/NethermindEth/pluto/pull/715) | Stopped ignored OTLP header values from leaking into WARN logs; the warning now records only the header count | ![state](https://img.shields.io/github/pulls/detail/state/NethermindEth/pluto/715?style=flat-square&label=) |

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
