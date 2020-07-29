# Sparta DevOps Security Audit :lock:

### Areas of Risk In Our DevOps Tasks

1. ssh keys being exposed to GitHub
2. passwords being exposed on GitHub
3. Security rulings for our AWS instances
4. ssh keys for different software e.g. Jenkins
5. AWS credentials (*High Risk!*)

### Operations assigned with these areas of Risk

1. Creating machines with Ansible -> Use Ansible Vault
2. Private SSH keys should be added to .gitignore
3. Anything private such as passwords should be placed in .gitignore before pushing to GitHub
4. Security Groups and NACL's should have port 22 open only to your IP.
5. Dynamic IP variables should be kept in gitignore
6. Any form of credentials should be encrypted or ignored (Important!)

### Best practices with areas of risk and tools

1. Add any ssh private keys to .gitignore
2. Where using Ansible use the encrypted and password locked Vault
3. Keep an eye out for any GitGuardian notifications
4. When using software try to make use of encryption files and plugins
5. Do not push any files with passwords or credentials to github
6. GitHub repo's can be set to private if need be!




