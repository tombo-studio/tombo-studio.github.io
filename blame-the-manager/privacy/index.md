# Blame the Manager privacy policy

Version: 2026-11-08

Leia em português: https://tombo-studio.github.io/blame-the-manager/privacidade/

Blame the Manager only sends anything off your computer if you accept. This
page says what leaves, what stays, where it goes and how to change your mind.

The game asks two separate questions, one for each level of sending. Crash
reports serve to find and fix crashes and bugs. How you play serves to measure
where people get lost in the game in order to improve it, and also to
reproduce a bug. Each answer covers only its own level: if you accept one and
decline the other, only what you accepted is sent.

## 1. Who is responsible for the data?

JMC Tecnologia da Informação Ltda., CNPJ 54.004.699/0001-97, based in Brazil,
which operates the Tombo Studio label and publishes the game. It is the data
controller under the LGPD (Brazilian Law 13,709/2018) and the GDPR. Contact:
juliano@jmcoimbra.eng.br.

## 2. What does the game send, and what does it leave out?

Nothing leaves without your consent, and each level has its own. The full
record of every session always stays on your computer, in the game's log
folder, with or without consent.

### Crash reports

If you accept this level, this is what leaves when the game crashes or hits an
error:

| Leaves | Kept out of the uploaded report |
|---|---|
| The error message and stack, with the folder path of your computer and the name of a saved career removed | The folder path, the machine name and your system user name |
| For an error in the game and for a stall, the names of the last 20 game events before it, each with the time it happened | What those events contain: decisions, numbers and names stay on your computer |
| The session identifier (8 characters, drawn again for every session), once the session has opened, the game version and the origin of the session | Any installation, account or personal identifier: the report's user identifier is zeroed |
| For an error in the game, the operating system name and the graphics card's vendor and family; for an error in the game engine, also the system version and the device model, as the system reports them | For an error in the game, the system version, the device model and name, the screen resolution, and the graphics card's identifiers and driver version |
| When the game stops responding for 30 seconds, the open screen, the season, the week and how many seconds it was stuck | The stack: the game does not send it in this case |
| On a crash that closes the game, the technical report of the moment it failed (minidump), with the system and the device, sent at the next launch | The minidump is the exception to this column: it copies fragments of the game's memory at that moment and can carry any text that was in it, including a name you typed or a folder path |

A report's session identifier only links to a stored record when you also
accept the second level. With only this level accepted, the record of that
session stays on your computer.

### How you play

If you accept this level, this is what leaves during your career:

| Leaves | Kept out of the uploaded record |
|---|---|
| A session identifier of 8 characters, drawn again for every session (every time the game opens and every career started or loaded), and a random number for the same session that only tells apart, in storage, two sessions with the same identifier; a career identifier, drawn when the career starts and stored in its save (for a career started in a version of the game that did not store it yet, computed on loading from the world seed and the starting club, without being stored), which goes on every line once the career is open; with them, the game version, the world seed, the operating system, the language and the origin of the session | Your name, your e-mail and your Steam or itch.io account |
| The session's events: screens opened, moments you marked with F8 or M (the screen, the week and the minute; the note you type stays on your computer), decisions made, match results, and errors, with the message and stack without the folder path | The names you type for the chairman, the club or the career, and the names of players, coaches and staff, including those from a name pack you imported: the game removes them from the session record before sending |
| One line per session with the major system version, the graphics card's vendor and family, the nearest standard resolution (or none, when the screen is far from all of them), the display scale, the renderer and whether the device is a Steam Deck (worked out from the graphics card name, with no identifier) | Any installation, account or personal identifier |
| For each chunk, what triggered cutting it for upload and its number | Your answers to these two questions: they stay only in the record on your computer |

The session identifier changes with every session. The career identifier is
the same in every session of a career, and it only serves to link them to each
other: two careers with a stored identifier have different identifiers, and it
says nothing about the computer or about who plays. The world seed goes on
every line because it is what reproduces a bug, and it is also the same in
every session of a career. The device line also repeats across sessions on the
same computer. None of this says who you are, and we do not use the data to
try to find out who played.

