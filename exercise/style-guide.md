# Style Guide — Nexus Docs Pipeline API

Apply these rules across all documentation for the Nexus Docs Pipeline API.

---

## Voice and tone

**1. Active voice only.** The subject does the action.
- ✓ "The API returns a `Build` object."
- ✗ "A `Build` object is returned by the API."

**2. Second person.** Address the reader directly as "you."
- ✓ "You can filter results by status."
- ✗ "Users can filter results by status."

**3. Present tense.** Describe what the API does now, not what it will do.
- ✓ "The endpoint returns a `201` status code."
- ✗ "The endpoint will return a `201` status code."

---

## Word choices

**4. "lets you" — not "allows you to" or "enables you to."**
- ✓ "The `notify_on_complete` parameter lets you receive an email when the build finishes."
- ✗ "The `notify_on_complete` parameter allows you to receive an email when the build finishes."

**5. No "simply," "just," "easily," or "quickly."** These minimize difficulty the reader may not share.

**6. No vague quantifiers.** Replace "various," "several," "many," and "a number of" with specific counts or remove them.
- ✓ "The `status` field has five possible values."
- ✗ "The `status` field has various possible values."

**7. No Latin abbreviations.** Write "for example," "that is," and "and so on" in full.

---

## Parameters and field descriptions

**8. Describe behavior, not type.** A description should answer "what does this do?" — not "what is this?"
- ✓ "`limit` — Maximum number of builds to return. Defaults to 20. Maximum is 100."
- ✗ "`limit` — An integer representing the limit."

**9. Always state defaults and constraints.** If a parameter is optional, say what happens when you omit it.
- ✓ "When omitted, the build targets `production`."

**10. Document nullable fields explicitly.** If a field can be null, say when and why.
- ✓ "`completed_at` — Timestamp when the build finished. Null if the build is still in progress."

---

## Endpoint descriptions

**11. Every endpoint description answers three questions:**
1. What does this endpoint do? (one sentence)
2. When would you call it?
3. What should you do next with the response?

**12. Examples are required.** Every endpoint must have at least one request example and one success response example. Examples must use realistic values — not `string`, `integer`, or `<value>`.
