---
name: Aero-Vault
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#393939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#c8c5cf'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#918f99'
  outline-variant: '#47464e'
  surface-tint: '#c2c2f2'
  primary: '#c2c2f2'
  on-primary: '#2b2d53'
  primary-container: '#1a1b41'
  on-primary-container: '#8283af'
  inverse-primary: '#5a5b84'
  secondary: '#c7c6c4'
  on-secondary: '#303130'
  secondary-container: '#464746'
  on-secondary-container: '#b5b5b3'
  tertiary: '#00dbe9'
  on-tertiary: '#00363a'
  tertiary-container: '#002427'
  on-tertiary-container: '#00969f'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e1e0ff'
  primary-fixed-dim: '#c2c2f2'
  on-primary-fixed: '#16173d'
  on-primary-fixed-variant: '#42436b'
  secondary-fixed: '#e3e2e0'
  secondary-fixed-dim: '#c7c6c4'
  on-secondary-fixed: '#1b1c1b'
  on-secondary-fixed-variant: '#464746'
  tertiary-fixed: '#7df4ff'
  tertiary-fixed-dim: '#00dbe9'
  on-tertiary-fixed: '#002022'
  on-tertiary-fixed-variant: '#004f54'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  headline-lg:
    fontFamily: JetBrains Mono
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: JetBrains Mono
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-sm:
    fontFamily: JetBrains Mono
    fontSize: 18px
    fontWeight: '600'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.6'
  label-md:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.0'
    letterSpacing: 0.05em
  code-sm:
    fontFamily: JetBrains Mono
    fontSize: 11px
    fontWeight: '400'
    lineHeight: '1.2'
spacing:
  unit: 4px
  gutter: 16px
  margin: 32px
  container-max: 1440px
---

## Brand & Style

The visual identity of this design system is built on the concept of "Industrial Hardening." It is designed to evoke absolute trust, immutability, and aerospace-grade precision. The target audience includes supply chain auditors, aerospace engineers, and security officers who require a high-density, no-nonsense interface for verifying critical components.

The style is a hybrid of **Industrial Brutalism** and **Tactile Skeuomorphism**. It rejects soft aesthetics in favor of raw, structural honesty. Interfaces should feel like "software-as-hardware," mimicking the physical characteristics of milled aluminum, brushed steel, and control room instrumentation. Every element is designed to feel heavy, bolted down, and indestructible.

## Colors

The palette is strictly functional and high-contrast to ensure readability in industrial environments. 

- **Matte Black (#121212)**: Used for the primary "chassis" of the UI. It provides the deep, non-reflective base layer.
- **Deep Indigo (#1A1B41)**: Utilized for structural accents, sidebars, and deep-recessed areas. It adds a layer of "secure" depth without breaking the dark mode aesthetic.
- **Platinum Silver (#E5E4E2)**: The primary text and "metallic" surface color. It provides a cold, high-performance finish.
- **Verification Glow (#00F0FF)**: A vibrant cyan used exclusively for active authentication states and blockchain "heartbeat" indicators.

Surface textures should utilize a subtle grain or "brushed" noise to simulate metallic finishes on Platinum Silver surfaces.

## Typography

This design system employs a dual-font strategy to balance human readability with technical precision. 

**JetBrains Mono** is reserved for headings, data points, and labels. Its monospaced nature reinforces the "technical readout" feel and ensures that alphanumeric serial numbers are easily distinguishable. **Inter** is used for body copy and descriptions where long-form legibility is paramount. 

All headers should be set with tight line-heights to feel "compressed" and sturdy. Use uppercase styling for labels and secondary headers to simulate stamped metal plates.

## Layout & Spacing

The layout follows a **Fixed Grid** philosophy, emphasizing a structured, modular "dashboard" feel. The interface is divided into functional zones using heavy borders rather than whitespace.

- **Grid**: A 12-column system with 16px gutters.
- **Rhythm**: All spacing must be multiples of 4px.
- **Containment**: Content is housed within defined structural regions that feel like physical compartments. 

Margins are generous (32px) to prevent the UI from feeling cluttered despite the heavy border weights. Use explicit dividers (2px weight) to separate information hierarchies.

## Elevation & Depth

Depth in this design system is achieved through **Recession rather than Projection**. Traditional drop shadows are discarded. Instead, use:

1.  **Inset Shadows**: Create a "stamped" or "engraved" look for cards and input fields.
2.  **Tonal Stacking**: Surfaces get lighter as they "rise" toward the user. The background is Matte Black, while primary interaction surfaces are Deep Indigo.
3.  **Heavy Borders**: Use 2px solid borders in Platinum Silver or Deep Indigo to define the physical boundaries of elements.
4.  **Outer Glows**: Reserved exclusively for "Authenticated" states. A soft cyan outer glow (5px to 10px blur) indicates a live, verified blockchain connection.

## Shapes

The shape language is strictly **Sharp (0px radius)**. There are no rounded corners in this design system. 

The use of 90-degree angles conveys rigidity, structural integrity, and a "milled" manufacturing quality. Any diagonal elements (such as "dog-ear" corners on badges) must be cut at 45-degree angles to maintain the geometric, industrial feel.

## Components

### Buttons
Buttons are "Heavy-Action" components. They feature a 2px solid Platinum Silver border. In the "Active" state, they utilize a subtle inner bevel effect. The hover state should invert the colors (Platinum Silver background with Matte Black text).

### Industrial Cards
Cards are styled as "recessed plates." They use a Deep Indigo background with a 1px inset shadow and a 2px outer border. Each card should feature a small "ID Label" in the top-left corner using JetBrains Mono.

### Authentication Badges
These are the focal point of the platform. When verified, the badge features a sharp 2px cyan border and a high-contrast cyan glow. The text inside uses JetBrains Mono Bold.

### Input Fields
Inputs must look like data entry terminals. Use a Matte Black background with a Platinum Silver 1px border. On focus, the border changes to the Verification Glow color (#00F0FF) with a faint inner glow.

### Status Indicators
Blockchain verification statuses use high-contrast signals: 
- **Verified**: Solid Cyan (#00F0FF) with pulse animation.
- **Warning**: Solid Amber (#FFBF00) with "Warning Striped" background patterns.
- **Critical/Failed**: Solid Red (#FF3131).

### Additional Components
- **Data Tables**: High-density with 1px Platinum Silver grid lines and alternate-row shading in Deep Indigo.
- **Terminal Consoles**: Monospaced log readouts at the bottom of the interface for real-time blockchain transaction viewing.