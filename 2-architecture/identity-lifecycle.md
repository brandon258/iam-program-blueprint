# Identity Lifecycle Design

1. **Joiner**: HR triggers SCIM → IdP → SSO role/group assigned
2. **Mover**: Change in department → role re-evaluated
3. **Leaver**: Termination triggers deactivation → revokes sessions, access
4. **Exceptions**: Break-glass, short-term accounts (contractors)
