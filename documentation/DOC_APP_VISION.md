# App vision & goals

> **Vision status:** `ACTIVE`

Static product brief for What to Do. Agents read this before ambiguous product or UX work. **SSOT** for problem, persona, and the app’s role relative to users.

---

## Problem statement

People around 30 who want to hang out and do fun things with friends don't keep track of everything that is going on in Utrecht. To find out, they check the Utrecht UiT agenda, neighbourhood magazines, posters at bus stops and the agendas of the major venues. That means checking many places, because nothing aggregates them. Filtering and search on those sites are poor: the categories don't let you refine, so if you like a certain music genre you can't find music like that. Even the biggest agenda, the UiT agenda, covers only cultural activities (no pub quizzes, for example) and shows part of what's going on, not everything. Smaller agendas, down to single neighbourhoods, each cover another piece.

---

## User persona

- **Label:** a Utrecht resident around 30 who likes going out with friends
- **Goals:** find fun things to do in the city that match what they're into
- **Frustrations:** too many places to check, filters on categories that don't make sense, keyword search that misses what they mean, and a narrow selection on each site

---

## App’s role

What to Do crawls the event agendas of Utrecht, from the UiT agenda down to neighbourhood level, aggregates them in one place, and refers back to the website each event came from. People find things with one search bar that understands what they mean (semantic search over a vector embedding per event, not keyword search), with date and location filters outside the search bar, instead of endless category filters. Good metadata per event supports this.

- **In one sentence, this app:** gathers everything there is to do in Utrecht in one place and makes it easy to find what you're into.
- **It is not:** a ticket seller, a tool for planning outings, an app with user accounts, a place where people or venues submit events (not in v1), or a guide to cities other than Utrecht.
- **Integrates with / assumes:** the event websites and agendas of Utrecht, which it crawls and links back to.

---

## North-star goals

- **Goal 1 (coverage):** anything listed on another Utrecht "things to do" website is also on What to Do.
- **Goal 2 (findability):** anything from another site is easier to find on What to Do than on that site itself.

---

## Open questions

- **How people and agents reach the data:** a standard web interface for filtering the database, access for any web agent (for example Gemini reading the site), an MCP server so people connect the database to their own assistant such as Claude, or the app's own agentic search. The leaning is away from an own agentic search and toward semantic search combined with date and location filters; the access channel is still open.
