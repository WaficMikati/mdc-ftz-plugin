# Miami Dade FTZ Knowledge Base (plugin)

Answers questions about U.S. Foreign-Trade Zones from Miami Dade College's FTZ Specialist Certificate knowledge base: the current FTZ regulations (19 CFR Part 146 and 15 CFR Part 400, refreshed daily from eCFR), the CBP Foreign-Trade Zones Manual, CBP forms, and the program's course materials. Every answer cites its source.

## Contents

- `skills/ftz-knowledge-base`: when to use the knowledge base and how to answer from it (search first, cite every claim, nothing from memory)
- `.mcp.json`: the FTZ connector (`https://mdc-ftz.4geeks.workers.dev/mcp`)

## Set up

1. In Claude, go to **Customize > Plugins > Add > Add marketplace**, enter `WaficMikati/mdc-ftz-plugin`, then install **Miami Dade FTZ Knowledge Base**.
2. Open the plugin's **Connectors** tab and click **Connect** on the FTZ connector. Sign in with your Miami Dade FTZ Knowledge Base email and password, then click **Allow**.
3. In **Customize > Connectors > Miami Dade FTZ Knowledge Base**, set the read-only tools to **Always allow**.

## Data

Questions are sent to the FTZ connector, run by 4Geeks on Cloudflare, which searches the knowledge base and returns passages. The connector doesn't store questions or conversations.
