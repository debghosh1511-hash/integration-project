# 1) Create folder and initialize git
mkdir integration-project
cd integration-project
git init

# 2) Create folders
mkdir -p .github/workflows .vscode apps libs tools

# 3) Create files (use an editor to paste the content below)
echo "# Integration project" > README.md
echo "NODE_ENV=example\nNETSUITE_URL=\nOPS_DB=\nMES_API=\n" > .env.example
echo "node_modules/\n.vscode/\n.env\n.DS_Store\n" > .gitignore
echo "## Changelog\n\n- v0.1 - repo created" > CHANGELOG.md
echo "Code of conduct placeholder" > CODE_OF_CONDUCT.md

# 4) First commit and push to GitHub
git add .
git commit -m "Initial repo structure"
# create repo on github and then:
git remote add origin git@github.com:your-username/integration-project.git
git branch -M main
git push -u origin main
