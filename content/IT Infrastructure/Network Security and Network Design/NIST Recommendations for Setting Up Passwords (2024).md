---
tags:
- inti
- topic
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Network Security and Network Design]]"
---

# NIST Recommendations for Setting Up Passwords (2024)

To enhance security in password management, the National Institute of Standards and Technology (NIST) provides updated guidelines:

- For user-generated passwords, aim for a minimum of 8 characters; machine-generated passwords should have at least 6 characters.
- Store passwords securely by hashing and salting, ensuring they are not cut off.
- Disallow sequential characters (like "1234") or repeated characters (like "aaaa") to increase complexity.
- Skip unnecessary complexity requirements, such as mandating special characters.
- Avoid knowledge-based questions (e.g., "Your first pet’s name") as authentication methods.
- Implement lockout policies after a specified number of failed login attempts, typically 10 tries.
- Prohibit users from including context-specific words in their passwords to enhance uniqueness.
- Allow users to create long passwords (up to 64 characters) using a wide range of characters, including emojis and spaces.
- Check for previously compromised passwords and reject any that have appeared in data breaches.
- Eliminate password expiration dates to reduce user frustration.
- Refrain from using SMS for two-factor authentication codes, as it is less secure.
- Dismiss password hints, which provide little security value.