---
name: herdr-intercom
description: "Patterns of communication with agents via Herdr."
---

Prefix messages with `[<agent name or pane ID>]`:

```sh
herdr agent get "$HERDR_PANE_ID" | jq -r '.result.agent.name // .result.agent.pane_id'
```

Reply to agents, not the user, unless the user should see it.
