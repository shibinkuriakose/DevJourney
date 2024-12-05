# Initial Project Setup Journey
Date: 2024-01-12

## Context
Setting up two new projects: WinLat3 (LaTeX converter) and DevJourney (learning documentation).

## Challenges Encountered

### 1. Git Configuration Issues
- **Error**: Unable to auto-detect email address
- **Solution**: Manually configured Git with email and name
- **Learning**: Git requires proper user configuration before first commit
- **Reference**: [Git Configuration Entry](../errors/2024-01-12-git-config.md)

### 2. Windows PowerShell Directory Creation
- **Error**: PowerShell couldn't create multiple directories with Unix-style paths
- **Solution**: Created directories individually using Windows path style
- **Learning**: Windows PowerShell uses different path separators and command syntax
- **Command Used**: `mkdir dir1; mkdir dir2` instead of `mkdir -p dir1/dir2`

### 3. Repository Structure Decisions
- **Challenge**: How to organize learning documentation across projects
- **Solution**: Created two-level approach:
  1. Project-specific dev-journal in each project
  2. Central DevJourney repository for cross-project learning
- **Benefits**: 
  - Project-specific issues stay with projects
  - Common knowledge is centralized and shared
  - Better searchability and organization

## Tools and Concepts Learned

### 1. YAML
- Human-readable data format
- Used for configuration files
- Simpler than JSON or XML
- [Details](../../shared-knowledge/best-practices/documentation-and-devops.md#yaml-explained)

### 2. CI/CD
- Continuous Integration/Continuous Deployment
- Automated building and testing
- GitHub Actions for automation
- [Details](../../shared-knowledge/best-practices/documentation-and-devops.md#cicd-continuous-integrationcontinuous-deployment)

### 3. Documentation Tools
- MkDocs for documentation websites
- Markdown for content writing
- GitHub-flavored Markdown features
- [Details](../../shared-knowledge/best-practices/documentation-and-devops.md#documentation-tools)

## Project Setup Achievements

### WinLat3 Setup
1. ✅ Basic repository structure
2. ✅ Documentation framework
3. ✅ CI/CD pipeline
4. ✅ Issue templates
5. ✅ Project milestones

### DevJourney Setup
1. ✅ Central learning repository
2. ✅ Organized knowledge structure
3. ✅ Cross-project documentation
4. ✅ Error tracking system

## Best Practices Implemented

1. **Documentation**
   - Immediate documentation of issues
   - Clear structure for knowledge sharing
   - Cross-referencing between related topics

2. **Version Control**
   - Proper Git configuration
   - Clear commit messages
   - Branch protection rules

3. **Project Organization**
   - Separated concerns
   - Clear directory structure
   - Easy to navigate

## Next Steps

1. Set up C++/WinRT project structure for WinLat3
2. Create more documentation templates
3. Implement additional GitHub workflows
4. Begin actual development

## References
- [Git Documentation](https://git-scm.com/doc)
- [PowerShell Documentation](https://docs.microsoft.com/en-us/powershell/)
- [GitHub Actions](https://docs.github.com/en/actions)
- [MkDocs](https://www.mkdocs.org/) 