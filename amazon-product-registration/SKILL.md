---
name: amazon-product-registration
description: Prepare, review, and troubleshoot Amazon Japan product registration, bulk-upload templates, product-type and browse-node selection, variation relationships, and source-master mapping. Use for Seller Central catalog creation and listing-data preparation; do not treat ordinary inventory or price-only updates as new product registration.
---

# Amazon Product Registration

Use the current Amazon Japan Seller Central template and help available at execution time. Templates, required fields, valid values, variation themes, and UI labels can change.

## Start by classifying the task

Determine whether the request is:

- creating a new Amazon catalog item or ASIN;
- adding an offer to an existing ASIN;
- preparing a bulk product-registration template;
- creating or repairing a variation family;
- updating product-page content;
- or only updating inventory, price, lead time, or fulfillment data.

Do not use product-registration rules as authority for an inventory-only update. Read [references/official-sources.md](references/official-sources.md) when the distinction or current Seller Central flow matters.

## Core workflow

1. Confirm scope, marketplace, account/store, source files, target template, and whether the action is draft preparation or live submission.
2. Confirm whether the product matches an existing ASIN before creating a new catalog item.
3. Select the product type first. Then use the fields, valid values, and conditional requirements in the generated template.
4. Map source data by semantic field meaning, not by fixed Excel column letters alone.
5. Separate confirmed values, derived values, and unknown values. Never silently invent a value required for submission.
6. For uncertain category, product type, browse node, material, package, safety, or compliance fields, record the uncertainty and request evidence or owner confirmation.
7. Start with one to three products, review the processing report, and expand only after errors are resolved.
8. Report what was entered, what was inferred, what remains blank, and what must be confirmed before upload.

Read [references/bulk-registration.md](references/bulk-registration.md) for template preparation and test uploads. Read [references/variations.md](references/variations.md) for parent-child work. Read [references/source-master-mapping.md](references/source-master-mapping.md) when transferring from a supplier or client master.

## Non-negotiable checks

- Preserve identifiers exactly: SKU, ASIN, JAN/EAN/UPC, parent SKU, child SKU, and product type.
- Copy identifiers instead of retyping where possible. Japanese-market ASINs are normally 10 characters; verify against Seller Central or the product URL.
- Confirm current required and conditionally required fields from the actual template.
- Do not equate product weight with package weight unless the source explicitly establishes that they are the same.
- Do not infer price, cost, package dimensions, legal claims, battery details, dangerous-goods status, or country of origin without evidence.
- Treat upload or live Seller Central submission as a separate external action requiring explicit authorization.
- Preserve client source data and generated drafts separately. Do not overwrite the source master.

## Canonical knowledge

For the user's company, Google Drive is the canonical knowledge and output store. The public GitHub skill contains reusable workflow rules only. Client data, credentials, prices, account details, processing reports, and approved deliverables remain in authorized Google Drive locations.
