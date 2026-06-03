# Packard Leaf Shutter Mechanism

This mechanism defines how the Packard leaf is actuated using the existing hardware models in this directory.

## Mechanism Overview
- **Leaf**: `Components/Leaf.SLDPRT`
- **Actuation pin**: `Hardware/CaptivePin.SLDPRT`
- **Pneumatic control**: `Hardware/Flow Valve.SLDPRT`

## Actuation Sequence
1. In the resting state, the leaf remains closed against the aperture.
2. Air pressure applied through the flow valve drives the captive pin linearly.
3. Captive pin travel pulls the leaf open to expose the aperture.
4. Releasing pressure returns the captive pin and allows the leaf to close.

## Exposure Modes
- **Bulb**: hold valve pressure to keep the leaf open; release to close.
- **Time**: pulse valve pressure for a repeatable open/close cycle.

## Integration Notes
- Keep pin travel concentric with the leaf pull point to avoid binding.
- Valve flow setting controls opening speed and helps reduce leaf bounce.
