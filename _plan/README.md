# Project Planning Directory

This directory contains all the planning documents and workflows for the PM tool project.

## Directory Structure

- `roles/` - Contains role definitions and responsibilities
  - `pm.md` - Project Manager role description
  - `dev.md` - Developer role description
- `scope/` - Contains project scope documents
- `tasks/` - Contains task management directories
  - `ToDo/` - Tasks waiting to be picked up
  - `In-Progress/` - Tasks currently being worked on
  - `Completed/` - Finished tasks
- `workflow.md` - Detailed workflow for PM and developer responsibilities

## Purpose

This structure is designed to facilitate clear project management and task tracking for the PM tool development. Each subdirectory serves a specific purpose in organizing project information and tracking progress according to the defined workflow.

## Task File Schema

Each task in the `tasks/` directory follows a standardized schema. Here's the template for creating new task files:

```
# Task: [Brief title of the task]

**Description**: [Detailed description of what needs to be done]

**Status**: TODO

**Dependencies**: [None or list any tasks that must be completed before this one]

**Priority**: [1-5 scale, with 1 being highest priority]

**Effort**: [Low/Medium/High estimate]

**Assigned Role**: [Worker/Developer/PM/Observor]

**Notes**:
- [Any specific instructions or considerations]

Result: {
  "taskId": "[Unique identifier for the task]",
  "status": "not-started",
  "output": "",
  "updatedNotes": [],
  "issues": [],
  "nextSteps": ""
}
status: TODO
```

### Field Descriptions

- `Task`: A concise title that describes the task
- `Description`: A detailed explanation of the task requirements
- `Status`: Current status of the task (TODO, IN_PROGRESS, COMPLETED)
- `Dependencies`: List of any prerequisite tasks that need completion first
- `Priority`: Number from 1-5 indicating importance (1=highest priority)
- `Effort`: Estimated effort level required to complete the task
- `Assigned Role`: Role responsible for completing the task
- `Notes`: Specific instructions or additional context
- `Result`: JSON block capturing execution results when task is processed
- `status`: Final status indicator for tracking purposes