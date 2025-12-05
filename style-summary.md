# Website Style Customization Summary

This document summarizes the key locations within the `random-name-picker` project where design elements can be modified. This information can be used for future reference and LLM processing to streamline design changes. 

Note: This summary are not verified for completeness, and further analysis may be needed for specific design changes.

## Key Modification Areas:

*   **Text Content**:
    *   **File:** `src/pages/landing.pug`
    *   **Description:** Contains all user-facing text content and the basic HTML structure of the main page.
    *   **Key Elements:** `h1.settings__title`, `label.input-label`, `textarea.input-field`, `button#draw-button`

*   **Logo**:
    *   **File:** `src/assets/images/title.svg`
    *   **Description:** The main logo/title graphic displayed on the page. To change, edit or replace this SVG file.

*   **Color Scheme**:
    *   **File:** `src/assets/scss/_colors.scss`
    *   **Description:** Defines all primary color variables used throughout the application.
    *   **Key Elements:** `$color-white`, `$color-red-step1`, `$color-yellow`, `$color-button-default-background` (and other `$color-*` variables)

*   **Background & Fonts**:
    *   **File:** `src/assets/scss/_base.scss`
    *   **Description:** Sets global styles, including the background `linear-gradient` and imports/applies the primary font ('Nunito Sans').
    *   **Key Elements:** `@import url('https://fonts.googleapis.com/css2?family=Nunito+Sans...')`, `font-family: 'Nunito Sans', ...`, `background: linear-gradient(...)`

*   **Visual Effects (Lucky Draw Animation)**:
    *   **File:** `src/assets/js/Slot.ts`
    *   **Description:** Likely contains the logic for the slot machine animation, which is the primary visual effect of the lucky draw. Further analysis may be needed to pinpoint exact modification points.

*   **Sound Effects**:
    *   **File:** `src/assets/js/SoundEffects.ts`
    *   **Description:** Central location for managing and triggering sound effects for the application. Further analysis may be needed to pinpoint exact modification points.

*   **Main Application Entry Point (Coordination)**:
    *   **File:** `src/assets/js/app.ts`
    *   **Description:** Likely initializes and coordinates the UI, including the slot machine and sound effects. This file might be relevant for integrating new visual/sound components or modifying how existing ones are invoked.
