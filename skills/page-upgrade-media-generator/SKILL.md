---
name: page-upgrade-media-generator
description: Audit, plan, generate, preview, and place content-connected media for webpage upgrades. Use when a page rewrite, SEO refresh, CMS optimization, or content upgrade involves featured images, section graphics, infographics, screenshots, embedded video, stock-photo replacement, media relevance auditing, or media placement. Produces one topical featured image, at least two section-specific secondary images, and an appropriate video recommendation or embed plan. Never publishes without explicit approval.
---
 
# Page Upgrade Media Generator
 
## Purpose
 
Create a complete, content-connected media package for an upgraded webpage.
 
Media must explain, reinforce, or demonstrate the surrounding content. It must never be added merely for decoration.
 
A complete media package normally includes:
 
* Exactly one featured image
* At least two secondary images
* One relevant video, when an appropriate brand-owned video exists
* Descriptive filenames, alt text, captions, and placement instructions
* A self-contained preview showing every asset in context
* Post-publication verification, but only after explicit approval
## Core Principle
 
Every media item must answer this question:
 
> What specific idea, process, comparison, mechanism, example, or argument from the surrounding section does this media help the reader understand?
 
Reject or replace media that cannot answer this clearly.
 
---
 
# Required Inputs
 
Collect or infer the following before beginning:
 
```text
Page URL: {{Page_URL}}
Primary keyword: {{Primary_Keyword}}
Upgraded content outline: {{Content_Outline}}
Existing media inventory: {{Existing_Media}}
Brand colors: {{Brand_Colors}}
Brand wordmark: {{Brand_Wordmark}}
Brand video library: {{Brand_Video_Library}}
CMS type: {{CMS_Type}}
CMS upload or embed method: {{CMS_Upload_Method}}
Additional instructions: {{Additional_Instructions}}
```
 
If essential information is missing, request only the information required for the next step.
 
Do not invent:
 
* Brand assets
* Existing media
* CMS capabilities
* Video ownership
* Live-page verification results
* Publication status
---
 
# Non-Negotiable Rules
 
## 1. Audit Before Generating
 
Inspect the live rendered page whenever access is available.
 
Do not rely only on the CMS content field. Themes, plugins, templates, metadata, widgets, and render-time hooks may inject media that is not visible in the post editor.
 
Inventory all existing media:
 
* Featured image
* In-content images
* Screenshots
* Diagrams
* Galleries
* Embedded videos
* Background images that function as content
* Media injected by themes or plugins
For every item, record:
 
```text
Asset:
Type:
Current location:
Section:
Source or storage location:
Relevant to surrounding content: Yes / Partially / No
Accessibility issue:
Brand issue:
Recommended action: Keep / Replace / Remove / Investigate
Reason:
```
 
Flag the following as defects:
 
* Generic or decorative stock photography
* Images unrelated to the surrounding section
* Screenshots from the wrong product, channel, or workflow
* Competitor or third-party promotional videos
* Empty, vague, duplicated, or keyword-stuffed alt text
* Missing captions where context is needed
* Low-resolution or visibly compressed assets
* Text that becomes unreadable on mobile
* Unknown media storage or injection source
* Duplicate media caused by both content embeds and render-time hooks
Never assume that editing the post body will replace media injected elsewhere.
 
---
 
## 2. Featured Image Requirements
 
Create exactly one featured image.
 
The featured image must:
 
* Be based on the primary keyword and central page topic
* Include a concise headline containing or naturally reflecting the primary keyword
* Use a topical scene or visual metaphor
* Match the visual style of the site’s existing post thumbnails
* Work as both a page thumbnail and social-share image
* Remain legible at small card size
* Use a 16:9 aspect ratio
* Be at least 1200 × 675 pixels
* Be rendered at 2× scale when generated
* Include an SEO-friendly filename
* Include descriptive alt text
The featured image must not:
 
* Be an infographic
* Be a dense diagram
* Contain small body text
* Use generic business imagery unrelated to the topic
* Depend on tiny details to communicate its meaning
* Repeat the full page title when a shorter headline is clearer
Recommended metadata format:
 
```text
Filename: primary-keyword-featured-image.jpg
Alt text: A concise description of the topical scene and its relationship to the page topic.
Title: Human-readable asset title
Purpose: Featured image and Open Graph image
```
 
---
 
## 3. Secondary Image Requirements
 
Create or select at least two secondary images.
 
Prefer original, branded informational graphics over generic stock photography.
 
Suitable formats include:
 
* Process diagrams
* Mechanism chains
* Before-and-after comparisons
* Two-column comparisons
* Decision trees
* Checklists
* Framework diagrams
* Annotated screenshots
* Timelines
* Data visualizations
* Mistake-versus-best-practice graphics
Each image must visualize one exact section argument.
 
