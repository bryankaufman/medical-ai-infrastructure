# Security Policy

## Reporting Vulnerabilities

Please report security vulnerabilities to: **bryankaufman@mac.com**

We take all security reports seriously and will respond within 48 hours.

## HIPAA Compliance

**⚠️ For Healthcare Repositories**: This software may handle Protected Health Information (PHI). All contributors must:

- Follow HIPAA Security Rule guidelines
- Never commit PHI to version control
- Use approved encryption for PHI at rest and in transit
- Report any potential PHI exposure immediately
- Complete required HIPAA training before contributing

## Supported Versions

| Version | Supported          |
| ------- | ------------------ |
| 1.x     | :white_check_mark: |
| < 1.0   | :x:                |

## Security Best Practices

### Development
- Never commit secrets, API keys, or credentials
- Use environment variables for sensitive configuration
- Review code for SQL injection, XSS, and other vulnerabilities
- Keep dependencies up to date
- Run security linters (ruff, bandit for Python)

### Data Handling
- Anonymize PHI in test fixtures
- Use approved de-identification methods
- Log only non-PHI data
- Implement audit trails for PHI access

### Infrastructure
- Use HTTPS/TLS for all network communication
- Implement proper authentication and authorization
- Apply principle of least privilege
- Regular security audits and penetration testing

## Responsible Disclosure

We request that security researchers:

1. Allow us reasonable time to investigate and fix issues before public disclosure
2. Make good faith efforts to avoid privacy violations and data destruction
3. Do not exploit vulnerabilities beyond demonstration
4. Contact us first before any public disclosure

Thank you for helping keep our projects secure!
