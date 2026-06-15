# User Assistance Exercise: Nexus Docs Pipeline API

You've just joined the documentation team at **Nexus**, a fictional SaaS company. The engineering team shipped the **Nexus Docs Pipeline API** - a REST API that lets teams manage their docs-as-code publishing workflow programmatically. Your job: write the public-facing docs.

---

## What you'll practice

- Completing and improving an API reference (OpenAPI 3.0)
- Rewriting an engineer-authored draft for a user audience
- Applying a style guide consistently across deliverables

---

## Files

| File | What it is |
|---|---|
| `exercise/openapi-stub.yaml` | A partially completed OpenAPI 3.0 spec. Some endpoints are fully documented as examples; others have `# TODO` markers for you to fill in. |
| `exercise/getting-started-draft.md` | A rough first draft of the Getting Started guide, written by an engineer. Rewrite it for a technical (but non-engineer) audience. |
| `exercise/style-guide.md` | The editorial rules to apply across all your deliverables. |

---

## Tasks

### Task 1 - Complete the OpenAPI spec (~45 min)

Open `exercise/openapi-stub.yaml`. Find every `# TODO` comment and complete it:

- Write user-facing descriptions for all endpoints and parameters
- Add request/response examples wherever marked
- Complete the `ContentItem` schema and the error schemas

**Acceptance criteria:**
- All `# TODO` markers are removed
- Every parameter description answers "what does this do?" — not just "what type is this?"
- Every endpoint has at least one request example and one success response example

---

### Task 2 - Rewrite the Getting Started guide (~30 min)

Open `exercise/getting-started-draft.md`. Rewrite it following the style guide. The draft works as an implementation note but reads like it was written for engineers, not users.

**Acceptance criteria:**
- Active voice throughout
- No jargon without a brief explanation the first time it appears
- Includes a complete, working example of the full authentication → build → poll flow
- Ends with a clear next step

---

### Task 3 - Style guide audit (~15 min)

Review your completed work against `exercise/style-guide.md`. Use this checklist:

- [ ] Active voice in all descriptions and narrative text
- [ ] "lets you" — not "allows you to" or "enables you to"
- [ ] No "simply," "just," "easily," or "quickly"
- [ ] No vague quantifiers ("various," "several," "many")
- [ ] Every parameter description states its effect, default value, and constraints
- [ ] No Latin abbreviations (e.g., i.e., etc.)

---

## Submitting your work

Create a `solution/` folder and save your completed files there:

```
solution/
  openapi-complete.yaml
  getting-started.md
```

Commit and push to `main`.

---

## Background: the Nexus Docs Pipeline API

Nexus is a platform that builds and publishes documentation from Markdown source files stored in Git. The API lets teams:

- Trigger doc builds from CI/CD pipelines
- Monitor build status and retrieve logs
- Publish approved builds to staging or production
- Manage content metadata without going through the Nexus UI

The primary users of this API are DevOps engineers and technical writers who want to automate their docs publishing workflow.
