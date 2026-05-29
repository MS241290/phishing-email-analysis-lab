Date: 29/05/2026
Analyst: Matt Stokes

# Phishing Incident Investigation Report

## Executive Summary

A phishing website was identified via PhishTank under submission ID 9437467.

The website impersonates a government parking payment service and appears designed to deceive users into submitting sensitive information.

The phishing page was confirmed as active and validated by the PhishTank community.

Risk Level: High

---

## Initial Triage

| Item | Value |
|--------|--------|
| Phish ID | 9437467 |
| URL | hxxps://www.gov-parkingqq[.]cyou/com |
| Status | Online |
| Verification | Verified Phish |
| Threat Type | Credential Harvesting / Payment Fraud |
| Analyst | Matt Stokes |

---

## Indicators of Compromise (IOCs)

### Domains

gov-parkingqq.cyou

### URLs

hxxps://www.gov-parkingqq[.]cyou/com

---

## Initial Findings

The domain attempts to impersonate a legitimate government parking payment service through the use of deceptive naming conventions.

The use of the .cyou top-level domain is unusual for legitimate government services and increases suspicion.

The phishing site was reported as active and verified by multiple PhishTank users.

## Technical Analysis

### Infrastructure Analysis

The phishing domain resolved to infrastructure hosted within the following network:

| Item | Value |
|--------|--------|
| Network Range | 43.156.0.0/18 |
| ASN | AS132203 |
| Provider | Tencent Cloud |
| Status | Active |

### Infrastructure Assessment

The phishing site was hosted on Tencent Cloud infrastructure.

No WHOIS registration information was available at the time of investigation, which limited attribution efforts.

The hosting provider information and active status indicate that the phishing site remained operational during the investigation.

## Website Accessibility

During the investigation, an attempt was made to access the phishing URL directly.

The website returned an ERR_CONNECTION_REFUSED error and was not accessible from the analysis environment.

This may indicate one of the following:

- The phishing infrastructure was taken offline after reporting.
- The hosting provider removed the content.
- The threat actor restricted access by geographic location or IP address.
- Temporary service disruption.

Although inaccessible during analysis, the phishing URL remained listed as active within PhishTank and had been verified as a valid phishing site.

### Evidence

A direct connection attempt to the phishing URL resulted in an ERR_CONNECTION_REFUSED response.

## Containment Actions

If this phishing site had been detected within a production environment, the following actions would be recommended:

1. Block the domain at DNS filtering and web proxy layers.
2. Block associated IP ranges where appropriate.
3. Search email gateways for messages containing the phishing URL.
4. Identify users who accessed the phishing site.
5. Reset credentials for affected users.
6. Review authentication logs for suspicious activity.
7. Submit indicators to security monitoring tools.
8. Notify affected users and stakeholders.
9. Report the phishing site to the hosting provider.
