# JSGF Russian localization

1. **The task**

NLP Challenge: JSGF Development

Background:
Below is a Context-Free Grammar written using the Java Speech Grammar Format (JSGF) (http://www.w3.org/TR/jsgf/):
~~~
#JSGF V1.0 utf-8 en;
grammar music_play;
public <music_play> =
[can you] (put on | play) (<artist> | <song>);
<artist> =
the beatles |
radiohead |
lady gaga |
pink floyd;
<song> =
comfortably numb |
paranoid android |
let it be |
hey jude;
~~~

This grammar is intended for creating utterances expressing the intent to play music, which will serve as training data for statistical intent recognition and classification models. For reference, this grammar can generate utterances like the following using a custom parser:

To better understand the parsing process, keep in mind:

- Rules containing named entities that are used within the music play intent are used as tags for those entities (in this grammar, it applies to <artist> and <song>).
- Everything else is tagged as unknown (<unk>) by the parser.

Tasks:

Task 1: Extend the English Grammar
1.1 Extend the English JSGF grammar to cover at least the following utterances:
~~~
[i want to listen to]<unk> [jazz]<genre> [music]<unk>
[play me]<unk> [ummagumma]<album> [by]<unk> [pink floyd]<artist>
[put]<unk> [lady gaga]<artist> [on]<unk>
~~~

Task 2: Localize the JSGF Grammar in Your Language
2.1 Localize the extended English grammar from Task 1.1 in Russian. Feel free to add everything you think could help improve the quality of the generated utterances.

2.2 Provide some sample utterances the JSGF can produce using the localized grammar.

2.3 What possible issues do you think you could run into if you were asked to extend the grammar considerably, and how would you suggest overcoming them? There is no single correct response to this question, so please share any potential issues that come to mind.

2.4 Which features of your language complicate the localization or writing of the grammar? How would you solve or work around these complications?

2. **Task 1.1**

Let`s extend the JSGF file manually and see if results will satisfy the requirements.
   


