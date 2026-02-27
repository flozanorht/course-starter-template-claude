# Project Context

Red Hat Product Enablement course for IT professionals (developers/sysadmins).

## Critical Constraints

**MUST initialize course project using the included skill before adding any content**

**NEVER modify**:
- `antora-playbook.yml`
- `*.sh` scripts, `devfile.yaml`, `package.json`
- `ui-assets/`, `ui-bundle/`, `supplemental-ui/`, `templates/`

**Watch mode**: Run both `npm run watch:adoc` AND `npm run serve` as background tasks.
- Restart both if `antora.yaml` changes.
- Kill all `npm run watch:adoc` and `npm run serve` processes, if any, before starting or restarting watch mode.

**Autostat watch mode**: start watch mode before making any changes to course content, if not active already. Kill background processes and restart watch mode when necessary.

## Content Structure
This is an Antora documentation project:
- `antora.yml`: course book structure (chapters) and main navigation, chapter ordering
- `modules/`: course content, each subdirectory is a chapter
   - `nav.adoc`: chapter navigation, section or page ordering
   - `pages/`: sections or pages of a chapter, one asciidoc file (`*.adoc`) per section
   - `images/`: optional sudirectory for images of a chapter
   - `attachments/` optional subdirectory for downloadable content of a chapter

## Hints
- Read the AsciiDoc reference: [USAGEGUIDE.adoc](USAGEGUIDE.adoc) when needed
