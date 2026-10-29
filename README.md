# CRM Cutover Checker

A browser-local CRM snapshot comparison tool by Orr Yoffe.

[Use the live checker](https://rs.co.il/our-experts/orr-yoffe/tools/crm-cutover-checker/) · [Download the offline ZIP](https://rs.co.il/our-experts/orr-yoffe/tools/crm-cutover-checker/crm-cutover-checker.zip) · [CRM cutover guide](https://rs.co.il/our-experts/orr-yoffe/guides/crm-migration-cutover-reconciliation/)

## Run offline

Download this repository, keep index.html, checker.js and checker.css together, and open index.html in a modern browser. No build step or external libraries are required.

## Inputs

Supply source and target JSON arrays. Each row requires source_id (string), company_id (string or null), email_opt_in (boolean) and sms_opt_in (boolean). The page includes synthetic examples and an optional list of excluded source IDs.

The checker reports duplicate IDs, missing or unexpected rows, company association differences and subscription preference differences. Export exceptions as JSON. Limit: 25,000 rows and 12 MB per snapshot.

## Privacy and limits

Snapshot data is processed locally in your browser. The checker has no upload endpoint, analytics or persistent storage. Portfolio links are ordinary outbound links.

This compares supplied snapshots. It does not certify a complete migration, validate consent provenance, replay events, transfer send authority or replace a cutover plan. Start with synthetic data and follow your organization's data-handling requirements.

## Author

[Orr Yoffe](https://rs.co.il/our-experts/orr-yoffe/) builds web products, acquisition funnels and connected operating systems.
