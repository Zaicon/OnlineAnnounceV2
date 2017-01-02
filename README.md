# AIO
![Version 1.0.0](https://img.shields.io/badge/Version-1.0.0-blue.svg)
![API 2.0](https://img.shields.io/badge/API-2.0-green.svg)

Introduction
-----
This plugin allows players to "announce" when their online status changes (joining or leaving the server).

Commands
-----
`/greet <announcement>` `/leave <announcement>`<br />
Sets the user's greeting or leaving announcement.

`/readgreet <player>` `/readleave <player>`<br />
Reads the specified player's greeting and leaving announcements.

`/setgreet <player> <announcement>` `/setleave <player> <announcement>`<br />
Sets the specified player's greeting or leaving announcement.

Permissions
-----
`oa.greet`<br />
Allows use of: `/greet` `/leave`

`oa.mod`<br />
Allows use of: `/readgreet` `/readleave` `/setgreet` `/setleave`<br />
Allows use of color tags in announcements.

Database
-----
_onlineannounce_

| Column Name | Type | Length |
| --- | --- | --- |
| userid | Int32 | 6 |
| greet | VarChar | 100 |
| leaving | VarChar | 100 |