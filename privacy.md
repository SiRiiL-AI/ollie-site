---
layout: default
title: Privacy Policy
---

# Ollie — Privacy Policy

**Last updated:** 14 July 2026

Ollie is a desktop application that runs entirely on your own computer. This policy
explains what it does with your data, and — more importantly — what it does not.

## The short version

**We do not operate any servers, and we never receive your data.** Ollie has no backend
of ours to send anything to. Your email, files, chats and everything Ollie remembers are
stored in databases on your own machine.

## What Ollie accesses

With your explicit consent, Ollie can read:

| Source | Google scope | Why |
|---|---|---|
| Gmail | `gmail.readonly` | To read your recent email so it can answer questions about it |
| Google Drive | `drive.readonly` | To find and read documents you ask about |
| Your email address | `userinfo.email` | To label the connected account in the app |

Ollie only ever **reads**. It cannot send email, delete anything, or modify your files —
the permissions it asks for do not allow it.

## Where your data goes

**Stored on your computer only.** Ollie keeps everything it reads, and everything it
remembers, in a Postgres and a Neo4j database inside `%LOCALAPPDATA%\Ollie` on your
machine. Your Google access tokens are stored there too, encrypted. Uninstalling Ollie
leaves that folder in place; deleting the folder destroys all of it permanently.

**Sent to the AI model you configure.** This is the one place data leaves your machine,
and you should understand it clearly. To answer your questions, Ollie sends the relevant
parts of your content — an email body, a document excerpt, your message — to the language
model provider you configured with your own API key (by default,
[OpenRouter](https://openrouter.ai), which routes to the model you select). That provider
processes it under its own privacy policy and terms. If that is unacceptable to you, do
not connect accounts whose contents you are unwilling to send to a model provider.

**Sent to Google.** Ollie talks directly to Google's APIs from your computer, using your
own authorisation. Nothing is proxied through us.

## What we collect

**Nothing.** No analytics, no telemetry, no crash reporting, no account, no sign-up. We
have no way of knowing you use Ollie.

## Google API Services User Data Policy

Ollie's use and transfer of information received from Google APIs adheres to the
[Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy),
including the Limited Use requirements.

Specifically: data obtained from Google APIs is used only to provide and improve the
features you can see in the app; it is not sold, not transferred to third parties except
the AI model provider you yourself configure (in order to fulfil your own request), and
not used for advertising. No human at Ollie reads your Google data — we cannot, because
it never reaches us.

## Removing access

- **In Ollie:** Connections → Disconnect.
- **In Google:** revoke Ollie at
  [myaccount.google.com/permissions](https://myaccount.google.com/permissions).
- **To erase everything Ollie stored:** delete the folder `%LOCALAPPDATA%\Ollie`.

## Children

Ollie is not directed at children under 13 and should not be used by them.

## Changes

If this policy changes materially, the updated version will be published at this URL with
a new date at the top.

## Contact

Questions about this policy: **agentic.siriil@gmail.com**
