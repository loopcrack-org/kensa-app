# Contributing

**Kensa's source is not public.** This repository holds the releases and the
issue tracker — there is nothing here to send a pull request to.

That is not a brush-off. A problem report with clear steps is worth more to us
than a patch, because it is the thing we cannot produce ourselves: we only see
the bugs that happen on our own machines. Yours are the ones we are missing.

## What belongs here

**Things that are broken.** That is the whole scope of this tracker.

Not ideas, not feature requests, not questions, not support. Those get closed
with `out-of-scope` and a reason — not because they are unwelcome as thoughts,
but because there is no one watching a channel for them, and an issue nobody
will action is worse than an honest "no": it looks like it is being handled.

If something is broken, we want to hear it even if your report is thin. "It
stops responding when I click Start Review" is useful. Send it.

## How to report

**Two ways, and they are genuinely different.**

### 1. [kensa.ai/report](https://kensa.ai/report) — no account needed

> **Not live yet.** This page ships with the next website release; until then it
> answers 404 and the GitHub route below is the only one. Said here rather than
> quietly linked, because a dead link in a contributing guide is how somebody
> concludes the project is abandoned.

Use this if you do not have a GitHub account, or do not want to use it. A form
that demands sign-in breaks exactly when sign-in is the thing that broke, so
this one never asks.

**Save the link we give you.** This matters and it surprises people: an issue
filed through the form is created by our account, not yours. You are not the
author and **you will not be notified of anything** — not a reply, not a fix,
not a close. The URL we return is your only way back to it.

### 2. Opening an issue here directly

Use this if you have a GitHub account. It is the better channel for one
concrete reason: **you are the author, so we can actually reach you.** If your
report needs a follow-up question, this is the only place we can ask it.

## What happens next

Your report arrives labelled `needs-triage`. A classifier reads it, adds a
summary and labels, and marks its own work `triaged:ai` — because a machine's
classification is a guess, not a verdict. A person removes that label once they
have actually looked.

The classifier never closes an issue and never replies. Those are decisions,
and decisions are not made by something that cannot be argued with.

### The labels, and which ones you can influence

| Family | What it means |
|---|---|
| `impact:*` | How much of Kensa still works. **You state this** — it is a fact, not an opinion. |
| `priority:*` | **Computed** from impact and what your session proved. Never asked for, because everyone's own broken thing is genuinely the most urgent thing in their day. |
| `reporter:*` | **Verified** from the request. You cannot set it. |
| `claimed:*` | **What you told us** about yourself. Useful, never treated as evidence. |
| `surface:*` | Where it failed — desktop, web, install, account. |
| `confirmed` | We reproduced it. Different from "someone reported it". |

`reporter:` and `claimed:` are separate on purpose. One is what we checked, the
other is what was said, and merging them would make every label in this tracker
untrustworthy.

## Security problems do NOT go here

**Do not open an issue for a vulnerability, and do not use the report form.**
Both publish immediately, to everyone, before anything can be fixed.

Read [SECURITY.md](./SECURITY.md). It takes a minute and it is the difference
between a fix and a zero-day.

## Before you attach a screenshot

Attachments go to a **public** bucket. The URL is the only access control,
nothing expires, and **deleting the issue does not delete the file**. Crop out
anything you would not publish — tokens, private repository names, customer
data, other people's faces.

We strip location and camera metadata from PNG and JPEG. GIF, WebP and video
are stored exactly as you sent them.

## Pull requests

We cannot accept them. The source is private, so a pull request here could only
touch what is actually in this repository — the README, the changelog, this
file, the security policy and the issue templates. The first two are written by
our release process and would be overwritten on the next release; the rest are
generated from the private repository, so a change here would be reverted the
next time they are regenerated rather than merged.

GitHub does not let a public repository turn forking off, so nothing stops you
opening one. It will be closed with a pointer back to this file. That is not
rudeness; there is genuinely nowhere for it to go.
