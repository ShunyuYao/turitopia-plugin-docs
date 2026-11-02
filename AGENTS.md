# Documentation maintenance

- This repository maintains shared README context and templates for Turi Topia (吐梨邦) plugins and related developer tools.
- Keep the introduction brief, followed by https://turitopia.com/ and the public scaffolding, SDK types, and registry links.
- The user's convention, confirmed on 2026-11-02, applies to all plugin-related READMEs and every existing language version.
- Preserve product attribution: a plugin runs within Turi Topia; a developer tool must describe its actual ecosystem role.
- Keep README.md, README.en.md, templates/, and snippets/ consistent. The marked context block must match its language's snippet.
- Every plugin README must state actual marketplace status, listed version, last verification date, evidence, and in-app verification separately. Keep all language versions consistent; use Not applicable for documentation and developer tools. The marked marketplace block must match its language's snippet.
- Verify live registry and blocklist data by plugin ID/version. Do not infer listing from public source, a GitHub Release, or an unmerged PR; do not infer successful in-app installation from registry data alone. Preserve the old listed version when a newer version is under review. Failed lookups mean Unverified, not Not listed.
- Keep repository and package identifiers unchanged. The English product name is Turi Topia.
- Do not add API claims or copy version-sensitive SDK tables here; link to the owning public repository.
- Do not expose restricted host installers, update feeds, storage locations, credentials, local account data, or private repository links.
- Review actual published files and relative links before pushing. Documentation-only changes do not require application E2E.
- Creating or updating these templates does not automatically update other repositories. Report adoption only when the corresponding changes have actually been committed.
