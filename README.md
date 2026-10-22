# Razin plugins for Claude Code

## Deputy

Deputy lets Claude Code use the browser you already have open, signed in as you. It turns the page in front of you into typed tools: a whole form is one call, and the page never has to be screenshotted to be understood.

### Install

1. **Add the Deputy extension to Chrome** (or Edge, Brave and other Chromium browsers): [Chrome Web Store](https://chromewebstore.google.com/detail/deputy/ofcadhlipiciahelmcjofblnjhmjoepm). Pin it to your toolbar.
2. **Add the plugin in Claude Code:**

   ```
   /plugin marketplace add RazinAI/claude-plugins
   /plugin install deputy@razin
   ```

3. Run `/deputy:setup`. Claude checks that Deputy is connected and tells you what is missing, if anything.

Deputy needs [Node.js](https://nodejs.org) 20 or later; the plugin starts it with `npx -y deputy-mcp`. Once installed, Deputy works in every project.

Added Deputy before with `claude mcp add`? Remove that entry, so Deputy doesn't run twice: `claude mcp remove deputy` (add `--scope user` if you added it that way).

### Free and Pro

| | Free | Pro |
|---|---|---|
| Open pages, read them, fill forms, click | ✓ | ✓ |
| Screenshots, tabs, scrolling, waiting, resizing | | ✓ |
| Console, network, uploads, downloads, inspect | | ✓ |
| Hosted models that read pages for Claude (`browser_ask`, `browser_look`, `delegate_goal`) | | ✓ |
| Price | $0 | **$9.99 a month** or **$95.99 a year** |

Free gives Claude 10 tools. Pro gives all 27, plus 5,000 hosted actions a month (500 a day).

**Get Pro:** [deputy.razin.ai/buy](https://deputy.razin.ai/buy). Your license key appears on the page right after you pay. Paste it on Deputy's setup page: click the Deputy icon in your toolbar, then **Setup & Pro**. Claude gets the Pro tools within seconds; if it still lists 10, run `/mcp` to reconnect.

**Cancel any time** at [deputy.razin.ai/manage](https://deputy.razin.ai/manage) with your key. Your key keeps working to the end of the period you paid for. Full refunds within 14 days of a payment: [refund policy](https://deputy.razin.ai/refunds). Creem, our merchant of record, handles payment, tax and receipts.

### Try it

- "Use Deputy to fill this form with my details from notes.md"
- "What's the cheapest result on my open tab?"
- "Open my GitHub repositories and list the five most recently updated"
- With Pro: "Check the page at localhost:3000 on a phone-sized screen and fix anything that overflows"

On a form that changes something (a payment, a post, a booking), Deputy fills it and asks you before submitting: on the page itself, and in Claude Code. While Claude works in a tab, a small panel in the corner shows each call and Deputy's answer.

### Privacy

Deputy runs on your computer: pages, form values and cookies go only between your browser and the Deputy program on `127.0.0.1`, and from there to Claude. With Pro, when Claude asks Deputy's hosted models to read a page (`browser_ask`, `delegate_goal`), the page text and question go to our server and a zero-data-retention model; a screenshot goes only if you switch that on (`browser_look`). We store neither. Details: [privacy policy](https://deputy.razin.ai/privacy).

### Help

Docs: [deputy.docs.razin.ai](https://deputy.docs.razin.ai) · Support: [hello@razin.ai](mailto:hello@razin.ai) · Site: [deputy.razin.ai](https://deputy.razin.ai)