Do not create a generic illustration for a broad topic when a specific process, claim, or comparison can be visualized instead.
 
For every secondary image, provide:
 
```text
Target section:
Concept illustrated:
Image format:
Filename:
Alt text:
Caption:
Placement:
Surrounding-copy reference:
Source: Existing asset / Newly generated
```
 
Placement is part of the task.
 
Each secondary image must:
 
* Appear after the heading of the section it supports
* Appear before the next heading of the same or higher level
* Be referenced by nearby copy
* Include a caption when the image benefits from interpretation
* Use descriptive alt text based on the actual visual
* Use an SEO-friendly filename
* Follow the brand’s visual system
Add a natural reference in the surrounding copy, such as:
 
* “As the diagram shows…”
* “The comparison below highlights…”
* “The process can be understood in three stages…”
* “The annotated example illustrates…”
Do not claim that placement is correct until heading order has been verified.
 
---
 
## 4. Existing Asset Reuse
 
Before generating a secondary image, determine whether the site already contains an asset that accurately supports the section.
 
Reuse an existing asset only when it:
 
* Directly matches the section topic
* Uses current branding
* Is sufficiently high resolution
* Has no licensing uncertainty
* Does not contain outdated interfaces or claims
* Improves understanding as well as a newly generated asset would
Do not reuse an asset merely because it is available.
 
Record the source URL or asset identifier for every reused item.
 
---
 
## 5. Video Requirements
 
Prefer the organization’s own videos in this order:
 
1. Product tutorials
2. Educational explainers
3. Webinars
4. Demonstrations
5. Interviews with internal experts
6. Other relevant brand-owned videos
Avoid third-party videos on commercial pages unless the user explicitly approves them and there is no reasonable owned alternative.
 
Never retain:
 
* Competitor videos
* Videos promoting another service provider
* Videos unrelated to the surrounding section
* Broken, private, removed, or region-blocked videos
* Videos with misleading titles or thumbnails
For each proposed video, provide:
 
```text
Video title:
Owner:
URL:
Target section:
Reason it fits:
Embed method:
Connective sentence:
Caption:
Related internal page:
```
 
Add a connective sentence immediately before the video.
 
Add a caption that explains its relevance and, where appropriate, links to a related internal resource.
 
When raw iframes are removed by the CMS sanitizer, use the platform’s native embed format. For WordPress, this may mean placing a supported video URL on its own line rather than inserting raw iframe HTML.
 
After publication, inspect the live page for duplicate videos. A prior video may still be injected through metadata, a block, a shortcode, a theme template, or a render-time hook.
 
---
 
# Media Generation Pipeline
 
## Preferred Generation Method
 
Use an approved image-generation or design tool when one is available.
 
For each generated asset:
 
1. Create the initial asset.
2. Render it at the required dimensions.
3. Inspect it visually.
4. Correct text overflow, clipping, malformed text, collisions, weak contrast, and alignment problems.
5. Re-render.
6. Repeat until the asset passes the quality gate.
7. Optimize the final file.
8. Record filename, dimensions, format, alt text, and intended placement.
Never deliver an unchecked render.
 
## Fallback Method Without an Image API
 
When no AI image API or design tool is available:
 
### Diagrams
 
* Author diagrams as SVG.
* Use the configured brand palette.
* Use a system-safe font stack.
* Keep labels concise.
* Maintain generous padding.
* Use consistent box sizes and connector styles.
* Render at 2× scale using headless Chromium or an equivalent browser renderer.
* Export as optimized PNG when required by the CMS.
### Photo-Style Featured Images
 
* Build the composition as an HTML/CSS scene.
* Use gradients, shapes, icons, illustrations, or licensed visual elements.
* Render through a browser at 2× scale.
* Export as progressive JPEG at approximately quality 85 when gradients or photographic effects are present.
### Optimization
 
Use:
 
* Quantized PNG for flat-color diagrams
* Progressive JPEG for gradient-heavy or photo-style scenes
* SVG only when the CMS and frontend safely support it
Preserve visual quality and text sharpness.
 
---
 
# Upload Fallback
 
When direct CMS access is unavailable but an authenticated browser session and approved upload endpoint are available:
 
1. Reconstruct the SVG or canvas asset in the page context.
2. Render it to a canvas at 2× scale.
3. Convert it with `toBlob`.
4. Upload it through the site’s approved one-time upload endpoint using `FormData`.
5. Set the title, filename, and alt text during upload.
6. Record the returned media URL and identifier.
7. Verify the uploaded asset can be opened directly.
Do not use an undocumented endpoint or bypass authentication controls.
 
