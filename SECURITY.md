# Security

## Report a vulnerability privately

**[Open a private security advisory](https://github.com/loopcrack-org/kensa-app/security/advisories/new)**

That form is private between you and us. GitHub hosts it; nothing is published
until we publish it, and you can see what we are doing about it the whole time.

## Do not use the normal channels

Neither [kensa.ai/report](https://kensa.ai/report) nor a regular issue is safe
for this. Both publish **immediately and permanently**, to everyone, before
anyone can fix anything.

This is worth being blunt about, because the mistake is easy and it cannot be
undone:

- An issue is public the second it exists. Search engines index it.
- Deleting it afterwards does not recall it — it was already readable, and
  anything that scraped it still has a copy.
- A screenshot proving the vulnerability goes to a **public** bucket where the
  URL is the only access control, nothing expires, and deleting the issue does
  **not** delete the file.

So a well-meant report through the wrong door is a working exploit, published
by us, with instructions.

## What counts

If you are unsure, use the private channel. A false alarm there costs us five
minutes; a real vulnerability in the public tracker costs everyone.

Some examples of things that belong here rather than in an issue:

- Anything that exposes credentials, tokens, or another user's data
- Anything that lets code run that the user did not ask for
- Anything that lets someone act as another user, or reach a repository they
  were not granted
- Anything where the words "I could read/write/delete something I should not
  have been able to" apply

## What to expect

We are a small team. We will confirm receipt, tell you honestly whether we can
reproduce it, and say what we are doing. If we decide not to fix something, we
will say that and why rather than let the thread go quiet.

We do not run a bug bounty and cannot pay for reports. We will credit you in
the advisory if you want to be credited, and not if you do not.

## Scope

This repository holds Kensa's releases. The vulnerability you found is probably
in the desktop app, the website, or the backend behind them — report it here
regardless. Kensa's source lives in a private repository, so this is the right
front door for all of it.
