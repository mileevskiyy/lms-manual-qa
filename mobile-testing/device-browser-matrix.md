# Device / Browser Test Matrix

| Platform | Browser | Priority | Key checks |
|---|---|---:|---|
| macOS | Chrome | High | Core functional flow, DevTools |
| macOS | Safari | High | Layout, authentication, upload |
| iPhone | Safari | High | Touch, keyboard, photo/file upload, orientation |
| Android | Chrome | Medium | Responsive UI, upload, navigation |
| Windows | Chrome | Medium | Main cross-platform regression |

## Mobile-specific checks

- virtual keyboard does not cover CTA buttons
- file picker opens correctly
- photo upload works
- portrait / landscape
- modal dialogs remain scrollable
- no horizontal overflow
- slow network behavior