---
 
# Brand Configuration
 
Use the supplied brand system whenever available.
 
Default example configuration:
 
```text
Navy: #14243F
Blue: #2E6BF0
Light: #F4F6FA
Muted: #5B6B85
Green: #0E8A4D
Red: #C0392B
 
Font stack:
-apple-system, "Segoe UI", Roboto, Helvetica, Arial, sans-serif
 
Wordmark:
NYTRO in blue
SEO in navy
nytroseo.com beneath or beside the wordmark
Preferred position: bottom center
 
Diagram style:
- Rounded corners: 12–14px
- Alternating navy and blue fills
- White titles
- #C9D4E8 supporting text
- Brand-blue arrows and connectors
```
 
Treat these values as defaults, not universal requirements. Replace them with the actual site brand configuration when supplied.
 
Apply the wordmark only when permitted by the brand guidelines and appropriate for the asset.
 
---
 
# Workflow
 
## Phase 1: Audit
 
1. Inspect the live rendered page.
2. Inventory all existing media.
3. Identify how each asset is stored or injected.
4. Judge relevance, accessibility, quality, ownership, and brand fit.
5. Recommend keep, replace, remove, or investigate.
6. Report all defects before generating replacements.
Deliverable:
 
```text
Media Audit
- Existing asset inventory
- Relevance verdicts
- Accessibility issues
- Brand and ownership issues
- Injection or storage concerns
- Recommended actions
```
 
## Phase 2: Plan
 
Map media to the upgraded content outline.
 
For each planned asset, specify:
 
```text
Asset number:
Asset type:
Target heading:
Purpose:
Visual concept:
Source:
Placement:
Required surrounding-copy change:
```
 
The plan must include:
 
* One featured image
* At least two secondary images
* A video selection or a clear statement that no suitable video is available
Do not force a video into the page when no suitable brand-owned video exists.
 
## Phase 3: Generate or Select
 
1. Generate the featured image.
2. Generate or select at least two secondary images.
3. Select the most appropriate video.
4. Create filenames, alt text, captions, and placement instructions.
5. Inspect every generated asset.
6. Correct visual defects.
7. Optimize the final files.
## Phase 4: Build Preview
 
Create a single self-contained HTML preview showing:
 
* The featured image
* All secondary images
* Captions
* Alt text in the markup
* Video placement or a clearly labeled video placeholder
* Relevant headings and enough surrounding copy to judge context
* Final asset order
Inline local preview assets when practical so the preview does not depend on temporary URLs.
 
Run or perform a heading-order check confirming that each secondary image appears:
 
1. After its assigned section heading
2. Before the next heading of the same or higher level
Confirm that every image loads in the preview.
 
## Phase 5: Stop for Approval
 
Deliver:
 
1. Media audit
2. Asset files
3. Media metadata
4. Self-contained HTML preview
5. Placement map
6. Any unresolved issues
Then stop.
 
Do not:
 
* Upload to the production CMS
* Change the featured image
* Modify the live post
* Replace live embeds
* Update publication dates
* Claim the page has been published
Proceed only after explicit user approval.
 
## Phase 6: Publish After Approval
 
After explicit approval:
 
1. Upload each approved asset.
2. Apply approved filenames, titles, captions, and alt text.
3. Set the approved featured image.
4. Replace preview or placeholder URLs with permanent media URLs.
5. Apply the upgraded content.
6. Apply the approved video embed method.
7. Update the publication date to the current date when required.
8. Never set a future publication time unless explicitly requested.
9. Update FAQ schema when FAQ content changed.
10. Update the tracking dashboard when indexation status changed.
11. Preserve CMS revisions or another rollback path.
## Phase 7: Verify the Live Page
 
Re-open the live rendered page after publication.
 
Verify the actual result of each check:
 
```text
[ ] Featured image loads
[ ] Featured image is the approved asset
[ ] Featured image headline is legible
[ ] All secondary images load
[ ] Each secondary image appears in its assigned section
[ ] Captions display correctly
[ ] Alt text is present in rendered markup
[ ] Video loads and plays
[ ] No duplicate video appears
[ ] No outdated media remains
[ ] No broken image URLs appear
[ ] Schema remains valid
[ ] FAQ schema matches visible FAQ content
[ ] Page template is intact
[ ] Mobile layout remains usable
[ ] Publication date is correct
[ ] No future date was introduced
[ ] Internal links work
[ ] Rollback revision exists
```
 
Do not report a check as passed without observing its actual result.
 
---
 
# Output Contract
 
Deliver outputs in this order.
 
## Before Approval
 
### 1. Media Audit
 
