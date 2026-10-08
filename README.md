# Home Assistant blueprints

Reusable Home Assistant automation blueprints.

## Shelly one-to-four-button light controller

Maps between one and four Shelly button event entities to light targets:

- Button 1 is required; buttons 2–4 are optional.
- Single press toggles the corresponding light target.
- Long press optionally turns the target on at 100% brightness.
- Button 3 long press is disabled by default.
- Automation runs are queued so rapid presses are handled in order.

Requires Home Assistant 2026.4 or newer. Each Shelly input must be configured in **Button** mode and expose `single_push` and `long_push` event types.

[View the blueprint source](blueprints/automation/jonathan-ashley/shelly_four_button_lights.yaml)
