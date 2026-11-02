# Engineering Roadmap

## P0 — Safety, consent and reliability

- [ ] Audit SOS flows on physical Android devices and document exact behaviour for each permission state.
- [ ] Make it explicit when the app opens the SMS composer versus sending a message directly.
- [ ] Require user confirmation before sharing live location or contacting trusted contacts.
- [ ] Handle denied, permanently denied and revoked location/microphone/camera/Bluetooth permissions.
- [ ] Add visible GPS accuracy and stale-location indicators; never imply that a location is guaranteed.
- [ ] Document that the app is not a certified emergency service or sole safety channel.

## P1 — Testability

- [ ] Add unit tests for navigation state, voice-command parsing and emergency-contact validation.
- [ ] Add widget tests for onboarding, SOS setup and accessibility settings.
- [ ] Add integration tests for permission denial, GPS loss and offline behaviour.
- [ ] Add CI with Flutter format, analyze and test steps.
- [ ] Add a reproducible release checklist and verify release tag / APK version consistency.

## P1 — Accessibility

- [ ] Audit semantics labels, focus order, screen-reader announcements and touch target sizes.
- [ ] Support text scaling without clipping.
- [ ] Provide a non-voice path for all essential actions.
- [ ] Test TalkBack, high contrast and reduced animation settings.

## P2 — Product completeness

- [ ] Clearly separate implemented features from prototypes and planned AI capabilities.
- [ ] Add an architecture diagram and service responsibility notes.
- [ ] Document supported Android versions and device test matrix.
- [ ] Add privacy policy and data-handling documentation before wider distribution.

## Acceptance criteria

- Core screens remain usable with TalkBack and large text.
- Permission denial never crashes or traps the user.
- SOS behaviour is transparent, consent-based and verified on-device.
- README claims match features demonstrated in a tested build.
