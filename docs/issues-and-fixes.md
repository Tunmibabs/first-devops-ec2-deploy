# Issues Encountered & Fixes

## 1. File Overwrite Error
**Issue:**
Deployment failed with tar error when index.html already existed.

**Cause:**
CI/CD tool tried to extract files into an existing directory.

**Fix:**
Deploy to a temporary directory, then move files into the web root.

---

## 2. Permission Denied Error
**Issue:**
ubuntu user could not write to /var/www/html.

**Cause:**
Directory owned by root.

**Fix:**
Used sudo during deployment to move files securely.

---

## 3. SSH Security Risk
**Issue:**
Password-based SSH and open ports.

**Fix:**
Enabled UFW firewall and disabled password authentication.
