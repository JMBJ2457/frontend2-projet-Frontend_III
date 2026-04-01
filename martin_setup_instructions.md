# Martin Bogarin - Setup Instructions

## Current Status
✅ Branch `martin-bogarin` is created and ready
✅ Git user configured: Martin Bogarin <juan.bogarinjuarez@cesunbc.edu.mx>

## Required: GitHub Personal Access Token

GitHub no longer supports password authentication. You need to create a Personal Access Token:

### Steps to Create Token:
1. Go to: https://github.com/settings/tokens
2. Click "Generate new token" → "Generate new token (classic)"
3. Fill in:
   - **Note**: "frontend2-project"
   - **Expiration**: Choose appropriate time period
   - **Scopes**: Check `repo` (full control of private repositories)
4. Click "Generate token"
5. **Copy the token immediately** (you won't see it again)

### Setup Commands:
```bash
# Clone the repository (if not already done)
git clone https://github.com/JMBJ2457/frontend2-projet-frontend_iii.git
cd frontend2-projet-frontend_iii

# Switch to Martin's branch
git checkout martin-bogarin

# Configure Git user
git config user.name "Martin Bogarin"
git config user.email "juan.bogarinjuarez@cesunbc.edu.mx"

# Set up remote with token (replace YOUR_TOKEN with the actual token)
git remote set-url origin https://JMBJ2457:YOUR_TOKEN@github.com/JMBJ2457/frontend2-projet-frontend_iii.git

# Push the branch
git push --set-upstream origin martin-bogarin
```

### Alternative: Use Git Credential Manager
```bash
# Configure credential helper
git config --global credential.helper manager-core

# First push will prompt for username and token
git push --set-upstream origin martin-bogarin
# Username: JMBJ2457
# Password: [paste your token here]
```

## Ready to Work
Once authenticated, you can:
- Make changes: `git add . && git commit -m "your message"`
- Push changes: `git push`
- Pull updates: `git pull`

## Branch Information
- **Branch**: `martin-bogarin`
- **Username**: JMBJ2457
- **Email**: juan.bogarinjuarez@cesunbc.edu.mx
