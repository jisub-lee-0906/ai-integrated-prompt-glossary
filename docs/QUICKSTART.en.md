# AI Prompt Examples for Design, Video & Development

**12 practical examples for design, video and development.**

[English overview](../README.en.md) · [English A–Z glossary](../glossary/ENGLISH_INDEX.md) · [Reference by field](../glossary/README.md) · [Korean production briefs](../examples/README.md)

Use **subject + action + constraints + settings + deliverables + acceptance checks**. Replace the project assumptions and sample numbers before using an example. For image and video tools, use the visual instruction for generation and apply file-format or timing requirements in the relevant export or editing tool. For coding tasks, specify your existing stack and ask for actual execution evidence.

The complete term explanations and book are primarily Korean. These English examples are a separate starting guide, not a full translation or a claim that every tool supports every request.

## Contents

1. [Responsive landing page](#01-responsive-landing-page)
2. [Multilingual design system](#02-multilingual-design-system)
3. [Print-ready brochure](#03-print-ready-brochure)
4. [Game-ready 3D prop](#04-game-ready-3d-prop)
5. [Product reveal shot](#05-product-reveal-shot)
6. [Seamless brand animation](#06-seamless-brand-animation)
7. [Interview edit and captions](#07-interview-edit-and-captions)
8. [Screen replacement](#08-screen-replacement)
9. [Booking API](#09-booking-api)
10. [Large searchable list](#10-large-searchable-list)
11. [Background image-processing jobs](#11-background-image-processing-jobs)
12. [Cross-discipline campaign handoff](#12-cross-discipline-campaign-handoff)

## 01. Responsive landing page

**Vague:** “Make a modern landing page.”

```text
Build a landing page for a small-team project management service using the
existing project stack. Make the core value and one primary trial CTA clear.
Use reusable Button and FeatureCard components with semantic design tokens.
Use a 12-column desktop grid and a single-column mobile layout as a starting point.
Check long labels, keyboard navigation, visible focus, and content overflow
at 320, 768 and 1280 CSS pixels. Connect the CTA to its real destination.
Deliver the working project and report the build and checks actually run.
```

**Check:** Intermediate widths also work; a screenshot does not establish working navigation.

[Visual Hierarchy](../glossary/D2.md#d2-01) · [Design Tokens](../glossary/D2.md#d2-07) · [Responsive Breakpoint](../glossary/S1.md#s1-02)

## 02. Multilingual design system

**Vague:** “Create consistent components.”

```text
Define semantic color, typography, spacing and radius tokens for a dashboard.
Create Button, Input, Alert and Card variants with explicit size, intent and state.
List valid combinations, including loading, disabled and error states.
Support Korean, English and long translated labels through content-driven layout.
Provide editable components, token data and rendered examples of each valid state.
Verify light and dark themes, contrast, focus and text expansion.
```

**Check:** Changing a semantic token updates the intended components without changing unrelated roles.

[Component Variants](../glossary/D2.md#d2-06) · [Auto Layout](../glossary/D2.md#d2-04) · [Font Embedding](../glossary/D3.md#d3-10)

## 03. Print-ready brochure

**Vague:** “Export a professional PDF.”

```text
Prepare separate digital-reading and print-delivery PDFs for this brochure.
Keep searchable text, embedded fonts and navigation links in the digital edition.
For print, obtain the printer's final trim size, bleed, color profile and PDF
requirements before applying them. Check effective image PPI at placed size,
spot colors and overprint behavior. Keep headings with the following content.
Render every final page and report unresolved production requirements.
```

**Check:** A filename or color-mode label alone does not prove compliance with the printer's specification.

[Bleed](../glossary/D4.md#d4-06) · [ICC Profile](../glossary/D4.md#d4-02) · [Preflight](../glossary/X1.md#x1-10)

## 04. Game-ready 3D prop

**Vague:** “Make a low-poly supply crate.”

```text
Create an editable supply-crate asset for the specified game engine.
Confirm units, triangle budget, material count and texture resolution first.
Keep the handle, hinge and label positions consistent across reference views.
Prioritize silhouette and moving parts in topology. Check UV distortion,
padding and texel density. Bake fine detail into the appropriate normal-map space.
Deliver the mesh, textures and an engine-import check, not just a rendered image.
```

**Check:** The asset imports at the expected scale with correct normals, materials and pivot placement.

[Topology](../glossary/D8.md#d8-01) · [UV Unwrapping](../glossary/D8.md#d8-03) · [Normal Map](../glossary/D8.md#d8-06)

## 05. Product reveal shot

**Vague:** “Make it cinematic.”

```text
Create a slow dolly-in toward the stationary product, moving from a medium shot
to a close-up. Preserve its silhouette, button count, logo position and proportions.
Let background parallax and reflections change naturally with camera movement.
Use controlled soft lighting and avoid abrupt path changes or object morphing.
In the editing/export stage, apply the agreed duration, aspect ratio, frame rate
and delivery codec; verify the exported file's actual metadata.
```

**Check:** Camera movement should not be replaced by product growth or a fixed-position zoom.

[Dolly In / Out](../glossary/V1.md#v1-03) · [Zoom](../glossary/V1.md#v1-05) · [Frame Rate](../glossary/V5.md#v5-02)

## 06. Seamless brand animation

**Vague:** “Make the logo loop smoothly.”

```text
Animate a four-second logo loop at 24 fps in an editable timeline.
Define periodic motion with continuous position and velocity across the loop boundary.
Export 96 frames sampled from frame 0 through 95; do not append a duplicate start frame.
Keep lighting, shadows and any background motion continuous as well.
Provide the editable curves and a preview that repeats ten times for inspection.
```

**Check:** Matching the first and last image is not sufficient if the motion changes speed abruptly at the seam.

[Seamless Loop](../glossary/V3.md#v3-04) · [Easing](../glossary/V3.md#v3-02) · [Keyframe](../glossary/V3.md#v3-01)

## 07. Interview edit and captions

**Vague:** “Clean up the interview.”

```text
Edit the interview for clarity while preserving the speaker's meaning.
Use J and L cuts where appropriate and retain natural word endings and breaths.
Match dialogue levels and apply noise reduction conservatively.
Set loudness and true-peak limits from the destination's confirmed specification.
Provide timed captions with readable line breaks, speaker identification when needed,
and meaningful non-speech information. Check the final encoded program.
```

**Check:** Listen for altered meaning, missing syllables, excessive denoising and caption timing errors.

[J-cut / L-cut](../glossary/V2.md#v2-02) · [Loudness](../glossary/V6.md#v6-02) · [Captions](../glossary/V6.md#v6-09)

## 08. Screen replacement

**Vague:** “Put this graphic on the laptop.”

```text
Replace the laptop display with the supplied graphic using a planar track.
Maintain the screen's perspective and inspect the track during blur and occlusion.
Rotoscope foreground fingers where needed. Match reflections, grain, exposure
and motion blur to the plate. Check straight versus premultiplied alpha handling.
Deliver the editable composite, tracked corner-pin data and final rendered shot.
```

**Check:** Look for corner drift, graphics covering fingers, matte halos and mismatched sharpness.

[Planar Tracking](../glossary/V4.md#v4-06) · [Rotoscoping](../glossary/V4.md#v4-02) · [Alpha Interpretation](../glossary/V4.md#v4-04)

## 09. Booking API

**Vague:** “Build reservations without errors.”

```text
Define the reservation API's input, output, validation and error contracts first.
Authenticate the caller and enforce resource ownership on the server.
Prevent double booking with database constraints and an atomic transaction boundary.
Define idempotency-key scope, request-body matching, retention and concurrent-retry behavior.
Reuse an existing result for the same valid key. Handle payment-provider side effects
separately from the local database transaction. Test concurrency and lost responses.
```

**Check:** Retrying after a lost response does not create another reservation; other users cannot access it.

[Idempotency](../glossary/S2.md#s2-06) · [Transaction](../glossary/S3.md#s3-05) · [Authorization](../glossary/S6.md#s6-01)

## 10. Large searchable list

**Vague:** “Make search fast.”

```text
Use server pagination with a deterministic createdAt-plus-id ordering.
Keep the query in the URL and use a 300 ms debounce as an initial design choice.
Keep typing responsive and prevent stale responses from overwriting newer results.
Define loading, empty, error and retry states. Inspect the query plan and avoid N+1 reads.
Measure response latency under representative data volume and report the test conditions.
```

**Check:** Artificially delay an older request and confirm it cannot replace the latest search results.

[Pagination](../glossary/S2.md#s2-05) · [Query Plan](../glossary/S3.md#s3-10) · [Race Condition](../glossary/S7.md#s7-05)

## 11. Background image-processing jobs

**Vague:** “Process uploads in the background.”

```text
Return a job ID from the API and process images through a bounded worker queue.
Define queued, running, succeeded, failed and cancelled states.
Set concurrency and memory limits, timeouts, retry eligibility and retry budgets.
Make repeated job delivery safe and define recovery after a worker exits.
Carry a job ID through logs and traces. Test queue saturation, worker failure,
duplicate delivery and cancellation before claiming the workflow is complete.
```

**Check:** Queue growth and resource use stay bounded, and completed work is not duplicated after recovery.

[Queue / Backpressure](../glossary/S7.md#s7-07) · [Retry / Backoff](../glossary/S7.md#s7-08) · [Observability](../glossary/S8.md#s8-03)

## 12. Cross-discipline campaign handoff

**Vague:** “Create the whole campaign.”

```text
Define fixed product features and shared brand tokens before creating variants.
Prepare the image crops, product video, loop and responsive landing as separate deliverables.
Keep an asset manifest with stable IDs, versions, source files and approved derivatives.
Assign generation, editing and export responsibilities to the appropriate tools.
Verify actual dimensions, alpha, codecs, captions and website behavior against each specification.
Deliver editable sources and identify unresolved dependencies or unverified requirements.
```

**Check:** A second person can identify the approved assets and reproduce the required derivatives.

[Asset Manifest](../glossary/X1.md#x1-06) · [Delivery Specification](../glossary/X1.md#x1-04) · [Reference Consistency](../glossary/X2.md#x2-10)

---

Written with AI assistance. © 2026 이지섭 (Jisub Lee). [Usage terms](../LICENSE.md) · [Suggest a correction](https://github.com/jisub-lee-0906/ai-integrated-prompt-glossary/issues/new?template=correction.yml)
