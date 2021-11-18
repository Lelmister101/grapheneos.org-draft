# GrapheneOS features page additions
Filesystem access hardening:
- hardened mount permissions
- file spoofing mitigations enabled
- link race mitigations enabled

Dynamic code execution disabling in the base OS:
- Zygote has dynamic code execution disabled as well as its exceptions
- Base apps have dynamic code execution exceptions disabled

Vanadium:
- minimal changes to prefer privacy and security over convenience (some media is click to play, popular sites are not shown by default)
- site isolation improved
- better WebRTC IP handling
- sensors access blocked from sites by default
- Battery API stubbed, so sites cannot see the device's battery level
- default search engine is DuckDuckGo
- JIT toggle added to disable the browser's just-in-time compiler, which reduces attack surface
- -fstack-protector-strong enabled, adding more stack canaries than normal Chromium
