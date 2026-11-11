# Brawl on the Mall

Static tournament website. No build step or OpenAI hosting dependency.

GitHub Pages: Settings → Pages → Deploy from a branch → main → / (root).

The deployment files live together at the repository root for direct publishing. HTML files are the homepage, historic results and brand guide; JavaScript handles the demo fixtures, box scores, standings and historic records. Images and SVGs are the public website assets.

The homepage is explicitly demo data. Historic results include confirmed details and labelled gaps.

No contracts, planning documents or original design files are included. Logos and artwork remain the property of their respective owners.

Custom domain: brawl.gwmensrugby.com. Configure this in Pages before setting the brawl CNAME at WordPress to gwrfc.github.io.

## Video and livestream

`video.html` lists the tournament replays; each `replay-*.html` page embeds its corresponding YouTube video. `replays.json` documents the source IDs and titles.

To schedule a livestream, edit `stream-config.js`: set `videoId` to the 11-character YouTube broadcast ID and set `status` to `upcoming`. Use `live` only while broadcasting; the homepage then shows “Live now”. Set `offline` afterwards. A broadcast must be public or unlisted, embeddable, and have live embedding enabled by the channel. No automatic live-status detection is used.

The Google map centers on 38.887536, -77.033543. Named parking and bathroom pins require confirmed coordinates before adding them.
