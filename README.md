# Fiatto for Claude

Fiatto is a procurement and finance platform for European companies: purchase
requests, purchase orders, invoices, contracts, sales and the general ledger in
one place. This plugin adds the Fiatto connector to Claude together with six
ready-made tasks, so you ask for the result instead of working out which data
to fetch.

## What you can ask

| Task | Ask for example |
|---|---|
| Open invoices | "Which purchase invoices are overdue or due this week?" |
| Supplier dossier | "Prepare my meeting with Acme: contracts, orders, invoices." |
| Approval queue | "Which purchase requests are waiting for approval, and what stands out?" |
| Trial balance review | "Review the trial balance as of last month-end." |
| Receivables follow-up | "Who owes us money, and draft a reminder for the oldest." |
| Contract renewals | "Which contracts can we still cancel in the next 90 days?" |

The tasks work in Dutch, English and any other language you write in.

## Getting started

1. An administrator turns on assistants for the company in Fiatto, under
   Settings, Integrations. This is off by default.
2. Add this plugin, open its **Connectors** tab and connect Fiatto. Installing
   the plugin does not connect it: you sign in with your own Fiatto account,
   choose the company and confirm what Claude may read.
3. Ask one of the questions above.

## What it does not do

This version only reads. It never pays, releases payment batches, changes bank
details, posts to the ledger, approves anything, deletes anything or manages
users. A reminder is a draft for you to send yourself. Decisions stay in Fiatto.

## Your data

The plugin sends your questions to the Fiatto connector at
`https://fiatto.app/api/v1/mcp` and shows you what comes back. It stores nothing
itself and contacts no other service. Claude sees exactly what you may see in
Fiatto, and confidential contracts are left out. Journal entries and the trial
balance are only available to approvers and accountants. Every question is
recorded in the company's audit trail, and you can revoke the connection at any
time under Settings, Integrations.

Documentation: <https://fiatto.app/en/platform/assistenten>
Privacy policy: <https://fiatto.app/privacy>
Support: <support@fiatto.app>
