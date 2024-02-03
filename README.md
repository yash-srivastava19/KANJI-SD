## KANJI-SD

Kanji are basically japanese character which are basically used to give meaning of content words(basically logographic writing system). These are adapted from Chinese script, and although old, are still used apart from the subsequently derived scripts.
KanJI-SD is an attempt to generate novel meanings for words for which Kanji doesn't exist using a simple stable diffusion pipeline. This works because the text encoder part of the SD is fixed, and it can use interpolation the embeddings for unseen words.

Although I’m note someone who was aware of Kanji before, this problem certainly made me a fan of it. The huge challenge in this problem was forming the dataset, after that, the problem was pretty straightforward.These were the ‘challenges’ in the dataset : 
- XML files seemed to be unordered
- Porting from SVG to PNG was challenging using Python, as there are very few packages that tend to do that. This was particularly challenging as the SVG path files were in cubic bezier forms, not quadratic bezier forms, and that led to testing a lot of libraries.
- Testing the alignment between text and images.
