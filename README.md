# CyUtils
A Cython utilities library that that implements features that either I've winded up using on occation or multiple times in different libraries.
This is planned for being installed as a pypi package but the code can be copied and pasted if you need a quick and dirty shortcut. I'll make utilities
for installing these simillar to how (pythoncapi-compat)[https://github.com/python/pythoncapi-compat] works which was my alternative solution if pypi packages aren't required.

# Features
This new toolkit plans to possibly implement the following features Note that some of these are still being thought up and may not come true at all
but some of these I am certain will be added soon if not later...
- [ ] Msgspec's str or bytes Py_buffer view extraction which has been a very useful shortcut for me in cyares and cyjs so far...
- [ ] aiohttp's http writer with a few edits to the implementation to be acceptable for many different buffer types
- [ ] Json writer (Under Concept might go with msgspec's implementation for this one but I did think about bringing in yyjson for doing this)
- [ ] Somes of [Cyares's tools](https://github.com/Vizonex/cyares) are planned to go here so that developers can utilize these for speed.
- [ ] CPython's Socketmodule C-API which I've used while implementing [pywepoll](https://github.com/Vizonex/pywepoll) But a lot more completed
- [ ] [pythoncapi-compat cython bindings](https://github.com/python/pythoncapi-compat)
- [ ] might but winloop's newer shlex parser here and upgrade it soon to just be struct-only
- [ ] tools for splitting pyx to create a new pxd and pyx file.
- [ ] C Atomics which plans to just port CPython's newer py_atomic code over here but for binding these newer locking systems to older python libraries.
- [ ] Cyares's Future Object might be put here in a future release for those needing a faster Concurrent.Futures.Future Object to work with in cython.
- [ ] FSConverter for binding `PyUnicode_FSConverter` because Cython doesn't include this function and it does not exist anywhere.

# TODOS
Tutorials on how to bind or use in your own Cython libraries.

