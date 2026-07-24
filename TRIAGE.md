# Triage (internal)

How we run this repo. Not for reporters — this is for the team.

## The daily pass

Someone does a pass over `needs-triage` each working day:

1. **Duplicate?** Close it, label `duplicate`, link the original.
2. **Support question in the wrong place?** Point them to Support, close it.
3. **Missing detail?** Ask, label `needs-info`. Auto-close stale ones after a couple of weeks of silence.
4. **Real bug or good request?** Reproduce or accept it, then label `confirmed`. Remove `needs-triage`.
5. **From a Champion?** Add the `champion` label so we can filter their reports.

## Linear sync

The repo is connected to Linear with **GitHub Issues Sync**, pointed at the Support team.

- We gate on the `confirmed` label so the Support board only fills with triaged issues — not every raw report. (Set this in the sync config; confirm the exact behaviour when wiring it.)
- The sync is two-way: status changes and comments in Linear flow back to the GitHub thread, which is how the reporter stays informed.

## PII and security

- If someone pastes a token, key, or personal data, edit it out of the issue (or hide the comment) straight away.
- Security reports filed here by mistake: don't discuss the detail in public. Close, tell them to email security@streamelements.com, and delete the sensitive parts.
