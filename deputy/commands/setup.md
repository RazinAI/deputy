---
description: Check that Deputy is connected to your browser, and get Deputy Pro if you want it
---

Check the user's Deputy setup and tell them, in a few short lines, what works and what to do next.

1. Call `browser_tabs` with `action: "list"` if it is available, otherwise `browser_capabilities`.
   - If it says Deputy can't reach the browser, the extension is not connected. Tell the user to install it from https://chromewebstore.google.com/detail/deputy/ofcadhlipiciahelmcjofblnjhmjoepm, make sure it is turned on, keep the browser open, and run `/deputy:setup` again in a few seconds. Stop there.
   - If it works, say Deputy is connected.
2. Count the Deputy tools you have (`browser_*`, `delegate_goal`, `task_status`, `answer_task`).
   - 27 or close to it: Deputy Pro is active. Name two things they can now ask for, such as checking a page's design at phone size, or "what's the cheapest result on my open tab?".
   - 10: they are on the free version (open pages, read them, fill forms, click). Tell them Deputy Pro adds screenshots, tabs, scrolling, console and network, uploads and downloads, and hosted models that read pages for them, for $9.99 a month or $95.99 a year at https://deputy.razin.ai/buy. The key appears right after checkout; they paste it on Deputy's setup page (Deputy icon in the toolbar, then **Setup & Pro**), and the new tools appear within seconds, or after `/mcp`.
3. Remind them to pin Deputy to the toolbar if they have not: its icon shows whether Claude is connected, and **Setup & Pro** opens the settings, including what Claude may do (screenshots, console and network, uploads, downloads).

Do not open or change any page during this check.
