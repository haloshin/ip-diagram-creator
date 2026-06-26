# Security Policy

`ip-diagram-creator` may be used with personal photos, profile screenshots, creator bios, private drafts, and generated character assets. Treat these inputs as sensitive user materials.

## Do Not Commit

Do not commit:

- Original user photos or private screenshots.
- User-private character anchor sheets or action sheets.
- Client materials, account dashboards, private chat screenshots, contact details, or customer data.
- Access keys, local environment files, or private endpoints.
- Generated images that contain private people, private brands, or unpublished customer context.

## Safe Examples

Repository examples should use:

- Publicly authorized demo images.
- Placeholder personas.
- Redacted screenshots.
- Generic examples with no private path, account, customer, or access material.

## Suggested Pre-Push Scan

Before pushing, run your normal sensitive-content scanner and review all matches manually.

Also check for local machine paths, internal project names, customer names, private screenshots, and unpublished brand material. Documentation examples are acceptable; real private material is not.

## Reporting

If you find private material or a security issue in this repository, please open a GitHub issue without including the sensitive content itself. Describe the affected file and the type of issue so it can be removed or corrected.
