# Archblock Stablecoins Bug Bounty

Please contact security@archblock.com to responsibly disclose vulnerabilities.

## Assets in Scope

### Smart Contracts

- 1GBP: `eth:0x86B4dBE5D203e634a12364C0e428fa242A3FbA98`

### Websites

- *.archblock.com

## Bounty Award Ranges

|                 | Critical           | High             | Medium          | Low           |
| --------------- | ------------------ | ---------------- | --------------- | ------------- |
| Smart Contracts | 10,000-100,000 USD | 3,000-10,000 USD | 1,000-3,000 USD | 300-1,000 USD |
| Websites        | 3,000-30,000 USD   | 1,000-3,000 USD  | 300-1,000 USD   | 100-300 USD   |

In addition, we cap all bounty awards to 10% of funds directly affected.

## Severity Classification

### Smart Contracts

| Severity | Reported Vulnerability |
| -------- | ---------------------- |
| Critical | Unauthorized protocol takeover <br> Direct theft of user funds, other than unclaimed yield <br> Permanent freezing of user funds, other than unclaimed yield <br> Protocol insolvency |
| High     | Direct theft of unclaimed yield <br> Permanent freezing of unclaimed yield <br> Temporary freezing of user funds |
| Medium   | Losses due to block stuffing <br> Griefing (i.e., damage to users or protocol with no profit motive) <br> Theft of gas or unbounded gas consumption |
| Low      | Failure to deliver promised returns, without loss of value |

#### Out of Scope

The following smart contract vulnerabilities are considered out of scope:
- Theoretical exploits without a proof of concept.
- Best practice recommendations without an exploit chain demonstrating impact.
- Attacks requiring access to privileged addresses, leaked keys, or credentials, without demonstration of unauthorized privilege escalation.

### Websites

| Severity | Reported Vulnerability |
| -------- | ---------------------- |
| Critical | Arbitrary remote code execution <br> Taking down the website without DDoS <br> Direct theft of user funds <br> Exfiltration of extremely sensitive data, e.g., private keys or passwords <br> Sensitive state-modifying authenticated actions on behalf of a user, without interaction from that user <br> Subdomain takeover with an already-connected wallet <br> Modifying, substituting, or submitting transactions for an already-connected wallet |
| High     | Persistent static content injection or modification without JavaScript <br> Exfiltration of confidential user information, e.g., email address, phone number, physical address, etc. <br> Sensitive state-modifying authenticated actions on behalf of a user, with up to one click of user interaction <br> Subdomain takeover without an already-connected wallet
| Medium   | Reflected static content injection without JavaScript <br> Exfiltration of non-confidential user information, e.g., name, notification settings, etc. <br> Sensitive state-modifying authenticated actions on behalf of a user, requiring extensive or unusual user interaction <br> Non-sensitive state-modifying authenticated actions on behalf of a user, with up to one click of user interaction <br> Open redirect to malicious websites |
| Low      | Non-sensitive state-modifying authenticated actions on behalf of a user, requiring extensive or unusual user interaction <br> Taking over broken or expired outgoing links, e.g., social media handles, etc. <br> Temporarily preventing user access (except in cases of suspected abuse) |

#### Out of Scope

The following website vulnerabilities are considered out of scope:
- Theoretical attacks without an exploit chain demonstrating impact.
- Best practice recommendations without an exploit chain demonstrating impact.
- Reflected plaintext injection.
- Self-XSS without an exploit chain demonstrating impact.
- Logout CSRF (or any other non-state-modifying CSRF) without an exploit chain demonstrating impact.
- Missing HTTP Security Headers or cookie security flags without an exploit chain demonstrating impact.
- Any attacks that require the user to have first performed unprompted and unlikely actions.
- Leakage of server-side non-confidential or non-sensitive information, such as IPs, server names, or Etherscan/Infura API keys.

## Terms

### Proof of Concept Required

All vulnerability disclosures must include a full proof of concept demonstrating a non-theoretical impact.
- For smart contracts, we require submission of runnable code that can be simulated on a local fork.
- For website vulnerabilities, we require either source code for the exploit or an explicit step-by-step demonstration.

### Security Researcher Eligibility

Security researchers must undergo a KYC check (full legal name, photograph, and government-issued photo ID) before bounty award.
If paying out to a blockchain address, we may also require a digital signature to confirm that email and blockchain addresses are controlled by the same person.

We welcome vulnerability disclosures from our employees, auditors, and affiliates. However, they are not eligible for bounty award under this program.

### Known Vulnerabilities, Prior Disclosures, and Duplicates

Any vulnerabilities that have been previously reported are ineligible for award. This includes known and/or unfixed vulnerabilities from our audits and disclosures that have been first reported by others. We may determine that one disclosure is a duplicate of another, if we find that the attack vector is substantially the same or we already have a plan to fix the first.

### Prohibited Activities

The following activities are prohibited:
- Any public testing on mainnets or testnets.
- Public disclosure of a vulnerability before a fix has been deployed.
- Unauthorized whitehacking, i.e., theft of our funds _with_ the intent to return them, but _without_ prior express written agreement with us.
- Any attempts at phishing, social engineering, or physical entry, without prior express written agreement with us.
- Any execution of denial of service attacks, or any other automated testing that generates significant amounts of traffic.

### Program Modification, Severity Classification, and Award Determination

We may at our discretion modify or cancel this bug bounty program at any time, for any reason, without prior notice. The severity classification of a disclosed vulnerability, as well as the determination of its award amount, is also at our sole and absolute discretion.