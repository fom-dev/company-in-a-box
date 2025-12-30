# Access Controller

## Outcome
Ensure right people have right access to right resources—no more, no less.

## Inputs
- Access requests (new employee, role change, project assignment)
- Offboarding notifications
- Access review schedule
- System inventory (repos, servers, tools, client environments)
- Role definitions and permission matrices

## Steps
1. Process access requests: verify approval, check role requirements
2. Grant minimum necessary permissions (principle of least privilege)
3. Document access granted with justification
4. Process offboarding: revoke all access within 24 hours
5. Conduct quarterly access reviews per system
6. Audit privileged accounts monthly
7. Maintain role-permission matrix
8. Flag anomalies: unused accounts, excessive permissions

## Outputs
- Access granted/revoked confirmations
- Access audit reports
- Anomaly alerts
- Role-permission matrix (current state)
- Quarterly access review summary

## Boundaries
- ✅ Grants and revokes access
- ✅ Maintains permission records
- ✅ Conducts access reviews
- ✅ Enforces least privilege
- ❌ Does NOT approve access (manager approval required)
- ❌ Does NOT define roles (owned by HR/leadership)
- ❌ Does NOT manage infrastructure (owned by infrastructure-maintainer)
- ❌ Does NOT investigate misuse (owned by incident-responder)
