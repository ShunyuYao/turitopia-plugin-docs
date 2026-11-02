# Turi Topia Plugin Documentation

[简体中文](README.md) · English

<!-- turitopia:context:start -->
## About Turi Topia

**Turi Topia (吐梨邦) is an AI desktop companion app for chatting, interacting, and visiting friends' desktops. Plugins add new capabilities.**

Website: [turitopia.com](https://turitopia.com/)

## Plugin ecosystem

| Public repository | Purpose |
| --- | --- |
| [create-pet-plugin](https://github.com/ShunyuYao/create-pet-plugin) | Plugin scaffolding and development guide. Start a new plugin here. |
| [pet-plugin-types](https://github.com/ShunyuYao/pet-plugin-types) | Plugin SDK types and API contracts. Look up available capabilities and interfaces. |
| [pet-plugin-registry](https://github.com/ShunyuYao/pet-plugin-registry) | Marketplace registry, submission instructions, and review policies. |
<!-- turitopia:context:end -->

## What this repository provides

Shared introductions and bilingual README templates for Turi Topia plugins. Use a full template for a new plugin, or add a context block to an existing README while preserving its installation, configuration, and usage documentation.

| File | Purpose |
| --- | --- |
| [Chinese README template](templates/README.md) | A Chinese README to copy and customize for a new plugin. |
| [English README template](templates/README.en.md) | The matching English README. |
| [Chinese context block](snippets/context.zh-CN.md) | A short product introduction, website, and ecosystem links for existing Chinese READMEs. |
| [English context block](snippets/context.en.md) | The matching block for existing English READMEs. |
| [Chinese marketplace status block](snippets/marketplace.zh-CN.md) | Record listing status, marketplace version, verification date, and evidence. |
| [English marketplace status block](snippets/marketplace.en.md) | The matching status block for existing English READMEs. |

## How to adopt

1. For a new project, copy both templates to its root as `README.md` and `README.en.md`. Replace every `{{…}}` placeholder. Language-switch links are included.
2. For an existing project, place the appropriate context block near the beginning, before installation instructions. Keep the original content and filenames, and adjust language-switch links as needed. A bilingual README needs the context in both language sections.
3. Follow the shared context with the plugin's purpose, supported versions, installation, and configuration. Check these against the actual release; keep planned, unimplemented, and unreleased features clearly labeled.
4. Complete “Marketplace status” before installation instructions. Existing projects can copy the status block. Keep status, version, date, and evidence consistent across languages.

## Recording marketplace status

- Choose the actual state: Listed, Under review, Not listed, Delisted or blocked, or Unverified. Use Not applicable for SDKs, scaffolding tools, and this documentation repository.
- Check the plugin ID and version against the [official registry](https://github.com/ShunyuYao/pet-plugin-registry/blob/main/registry/plugins.json) and [blocklist](https://github.com/ShunyuYao/pet-plugin-registry/blob/main/registry/blocklist.json). Record the verification date and pinned commit links; link a real review PR for pending submissions. If verification fails, report Unverified rather than inferring Not listed.
- Distinguish the marketplace version from source versions and GitHub Releases. If an older version is listed while an update is under review, retain both states. Creating a Release or submitting a PR alone does not mean the plugin is listed.
- Record in-app visibility and download/installation checks separately. Registry verification does not replace running the app. A claim of a successfully verified launch needs marketplace visibility and installation evidence for that version; label incomplete checks as unverified.
- Update every language after listing, updates, removal, or blocking. The verification date records a point in time, not a guarantee of permanent availability.

This repository contains documentation and templates. Its marketplace status is Not applicable; it is not distributed as a marketplace plugin.

## Convention for all plugin-related READMEs

- Briefly explain Turi Topia, link its website, and link the three key public repositories near the beginning.
- Plugin READMEs must identify the project as a Turi Topia plugin. SDK, scaffolding, and registry READMEs should describe their actual role in the ecosystem.
- Use “吐梨邦（Turi Topia）” in Chinese and “Turi Topia (吐梨邦)” in English. Preserve repository names, package names, and API identifiers.
- Include this context in Chinese, English, and every other existing language version.
- This repository owns introductions, links, and README structure. API contracts remain in the types repository, project creation in the scaffolding repository, and marketplace policies in the registry.
- The website is the product information entry point. Do not include restricted host installers, update feeds, or storage locations. Public plugin source alone does not imply marketplace availability or compatibility with every host release.

This convention records the user's decision of November 2, 2026. Future plugin READMEs should follow it. Adoption in existing repositories is tracked by their actual commits; creating this repository does not mean the migration is complete.
