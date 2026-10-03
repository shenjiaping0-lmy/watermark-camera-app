---
name: "现场水印相机"
description: "面向户外现场记录的高对比市政导视式 Android 水印相机视觉系统。"
colors:
  ink-navy: "#0e1830"
  ink-soft: "#41506b"
  daylight-paper: "#f4f7fb"
  daylight-white: "#ffffff"
  mineral-line: "#cfd7e4"
  municipal-blue: "#114ccf"
  municipal-blue-deep: "#0a328f"
  safety-amber: "#f2b705"
  field-danger: "#b42318"
  field-success: "#137a46"
typography:
  headline:
    fontFamily: '"Noto Sans SC", "PingFang SC", "Microsoft YaHei", system-ui, sans-serif'
    fontSize: "1.35rem"
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: "-0.025em"
  title:
    fontFamily: '"Noto Sans SC", "PingFang SC", "Microsoft YaHei", system-ui, sans-serif'
    fontSize: "1.05rem"
    fontWeight: 700
    lineHeight: 1.15
    letterSpacing: "-0.02em"
  body:
    fontFamily: '"Noto Sans SC", "PingFang SC", "Microsoft YaHei", system-ui, sans-serif'
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.5
  label:
    fontFamily: '"Noto Sans SC", "PingFang SC", "Microsoft YaHei", system-ui, sans-serif'
    fontSize: "0.78rem"
    fontWeight: 800
    lineHeight: 1.5
    letterSpacing: "0.05em"
  action:
    fontFamily: '"Noto Sans SC", "PingFang SC", "Microsoft YaHei", system-ui, sans-serif'
    fontSize: "0.92rem"
    fontWeight: 850
    lineHeight: 1.5
  watermark:
    fontFamily: '"Noto Sans SC", "PingFang SC", "Microsoft YaHei", system-ui, sans-serif'
    fontSize: "clamp(0.9rem, 3.8vw, 1.12rem)"
    fontWeight: 800
    lineHeight: 1.28
    letterSpacing: "-0.015em"
rounded:
  control: "10px"
  action: "11px"
  shell: "18px"
  brand-cut: "10px 10px 3px 10px"
  pill: "999px"
  circle: "50%"
spacing:
  hairline-gap: "3px"
  compact: "7px"
  control: "10px"
  cluster: "14px"
  gutter: "18px"
  section: "20px"
components:
  button-primary:
    backgroundColor: "{colors.municipal-blue}"
    textColor: "{colors.daylight-white}"
    typography: "{typography.action}"
    rounded: "{rounded.action}"
    padding: "10px 14px"
    height: "52px"
  button-primary-hover:
    backgroundColor: "{colors.municipal-blue-deep}"
    textColor: "{colors.daylight-white}"
    typography: "{typography.action}"
    rounded: "{rounded.action}"
    padding: "10px 14px"
    height: "52px"
  button-secondary:
    backgroundColor: "{colors.daylight-white}"
    textColor: "{colors.ink-navy}"
    typography: "{typography.action}"
    rounded: "{rounded.action}"
    padding: "10px 14px"
    height: "52px"
  input-field:
    backgroundColor: "{colors.daylight-white}"
    textColor: "{colors.ink-navy}"
    typography: "{typography.body}"
    rounded: "{rounded.control}"
    padding: "11px 13px"
    height: "50px"
  segment-option-selected:
    backgroundColor: "{colors.municipal-blue}"
    textColor: "{colors.daylight-white}"
    typography: "{typography.label}"
    rounded: "{rounded.control}"
    height: "44px"
  watermark-address:
    backgroundColor: "{colors.municipal-blue}"
    textColor: "{colors.daylight-white}"
    typography: "{typography.watermark}"
    padding: "8px 11px 9px"
---

# Design System: 现场水印相机

## Overview

**Creative North Star: "The Enamel Street Plate"**

The system feels like a piece of civic field equipment: daylight white and mineral gray form the work surface, while municipal blue supplies the authority and instant recognition of an enamel address sign. Ink navy keeps information legible without the glare of pure black, and a narrow safety-amber signal marks decisive capture-related moments.

The visual language is dense, direct, and structural. Full-width rails, visible alignment, and compact labels organize information without relying on floating cards. Mildly rounded controls remain practical for touch, while square-cut sign geometry preserves the municipal character. Expression always yields to capture state, metadata legibility, and outdoor contrast.

**Key Characteristics:**

- Municipal blue as the single dominant identity and interaction color.
- Daylight-ready contrast with ink navy text on white or mineral-gray surfaces.
- Structural rails and shared gutters instead of decorative card stacks.
- Compact information density with touch targets of at least 44px.
- Square-cut enamel-sign geometry balanced by restrained control rounding.
- One purposeful capture-stamp motion moment, with reduced-motion support.

