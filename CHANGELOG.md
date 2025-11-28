## [0.7.8-beta] — 2025-11-28

- First public beta release.
- Updated `bl_info` metadata for clearer presentation in Blender:
  - Name: **Smart Empties [ MODLR ]**
  - Location path: **3D Viewport > Sidebar (N-panel) > MØDLR SMART > Smart Empties [ SMART ]**
  - Description now references the **MØDLR SMART Tools** suite.
- Added live documentation and issue links (`doc_url` and `tracker_url`) pointing to the MØDLR Studio GitHub repository.
- Added a **“Beta release”** warning in `bl_info["warning"]` to clearly indicate pre-stable status.
- Aligned UI branding with metadata: panel label set to **Smart Empties [ SMART ]** and N-panel category set to **MØDLR SMART**.

---

## [0.7.8] — 2025-09-29

- Added DEV_BUILD gating to safely separate development and release builds.
- Improved placement accuracy with stronger handling of triangles, quads, and edge cases.
- Streamlined internal modules (collections, naming, utils) for cleaner structure and easier maintenance.
- Operators tightened for safer polling, execution, and more reliable reporting.
- Properties expanded and defaults clarified to support the updated placement and state behaviors.
- UI sections refined with consistent labels, clearer tooltips, and width-aware layout adjustments.
- Replace card now shows a disabled Auto-Move placeholder in dev builds; hidden in release builds for a cleaner layout.
- Cleanup section polished with clearer warnings, width-aware messaging, and improved responsiveness.
- Metadata and imports aligned for predictable UI rendering across dev/release modes.
- Overall behavior made more deterministic with clearer reports and safer execution paths.

---

## [0.7.7] — 2025-09-05

- Switched to a new global Preferences system for default prefix, shape, size factor, and auto-size behavior.
- Adopted a WindowManager-first state for more reliable undo behavior and fewer unexpected flips.
- Replace tools improved with clearer warnings, better validation, and accurate behavior on non-unit-scale objects.
- Added new operators: a safe Cleanup tool with confirmation, and an info-chip operator for clearer feature impact.
- Expanded UI polish: refined tooltips, clearer labels, and updated EMPT [ MØDLR ] branding across the panel.
- Settings, Size, and Management sections are now collapsible for a cleaner daily workflow.
- Replace card improves clarity with dynamic enable/disable behavior and helpful tooltips when unavailable.
- Cleanup tool is now safer and more transparent, with clearer messaging and width-aware warnings.
- Footer now includes direct Help and Report links wired to the add-on’s official documentation and issue tracker.

---

## [0.7.6] — 2025-09-02

- Unified all layout breakpoints behind a single set of constants for predictable, stable responsive behavior.
- Actions row (Create + Replace) now switches cleanly between full labels, two-column, and stacked layouts.
- Target chips now stack consistently in narrow layouts and stay horizontal when space is reasonable.
- Added a clear “EXTREME” banner for ultra-narrow widths to prevent unreadable layouts and layout jitter.
- Settings, Size, Move/Select, and Collections now follow the same width rules for cleaner, more consistent section behavior.
- Improved readability by keeping controls in single-row layout until space truly runs out.
- Overall UI now feels more stable: fewer breakpoints, clearer transitions, and a more polished responsive foundation.

---

## [0.7.4] — 2025-09-02

- Replace now runs instantly using the N-panel defaults for Duplicate Type and Hide Empties — no dialogs, no redo panel needed.
- Scope-aware Replace correctly respects Smart / Non-Smart / All and gives clear messages when items are filtered or skipped.
- Replacing with a non-unit-scale source now warns appropriately and preserves correct scale in the result.
- Select helpers are smarter: visibility-aware, better at retaining the active object, and provide clear summaries.
- Duplicate Type is now shown as radio buttons (Linked | Unique) for faster access and clearer state.
- Create and Replace actions unified into a single responsive Actions row that adapts cleanly to narrow or wide sidebars.
- Target chips (Smart / Non-Smart / All) now adapt gracefully in extremely narrow layouts for better readability.
- Breakpoints across Actions, Settings, Size, and Management are now fully harmonized to prevent layout jitter.
- Overall UI feels more stable and predictable — clearer warnings, fewer surprises, and more accurate behavior across Replace and Select.

---

## [0.7.2] — 2025-09-01

