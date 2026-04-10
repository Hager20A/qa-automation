# Locator Strategy for Dynamic Elements

## The Problem
All input elements have identical attributes except `slot="field-XXX"` which changes on scroll.

## The Solution
Instead of relying on the unstable `slot` attribute:

1. Find the stable parent div with `class="field-group"`
2. Locate it by the visible label text (e.g., "User 45")
3. Traverse to the child input/select/checkbox

## Example

Instead of:     [slot="field-45"]
Use:            find parent containing text "User 45" → then find input

## Why This Works
- Label text is stable and user-facing
- Parent-child relationship doesn't change
- No dependency on dynamically generated numbers