## Colors

The palette combines civic authority with field-tool clarity: blue establishes trust and selection, amber signals decisive action, and cool neutrals carry almost all remaining structure.

### Primary

- **Municipal Blue** (`colors.municipal-blue`): Brand marks, selected segments, primary actions, focus emphasis, selection color, and the address-plate field.
- **Deep Municipal Blue** (`colors.municipal-blue-deep`): Hover reinforcement for blue actions; it is a state color, not a second accent.

### Secondary

- **Safety Amber** (`colors.safety-amber`): A scarce capture signal used for the decisive empty-state action, shutter feedback, and the lower rule on the address plate.

### Tertiary

- **Field Success** (`colors.field-success`): Positive, local-processing status only.
- **Field Danger** (`colors.field-danger`): Error feedback and blocking messages only.

### Neutral

- **Ink Navy** (`colors.ink-navy`): Primary text, dark overlays, and high-contrast feedback surfaces.
- **Soft Ink** (`colors.ink-soft`): Explanatory copy and secondary status text.
- **Daylight Paper** (`colors.daylight-paper`): The cool page field surrounding the tool.
- **Daylight White** (`colors.daylight-white`): Primary working surfaces and inverse text.
- **Mineral Line** (`colors.mineral-line`): Dividers and structural boundaries.

### Named Rules

**The Signal Color Rule.** Municipal blue carries identity and selection; safety amber appears only at capture-related moments or as the address-plate rule, never as generic decoration.

**The Daylight Contrast Rule.** Default to ink navy on daylight white and reserve translucent light text treatments for dark image-backed regions with a supporting overlay.

## Typography

**Headline Font:** Noto Sans SC with PingFang SC, Microsoft YaHei, system UI, and sans-serif fallbacks  
**Body Font:** Noto Sans SC with PingFang SC, Microsoft YaHei, system UI, and sans-serif fallbacks  
**Label Font:** The same system Chinese stack, using weight and spacing rather than a second family

**Character:** The typography is utilitarian, compact, and legible offline. Weight carries hierarchy, tight negative tracking keeps short titles crisp, and tabular numerals stabilize time displays.

### Hierarchy

- **Headline** (700, `typography.headline`): Short empty-state or instructional headings.
- **Title** (700, `typography.title`): Compact identity and tool titles.
- **Body** (400, `typography.body`): Field values and general interface copy.
- **Label** (800, `typography.label`): Rails, field labels, status labels, and compact control copy.
- **Action** (850, `typography.action`): Primary and secondary action labels where immediate recognition matters.
- **Watermark** (800, `typography.watermark`): Address content inside the enamel-sign treatment.

### Named Rules

**The Field-Legibility Rule.** Use the Chinese system sans stack and tabular numerals for timestamps; core comprehension must never depend on a downloaded font.

## Layout

The system is mobile-first and centered inside a single working shell. The shell fills the viewport on phones and stops at 620px on larger displays. Its primary structural inset is an 18px gutter, repeated across rails, fields, action zones, and supporting notes.

Viewfinder or media surfaces may run edge to edge inside the shell and use a 4:5 frame, with overlays aligned to 16px internal offsets. Secondary information stays compact and follows a 7–14px internal rhythm. Full-width rails separate modes or groups; they should not become floating containers.

At 390px and below, dense two-column control groups collapse to one column and nonessential badge text may reduce to an icon or status dot while preserving the touch target. At 760px and above, the shell gains outer breathing room and an 18px clipped corner; sticky phone chrome returns to normal document flow.

**The Structural Rail Rule.** Use full-width rails, shared 18px gutters, and visible one-pixel boundaries to establish hierarchy; do not replace them with a stack of detached cards.

## Elevation & Depth

Depth is neutral and functional. Tonal layering and one-pixel borders establish most hierarchy; shadows are reserved for the centered shell on wide screens, elevated actions, camera controls, transient feedback, and image overlays that must survive varied photography.

### Shadow Vocabulary

- **Shell Lift** (`0 0 0 1px rgba(0,0,0,.04), 0 24px 80px rgba(0,0,0,.1)`): Separates the bounded tool from the desktop paper field.
- **Floating Feedback** (`0 14px 36px rgba(8,30,72,.16)`): Supports toast-like transient feedback without turning it into a modal.
- **Primary Action Lift** (`0 9px 20px rgba(17,76,207,.26)`): Used only beneath the main blue action.
- **Image Overlay Lift** (`drop-shadow(0 6px 13px rgba(0,0,0,.34))`): Keeps sign-like overlays readable against unpredictable imagery.

### Named Rules

**The Flat-Until-Useful Rule.** Keep working surfaces flat at rest; add elevation only when it clarifies containment, action priority, or legibility over imagery.

