# Project Starting Point


## Team and GitHub


| Team name | GitHub repository |
|---|---|
| EchoAI  | https://github.com/kunjeshgupta/dso576_project |


## Selected project area


Emerging Artist Discovery 


## Why our team is interested in it
We are interested in this topic because finding new artists helps Spotify make better playlists and match the right songs to the right users. By using data instead of just guessing, we can help small creators get heard and keep users excited with fresh music. 


## Candidate Vision A


Lifecycle/retention manager at Spotify must decide which lapsing listeners to proactively re-engage this month, and which gateway artist to recommend to each.


## Candidate Vision B


Editorial curation lead at Spotify must decide which emerging artists to add to next month’s discovery playlists, and which listener segment to surface each one to.


## Side-by-side candidate assessment (used codex as assistant)


| Assessment | Vision A | Vision B |
|---|---|---|
| Evidence found so far | MLHD+: 583,000 listeners, 27B timestamped logs, median 4.5 year histories. Per user: registration date, first and last scrobble, playcount, age, gender, country. ListenBrainz: live per listen JSON with user_name, listened_at, MBIDs. Now 2.5B listens, dumped twice monthly. So lapse and return are both visible. | "Emerging" is definable from CC0 MusicBrainz alone: artist begin date, type, area, first release dates. No listening data needed. Growth curves come from the same 27B MLHD+ logs. ListenBrainz Spark dump already buckets listens into monthly JSON files |
| Core-data fit | Weak. There are inputs but no output. You’re looking at an example of someone who stopped scrobbling but not someone who stopped listening. Phone changed, plugin removed, and left Last.Fm, all the same as churn. But there’s nothing in any of these that qualifies as an intervention. | Strong. Both sides of the decision-making process (who the artist is and which segment to use) are aggregated; aggregation reduces the per-user error that ruins A. Backtest for free: stop at month t, identify artists, and check their actual growth at t+6. |
| Biggest risk | Unfalsifiable. The best possible prediction is who will return by themselves, which is not the correct target population. Additionally: MLHD gathered around 2013 to 2014, therefore it is outdated. Authors also point out that they can’t distinguish between genuine preference and recommendation algorithms. | Population relocation. They are not users of Spotify. ~58% males and 23% females, average age of 25.4, 57.5% aged 15 to 24 years old, mainly found in Northern Europe, North America, Australasia, voluntary enthusiasts. “Emerging here” does not necessarily imply an emerging mainstream. Can be bounded if mentioned. |


## Core data source we confirmed we can access


[Source, original link, and what successfully opened.]
https://musicbrainz.org/doc/MusicBrainz_Database/Download 
https://musicbrainz.org/doc/About/Data_License 
https://listenbrainz.org/data/


## Three questions we still need to resolve


1. Which listener sub communities are visible in the listen histories, and how far do their demographics (age, gender, country) diverge from a mainstream streaming population?
2. What specific quantitative threshold will we enforce to define an artist as "emerging" versus established?
3. What measure will determine which listener segment is the best fit for different emerging artists?


## Role-file progress


Use one of these status labels: **Not started**, **In progress**, **Ready for team review**, **Complete**, or **Not applicable**.


| Role file | Owner | Status |
|---|---|---|
| [`objectives.md`](objectives.md) | Lorelei Ventura | [Not started] |
| [`alternatives.md`](alternatives.md) | Navya Gupta | [In Progress] |
| [`data-fit.md`](data-fit.md) | Hosung Kim | [Not started] |
| [`auxiliary.md`](auxiliary.md) | Tony Lu | [Not Started] |
| [`technical.md`](technical.md) | Kunjesh Gupta| [Not Started] |
| [`objections.md`](objections.md) | N/A | [Not applicable] |


## Team check


- [x] We added our team name and the correct private GitHub repository link.
- [x] We selected the area based first on genuine team interest.
- [x] A and B are distinct candidate Visions within the same area.
- [x] The candidate comparison uses verified evidence rather than unsupported claims.
- [x] At least one data source opened, or we recorded the access blocker.
- [x] We preserved three real questions instead of hiding uncertainty.
- [x] Every active role file has an owner and a current status.
- [x] Every teammate reviewed this provisional starting point.

