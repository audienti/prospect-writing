---
name: prospect-writing
description: Write an email, LinkedIn comment or reply from a current Exo prospect plan and save it to Operator for review. Does not choose cadence or send outreach.
---

Read the selected methodology, experiment Approach, current plan, signal evidence and relevant profile activity. Use prospect-planning with operation context to get facts, then check that the plan is current. Refresh planning first if facts or timing changed. The host agent writes the message. No separate model API is needed.

Inspect saved engagementHistory and any available connected conversation history before writing. Distinguish a confirmed new conversation (complete history with no events) from unavailable history. Never set complete merely because Exo has no events. If external history cannot be checked, prepare the draft with that uncertainty and leave cadence blocked. Do not ask the human to research routine facts. An inbound message takes priority over a prepared opener. An opt-out is a stop, not a writing opportunity.

Write the actual words the recipient would see. Follow the workspace writing voice. Keep the agent's instructions and rationale out of the message. For validating approaches, seek an internal explanation or correction with one specific question. Do not assume pain, intent or informant/champion/buyer status. No product pitch, diagnostic or meeting request unless the Approach authorizes it.

Use the exact evidence, not a stronger paraphrase: a vacancy does not prove team growth, a new budget, a process failure or hiring ownership. A public comment must fit the actual post. Check saved provider activity payloads for the full text before making another provider call. If only a fragment is available, avoid claims about unseen content and fetch the full post when the proposed response depends on it. Do not manufacture a compliment or personal experience. Prefer useful, plain conversation over performative engagement. Vary questions across colleagues, considering what each role can know.

Save using the prospect-planning workflow with operation draft, personId, experimentPath, planId, and message {subject, body}. Email needs a subject. Comments and LinkedIn messages have only body. Include expectedRevision when replacing an existing draft. A repeated save of identical content is idempotent. Use the current record, never overwrite a person's edits from a stale copy.

Operator can edit, approve or skip. Editing resets content approval. Approval records acceptance of the wording only; it never authorizes delivery or changes the cadence hold. Nothing in this skill posts, sends, or consumes a touch. Keep research, context and decisions in Exo rather than only in chat.

The message schema is in references/message.schema.json. Exo checks plan identity, freshness and revision at save/review. The agent remains responsible for semantic fit and accurate wording.
