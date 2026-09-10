# Technical Discovery Checklist

Before building a paid pilot, verify the client environment rather than relying on assumptions.

## Workflow
- Obtain one real completed intervention example.
- Obtain one incomplete/problematic intervention example.
- Confirm mandatory fields for billing.
- Confirm who validates each field.
- Confirm peak intervention volume and concurrent users.

## Existing systems
For every system, record version, hosting model, owner/admin, integration method, authentication, import/export format, licensing constraint, and rollback method.

## Import/export proof
Before automating an import:
1. obtain the vendor/client template or a known-good export/import sample;
2. create one synthetic test record;
3. import into a backup/test company where possible;
4. verify every destination field;
5. test duplicate handling and errors;
6. document the exact encoding, delimiter, date/decimal format, mandatory columns, and naming rules.

Never infer a sales-document import schema from a different EBP product/version.

## Field channel proof
Test with two real technicians:
- text
- voice note
- photo of intervention slip
- photo of supplier receipt/part label
- weak network / delayed send
- duplicate send
- missing mandatory information

Measure time-to-submit and correction rate.

## Security
- No inbound port opening to the office LAN for a pilot unless formally justified.
- Keep credentials out of scenarios/logs where possible.
- Use least privilege.
- Define media retention and deletion.
- Confirm client approval for third-party processing of customer/technician data.

## Go/no-go
Do not move to production build until the critical path has been proven end-to-end with synthetic or non-sensitive test data.