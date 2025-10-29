# My Git Mastery Challenge Journey

## Student Information
- **Name:** Sailaja
- **Student ID:** 23P31A4207
- **Repository:** [https://github.com/sailajabevara/git-solved-23P31A4207](https://github.com/sailajabevara/git-solved-23P31A4207)
- **Date Started:**  29 October 2025
- **Date Completed:** 29 October 2025

---

## Task Summary
Cloned instructor's repository with pre-built conflicts and resolved all 
merge conflicts across multiple branches using proper Git workflows.

---

## Commands Used

| Command | Times Used | Purpose |
|---------|------------|----------|
| git clone | 1 | Clone instructor's repository |
| git checkout | 20+ | Switch between branches |
| git branch | 10+ | View and manage branches |
| git merge | 2 | Merge dev and conflict-simulator into main |
| git add | 30+ | Stage resolved conflicts |
| git commit | 15+ | Commit resolved changes |
| git push | 10+ | Push to my repository |
| git fetch | 2 | Fetch updates from instructor |
| git pull | 1 | Pull updates |
| git stash | 2 | Save temporary work |
| git cherry-pick | 1 | Copy specific commit |
| git rebase | 1 | Rebase feature branch |
| git reset | 3 | Undo commits (soft/mixed/hard) |
| git revert | 1 | Safe undo |
| git tag | 2 | Create release tags |
| git status | 50+ | Check repository state |
| git log | 30+ | View history |
| git diff | 20+ | Compare changes |

---

## Conflicts Resolved

### Merge 1: main + dev (6 files)

#### Conflict 1: config/app-config.yaml
- **Issue:** Production used port 8080, development used 3000  
- **Resolution:** Created unified config with environment-based settings  
- **Strategy:** Keep production as default, add dev as optional  
- **Difficulty:** Medium  
- **Time:** 15 minutes

#### Conflict 2: config/database-config.json
- **Issue:** Different database hosts and SSL modes  
- **Resolution:** Created separate profiles for production and development  
- **Strategy:** Restructured JSON to support both environments  
- **Difficulty:** Medium  
- **Time:** 10 minutes

#### Conflict 3: scripts/deploy.sh
- **Issue:** Different deployment strategies (production vs docker-compose)  
- **Resolution:** Added conditional logic based on DEPLOY_ENV variable  
- **Strategy:** Made script handle both environments dynamically  
- **Difficulty:** Hard  
- **Time:** 20 minutes

#### Conflict 4: scripts/monitor.js
- **Issue:** Different monitoring intervals and log formats  
- **Resolution:** Environment-based configuration object  
- **Strategy:** Used process.env.NODE_ENV to determine behavior  
- **Difficulty:** Medium  
- **Time:** 15 minutes

#### Conflict 5: docs/architecture.md
- **Issue:** Different architectural descriptions  
- **Resolution:** Merged both descriptions into comprehensive document  
- **Strategy:** Created sections for each environment  
- **Difficulty:** Easy  
- **Time:** 10 minutes

#### Conflict 6: README.md
- **Issue:** Different feature lists and version numbers  
- **Resolution:** Combined all features with clear environment labels  
- **Strategy:** Organized features by category  
- **Difficulty:** Easy  
- **Time:** 10 minutes

---

### Merge 2: main + conflict-simulator (6 files)

#### Conflict 1: config/api-endpoints.json  
- **Issue:** Different endpoint URLs and authentication types  
- **Resolution:** Unified both sets with versioning support  
- **Strategy:** Used conditional logic based on API version  
- **Difficulty:** Medium  
- **Time:** 10 minutes

#### Conflict 2: scripts/health-check.sh  
- **Issue:** One script used `curl`, another used `wget`  
- **Resolution:** Added compatibility for both commands  
- **Strategy:** Used fallback approach if one fails  
- **Difficulty:** Easy  
- **Time:** 8 minutes

#### Conflict 3: src/app.js  
- **Issue:** Mismatched feature imports  
- **Resolution:** Combined both imports safely  
- **Strategy:** Verified code by running tests  
- **Difficulty:** Medium  
- **Time:** 12 minutes

#### Conflict 4: package.json  
- **Issue:** Dependency version mismatches  
- **Resolution:** Updated all dependencies to latest compatible versions  
- **Strategy:** Tested build after merging  
- **Difficulty:** Medium  
- **Time:** 15 minutes

#### Conflict 5: README.md  
- **Issue:** Duplicate project descriptions  
- **Resolution:** Merged content with proper sectioning  
- **Strategy:** Added headings for clarity  
- **Difficulty:** Easy  
- **Time:** 5 minutes

#### Conflict 6: .gitignore  
- **Issue:** Different ignored file patterns  
- **Resolution:** Combined all unique patterns  
- **Strategy:** Avoided redundancy  
- **Difficulty:** Easy  
- **Time:** 5 minutes

---

## Most Challenging Parts

1. **Understanding Conflict Markers:** Initially confused by `<<<<<<<`, `=======`, and `>>>>>>>`. Learned that HEAD is the current branch, and the other side is the incoming changes.  
2. **Deciding What to Keep:** Needed to carefully review both sides before choosing.  
3. **Complex Logic Conflicts:** deploy.sh had completely different logic that required analysis.  
4. **Testing After Resolution:** Ensured merged code executed properly before committing.

---

## Key Learnings

### Technical Skills
- Mastered conflict resolution process  
- Understood merge conflict markers  
- Learned to use `git diff` and `git log` effectively  
- Practiced all major Git commands  

### Best Practices
- Always read both sides before resolving  
- Test code after resolving  
- Write clear commit messages  
- Use `git status` frequently  
- Commit in small, logical chunks  

### Git Workflow Insights
- Conflicts are normal, not errors  
- Take time to understand both changes  
- When unsure, ask for help  
- Document your strategy  
- Stay calm and patient  

---

## Reflection
This challenge taught me that merge conflicts aren’t failures — they’re opportunities to understand teamwork in Git.  
By practicing merges, rebase, cherry-pick, and reset, I learned how professional Git workflows handle collaboration.  
Now, I feel confident managing repositories and resolving conflicts independently.  

---

✅ **Documented Usage Summary:**  
- Used `git reset` (3 times)  
- Used `git revert` (1 time)  
- Created and pushed 2 annotated tags  
- All conflicts resolved successfully  
- Repository completed with documentation
