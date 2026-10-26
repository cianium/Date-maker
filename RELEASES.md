# Date-maker — GitHub Releases and Version History

**Reviewed:** 2026-10-26

## Verified releases

| GitHub Release | Classification | Published (UTC) | Tag commit | Attached Release assets |
| :-- | :-- | :-- | :-- | :-- |
| [v1.0](https://github.com/cianium/Date-maker/releases/tag/v1.0) | Pre-release | 2026-10-18 02:19:51 | `7edc37778f6dbe4fb2146fa08ff2ad83621576fa` | 0 |
| [v1.2](https://github.com/cianium/Date-maker/releases/tag/v1.2) | Pre-release | 2026-10-18 02:20:43 | `7edc37778f6dbe4fb2146fa08ff2ad83621576fa` | 0 |

**Important discrepancy:** Both tags reference **the exact same commit**. There is no verifiable source change between `v1.0` and `v1.2`; a higher version label alone does not establish updated functionality.

Release descriptions link externally uploaded `Make-a-Date-main.zip` and `Date-maker-main.zip` files via GitHub user attachments, **not** files in the official Release Assets section. Their contents and correspondence with the tagged source have **not** been verified.

The current `main` branch includes later commits, including repository documentation and removal of a hard-coded SMS recipient from `index.html`. This does **not** rewrite historical tags or remove the original value from Git history and already-copied distributions.

- [Compare v1.0 and v1.2](https://github.com/cianium/Date-maker/compare/v1.0...v1.2)
- [Compare v1.2 with main](https://github.com/cianium/Date-maker/compare/v1.2...main)
- [Current source](https://github.com/cianium/Date-maker/tree/main)

## Release description corrections — proposed, not applied

**For existing `v1.0` (keep Pre-release):**

Suggested title: `v1.0 — Original interactive page preview`

> Historical preview of a simple Persian/English static web interaction built with HTML, CSS and JavaScript. This is not a booking or calendar service. The source includes an image, an audio file and a client-side SMS launch flow.
>
> **Privacy notice:** This historical tag predates removal of a hard-coded SMS recipient. Check the source and any attached archive before reusing it or redistributing it.
>
> **Copyright notice:** Confirm permissions for bundled audio and images; public repository access does not grant redistribution rights.
>
> Tagged source: https://github.com/cianium/Date-maker/tree/v1.0

**For existing `v1.2` (keep Pre-release):**

Suggested title: `v1.2 — Historical preview tag (same source as v1.0)`

> This label points to **the same Git commit** as `v1.0`. There is no code diff between the tags. The ZIP file linked in the original description is an external user attachment and has not been inspected or matched to this tag.
>
> **Privacy notice:** This historical tag contains source predating the SMS-recipient cleanup. Do not reuse it as a privacy-safe build without review.
>
> Tagged source: https://github.com/cianium/Date-maker/tree/v1.2
>
> Diff: https://github.com/cianium/Date-maker/compare/v1.0...v1.2

These are **proposed edits to GitHub Release descriptions**. They have not been saved to the published releases because the currently connected GitHub tools do not support editing release metadata.

## Future release policy

1. Do **not** force-move historical `v1.0` or `v1.2` tags; preserve truthful history.
2. Never include personal phone numbers or private details in the new source or release archives.
3. Confirm copyright permission or replace/remove third-party media before packaging.
4. Test mouse, touch and keyboard access, narrow screens, dismissal of dialogs, respectful user choices and reduced-motion settings.
5. Review how the `sms:` link behaves on mobile; opening an SMS composer is **not** sending/delivering a message.
6. Publish a new pre-release only from a **new, tested commit**, with accurate notes and, if needed, an actual Release Asset ZIP whose contents correspond to the source.
7. Do not claim the project is a scheduling/booking application without implementing those capabilities.

**Release decision:** No additional GitHub Release or tag has been created in this documentation update.
