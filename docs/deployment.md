# Deployment Process

1. Developer pushes code to the main branch
2. GitHub Actions workflow triggers
3. Files are copied to a temporary directory on EC2
4. Existing production files are backed up
5. New files are moved to `/var/www/html`
6. Nginx is reloaded

This approach prevents direct overwrites and allows rollback.
