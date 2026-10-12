# Blame the Manager privacy policy

Version: 2026-10-12

Leia em português: https://tombo-studio.github.io/blame-the-manager/privacidade/

Blame the Manager only sends anything off your computer if you accept. This
page says what leaves, what stays, where it goes and how to change your mind.

Sending serves two purposes: finding and fixing crashes and bugs, and measuring
where people get lost in the game in order to improve it.

## 1. Who is responsible for the data?

JMC Tecnologia da Informação Ltda., CNPJ 54.004.699/0001-97, based in Brazil,
which operates the Tombo Studio label and publishes the game. It is the data
controller under the LGPD (Brazilian Law 13,709/2018) and the GDPR. Contact:
juliano@jmcoimbra.eng.br.

## 2. What does the game send, and what does it leave out?

Nothing leaves without your consent. The full record of every session always
stays on your computer, in the game's log folder, with or without consent.

If you accept, this is what leaves:

| Leaves | Kept out of the uploaded record |
|---|---|
| A session identifier of 8 characters, drawn again for every session (every time the game opens and every career started or loaded), and a random number for the same session that only tells apart, in storage, two sessions with the same identifier; a career identifier, drawn when the career starts and stored in its save (for a career started before this version, computed on loading from the world seed and the starting club, without being stored), which goes on every line once the career is open; with them, the game version, the world seed, the operating system, the language and the origin of the session | Your name, your e-mail and your Steam or itch.io account |
| The session's events: screens opened, decisions made, match results | The names you type for the chairman, the club or the career, and the names of players, coaches and staff, including those from a name pack you imported: the game removes them from the session record before sending |
| The message and stack of an error, with the folder path of your computer removed | The folder path, the machine name and your system user name |
| One line per session with the system version, the graphics card and its vendor, the resolution, the display scale and the renderer | Any installation, account or personal identifier |
| On a crash, the technical report of the moment it failed (minidump), with the system and the device | The minidump is the exception to this column: it copies fragments of the game's memory at that moment and can carry any text that was in it, including a name you typed or a folder path |

The session identifier changes with every session. The career identifier is
the same in every session of a career, and it only serves to link them to each
other: two careers started from this version on have different identifiers,
and it says nothing about the computer or about who plays. The world seed goes
on every line because it is what reproduces a bug, and it is also the same in
every session of a career. The device line also repeats across sessions on the same computer. None
of this says who you are, and we do not use the data to try to find out who
played.

As with any internet connection, your IP address reaches the providers below
so that the upload can happen. We do not store it (section 3).

## 3. Where does it go?

- **Crash reports:** Sentry, in its European Union region (Frankfurt,
  Germany). The game does not put your IP address in the report, and the
  project is configured not to store the connection's address.
- **Session records:** Cloudflare, in R2 storage owned by the game, created
  in the European Union jurisdiction: the records are stored in data centers
  inside the European Union. The server that receives the upload does not
  record your IP address; Cloudflare's network processes it in transit to
  deliver the connection.

Sentry and Cloudflare are United States companies. Both store the data
outside Brazil, in the European Union: Sentry in Germany, Cloudflare in the
European Union jurisdiction. Nobody beyond the two providers receives this data,
and it is never sold or used for advertising.

## 4. How long is it kept?

- **Session records:** 12 months, deleted automatically by a storage rule.
- **Crash reports:** the retention configured in the Sentry project, 30 days.

## 5. On what legal basis?

Consent: LGPD art. 7, I, and GDPR art. 6(1)(a). You give it on the card the
game shows the first time it opens, and you can withdraw it at any time with
the same effort.

## 6. How do I turn it off?

In Settings, on the Privacy card, switch sending off. The game stops sending
the record and error reports at once and deletes what was queued; the report
of a crash that closes the game stops from the next launch. The local record
stays on your computer, and so does the list of the ids of sessions already
sent (section 7). Declining or switching off changes nothing in the game.

## 7. How do I request access or deletion?

Write to juliano@jmcoimbra.eng.br with the session ids. In Settings, on the
Privacy card, the game shows the id of the open session, and the button Copy
the ids of sent sessions copies the ids of every session that has reached
Tombo Studio from this computer. That list is kept only on your computer, with
the id and the date of each session's first upload and nothing else, and switching sending off
does not delete it, because it is what lets you request deletion of what was
already sent. Since no data links a session to you, those ids are the only way
to find what was sent. The id has 8 characters and another session may share
it: a deletion request removes every stored session with that id.

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

The date at the top is the version. The game shows the version in force in
Settings, on the Privacy card, and asks for your consent again when it
changes. Earlier versions stay in this page's history.
