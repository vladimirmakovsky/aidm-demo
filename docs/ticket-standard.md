# Ticket Standard (Definition of Ready)

A ticket can be taken into development only when its description follows this structure.

## Required description structure

```markdown
## User Story
As a <role>, I want <capability>, so that <benefit>.

## Context
Why this is needed, links to related tickets and documents.

## Scope
- In scope: ...
- Out of scope: ...

## Acceptance Criteria
AC-1: <short title>
Given <precondition>
When <action>
Then <expected result>

## Business Rules Affected
List of rule IDs from docs/business-rules.md and how each one applies.

## Dependencies
Linked tickets with the type of dependency (blocked by / blocks / related to).

## Open Questions
Questions that are still unanswered, each addressed to a specific person.
```

## Rules for acceptance criteria

- Written in Given / When / Then format.
- Each criterion is testable and checks one behavior.
- Cover the happy path, validation errors, and edge cases.
- Use terms from docs/glossary.md only.
- Include concrete values (amounts, limits, texts) instead of words like "correct" or "appropriate".
- Reference a business rule ID when a criterion comes from a rule.

## Definition of Ready checklist

- [ ] User story is filled in
- [ ] Scope lists what is in and what is out
- [ ] At least 5 acceptance criteria, including negative cases
- [ ] No contradictions with docs/business-rules.md
- [ ] All attachments and comments are reflected in the description
- [ ] Dependencies are linked
- [ ] No open questions that block development

## How to ask clarifying questions

- Post them as one comment in the ticket, numbered.
- Address each question to a person with @mention.
- For each question, explain why it matters and offer a default assumption.
- Add the label `needs-clarification` while questions are open.
