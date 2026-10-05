echo ".vscode/" >> .gitignore
echo "src/.vscode/" >> .gitignore
git reset --soft HEAD~1
git rm --cached .vscode/browse.vc.db 2>/dev/null || true
git rm --cached src/.vscode/browse.vc.db 2>/dev/null || true
git add .
git commit -m "Primeiro commit limpo"
git push -u origin main --force
