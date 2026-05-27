# SLICC Presentation — IKEA Manual Format

## Meta

- **Event**: AI Native DevCon (Tessl)
- **Date**: June 1, 2026
- **Duration**: 30 min
- **Format**: Demo / Tools-in-action
- **Track**: The Latent Space
- **Title**: The Agent Enablement Platform
- **Subtitle**: Building AI agents in the browser, for the browser, of the browser
- **Speaker**: Lars Trieloff, Principal Scientist at Adobe

## Narrative Structure

**Duarte Sparkline** with **Hero's Journey bookends**.

The presentation runs as a full-screen SLICC sprinkle. The audience believes they are watching a normal slide deck. At the midpoint (the physical paper flip-over), Lars minimizes the sprinkle, revealing the SLICC interface underneath. The S.T.A.R. moment: the presentation WAS the demo all along.

## Format

- 24 panels (12 front / 12 back)
- IKEA construction manual aesthetic (justified by the origin story)
- First and last panels bookend: "absurd" → "enticing"
- The fold flip-over IS the dramatic reveal

## Takeaways

1. The browser is a powerful agent runtime — nay, "agent funtime"
2. SLICC is not a toy: used actively by hundreds of people doing real work
3. Try SLICC, give it a lick: `npx sliccy`

---

## Front Side (Panels 1–12): "The Presentation"

The audience sees what looks like a normal slide deck.

### Panel 1 — Bookend Open

"End of February I stood at the IKEA restaurant, hot dog in one hand, soft serve ice cream in the other, and thought about lobsters. I should clarify: I thought about OpenClaw. I'm not an overly cautious person (as you'll see), but the thought of an agent taking over my entire computer seemed absurd."

### Panel 2 — What Is #1: Disembodied Agents

AI agents today: cloud containers, remote sandboxes, terminal-only harnesses. Powerful but disembodied. They can't see what you see. They can't act where you act.

### Panel 3 — What Could Be #1: Browser-Native

What if the agent ran where your life already happens? The browser. Not adjacent to it — inside it.

### Panel 4 — What Is #2: The Chat-Panel Trap

Every product team ships their own confined AI chat box. Each one blind to the next tab over. Every one of them is XKCD 927.

### Panel 5 — What Could Be #2: One Agent, Unconfined

One agent that sees your Slack, your email, your CMS, your code. Not because it has special API access — because it IS the browser.

### Panel 6 — What Is #3: Skill Issues

Agents don't lack capability. They lack context. You can't hardcode every workflow into a product.

### Panel 7 — What Could Be #3: Skills as Markdown

Skills are fancy markdown files. Teach, don't build. Install from a marketplace, reverse-engineer from a HAR file, or author one in 5 minutes.

### Panel 8 — What Is #4: "Can You See My Browser?"

March 2025. I ask Claude: "Can you see what's on my browser?" Response: "I cannot access your device or view what's on your screen."

### Panel 9 — What Could Be #4: The Self-Licking Ice Cream Cone

SLICC: Self-Licking Ice Cream Cone. A browser-native agent. It runs IN the browser. It controls THE browser. It IS the browser.

### Panel 10 — What Is #5: Things Your Browser Can't Do

Things you know your browser can't do: take photos, convert videos, play audio files, be a web server.

### Panel 11 — What Could Be #5: You're Wrong

You're wrong. All of it. ffmpeg captures your webcam. say speaks aloud. serve hosts files over HTTP. The browser can do everything — we just forgot to ask.

### Panel 12 — S.T.A.R. / The Flip

"Let me show you what this looks like in practice."

*Lars minimizes the sprinkle. The SLICC interface is revealed underneath. The presentation was running inside the agent the entire time.*

---

## Back Side (Panels 13–24): "The Demo"

Post-reveal. Lars is now in live demo mode. These panels serve as reference cards shown during the demo and as leave-behind material.

### Panel 13 — Sprinkles

What you just saw. Persistent UI panels — rich generative interfaces created on the fly by a scoop. This entire presentation is a sprinkle.

### Panel 14 — Licks + Live QR Demo

Licks: asynchronous events from the outside world. Webhooks, cron jobs, external signals.

*Live demo: sets up a webhook, generates a QR code, challenges the audience to scan and send a request. Messages arrive in real-time throughout the rest of the talk.*

### Panel 15 — Dips

Inline widgets in chat. Ephemeral, interactive, lick-only. Buttons, forms, visualizations — zero overhead. No scoop needed.

### Panel 16 — Scoops

Parallel sub-agents with isolated sandboxes. Own filesystem, own context, own skills. The cone orchestrates; scoops do the heavy lifting.

### Panel 17 — Architecture

The technical underpinnings: pi-agent (the agent loop), just-bash (shell runtime), durableworker (persistent execution), WASM (portable compute). The browser IS the container.

### Panel 18 — Protocols

HTTP (duh), WebRTC (peer-to-peer), WebSockets (real-time), CDP (Chrome DevTools Protocol). The full network stack, running client-side.

### Panel 19 — Dev Tools

A real shell environment. git, node, python, playwright, ffmpeg, magick. If it runs in a browser, it runs here. Write .jsh scripts to extend.

### Panel 20 — MCP via CLI

`mcp add <url>` — one command to register any MCP server. Every tool surface becomes a shell command. No config files, no plumbing.

### Panel 21 — Electron + Tray

Inject into Slack, Outlook, Cursor — any Electron app becomes a remote-controllable target. Join the tray. Multi-browser sync in real time.

### Panel 22 — oauth-token --intercept

Piggyback browser sessions for good. The agent uses your existing auth. No API keys, no config files, no secrets in environment variables. You're already logged in.

### Panel 23 — Photo Roast (Live Demo)

*Live demo: ffmpeg captures a photo of Lars presenting. Vision model analyzes and roasts it. `say` delivers the verdict aloud through the speakers.*

### Panel 24 — Bookend Close

"...and now you see why the thought of an agent taking over your entire browser should seem enticing. Give it a lick."

`npx sliccy`

---

## Production Notes

- Panel images: generate with Wavespeed (IKEA instruction manual style illustrations)
- The sprinkle runs the Three.js paper-folding simulation as navigation
- Panel 14 (licks): wire up a real webhook + QR code generator before the talk
- Panel 23 (photo roast): wire ffmpeg capture → vision → say into the presentation flow
- Panel 12 (the flip): the physical paper fold-over animation IS the reveal transition
