# Git Workflow Guide

## Commit convention

Format: `<type>(<scope>): <message>`

Types: `feat`, `fix`, `docs`, `refactor`, `chore`

## Examples

**Toàn - Wargame:**
```
git commit -m "feat(wargame): level 1 complete"
git commit -m "feat(wargame): level 5 complete"
```

**Toàn - Extra credit:**
```
git commit -m "feat(extra-credit/return-to-libc): exploit successful"
```

**Lượng - Wargame:**
```
git commit -m "feat(wargame): level 6-10 complete"
```

**Lượng - Extra credit:**
```
git commit -m "feat(extra-credit/buffer-overflow): exploit finished"
```

**Organize:**
```
git commit -m "refactor(src): organize payloads and code"
```

**Report:**
```
git commit -m "docs(report): final PDF ready for submission"
```

## Workflow

**Toàn (người tạo repo):**
```
git add src/wargame/level_0X_*
git commit -m "feat(wargame): level X complete"
git push origin main
```

**Lượng (người clone):**
```
git pull origin main
git add src/wargame/level_0X_*
git commit -m "feat(wargame): level X complete"
git push origin main
```

## Check history
```
git log --oneline
git log --graph --oneline --all
```