- Unified Create + Replace into one clean action row that adapts automatically to sidebar width.
- Improved Scope row (Smart / Non-Smart / All) with clearer visibility and consistent horizontal layout.
- Repositioned action info chip for better readability and flow.
- Create options now adjust layout intelligently: single-row when wide, compact stacked layout when narrow.
- Added three responsive warning tiers (Soon / Compact / Extreme) based on available panel space.
- Settings section is now always visible with a clear two-column or stacked layout depending on space.
- Standardized layout rules so Size, Move/Select, and Collections groups behave consistently on all widths.
- Cleanup and Links remain collapsible by default to keep the panel clean and focused.
- Overall panel now behaves predictably at every width: no label clipping, smoother stacking, and clearer structure.

---

## [0.7.0] — 2025-08-30

- No core logic updates — fully focused on UI/UX structure and responsive layout.
- Introduced collapsible sections using new WindowManager properties (collapsed by default where appropriate).
- Promoted **Targets**, **Settings**, and **Cleanup** into dedicated groups for clearer visibility.
- Merged Move, Select, and Collections into a unified **Management** section with simplified sub-labels.
- Added a new **Links** section for future features, collapsed by default.
- Tightened responsive layout: improved breakpoints, cleaner stacking, and prevention of label clipping.
- Reduced vertical bloat by ~16–18 rows for a faster, more professional panel.
- Improved discoverability — Prefix/Shape settings and destructive ops now stand out clearly.
- Established a polished, predictable UI layout baseline for future builds.

---

## [0.6.14] — 2025-08-30

- Improved accuracy for Select helpers across the View Layer and active collection.
- Tightened Create logic for better alignment, cleaner mode switching, and consistent preconditions.
- Unified source-of-truth so all operators read from the same data path.
- Updated panel labels and toggles to accurately reflect the add-on’s configuration state.
- Enhanced reliability with clearer CANCELLED reports and fewer undo anomalies.
- Refinement milestone: more consistent, truthful UI feedback and more predictable operation outcomes.

---

## [0.6.13] — 2025-08-16


- Updated registration, metadata, and property definitions to match the current framework.
- Refined Create, Move, and Select flows for predictable operation and accurate reporting.
- Clarified operator polling and execution paths for improved stability across modes.
- Adjusted panel layout and copy for better clarity without disrupting muscle memory.
- Reduced edge-case failures and eliminated ghost undo steps.
- Stability milestone: smoother operation, fewer surprises, and tighter alignment between UI and internal behavior.

---

## [0.6.12] — 2025-08-16

- Refined Create and Move flows for consistency with current panel toggles and visual feedback.
- Updated registration and property setup to match recent internal changes.
- Improved stability in edge cases with clearer CANCELLED messages and safer undo handling.
- Adjusted panel layout and labels for better clarity while preserving familiar control placement.
- Polishing milestone: operators behave more predictably, UI text is cleaner, and stability continues to strengthen.

---

## [0.6.11] — 2025-08-15

- Updated registration and metadata alignment for compatibility with the evolving package structure.
- Polished Create flow for more consistent results and accurate reporting.
- Adjusted panel layout for improved readability while maintaining familiar control placement.
- Reduced ghost undo effects and refined CANCELLED feedback during invalid operations.
- Reliability milestone: cleaner operation flow, more accurate status reporting, and a more predictable user experience.

---

## [0.6.10] — 2025-08-15

- Refined Move and Select behavior for greater consistency and improved mode handling.
- Updated add-on registration and metadata to align with current conventions.
- Improved UI labeling and spacing for a more compact, legible panel.
- Further reduced ghost undo issues and added clearer CANCELLED feedback for invalid actions.
- Stability milestone: smoother interaction flow, stronger visual consistency, and reliable undo behavior.

---

## [0.6.9] — 2025-08-15

- Improved Move and Select operations for more predictable results and consistent reporting.
- Updated add-on registration to align with current structure and naming standards.
- Applied UI copy and spacing refinements for a cleaner, more legible layout.
- Enhanced stability under edge conditions, reducing ghost undo steps.
- Polishing milestone: smoother everyday performance with a cleaner, tighter interface.

---

## [0.6.8] — 2025-08-13

- Refined Move and Select flows for consistent behavior across visibility and selection states.
- Updated registration and property setup to match the current code layout.
- Maintained familiar control placement while tightening copy and spacing for clarity.
- Improved reliability during undo and redo cycles for smoother workflow behavior.
- Refinement milestone: more predictable operation and a panel that feels more cohesive in daily use.

---

## [0.6.7] — 2025-08-13

