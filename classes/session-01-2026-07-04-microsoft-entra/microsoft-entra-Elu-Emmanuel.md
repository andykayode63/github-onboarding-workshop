# My Notes — Elu Uchenna Emmanuel

---

## Key Concepts I Learned

<!-- Write the main ideas covered in today's session -->

-Securing access to resources using MS entra
-We focussed on authentication, MFA, CA and PIM  

---

## Lab / Hands-On Work

<!-- Describe what you did in the lab. Include steps, commands, or screenshots descriptions -->

### What I did
I enabled authentication policy needed for the platform (Microsoft authenticator, TAP and Email) 
I disabled authenticator policy not needed (SMS, Call, Fido etc).
Modified the lockout threshold, duration and created custom banned password.
I created a CA policy to require MFA, assigned it to all users, target all resources and from any location.
<img width="1587" height="678" alt="Screenshot 2026-07-10 113548" src="https://github.com/user-attachments/assets/315a10c2-5fc5-4f78-94d2-c6babd8a66d8" />

I created a CA policy to blocked MS admin portal, included all users and excluded the admin and break glass account, then I targeted the MS admin portals and configured the grant to block access and turned the policy to On.
<img width="719" height="642" alt="Screenshot 2026-07-10 112912" src="https://github.com/user-attachments/assets/89bf9999-f0a4-4913-bfe5-e50bc281478f" />


### What happened / Result
All user were prompted to register for MFA on first login and to authenticate with MFA on future login.
User were prevented from accessing MS admin portal except for the Admin and breakglass account.

### Challenges I faced
The configs were successful. 
Could not practice PIM due to license limitation
---

## My Takeaways

<!-- What was most valuable to you personally from this session? -->
Ability to confidently establish a CA policy without hassle

---

## Questions I Still Have

<!-- Anything you want to follow up on or ask the mentor -->

-Need guide to create API plugins for agents
---

## Resources I Found Useful

<!-- Any links, docs, or Microsoft Learn modules you found helpful -->

-https://learn.microsoft.com/en-us/training/paths/secure-access-resources-entra/
-https://www.youtube.com/watch?v=R7zxI-k3NoQ&t=139s
---

*Submitted by: Elu Uchenna Emmanuel · eluemma*
