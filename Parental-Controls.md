# Parental-Controls
**Lab:** Windows 11 Multi-User Administration & Security Hardening  
**Section:** Child Account — Parental Controls  
**Device:** Windows 11 Pro (Device name: ELEVEN)  
**Child account:** Emma

---

## 1) Purpose
Parental controls were configured to enforce age-appropriate access, restrict unsafe content and applications, limit screen time, and require permission for purchases. These settings mimic real-world access control and policy enforcement practices for shared or restricted user environments.

---

## 2) Account Scope
- **Account type:** Child (Standard user)  
- **Management platform:** Microsoft Family Safety  
- **Admin role:** Local administrator responsible for configuration and validation  
- **Policy scope:** Settings apply across all of Emma’s activities

---

## 3) Screen Time Configuration
**Status:** Enabled  
**Scope:** Windows device (ELEVEN)

| Day        | Time Limit | Available Hours        |
|------------|------------|------------------------|
| Sunday     | 2 hours    | 07:00 AM – 08:00 PM    |
| Monday     | 1 hour     | 07:00 AM – 08:00 PM    |
| Tuesday    | 1 hour     | 07:00 AM – 08:00 PM    |
| Wednesday  | 1 hour     | 07:00 AM – 08:00 PM    |
| Thursday   | 1 hour     | 07:00 AM – 08:00 PM    |
| Friday     | 1 hour     | 07:00 AM – 08:00 PM    |
| Saturday   | 2 hours    | 07:00 AM – 08:00 PM    |

**Behavior:**  
- Device access is restricted to the defined time windows.  
- Once the daily limit is reached, further usage is blocked.

---

## 4) Content & Safety Controls

### 4.1 Age Rating
- **Setting:** Age limit for apps, games, and media  
- **Configured value:** 8

**Effect:** Filters out age-inappropriate content and media.

---

### 4.2 Web Safety
- **Setting:** Web and search filtering  
- **Configured value:** Enabled

**Details:**  
- Unsafe browsers and mature content are blocked.  
- SafeSearch is enforced on Bing.  
- Only approved browsers (e.g., Microsoft Edge) are permitted.

**Purpose:** Reduces exposure to inappropriate online content.

---

## 5) Purchase & Permission Controls

### 5.1 Ask to Buy
- **Setting:** Purchase approval  
- **Configured value:** Enabled

**Behavior:**  
- Requires organizer permission for all purchases.

**Purpose:** Prevents unauthorized purchases.

---

## 6) Activity Reporting & Notifications

### 6.1 Weekly Email Report
- **Setting:** Weekly activity summary  
- **Configured value:** Enabled

**Behavior:**  
- Weekly activity usage reports are sent to organizers and the child.

### 6.2 On-Demand Activity Email
- **Setting:** Activity reporting via email  
- **Configured value:** Enabled

---

## 7) Apps & Games Restrictions

### 7.1 Enforcement Model
Application access is restricted by explicitly blocking all applications except those that are critical for usage or explicitly permitted.

### 7.2 Allowed Applications
- **Microsoft Edge** (filtered web browsing)
- **Roblox game client** (only game permitted)

These applications are visible under “Installed apps, features, and games” with unrestricted access. Edge is permitted to support web safety and filtered browsing. Roblox is permitted for gameplay.

### 7.3 Blocked Applications
All other listed applications are explicitly set to blocked status, including but not limited to:
- Microsoft Store
- Click to Do
- Dev Home
- DTS Audio Processing
- LG Monitor App Installer
- Microsoft 365 Copilot
- Microsoft Clipchamp
- Microsoft Photos
- Microsoft Sticky Notes
- Microsoft Teams
- Microsoft To Do
- MSN Weather
- News
- Outlook for Windows
- Paint
- Phone Link
- Power Automate
- Quick Assist

**Purpose:** Only approved applications are usable; all others are blocked to reduce risk and unapproved access.

### 7.4 Application Risk Mitigation
While Roblox is permitted, the following additional controls are in place to mitigate risks:
- Age rating enforcement filters in-game content.
- Ask to Buy prevents unauthorized purchases.
- Screen time limits apply.
- Activity reporting provides usage visibility.

---

## 8) Validation / Evidence
**Screen Time:** Verified schedule reflects daily limits and availability windows.  
**Web Safety:** Confirmed Unsafe content filtering and SafeSearch enforcement.  
**Apps & Games:**  
- Roblox and Edge launch successfully under the child account.  
- All other applications show “Blocked.”  
- Microsoft Store access is blocked, preventing new installs.

**Evidence:**  
- Screenshots captured showing settings screens and blocked app statuses.

---

## 9) Issues / Notes
- Microsoft Family Safety does not expose a single “allow-only” toggle; allow-listing is achieved through explicit blocking of all other applications and usage limits.

---

## 10) Final Status
Parental controls were successfully configured to enforce age-appropriate access, content filtering, screen time limits, purchase approval, and application restrictions for the child account.

**Status:** ✅ Completed  
**Last updated:** 2026-01-05

