Business rulebook version: v211 | index: instructions.md | rule text: the rules files named in the index | updated: 2026-11-11

# Tools register

Reviewed tools, by the roadmap stage they're for. A project suggests a tool only at its stage or later, and never installs one without reading all its files and getting the owner's yes. Prices and terms change: check them on the day.

## Any stage
- Customer panel (github.com/Jakeschincariol/founder-skill, consumer part), reviewed 9 November 2026: simulates buyers to test a message or offer. Clean: standard Python, no network. Use it to rank messages before real sends, never to forecast reply or buy rates; calibrate it on a message already sent with known results first.
- Video-making skill (built into Claude): animated text and chart videos, free, in chat.
- find-skills (adapted from github.com/vercel-labs/skills): suggests a better skill only when one clearly helps; never installs without a yes.

## From S3 (content and paid ads: L60, L61)
- Higgsfield official connector (https://mcp.higgsfield.ai/mcp), reviewed 10 November 2026: realistic AI video inside Claude. Paid plan needed (from $15 a month for 200 credits). A 10-second clip is about 70 credits at 720p and 160 at 1080p; expect 2 to 4 attempts per clip, so roughly $30 to $50 per finished 30-second ad. Start on the smallest plan and measure the real retry rate. Real footage of the owner first; AI people never presented as real (W1, X13).
- Meta Ad Library research skills, reviewed 10 November 2026: show what competitors are running. The Library shows no spend or results for UK and US commercial ads, so "winning" only means "running a long time". Learn angles and formats; never copy creatives or exact copy.
- Remotion official skills (github.com/remotion-dev/skills), reviewed 9 November 2026: higher-quality animated video, captions, voiceover. Free for individuals and very small companies; needs Claude Code on the owner's computer. The owner's chosen animation tool (10 November 2026). Setup when the stage arrives: install Claude Code, open an empty folder and ask for a vertical 1080x1920 reel project; paste the script and ask for one animated scene per sentence (headlines, app windows, counters, charts); add the voiceover file and ask for animations timed to it, captions on every word, and an mp4 render. Use the official skills only, never an unread skill sent by direct message. Before S3, a one-off sales explainer can be made with the video-making skill above.
- fal.ai video skills: pay per use (about $0.25 for a 5-second clip on some models), needs Claude Code and an API key.
- Artflow (app.artflow.ai), reviewed 9 November 2026: AI likeness of the owner in photos and video. Trust risk with sceptical buyers; always label as AI.

## After the first target
- Apify lead-list skills, reviewed 10 November 2026: build lists from Google Maps and websites. Paid per result; personal emails and LinkedIn often missing or guessed; Google's terms prohibit Maps scraping (prefer official APIs). Apply the country's outreach law (UK: PECR, UK GDPR; US: CAN-SPAM) before any send.
- Replica (github.com/Jakeschincariol/replica-skill), reviewed 10 November 2026: skills for cloning apps, not for video. Its review-reading part is useful for spotting what users hate about an existing product.

## Don't use
- Open-Higgsfield-AI (github.com/Anil-matcha/Open-Higgsfield-AI): a copycat front end for another paid service; unsigned installers that ask to switch off security checks; sold on "no content filters".
- FreeLLMAPI (github.com/tashfeenahmed/freellmapi): stacks free AI tiers; free tiers may use what's sent to train models, so never use it with client or prospect data. The author says it's for experiments only.
