# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [1.2.0] - 2025-05-11

### Added
- **i18n system** — Full internationalization support with `I18N` dictionary, `t()` helper, and language switcher dropdown (zh-CN / en / ja) stored in `localStorage`
- **Language switcher** integrated into the settings panel (Task 4-b A)
- **Float panel title bar** now follows the selected language (Task 4-b B)
- **Modal scrollbar beautification** — custom thin accent-colored scrollbar for edit modal (Task 4-a C)
- **IndexedDB save slots** — `slotManager` migrated from `localStorage` to IndexedDB `slots` objectStore; falls back gracefully to localStorage (Task 5-P3)
- **DB version bump** to v4 with new `slots` objectStore
- New `dbManager` helpers: `setSlot`, `getSlot`, `getAllSlots`, `deleteSlot`

### Changed
- **@icon** and CSS floating button background replaced with custom PNG (46561231.png) (Task 1)
- **@version** bumped to `1.2.0`
- **Card width slider** range expanded from `120–320 px` to `100–400 px` (Task 4-a D)
- **"识别元数据" button** style unified with `.action-btn` class (Task 4-a H)
- **Workspace buttons** gain `title` attribute for tooltip on overflow (Task 4-a J)
- **`blobUrlManager.cleanup()`** changed to differential cleanup — only revokes blob URLs no longer in the new view, reducing GC pressure (Task 5-P6)
- **View-mode switches** (gallery/masonry/list) now cache `collapsedIds` in a `Set` instead of re-querying the DOM (Task 5-P5)
- **`renderApp` patches** (catSort, defaultCollapsed, categoryRestore) merged into a single `_postRenderHooks` registry, eliminating repeated wrapper stacking (Task 5-P7)

### Fixed
- **Edit modal** now correctly scrolls on small/mobile screens — added `max-height: 100dvh`, `overflow-y: auto`, and `-webkit-overflow-scrolling: touch` (Task 3)
- **Mobile full-screen modal** (≤480 px) now forces `overflow-y: auto` and `max-height: 100dvh` to prevent clipping (Task 3)
- **`initPointerSortable`** and **`initCategorySortable`** `attachDynamicListeners` wrapper now guarded with `__ptrSortPatched` flag to prevent double-patching on hot reload (Task 5-P2)

---

## [1.1.0] - 2025-04-xx

### Added
- Batch metadata parser + thumbnail regeneration button (`parse-all-meta-btn`)
- Multi-workspace support with drag-to-reorder
- Tree editor modal
- Save slots (localStorage)
- Dual-tone card background mode
- NAI params editor in edit modal (sampler, scheduler, guidance, rescale, seed)
- Masonry (waterfall) layout mode
- IndexedDB image storage with auto-thumbnail generation

### Fixed
- Gallery drag/zoom bug
- Card collapse state persistence across re-renders

---

## [1.0.0] - 2025-03-xx

### Added
- Initial release
- Floating panel with resizable iframe
- Prompt card CRUD (create, read, update, delete)
- Category hierarchy with drag-and-drop sorting
- Image upload / preview per card
- Light/dark theme toggle
- ZIP export/import
