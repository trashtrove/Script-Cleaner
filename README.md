Okay to all my typesetters out there that use TypeR or just I guess just TS-ers in general, I made a website and some code that should edit PR-ed scripts into a simple consistent set up. This has been an on-going mini project I've been working on and I think she's finally useable enough. That being said, there will obv be some kinks and bugs to work out, so if you encounter any of them let me know. Or if you've got a suggestion/feature addition~

Here's what it does organized by category:
1. Clean-up and formatting.
- It'll remove hidden HTML, double spaces and non-breaking spaces that often cause formatting issues when copying stuff from Google Docs
- It will identify and remove staff internal notes that aren't super necessary for our job. Like TL/N to PR for example
- It will detect page markers (e.g., "Page 1" or "162.png") and ensure they are properly spaced and adds a clear separation to keep the script organized

2. SFX Handling
- It detects whether the original SFX is in Korean, Japanese, or Chinese
- Regardless of how the SFX was pasted (whether it used colons, spaces, or mixed formats), it forces them into a standardized, clean format (e.g., jsfx: [Original] followed by sfx: [Translation]). This way in a program like TypeR, you can set under tags to ignore: jsfx, ksfx, or csfx so it doesn't paste the original language and you don't have to go back and delete that. 

3. Smart Review Engine (cause I kept breaking everything with each new change)
-When it sees consecutive lines that look like revisions (i.e., they contain very similar wording), it automatically groups them together.
- Instead of silently deleting lines (which risks deleting the wrong one, which kept happening so damn often with this code, this became necessary), it presents them in a smart review UI. 
- It will pre-select what it thinks is the correct final version but allows you to "toggle" any version of a line on or off. The output box updates in real-time, allowing you total control before you copy the final result

4. Technical Shit
- It won't just guess based on the "Tag." it looks at the actual words in the sentences. If it sees two lines for the same character that are 25%+ similar, it will treat them as a revision group. If they are two completely different sentences, it will treat them as separate bubbles, ensuring you never accidentally lose dialogue. 
- You can paste everything right from Google Docs, and it'll keep the OG formatting so you can directly compare the final version to the original to check for potential mistakes. 
