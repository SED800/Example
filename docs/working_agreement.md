# Working Agreement

## Purpose
This repository serves as both our software development project and an example repository for future student teams to follow. As such, all team members are expected to maintain a professional standard in communication, documentation, coding practices, and collaboration.

---

# 1. Team Meetings

## Weekly Scrum Meetings
- Meetings will take place every **Friday at 12:35 PM**.
- Additional meetings may be scheduled as needed by the team.
- All meetings will be conducted through our **Discord server** unless otherwise specified.

## Attendance Expectations
- All team members are expected to attend meetings on time and actively participate.
- Team members should notify the group as early as possible if they cannot attend.

## Penalties

### Missing Meetings
- Missing a meeting without prior notice may result in:
  - Loss of assigned responsibilities for the sprint
  - Reduced peer evaluation scores
  - Additional assigned tasks/documentation work

### Late Attendance
- Arriving more than **10 minutes late** without prior notice counts as a late attendance.
- Repeated lateness may result in:
  - Reduced peer evaluation scores
  - Additional review/documentation responsibilities

### Repeated Absences
- Multiple unexcused absences may result in the issue being escalated to the instructor/project supervisor.

---

# 2. Communication Rules

## Primary Communication Channel
- Discord will be used for:
  - Team communication
  - Meeting coordination
  - Sprint discussions
  - Technical questions
  - Announcements

## Response Expectations
- Team members should respond to important messages within:
  - **24 hours during weekdays**
  - **48 hours during weekends**

## Professional Conduct
All members are expected to:
- Be respectful during discussions
- Avoid hostile or dismissive language
- Accept constructive criticism professionally
- Help maintain a collaborative environment

---

# 3. Branching and Pull Requests

## Main Branch Protection
- Direct pushes to the `main` branch are **strictly prohibited**.
- All changes must be merged through a **Pull Request (PR)**.

## Branch Naming Convention
Branches should follow a clear naming pattern:

```text
feature/feature-name
bugfix/bug-description
hotfix/hotfix-description
docs/documentation-update
```

Examples:

```text
feature/user-authentication
bugfix/login-validation
docs/update-readme
```

## Pull Request Rules
Before opening a Pull Request:
- Code must compile successfully
- Automated tests must pass
- Relevant documentation must be updated
- The branch must be up to date with `main`

## PR Review Requirements
- Every Pull Request must be reviewed by at least **one other team member**
- Authors should not merge their own PR without approval unless explicitly authorized
- Review comments should be addressed before merging

## Merge Strategy
- Keep commit history clean
- Commit messages should be descriptive and meaningful

Examples:

```text
Add JWT authentication middleware
Fix memory leak in file parser
Update README with setup instructions
```

---

# 4. Coding and Documentation Standards

## Markdown Standards
- All documentation must use **standard GitHub-compatible Markdown**
- Only syntax properly rendered by GitHub should be used
- Avoid HTML unless absolutely necessary

## Documentation Expectations
The repository should always contain:
- A clear `README.md`
- Setup instructions
- Build/run instructions
- Contribution guidelines
- Example usage where applicable

## Code Quality Expectations
Team members are expected to:
- Write readable and maintainable code
- Use meaningful variable and function names
- Avoid unnecessary complexity
- Add comments where clarification is needed

---

# 5. Deliverables and Deadlines

## Early Submission Requirement
Deliverables should be completed **at least 48 hours before deadlines** whenever possible.

This allows time for:
- Peer review
- Testing
- Bug fixes
- Documentation updates

## Responsibility of Contributors
The contributor is responsible for:
- Verifying their code works
- Updating documentation
- Responding to review feedback promptly

## Incomplete Deliverables
Pull Requests submitted too close to deadlines may:
- Be rejected from the sprint
- Be deferred to the next iteration
- Receive limited review due to time constraints

---

# 6. Automated Testing

## Testing Expectations
All major deliverables should include:
- Automated tests where appropriate
- Validation of expected behavior
- Regression protection for existing features

## Required Before Merge
A Pull Request should not be merged if:
- Existing tests fail
- New features are untested
- The build pipeline is broken

## Preferred Testing Workflow
- Run tests locally before pushing
- Use GitHub Actions (or equivalent CI tools) whenever possible
- Keep tests lightweight, repeatable, and maintainable

---

# 7. Repository Professionalism

Since this repository serves as an example for future teams:
- Documentation should remain polished
- Commit history should remain clean
- Pull Requests should remain professional
- Issues should be descriptive and properly labeled

The goal is to demonstrate professional software development practices that future students can learn from and emulate.

---

# 8. Conflict Resolution

If disagreements occur:
1. Discuss the issue respectfully as a team
2. Attempt to reach consensus
3. Escalate unresolved issues to the instructor/project supervisor if necessary

---

# 9. Agreement Acceptance

By contributing to this repository, all team members agree to follow this working agreement and uphold the professional standards outlined within this document.
