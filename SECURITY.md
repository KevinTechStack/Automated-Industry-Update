# Security Policy

## Supported Versions

| Version | Supported |
|---|---|
| Latest | ✅ Yes |
| Older | ❌ No |

---

## Reporting a Vulnerability

If you find a security issue:

1. Do NOT open a public GitHub issue
2. Message the repository owner privately via GitHub
3. Describe the vulnerability and steps to reproduce
4. Allow reasonable time for response before public disclosure

---

## Security Notes for Users

### API Keys — Critical
- Never commit API keys to your repository
- Store all keys as n8n credentials only
- Keys to keep private:
  - NewsAPI key
  - Groq API key
  - Gmail OAuth Client ID and Client Secret

### Before Sharing workflow.json
- Open the file and verify no API keys are embedded
- n8n credentials are stored separately and should not appear in the export
- Check all HTTP Request nodes for hardcoded keys in query parameters

### Self-Hosted n8n
- Do not expose port 5678 to the public internet
- Use a strong password for your n8n account
- Keep the n8n Docker image updated regularly

---

## What This Project Does NOT Store

- No personal data of any kind
- No article content beyond in-memory processing during each run
- No information outside the configured Gmail delivery

---

*Last updated: March 2026*
