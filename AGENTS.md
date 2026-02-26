# Project Context

Red Hat Product Enablement course for IT professionals (developers/sysadmins).

## Critical Constraints

**MUST run before first commit**: `course-init.sh`

**NEVER modify**:
- `*.sh` scripts, `devfile.yaml`, `package.json`
- `ui-assets/`, `ui-bundle/`, `supplemental-ui/`, `templates/`

**Watch mode**: Run both `watch:adoc` AND `serve` as background tasks. Restart both if `antora.yaml` changes.

**Autostat watch mode**: start watch mode before making any changes to course content, if not active already.

## Content Structure

- Course content: `modules/` (Antora structure)
- Navigation: [antora.yml](antora.yml) + `nav.adoc` per chapter
- AsciiDoc reference: [USAGEGUIDE.adoc](USAGEGUIDE.adoc) (read when needed)
