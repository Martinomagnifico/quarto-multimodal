# Changelog

## [1.1.6] - 2026-09-16

### Added
- Focus moves into an open modal, the rest of the presentation is inert, and focus returns on closing
- In fullscreen, Escape closes an open modal before it leaves fullscreen (Chrome and Edge)

### Fixed
- Opening or closing a modal no longer shifts a centered slide
- The close button is no longer hidden from screen readers
- A closed modal no longer stays over the slides, invisible, when the browser skips the end of its fade. This happened.
- A closing modal no longer takes clicks while it fades out

## [1.1.5] - 2026-09-14

### Added
- Modals sync with the speaker view. Fixes [#8](https://github.com/martinomagnifico/reveal.js-multimodal/issues/8)
- HTML modals sync their scroll position with the speaker view (not iframes)

### Fixed
- The `overlaycolor` and `radius` options no longer fall back to the defaults after the first modal closes
- A `data-modal-overlaycolor` that matches the default colour now applies
- Classes from `data-modal-class` are removed after closing, also with `speed: 0`, and no other classes are
- Long HTML content was visible on the slide in the Markdown demo

### Changed
- Videos and autoplaying iframes are muted in the speaker view

## [1.1.0] - 2026-08-22

### Changed
- This new version is a rewrite built with Vite
- Updated for the use of the latest version of Reveal.js.
- Uses pluginToolkit to check if it is running in a module environment and will then not autoload the CSS
- Fixed the `closebuttonhtml` option: the default close button was assigned right after the option was applied, so a custom button was never used

## [1.0.1] - 2024-06-10

### Changed
- Completed documentation
- Fixed minor issues with paddings
- Fixed type-error with events not being dispatched
- Changed `border` option into `bordercolor` and `borderwidth`
- Prepared for Quarto version

## [1.0.0] - 2024-06-05

### Changed
- Fixed Firefox issue with the modals having extra space
- Newer version of devDependency Pug

## [0.1.6] - 2024-04-19

### Changed
- Fix overflow issue


## [0.1.5] - 2024-04-19

### Changed
- Change gulp header function


## [0.1.4] - 2024-04-17

### Changed
- Rounded scalecorrection variables.

### Added
- Added more details in the events that are dispatched to the deck.


## [0.1.3] - 2024-04-16

### Changed
- Fix for 'bodyscrolllock'. Opening a locknav-link no longer breaks on iOS. However, when the lock is enabled on iOS, somehow scrolling back up is still possible. The functionality may be removed (for iOS) in the future.
- Fix for situation where a first slide is a modal slide. On iOS, that modal was also opened when the user was on another section.

### Added
- Added a scalecorrection option. This makes sure that the close button is not reduced in size when the modal is scaled down. The same is also set up for the border around the modal.


## [0.1.1] - 2024-04-08

### Changed
- Fix for iOS video


## [0.1.0] - 2024-04-08

### Changed
- First public GitHub version
- Dispatch events to deck


## [0.0.9] - 2024-04-08
### Added
- Modals can now also be opened by triggers that are added later to the DOM.

### Changed
- Some tweaks to variable names.


## [0.0.8] - 2024-04-05
- Beta version