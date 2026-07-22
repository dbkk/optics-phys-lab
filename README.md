# OpticsPhysLab

OpticsPhysLab is an interactive browser app for learning optics and microscopy. It is designed as a companion to experimental physics lectures: choose a module, move the controls, and watch how light, electrons, probes, images, spectra, and forces respond.

The app runs entirely in the browser. It does not require login and does not send experiment data to a server.
It may store only the selected language (`optics-phys-lab-language`) in the browser's local storage.

## Modules

- Refraction and total internal reflection
- Diffraction and lens Fourier transform
- Chromatic aberration
- Spherical aberration and field curvature
- Kohler illumination and microscope layout
- Fourier optics, brightfield imaging, and phase contrast
- Fluorescence microscopy
- Confocal and two-photon microscopy
- Super-resolution localization
- Optical tweezers
- Cryo-electron microscopy, CTF, and particle averaging
- Atomic force microscopy
- Camera optics
- Human eye and glasses

Use the JP/EN toggle in the upper right to switch language. Each panel has a `?` button with the relevant physical explanation.

## What The Models Are

The simulations are educational, schematic models. They are not instrument-design, diagnostic, medical, or product-evaluation software.

- The microscope "illumination-limited NA" shown in the app is a display/model value affected by the aperture stop. It should not be read as a universal physical NA for every illumination condition.
- Camera depth of field uses an enlarged circle of confusion so the green depth band is visible in a small diagram.
- Fluorescence spectra and filters are schematic curves and rectangular bands based on representative DAPI, GFP, and mCherry peaks, not measured spectra.
- Confocal and two-photon views use scalar Gaussian/PSF approximations for teaching optical sectioning, not a full vector diffraction model.
- Electron-microscope images use the same deterministic schematic projection of a cytoplasmic-dynein motor domain for a negative-stain reference, one cryo particle, and an aligned average. The cryo views share one display window so that averaging improves visible SNR without independent contrast stretching. The weak-phase/CTF transfer and seeded counting noise are educational models, not experimental micrographs or a full 3D refinement.
- The AFM view uses a deterministic calibration relief, finite-tip morphological dilation, and a simplified first-order feedback response. It does not replace a full contact-mechanics, hydrodynamic, or FM-AFM model.
- Cell-like and HeLa-like sample drawings are schematic morphology, not experimental cell data.
- Glass names such as BK7 and SF10 are used in simplified educational dispersion models.

## Publication Status

The public site is intended to ship as built static files only. The development source code and project feedback notes are not part of the public app release at this stage.

## Copyright And Use

Copyright (c) 2026 Kyogo Kawaguchi. All rights reserved unless a separate written permission is given.

The public release is currently a viewable educational web app. Redistribution, source-code reuse, and derivative publication are not granted by this README. Third-party open-source dependencies remain under their own licenses as listed in `THIRD_PARTY_NOTICES.md`.

## AI-Assisted Development Disclosure

Development and scientific review: Kyogo Kawaguchi.

Portions of the implementation and drafting were produced with AI-assisted coding tools, including Anthropic Claude Code and OpenAI Codex. Kyogo Kawaguchi reviewed, edited, and is responsible for the scientific content, code, and public release.

## Notices

OpticsPhysLab is an unofficial educational demonstration. Product names, trademarks, fluorophore names, and glass names such as Zeiss, Tessar, Planar, BK7, SF10, DAPI, GFP, and mCherry belong to their respective owners.

Third-party dependency license notes are listed in `THIRD_PARTY_NOTICES.md`.
