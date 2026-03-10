---
id: "1773157140819-5skv5p8ro"
type: "prompt"
title: "ARC Extensions"
date: "2026-03-10T07:00:00.000Z"
tags: ["ARC","Extensions"]
metadata: {"context":"Abstraction and extensibility of ARC","model":"Claude 3.5 Sonnet"}
createdAt: "2026-03-10T15:39:00.819Z"
updatedAt: "2026-03-10T15:39:00.819Z"
isPublic: false
---

For the ARC core, as in the Symphony CMS core, each field type should be an extension, each content type should be an extension. That way, the core can contain the essential functionality of the original ARC Journal without the unnecessary bloat of the additional functionality. But, if someone wanted to add the ability to have custom fields and custom sections for this sort of specific use case of tracking Figma Make prompts, the necessary extensions could be easily installed and enabled, similar to a Symphony CMS install. This project would represent an extension to the core in the same way that Symphony CMS ensembles could be built to install only the necessary extensions to recreate the functionality desired. The installer would contain a manifest of all the extensions and their individual GitHub repositories to install them as submodules into the /workspace/extensions directory.

How could we manage such a feat where we do not have that kind of access to the file system to clone GitHub repositories?

Can we direct Figma Make to read a manifest, create placeholder files for the directories and files, then direct the user to copy and paste the relevant files into the system? This would avoid expending AI credits in the Figma Make system, and require as little manual copy and paste actions as possible to replicate the code for each extension exactly as written, designed, and tested.