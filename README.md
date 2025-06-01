Just found my first bug on a live site

Summary:
Found a public-facing [redact] page at [ www.sru.edu.in/[redact] ], leaking sensitive information such as [redact]version, stack trace and internal file structure.

Why it’s a security issue:
- Revealing [redact] version lets attackers know which exploits to use.
- Displaying file paths and stack traces exposes the server directory structure.
- Sensitive data like database queries, usernames, or tokens could also be leaked in some cases.
- This information can assist attackers in crafting targeted attacks.

Disclaimer:
This bug report does not disclose any sensitive user data or credentials.
It’s shared to raise awareness about the risks of exposing debug information on public websites.
