# Project Integration

The goal of this assignment is to help teams establish and organize the foundational project management and collaboration artifacts required for professional software development projects.

Students will use GitHub to create and manage documentation, planning artifacts, project tracking tools, and collaboration agreements for their CAPSTONE projects.

This assignment focuses on **Project Integration**, communication, collaboration, and repository organization rather than software implementation itself.

# Deliverables

Each group must create and maintain the following artifacts in their GitHub repository.

## 1. `README.md` File

A `README.md` file must be created in the **root of the repository**. This file should contain:

### Team Information Table

The file must include a table containing:

- Full name of each team member
- Student email
- Role within the project

Example:

| Name | Email | Role |
|------|------|------|
| Jane Doe | jane.doe@email.com | Backend Developer |
| John Smith | john.smith@email.com | Frontend Developer |

### Project Description

The `README.md` must also contain:

- A project title
- Two or three paragraphs explaining the project
- The explanation must use language understandable by a non-technical audience
- Avoid excessive technical jargon
- Clearly explain:
  - What problem the project solves
  - Who the intended users are
  - What the project does at a high level

---

## 2. `CHANGELOG.md`

Groups must create a `CHANGELOG.md` file documenting the evolution of the project.

### Location Requirement

The changelog **must NOT** be placed in the repository root. Instead, it must be located inside a `docs` folder:

```text
/docs/CHANGELOG.md
```

---

### Required Contents

Each changelog entry should include:

- Date of the change
- Short description of the change
- Link to the Pull Request associated with the change

Example:

```markdown
## 2026-05-05

### Added
- Added user authentication system #12 (this should be a link to the real PR - see example)
- Refactored navigation menu #15 (this should be a link to the real PR - see example)

```

## 3. Working Agreement

Each group must create a Markdown document describing how the team will collaborate throughout the project.

Suggested filename:

```text
/docs/WORKING_AGREEMENT.md
```


### Minimum Required Sections

The working agreement must contain:

#### Meeting Information

- Weekly meeting day and time
- Meeting platform or location
  - Examples:
    - Discord
    - Microsoft Teams
    - In-person
    - Zoom


#### Communication Expectations

- Expected response time for messages
- Preferred communication channels


#### Accountability Rules

- Agreed penalties or consequences for:
  - Missing meetings
  - Repeated lateness
  - Lack of participation
  - Failure to respond to teammates

Examples may include:
- Extra documentation duties
- Reduced participation in decisions
- Reporting concerns to the professor
- Reassignment of responsibilities

#### GitHub Workflow Agreement

The document must explain:

- How code is merged into the main branch
- Pull Request review expectations
- Whether direct pushes to `main` are allowed
- Naming conventions for branches

---

#### Testing Requirements

The agreement must define:

- Minimum testing expectations before merging code
- Required automated tests (if applicable)
- Verification responsibilities before approving Pull Requests

---

## 4. Project Backlog Using GitHub Issues

Groups are required to create a project backlog using GitHub Issues.

### Issue Title Requirements

Issue titles must be written as **User Stories**.

Example:

```text
As a User, I want to reset my password so that I can recover access to my account.
```

### Issue Body Requirements

At this stage:

- Issues that are already completed must contain full descriptions
- The first issue each student plans to work on must also contain a full description
- Remaining issues only require titles for now

### Issue Template

Students should use the following structure:

```markdown
## Description
Describe the feature or task.

## Acceptance Criteria
- [ ] Requirement 1
- [ ] Requirement 2

## Testing Criteria
- [ ] Test 1
- [ ] Test 2

## Notes
Additional implementation details.
```

## 5. Milestones

Groups must create multiple GitHub Milestones.

### Requirements

- Issues must be assigned to appropriate milestones
- Milestones should represent meaningful phases or deliverables of the project

Examples:

- Authentication
- Cart/Payment
- AI integration

## 6. Kanban Board

Groups must create and organize a GitHub Project Board (Kanban board).

### Requirements

Issues must be placed in the appropriate columns.

Suggested columns:

- To Do
- In Progress
- Reviewing
- Done

The board should reflect the current state of the project work.

---

# Final PDF Submission

After creating all GitHub artifacts, groups must generate a PDF document containing the following items in order:

1. The `README.md` File (**1.0 marks**)
2. The Working Agreement (**1.0 marks**)
3. The Current Changelog (**1.0 marks**)
4. Issue Screenshots (**2.0 marks**)
   - One screenshot of a fully written issue per student
   - The screenshot must clearly show:
      - The issue title
      - The issue body
       - The assigned milestone (if applicable)
5. Milestones Screenshot (**1.0 marks**)
6. Kanban Board Screenshot (**1.0 marks**)

# Submission Instructions

Submit a single PDF document containing all required artifacts and screenshots

# Evaluation Criteria

Each item will be marked from 0% to 100% as per the table below:

| Performance Level | Percentage Range | Description |
|---|---|---|
| Exemplary | 100% | The component is fully completed with exceptional quality, professionalism, accuracy, and attention to detail. All requirements are thoroughly addressed. |
| Proficient | 75% | The component is well completed and meets most requirements with good quality and organization. Minor issues or omissions may be present. |
| Satisfactory | 50% | The component demonstrates an acceptable level of completion but lacks consistency, detail, clarity, or depth in multiple areas. |
| Limited | 25% | The component is incomplete, poorly organized, or demonstrates minimal effort. Significant requirements are missing or inadequately addressed. |
| Not Submitted | 0% | The component was not submitted or does not provide sufficient evidence of completion. |

In addition, **3.0 marks** are allocated to presenting this Project Integration at our Scrum meeting. Marks will be allocated as per the table below:

| Performance Level | Percentage Range | Description |
|---|---|---|
| Exemplary | 100% | The presentation is exceptionally clear, professional, and well organized. The speaker demonstrates strong mastery of the subject matter, communicates ideas confidently, and answers questions accurately and thoughtfully. Visual aids and explanations significantly enhance understanding. |
| Proficient | 75% | The presentation is clear and organized, with good understanding of the topic demonstrated throughout. Most questions are answered correctly and with reasonable detail. Minor issues with clarity, pacing, confidence, or depth may be present. |
| Satisfactory | 50% | The presentation communicates the basic ideas of the topic but lacks clarity, organization, confidence, or sufficient detail in multiple areas. Responses to questions demonstrate only partial understanding of the material. |
| Limited / Insufficient | 25% | The presentation is poorly prepared, unclear, incomplete, or difficult to follow. The speaker demonstrates limited understanding of the material and is unable to adequately answer questions related to the topic. |

# Important Notes

- All Markdown files must render correctly on GitHub
- Use proper Markdown formatting throughout
- Keep documentation professional and well organized
- All team members are expected to contribute to the project management artifacts
- GitHub repositories should demonstrate evidence of collaboration and planning, not only code contributions
