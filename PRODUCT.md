# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

Delegated: plain static HTML, CSS, and JavaScript, chosen for a lightweight Android-first camera tool that can run without a framework or backend.

## Users

Primary users are people using an Android phone in field-work situations such as inspections, construction records, property checks, store visits, or everyday documentation. They need to take one photo and save a visibly time-and-address-stamped copy quickly.

## Product Purpose

The product lets a user open a mobile web page, take or select a photo, apply a date-time and address watermark, edit both values, and save the finished JPG. Success means the main task is obvious from the first screen and normally completes in under one minute.

## Positioning

The complete workflow runs as a focused, install-free mobile webpage. The image is composited locally in the browser and does not require accounts, cloud storage, automatic geolocation, or a map service.

## Operating Context

The product is used outdoors and on-site, often one-handed and under mixed lighting. Camera permission may be denied or unavailable, so selecting an existing photo is a required fallback. The watermark contains two lines: editable local date-time and editable address.

## Capabilities and Constraints

- Target recent Android Chrome and common Chromium-based Android browsers.
- Prefer the rear camera and fall back to the system camera/photo picker.
- Do not request location permission or collect coordinates.
- Prefill an editable address from a single configuration value.
- Allow restoring the configured default address and current local time.
- Generate the final JPG locally in the browser and provide save/share actions where supported.
- Correct common phone-photo orientation and preserve useful output resolution within device memory limits.
- Camera access requires HTTPS on most mobile browsers.
- Open decision: the real production default address is not yet supplied. The first prototype uses a clearly replaceable demonstration address.

## Evidence on Hand

The product requirements are recorded in `/tmp/手机拍照水印网页-需求文档.md`. No logo, brand assets, real default address, or production claims were supplied; these must not be fabricated as final business facts.

## Product Principles

- Start with the task, not a marketing introduction.
- Keep every critical action reachable with one hand.
- Make editable metadata visually honest and easy to verify before export.
- Preserve user privacy through local-first processing.
- Always provide a useful fallback when a browser capability is unavailable.

## Accessibility & Inclusion

Use large touch targets, visible focus states, readable Chinese text, high contrast in daylight, and controls that remain usable with enlarged browser text.
