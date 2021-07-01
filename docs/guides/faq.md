---
id: faq
title: 'Frequently Asked Questions'
---

### Do binaries get automatically deleted?

No, this package will **not** delete any binaries, so after an system / package upgrade the binaries may have to be cleaned manually.

### Why is there no documentation about class-options / interfaces in the documentation?

It is currently recommended to directly look at the TSDoc for these properties to get their type & documentation.

### Do testing database paths get cleaned up?

If the Database path is generated by this package, then it will automatically get cleaned up (ensured to run by process event `beforeExit`).  
If the Database path is provided, then it will not be automatically cleaned up, cleanup needs to be called explicitly like `.cleanup(true)` (parameter is to force-delete the directory).