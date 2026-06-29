## 2024-06-29 - Keyboard Accessible Dropzones
**Learning:** Custom file dropzones that hide the native `<input type="file">` break keyboard accessibility because users cannot tab to the hidden input.
**Action:** Always add `tabindex="0"`, `role="button"`, an `aria-label`, and an `onkeydown` handler for 'Enter'/'Space' on the visible dropzone element, and include a `:focus-visible` style to ensure keyboard users can navigate and use the uploader.