- Synchronized Create, Move, and Select flows for consistent toggle behavior and reporting.
- Clarified operator polling and execution paths for stronger stability across all modes.
- Updated registration and metadata to align with the unified structure.
- Preserved control layout for user familiarity while improving label readability.
- Continued refinement of reliability and undo safety.
- Consistency milestone: smoother, more predictable behavior with UI that accurately reflects tool state.

---

## [0.6.6] — 2025-08-13

- Updated registration and metadata for compatibility with the evolving modular layout.
- Refined panel layout and labels for clearer communication and consistent placement.
- Improved internal reliability and smoother workflow behavior in common modeling tasks.
- Maintenance milestone: clarity and consistency improvements laying groundwork for the stable 0.6.x line.

---

## [0.6.5] — 2025-08-12

- Updated registration and property definitions for consistency with the latest structure.
- Refined Create flow to better reflect panel toggles and prevent invalid actions.
- Polished UI copy and spacing for a cleaner, more professional appearance.
- Improved overall workflow stability and undo reliability.
- Foundation milestone: tighter control flow, cleaner visuals, and more reliable day-to-day operation.

---

## [0.6.3] — 2025-08-12

- Synchronized Create, Move, Select, and Operator flows for consistent execution and reporting.
- Streamlined internal modules (collections, naming, props, utils) to remove redundant logic.
- Adjusted panel labels and structure for clearer organization while keeping the familiar layout.
- Improved stability in edge cases with safer undo behavior and clearer CANCELLED messages.
- Structural cleanup milestone: more maintainable internally while remaining predictable to use.

---

## [0.6.0] — 2025-08-12

- Transitioned Smart Empties from a single script to a fully modular package.
- Split functionality into dedicated modules for creation, movement, deletion, selection, and UI.
- Preserved operator ID continuity to keep existing shortcuts functional.
- Reorganized panel drawing and property access for better consistency and lower desync risk.
- Ensured behavior parity across all operators for easier testing and future expansion.
- Foundational milestone: establishes a structured, maintainable architecture for long-term growth.

---

## [0.5.99] — 2025-08-11

- Introduced new toggle operators for faster Smart Collection management.
- Refined panel grouping and icons for smoother section navigation.
- Enhanced layout logic to reduce travel distance between related controls.
- Improved overall reliability and responsiveness in daily workflows.
- Milestone build: final pre-modular version establishing the 0.6.0 interaction style and UI rhythm.

---

## [0.5.4] — 2025-08-11


- Refined core logic for better stability and cleaner execution paths.
- Updated panel grouping and labels for improved readability and access to key actions.
- Adjusted icons and control spacing for a balanced, professional appearance.
- Added minor internal optimizations for smoother operation in typical modeling tasks.
- Usability milestone: improved visual flow while keeping the add-on stable and fast.

---

## [0.5.3] — 2025-08-11

- Polished internal logic for more reliable execution and consistent results.
- Refined panel labels, icons, and group hierarchy for better visual flow.
- Improved control spacing and interaction rhythm for faster modeling adjustments.
- Further stabilized general reliability and undo behavior.
- Usability milestone: subtle but meaningful improvements without changing workflows.

---

## [0.5.2] — 2025-08-10

- Unified Create, Move, and Select behavior for smoother, more consistent operation.
- Strengthened poll, invoke, and execute paths to prevent invalid actions.
- Improved undo handling with clearer CANCELLED feedback for predictable results.
- Stability milestone: more reliable responses and clearer feedback during modeling.

---

## [0.3.8] — 2025-08-09

- Unified Create, Move, and Select flows for consistent behavior across modes.
- Strengthened safety checks and execution paths to prevent invalid selections.
- Improved undo handling with clearer CANCELLED feedback when no action occurs.
- Refinement milestone: smoother, more predictable, and cleaner day-to-day behavior.

---

## [0.2.4] — 2025-08-08

- Increased reliability of Create, Move, and Select via refined polling and safer execution paths.
- Unified operator handling to eliminate redundant actions and handle invalid selections cleanly.
- Improved stability with consistent undo behavior and clearer visual/interaction feedback.
- Usability milestone: smoother, more predictable behavior across all common workflows.

---

## [0.1.0] — 2025-08-01

- Introduced the first Smart Empties prototype with normal-aligned placement.
- Added placement from vertices, edges, and faces with automatic Z-axis alignment.
- Added mode switching (Edit ↔ Object) with automatic return after execution.
- Implemented accurate logic for vertex, edge midpoint, and face-center placement.
- Linked spawned empties to the active collection with clean naming and default size.
- Foundation milestone: establishes Smart Empties as a fast, precise placement tool.