## Shapes

Controls use gently rounded rectangles: 10px for fields, segmented controls, and compact actions; 11px for large actions. The larger desktop shell uses an 18px corner, while rails and sign surfaces remain square to preserve the civic grid. The brand mark uses one clipped corner, echoing a mounted street plate without turning the whole system into a novelty shape language.

Pills are reserved for concise status, and circles are reserved for camera-native forms such as status lights, lenses, and the shutter. Borders are thin and mineral gray on light surfaces; image-backed controls use translucent white borders.

**The Civic Geometry Rule.** Keep rails and address plates square-cut, controls mildly rounded, and use pills or circles only when their meaning is inherently status- or camera-related.

## Components

### Buttons

Buttons feel compact, weighted, and field-ready rather than soft or promotional.

- **Shape:** Large actions use an 11px corner and a 52px minimum height; compact image-backed actions use a 10px corner and a 48px minimum height.
- **Primary:** Municipal blue with daylight-white text, heavy action typography, and a restrained blue lift.
- **Hover / Focus:** Hover deepens the blue; active state compresses to 98%; keyboard focus uses a high-contrast 3px blue outline with 3px offset.
- **Secondary:** White with a mineral-gray border and ink-navy text; hover shifts to a cool mineral wash.
- **Disabled:** Cool-gray surface and text, no shadow, no active transform.

### Status Chips

Status chips are compact operational indicators, never decorative tags.

- **Style:** Pill silhouette, 0.75rem bold text, and a 7px status dot.
- **State:** Light green supports local/safe status; image-backed status uses translucent ink navy, a thin white border, and blur for legibility.

### Cards / Containers

The system does not use generic floating cards. The primary container is a bounded working shell, and sections are separated by rails, tone, or a one-pixel line.

- **Corner Style:** Square section edges inside the mobile shell; 18px clipping only for the wide-screen shell.
- **Background:** Daylight white for working surfaces and a cool mineral wash for rails.
- **Shadow Strategy:** Flat within the shell; refer to the limited elevation vocabulary above.
- **Border:** One-pixel mineral-gray structural separators.
- **Internal Padding:** 18px horizontal gutters with 8–20px vertical spacing according to density.

### Inputs / Fields

Inputs are large enough for field use while retaining compact vertical rhythm.

- **Style:** Daylight-white fill, one-pixel medium mineral border, 10px corner, 50px minimum height, and 11px × 13px internal padding.
- **Focus:** Border shifts to municipal blue with a soft 3px blue focus halo; the global focus-visible outline remains available to keyboard users.
- **Supporting Copy:** Soft ink at compact caption size, placed directly below the field.

### Segmented Controls

Segmented controls communicate a small, mutually exclusive choice without expanding into navigation.

- **Style:** Two equal columns inside a 10px bordered frame; each option retains a 44px minimum height.
- **State:** The selected option fills with municipal blue and uses white text; unselected options remain transparent over a mineral wash.
- **Separation:** One-pixel dividers maintain the factory-record density.

### Address Plate

The signature component is a two-tier image overlay: a compact ink-navy time band above a municipal-blue address field with a safety-amber lower rule.

- **Typography:** Tabular timestamp numerals and a heavy, responsive address label.
- **Geometry:** Square-cut sign blocks with tight 3–4px separation; avoid card-like padding or ornamental borders.
- **Legibility:** White text and a neutral drop shadow preserve clarity over mixed imagery.
- **Motion:** Position changes use the emphasized spatial curve; the component itself does not continuously animate.

### Toasts

Toasts are compact, high-contrast operational feedback.

- **Style:** Ink-navy surface, white text, 10px corner, and floating-feedback elevation; errors replace ink navy with field danger.
- **Motion:** Enter by fading and translating upward over the emphasized curve; remain noninteractive and never block the task.

## Do's and Don'ts

### Do:

- **Do** use municipal blue for primary actions, selected states, focus, and the signature address plate.
- **Do** preserve 44px or larger touch targets even when labels and spacing remain compact.
- **Do** align related content to the shared 18px gutter and separate groups with rails, tone, or one-pixel lines.
- **Do** keep the system Chinese font stack and high daylight contrast for offline, outdoor legibility.
- **Do** reserve the capture-stamp animation for the moment an image becomes a committed record and honor reduced-motion preferences.

### Don't:

- **Don't** scatter safety amber across ordinary controls or secondary decoration.
- **Don't** turn every group into a rounded floating card or add ornamental gradients to working surfaces.
- **Don't** use low-contrast gray for critical state, metadata, or actionable text.
- **Don't** add continuous camera, watermark, or status animation; motion must confirm a state change.
- **Don't** introduce a webfont dependency, oversized display typography, or marketing-style spaciousness into dense field controls.