As with any internet connection, your IP address reaches the providers below
so that the upload can happen, on both levels. We do not store it (section 3).

## 3. Where does it go?

- **Crash reports:** Sentry, in its European Union region (Frankfurt,
  Germany). The game does not put your IP address in the report, and the
  project is configured not to store the connection's address.
- **How you play:** Cloudflare, in R2 storage owned by the game, created
  in the European Union jurisdiction: the records are stored in data centers
  inside the European Union. The server that receives the upload does not
  record your IP address; Cloudflare's network processes it in transit to
  deliver the connection.

Sentry and Cloudflare are United States companies. Both store the data
outside Brazil, in the European Union: Sentry in Germany, Cloudflare in the
European Union jurisdiction. Nobody beyond the two providers receives this data,
and it is never sold or used for advertising.

## 4. How long is it kept?

- **Crash reports:** the retention configured in the Sentry project, 30 days.
- **How you play:** 12 months, deleted automatically by a storage rule.

## 5. On what legal basis?

Consent, one for each level: LGPD art. 7, I, and GDPR art. 6(1)(a), and, for
players in the European Union, Directive 2002/58/EC (ePrivacy), art. 5(3). You
give it on the screen the game shows the first time it opens, before the board's
letter: neither question comes with an answer selected, Send and Don't send
are the same size, and the game only moves on once the questions on the screen
are answered. The game has no account, sign-up or login. You can withdraw each
consent at any time, with the same effort (section 6).

## 6. How do I turn it off?

In Settings (the ⚙ button), on the Privacy card, there is one switch for each level, and each
one stops only its own.

- **Send crash reports:** switched off, the game stops sending error reports at
  once; the report of a crash that closes the game stops from the next launch.
- **Send how you play:** switched off, the game stops sending the record at once
  and deletes what was queued. Switched on, sending starts with the next career
  you start, continue or load.

What already reached the server stays until the period in section 4 or a
deletion request (section 7). The local record stays on your computer, and so
does the list of the ids of sessions already sent. Declining or switching off changes nothing
in the game.

## 7. How do I request access or deletion?

Write to juliano@jmcoimbra.eng.br with the session ids. In Settings, on the
Privacy card, the game shows the id of the open session, and the button Copy
the ids of sent sessions copies the ids of every session whose record the game
has started sending to Tombo Studio from this computer. That list is kept only
on your computer, with the id and the date of each session's first upload and
nothing else, and switching sending off does not delete it, because it is what
lets you request deletion of what was already sent. Since no data links a
session to you, those ids are the only way to find what was sent. The id has 8
characters and another session may share it: a deletion request removes every
stored session with that id.

The list does not keep sessions that sent only crash reports, and the game
does not keep their ids anywhere. Those reports are deleted on their own after
30 days (section 4). To request deletion sooner, send the id of the open
session, which Settings shows: it only helps while the session of the error is
still open, and a crash that closes the game takes the session with it.

You can ask for confirmation of processing, access, correction,
anonymisation, blocking or deletion, portability, restriction of processing
and information on who the data was shared with; you can object to the
processing and withdraw your consent at any time (LGPD art. 18; GDPR arts. 7(3)
and 15 to 21). You can also complain to the ANPD in Brazil, or to the data
protection authority of your country.

JMC is a small-scale processing agent and, under ANPD Resolution CD/ANPD
No. 2/2022, art. 11, is exempt from appointing a data protection officer. The
e-mail above is the channel for data subjects.

## 8. What happens when this policy changes?

The date at the top is the version of the text, and the game shows it in
Settings, on the Privacy card. Each level also has the date of its scope, the
last time what it sends changed:

Crash reports scope: 2026-10-31

How you play scope: 2026-10-31

The game asks about a level again only when its scope changes, and the scope
changes when that level starts sending new data, to a new destination or for a
longer time. A correction to the text, an address or a translation changes only
the date at the top, and the question does not come back. If you answered the
single question of version 2026-10-31, the same answer stands on both levels; if
you answered in an earlier version, you see the question again.

Earlier versions stay in this page's history.
