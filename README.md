# lab-001-windows11-local-user-admin-security-baseline

This lab establishes a secure, predictable Windows 11 baseline intended to
mirror entry-level government and contractor workstation configurations.

## What This Lab Is
A practical Windows 11 Pro lab that simulates real Tier 1 IT support and entry-level security tasks.  
The lab focuses on configuring local user accounts, enforcing least privilege, and basic auditing.  
All actions are documented as internal IT notes rather than a tutorial.

## Environment
- **Operating System:** Windows 11 Pro
- **System Type:** Standalone local system (no domain)
- **Accounts Configured:**
  - Local Administrator account
  - Standard User account
  - Child / Restricted User account
- **Tools Used:**
  - Local Users and Groups
  - Local Security Policy (`secpol.msc`)
  - Event Viewer
  - Chris Titus Tech Utility (CTT)  
  Used to apply a controlled, Standard Windows configuration baseline.
  Aggressive debloating and service hardening were intentionally avoided
  to preserve lab stability, logging, and security controls.

## Repository Structure

- README.md — Lab overview, scope, and security concepts
- Lab-Objective.md — Purpose and framing of the lab
- Account-Setup.md — Account creation and administrator actions
- Local-Security-Policy.md — Password, lockout, and auditing policy configuration
- Permission-Testing.md — Validation of access controls across user roles
- Parental-Controls.md — Child account restrictions and testing
- Lessons-Learned.md — Reflections and takeaways from the lab
- evidence/ — Supporting screenshots for security policy configuration


## Skills Demonstrated
- Local user account creation and management
- Role-based access control using local accounts
- Enforcement of least privilege
- Permission testing across multiple user roles
- Enabling and verifying security auditing
- Clear, structured technical documentation

## Baseline Reference (CTT Standard)

The following screenshots document the CTT Standard configuration used as the
baseline for this lab.

This baseline:
- Reduces consumer features and telemetry
- Preserves Windows Update, Microsoft Defender, logging, and IPv6
- Avoids aggressive service hardening or debloating
- Maintains compatibility with certification labs and GovTech environments

![CTT Standard Baseline](screenshots/ctt-standard-baseline.png)
![CTT Tweaks Applied](screenshots/ctt-tweaks-standard.png)

## Validation and Final State

After applying the CTT Standard baseline, the system was validated to confirm
enterprise and lab compatibility.

Validation performed:
- Windows Update completed successfully post-hardening
- System rebooted without errors
- Microsoft Defender remained enabled and operational
- Core Windows services and logging preserved
- No aggressive service modifications applied

![Windows Update Complete](screenshots/windows-update-complete.png)


## Security Concepts Applied
- Least Privilege
- Account Separation
- Auditing and Accountability
- Basic Incident Response Readiness

This lab intentionally focuses on local account administration and security controls and does not include Active Directory, Group Policy, or enterprise tooling.

Note: This lab intentionally excludes Active Directory, Group Policy, and Entra ID to maintain focus on local endpoint security fundamentals.


