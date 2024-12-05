# Branch Protection Rules

## Why Branch Protection?
1. **Code Quality**: Ensure code meets standards before merging
2. **Collaboration**: Enforce code review practices
3. **Stability**: Prevent accidental pushes to important branches
4. **Documentation**: Maintain documentation quality
5. **Security**: Prevent unauthorized changes

## Protected Branches

### `main` Branch
Primary branch containing stable, production-ready code.

#### Rules:
1. **Require pull request reviews before merging**
   - At least 1 review required
   - Dismiss stale pull request approvals when new commits are pushed
   - Require review from Code Owners

2. **Require status checks to pass before merging**
   - Require branches to be up to date before merging
   - Required checks:
     - Build validation
     - Tests
     - Documentation build

3. **Require signed commits**
   - All commits must be signed with GPG
   - Ensures commit authenticity

4. **Include administrators**
   - Rules apply to everyone
   - No bypassing protections

### `develop` Branch
Main development branch for ongoing work.

#### Rules:
1. **Require pull request reviews before merging**
   - At least 1 review required
   - Allow approvals from project maintainers

2. **Require status checks to pass before merging**
   - Basic build validation
   - Unit tests

3. **Require linear history**
   - Prevent merge commits
   - Maintain clean history

## Branch Naming Convention

### Feature Branches
- Format: `feature/[issue-number]-brief-description`
- Example: `feature/123-add-latex-compiler`

### Bug Fix Branches
- Format: `fix/[issue-number]-brief-description`
- Example: `fix/456-compiler-crash`

### Documentation Branches
- Format: `docs/[topic]-update`
- Example: `docs/api-reference-update`

## Workflow

1. **New Feature/Fix**
   - Create branch from `develop`
   - Follow naming convention
   - Work on changes

2. **Code Review**
   - Create pull request to `develop`
   - Get required reviews
   - Pass status checks

3. **Merge to Develop**
   - Squash and merge
   - Delete feature branch

4. **Release**
   - Create release branch from `develop`
   - Final testing
   - Merge to `main`

## Setting Up Protection Rules

1. Go to repository Settings
2. Navigate to Branches
3. Add rule for each protected branch
4. Configure required status checks
5. Set review requirements

## Enforcement
- All team members must follow these rules
- No direct pushes to protected branches
- All changes through pull requests
- Regular audit of branch protection 