Include:
 
* Existing assets
* Current locations
* Relevance verdicts
* Accessibility issues
* Brand or ownership concerns
* Storage or injection findings
* Recommended actions
### 2. Media Plan
 
Include:
 
* Asset-to-section mapping
* Visual concepts
* Placement instructions
* Copy references
* Proposed video
### 3. Generated Assets
 
Include:
 
* Featured image
* At least two secondary images
* Optimized final files
* Dimensions and formats
* Filenames
* Alt text
* Captions
### 4. Preview
 
Include:
 
* One self-contained HTML preview
* Final media positions
* Surrounding headings and copy
* Working asset references
* Heading-order verification result
### 5. Approval Status
 
End with:
 
```text
Publication status: Not published
Approval required: Yes
```
 
## After Approval
 
### 6. Publish Log
 
Record:
 
```text
Asset:
CMS media ID:
Permanent URL:
Placement:
Alt text applied:
Caption applied:
Publish action:
Result:
```
 
### 7. Live Verification Report
 
Use explicit observed results:
 
```text
Featured image: Pass / Fail — observed result
Secondary image 1: Pass / Fail — observed result
Secondary image 2: Pass / Fail — observed result
Video: Pass / Fail — observed result
Duplicate-media check: Pass / Fail — observed result
Schema check: Pass / Fail — observed result
Template check: Pass / Fail — observed result
Publication-date check: Pass / Fail — observed result
Rollback availability: Pass / Fail — observed result
```
 
Never claim publication succeeded without re-reading the live page.
 
---
 
# Companion Content Rules
 
When the media work is part of a complete page upgrade:
 
* Set the publication date to the current date only when instructed by the page-upgrade workflow.
* Never create a future publication time accidentally.
* Update FAQ schema whenever visible FAQ content changes.
* Keep structured data synchronized with visible content.
* Update the tracking dashboard when indexation status changes.
* Preserve revision history or another rollback mechanism.
These actions remain subject to the approval gate.
 
---
 
# Failure Handling
 
## Live Page Is Inaccessible
 
* State that the live render could not be audited.
* Audit available CMS content or supplied screenshots instead.
* Mark render-time media injection as unresolved.
* Do not claim the audit is complete.
## CMS Storage Location Is Unknown
 
* Investigate post content, metadata, blocks, shortcodes, theme templates, and hooks.
* Mark the item as unresolved until its source is identified.
* Do not remove content blindly.
## No Suitable Brand Video Exists
 
* State that no suitable owned video was found.
* Do not substitute a competitor video.
* Recommend omitting the video or producing a new one.
## Asset Cannot Be Rendered Reliably
 
* Do not deliver the broken asset as final.
* Provide the source file and identify the rendering limitation.
* Mark the asset as incomplete.
## Publication Verification Fails
 
* Record the failed check.
* Restore the prior revision when the failure damages the page.
* Correct the issue and verify again.
* Never report success while defects remain.
---
 
# Quality Gate
 
Verify silently before returning deliverables.
 
## Featured Image
 
* Exactly one featured image exists.
* It is not an infographic.
* It reflects the primary keyword and topic.
* It uses a 16:9 ratio.
* It is at least 1200 × 675.
* It remains legible at thumbnail size.
* It has an appropriate filename and alt text.
## Secondary Images
 
* At least two secondary images exist.
* Each supports one specific section.
* Each is placed inside that section.
* Surrounding copy references each image.
* Each has a caption when needed.
* Each has descriptive alt text.
* Each follows the brand system.
## Video
 
* The video is brand-owned or explicitly approved.
* It matches the target section.
* The embed method is compatible with the CMS.
* A connective sentence appears before it.
* The live page contains no duplicate video after publication.
## Rendering
 
* Every generated image was visually inspected.
* No labels are clipped.
* No text overflows.
* No elements collide.
* Contrast is sufficient.
* Mobile readability is acceptable.
* Final files are optimized.
## Approval and Publication
 
* A preview was delivered before publication.
* Explicit approval was received.
* Publication occurred only after approval.
* The live rendered page was checked afterward.
* Verification results reflect observed behavior.
* A rollback path remains available.
---
 
# Final Status Language
 
Use precise status language.
 
Before approval:
 
```text
Assets generated: Yes
Preview completed: Yes
Published: No
Waiting for explicit approval: Yes
```
 
After successful publication and verification:
 
```text
Assets published: Yes
Live page verified: Yes
Outstanding defects: None
Rollback available: Yes
```
 
When verification is incomplete:
 
```text
Publication action completed: Yes
Live verification completed: No
Reason: {{Reason}}
Status: Unverified
```
 
Never replace an unknown result with an assumption.
