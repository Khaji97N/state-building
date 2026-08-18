SECURITY.md – Fork‑Cooperative Security Policy
1. Purpose

The project is deliberately built as a de‑centralised, fork‑co‑operative system.
No single person (including the original author) is the exclusive point of contact for security reports.
All vulnerability disclosures are handled through trusted fork repositories that are listed in FORKS.md.
2. How to report a security issue

    Pick a trusted fork – any repository that appears in FORKS.md and carries the label security‑coordinator.
    Open an Issue in that fork using the provided template security-report.yml.
    Title format: SECURITY: <short description> (e.g. SECURITY: SQL‑injection in Legal‑Container).
    Attach proof‑of‑concept (code snippet, log, screenshot).
    If the material is sensitive, mark the issue as private (GitHub → Settings → Options → “Enable private issues for security”).
    Contact the coordinator – each fork publishes a single‑use PGP public key in COORDINATORS.md.
    Encrypt the detailed report with that key if you need confidentiality; the key never contains a personal e‑mail address.

3. Distributed response process
Step	Who does it	Time limit
Triage	At least three coordinators (situated in different legal jurisdictions)	72 hours
Verification	Coordinators reproduce the issue in a controlled environment	48 hours after triage
Patch creation	Each coordinator creates a signed commit in their own fork (GPG‑signed)	24 hours after verification
Merge	All signed patches are combined into a single PR to the main repository (GPL‑3.0‑compatible “pull‑request‑merge‑by‑consensus”)	Within 7 days of the first patch

All signed commits can be verified with the public keys listed in COORDINATORS.md.
4. GPL‑3.0 licensing and diversification

    The entire code‑base (including legal modules, AI‑horde scripts, mycelium‑network definitions, etc.) is released under GNU GPL‑v3.
    GPL‑v3 guarantees that any fork can be used independently – even if the main repository is taken down or blocked, the community can continue development.
    The licence also obliges us to keep the source open, which makes hidden back‑doors impossible to hide.

5. PGP‑key management without personal data

    One‑time keys – each coordinator generates a fresh key valid for 90 days:
    bash

    gpg --quick-generate-key "Coop‑Sec‑$(date +%Y%m%d)" ed25519 sign,encrypt 90d

    Storage – the private key is stored encrypted in the repository (keys/<hash>.asc.gpg).
    The passphrase lives only in a GitHub secret called COOP_PGP_PASSPHRASE.

    Publication – the corresponding public key is uploaded to a static URL and referenced in COORDINATORS.md.

    Automatic rotation – a GitHub Actions workflow (rotate-pgp.yml) runs every 90 days, creates a new key, commits it, and updates COORDINATORS.md.

6. Example “Contact” paragraph (no personal e‑mail)
markdown

### How to report a problem (no personal contact data)

1. Choose any verified fork from `FORKS.md` (e.g. `github.com/coop-state-building/branch-A`).  
2. Open a new Issue using the `security-report.yml` template.  
3. Attach a proof‑of‑concept. If the details are confidential, mark the Issue as **private**.  
4‑5. Coordinators from different jurisdictions will review the report within 72 hours, publish signed patches in their own forks, and a consensus PR will merge the fixes into the main repository.

7. Why this model works under repressive regimes
Threat	How the fork‑co‑operative model mitigates it
Account seizure / e‑mail blocking	No single e‑mail address is published; communication happens through public Issues and encrypted PGP messages.
Legal pressure on a single maintainer	Coordinators are spread across several countries; any one of them can continue the work if another is detained or blocked.
Complete takedown of the central repo	GPL‑3.0 ensures every fork is a full, legally independent copy; the project survives even if the “origin” disappears.
Requirement for transparency (auditors, partners)	All patches are publicly signed, all issues are traceable, and the whole process is visible on GitHub.
8. Supporting files
File	Purpose
FORKS.md	List of officially recognised forks (repo URL, country, security‑coordinator label, public PGP key URL).
COORDINATORS.md	Mapping fork → current public PGP key. Updated automatically by the rotation workflow.
.github/workflows/rotate-pgp.yml	Generates new keys every 90 days, commits them, updates COORDINATORS.md.
.github/workflows/security-scan.yml	Runs TruffleHog, CodeQL, and GPG‑signature verification on every PR.
security-report.yml (issue template)	Enforces a uniform report format (severity, affected module, PoC, impact).
Sample `FORKS.md
markdown

# Official Fork‑Cooperative Repositories

| # | Repository | Host country | `security‑coordinator` label | Public PGP key |
|---|------------|--------------|------------------------------|----------------|
| 1 | https://github.com/coop-state-building/branch-A | Estonia | ✅ | https://example.com/keys/branchA.asc |
| 2 | https://gitlab.com/coop-state-building/branch-B | Taiwan | ✅ | https://example.com/keys/branchB.asc |
| 3 | https://codeberg.org/coop-state-building/branch-C | Switzerland | ✅ | https://example.com/keys/branchC.asc |
| 4 | https://codeberg.org/coop-state-building/branch-D | Israel | ✅ | https://example.com/keys/branchD.asc |

Sample COORDINATORS.md
markdown

# Current coordinator public keys (rotated every 90 days)

- **Fork A** – `https://example.com/keys/branchA.asc`
- **Fork B** – `https://example.com/keys/branchB.asc`
- **Fork C** – `https://example.com/keys/branchC.asc`

9. Do not do these things

    Never commit plaintext private keys, passwords, or API tokens.
    Never expose a personal e‑mail address in any public file.
    Never allow direct SSH access to production nodes without a bastion host and MFA.
    Never disable automatic GPG verification of commits on the main or fork branches.
