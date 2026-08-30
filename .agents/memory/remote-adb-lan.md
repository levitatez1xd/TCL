---
name: Remote ADB limitation
description: Limitation when attempting to operate devices on a user's private home network from the workspace session.
---

ADB connections to a device on the user's private LAN may work from the user's local computer but remain unreachable from the workspace session. Have the user run device commands locally and share the resulting files or output; never expose ADB to the public internet.

**Why:** The workspace network is isolated from the user's home network, even when the user's Mac can connect to the device.

**How to apply:** Treat local ADB output as user-executed evidence, keep destructive commands explicitly approved, and use small reversible batches with user-led functional checks.