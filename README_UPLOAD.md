This repository helper uploads the current `DeepSkilling` folder to the specified GitHub repository.

Usage options

- Recommended (interactive):
  1. Install and run `gh auth login` to authenticate.
  2. From the repository root run:

```powershell
Set-Location 'C:\Users\msasi\Desktop\pawan\DeepSkilling'
.\upload_to_github.ps1
```

- Non-interactive using a Personal Access Token (store in environment):

```powershell
$env:GITHUB_TOKEN = 'ghp_...'
Set-Location 'C:\Users\msasi\Desktop\pawan\DeepSkilling'
.\upload_to_github.ps1
```

Notes
- The default remote is `https://github.com/Pawan832/Cognizant-DN-5.0.git`. To push to a different repo, pass `-RepoUrl`.
- To use SSH, ensure your SSH key is added to GitHub and run the script with `-UseSSH`.
- This script will not store your credentials. Provide auth via `gh`, SSH keys, or `GITHUB_TOKEN`.
