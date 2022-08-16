---
id: trj657zpqnxx6mvu19y41ji
title: Leavers
desc: ''
updated: 1660231098587
created: 1660230431306
---

## Steps

1. HR Informs IT that employee has left
2. Microsoft 365 Steps
   1. Exchange Steps
      1. Convert UserMailbox -> SharedMailbox in Exchange Online
      2. Forward mail to users manager
      3. Delegate full access to users manager
      4. Notify manager
   2. 365 Steps
      1. Remove all assigned licenses
      2. Disallow login
3. On-Prem
   1. Disable account in AD
   2. Move user account to "Domain Users - Disabled" OU
   3. Take ownership of docs
   4. Archive docs
4. EFACS
   1. Set ismanager to false
   2. Set allowlogin to false
   3. Set iscurrentemployee to false
   4. Set enddate to employees leave date
