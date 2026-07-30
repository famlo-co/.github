# Security Policy

Famlo handles family data — including information about children — and processes
payments on behalf of the organizations that use us. We take reports seriously
and we will not take legal action against anyone who reports in good faith under
this policy.

## Reporting a vulnerability

Email **support@famlo.co** with `SECURITY` in the subject line, and include:

- What you found and where (URL, endpoint, or affected feature)
- The steps to reproduce it
- What an attacker could do with it
- Anything else that helps us reproduce — request/response pairs, screenshots, a
  short video

Please report privately. Do not open a public GitHub issue for a security
vulnerability, and please give us a chance to fix it before disclosing publicly.

If you would prefer an encrypted channel, say so in your first email and we will
arrange one.

## What to expect from us

| | |
|---|---|
| Acknowledgement of your report | within **3 business days** |
| Initial assessment and severity triage | within **10 business days** |
| Status updates while we work | at least every **10 business days** |
| Credit in our disclosure notes | on request, once fixed |

We will tell you when the issue is resolved, and we are happy to coordinate
timing on any public write-up you want to publish.

## Scope

**In scope**

- `famlo.co` and its subdomains
- `help.famlo.co`
- Our public GitHub repositories under [`famlo-co`](https://github.com/famlo-co)

**Out of scope**

- Denial-of-service, volumetric, or stress testing of any kind
- Social engineering, phishing, or physical attacks against our team, our users,
  or our vendors
- Automated scanner output submitted without a demonstrated, reproducible impact
- Reports that depend on a severely outdated browser or on an already-compromised
  device
- Missing security headers, cookie flags, or TLS configuration nits with no
  demonstrated exploit path
- Findings in third-party services we use (Stripe, AWS, and similar) — please
  report those to the vendor directly

## Testing guidelines

When investigating, please:

- **Use your own test accounts.** Do not access, modify, or retain data
  belonging to any other family, child, or organization.
- **Stop as soon as you have confirmed the issue.** Once you can demonstrate
  access, do not go further into the data.
- **Never exfiltrate data.** If you encounter personal information — especially
  anything about a minor — stop immediately, do not download or keep it, and
  tell us what you saw in your report.
- Do not degrade service for real users.

Testing that stays within these guidelines is authorized, and we consider it
good-faith research.

## Our own practices

- Payments are processed by [Stripe](https://stripe.com); we do not store card
  numbers on our infrastructure.
- Data is encrypted in transit and at rest.
- Access to production data is limited to the people who need it and is logged.
- Dependencies are monitored and patched on an ongoing basis.

---

Not a security issue? For product questions, billing, or account help, reach the
same team at [support@famlo.co](mailto:support@famlo.co) — no subject prefix
needed — or browse the [Help Center](https://help.famlo.co).
