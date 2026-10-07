# Miami Dade FTZ Knowledge Base: Claude plugin

A Claude plugin for Miami Dade College's FTZ Specialist Certificate program. It adds:

- **The FTZ connector** (`https://mdc-ftz.4geeks.workers.dev/mcp`): the current FTZ regulations (19 CFR Part 146 and 15 CFR Part 400, refreshed daily from eCFR), the CBP Foreign-Trade Zones Manual, CBP forms and the program's course materials.
- **A skill** that has Claude search the knowledge base and cite its sources whenever a question is about foreign-trade zones, even when the question doesn't mention the knowledge base.

Plugins need a paid Claude plan (Pro, Max, Team or Enterprise). On the Free plan, add the connector on its own instead: https://mdc-ftz.4geeks.workers.dev/add

## Install

1. In Claude, open **Customize > Plugins > Add > Add marketplace** and enter `WaficMikati/mdc-ftz-plugin`.
2. Install **Miami Dade FTZ Knowledge Base**.
3. Open the plugin's **Connectors** tab and click **Connect**. Sign in with your Miami Dade FTZ Knowledge Base email and password, then click **Allow**.

Updates arrive from this repository. To get one right away, select **Check for updates** on the marketplace, or turn on **Sync automatically**.

## Contents

```
.claude-plugin/marketplace.json     the marketplace: lists the plugin below
plugins/mdc-ftz-knowledge/          the plugin: skill and connector address
```

The connector's server code and data are in a separate private repository.
