# Issue Template Guide

This repository uses GitHub issue forms to make tickets consistent and easier
to plan, find, and hand off. Use the closest form when opening an issue rather
than a blank issue; blank issues are intentionally disabled.

## Choose the right form

### Project

Use a **Project** for a high-level initiative that spans multiple months and
contains several epics. Describe the intended outcome, success criteria,
timeline, stakeholders, dependencies, and risks.

Example: rebuilding the launch application.

### Epic

Use an **Epic** for a 1–2 month goal or feature that groups related stories.
Link its parent project when one exists. State the goal, acceptance criteria,
estimated timeline, dependencies, and important technical constraints.

Example: a CAN-decoder modernization effort within a larger telemetry project.

### Story

Use a **Story** for a 1–2 week outcome that delivers value to a user, operator,
or developer. Link the parent epic, write the user story in the form
`As a …, I want … so that …`, then define acceptance criteria and the tasks
needed to complete it. Include an effort estimate and priority.

Example: as a test engineer, I want to see live board status so that I can
diagnose a bench test without inspecting raw CAN traffic.

### Task

Use a **Task** for a concrete unit of work that should take a few hours. Choose
the task type, link its parent story if it has one, explain the work, and set
its priority. Add acceptance criteria when they make completion unambiguous.

Use `Bug` as the task type when the work is a small, well-understood fix.
Otherwise, use the separate Bug Report form when the behaviour still needs
reproduction or investigation.

### Bug report

Use a **Bug Report** for unexpected behaviour. Provide a clear description,
steps to reproduce it, expected and actual behaviour, and relevant logs or
screenshots. Include environment and version details when they could affect
the issue.

## Writing useful issues

- Let the form add the title prefix and type label; write a concise, action- or
  outcome-oriented title after it.
- Complete required fields and use concrete, testable acceptance criteria.
- Link related issues with `#<number>`. Link implementation pull requests from
  the code repository back to the tracking issue.
- Add an area label for the affected system, such as `omnibus`, `daqms`,
  `parsley`, `website`, `launch-app`, or `avionics-app`.
- Add cross-cutting labels where helpful: `bug`, `documentation`, `design`,
  `research`, `good first issue`, `help wanted`, or `autosequencing`.
- Keep implementation details in linked code repositories. This repository
  tracks the work, decisions, scope, and status; it does not contain
  application code.

## Recording technical decisions

Open an issue when a decision needs discussion, review, or a durable record.
Explain the context, options considered, decision, and consequences. Use an
appropriate area label and `design` or `research` where applicable. Link any
supporting Notion page, design file, or implementation pull request.

For a decision that produces implementation work, create or link the relevant
epic, story, or task so the rationale remains connected to the work it affects.
