# Wingy Flap routing metadata

This repository is the independent publication point for signed routing metadata. It does not receive backups or device data.

The publisher runs on the owner's Toshiba computer. Its signing key and repository deploy key remain there. Android clients trust the verification key included in their app, validate the exact signed payload, reject older revisions, and stop sending when the policy expires. Receiver connections also require HTTPS and the receiver identity authorized by the policy.

The signed policy can select a receiver, authorize fallback receivers, revoke an IP address, or pause delivery. Reading this repository does not grant backup consent or approve an additional transfer request.

The stable client file is `wingy-routing.signed` on the `main` branch. A file pinned to a commit does not receive routing updates. There is no promise of immediate cache propagation; clients must enforce expiry locally.
