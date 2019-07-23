SockyNotifier
=============

Throw a macOS notification when connection attempts to servers on the local host are observed. Designed to work
directly with [Socky](https://github.com/PeterUpfold/Socky)

This is designed to provide some level of visibility into any activities on your system where local servers
running on Well-Known (and merely well-known, if you catch my drift) ports are being enumerated.

Inspired by the proof of concept of this demonstrated by https://wybiral.github.io/wtf/

Icon is Public Domain https://thenounproject.com/search/?q=windsock&i=12523

**Note:** that this is not particularly serious or practical, but I wanted a project (Socky)
that let me work directly with the Core Foundation APIs in C, and this seemed a good opportunity. This is the Swift-based
recipient of the notification that Socky generates.

Installation
============

 * Install [Socky](https://github.com/PeterUpfold/Socky), as this component listens on the target ports and dispatches the notification.
 * Build and install `SockyNotifier.app` into `/Applications` or another appropriate path.
 * Copy `uk.org.upfold.SockyNotifier.plist` into `~/Library/LaunchAgents` to run on login (modify application path in plist if necessary).

