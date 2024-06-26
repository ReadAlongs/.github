# Welcome to the ReadAlongs project

Interactive story telling embeddable into any website!

This space on GitHub is dedicated to all the repos related to the ReadAlongs Project.

## What is Readalong Studio?

Readalong Studio is a program (actually a collection of programs) to help you make and view online "read-along" and "sing-along" audiobooks for language and literacy education. As the audio plays, the word currently being spoken is highlighted, and the student can click on any word to hear it pronounced in isolation.

![Screenshot of a read-along story in the Atikamekw language](https://readalongs.github.io/ICLDC-Docs/images/nikikw-small.png "A read-along story from the Atikamekw language")

You give the software two things, the text of the story, and a recording of someone speaking the story aloud. Inside, the software listens to the recording and tries to guess the exact time when each word starts and stops. (If you've ever used audio software like Audacity or ELAN, imagine measuring the exact time when every word starts and stops. You could totally do this, but it takes a long time and can be tedious; it usually takes about an hour to measure a minute of speech!)  Our software's guesses aren't perfect, but it can make these guesses in seconds.

## Key links

 - The Web app online:
   - [The ReadAlong Studio Web App](https://readalong-studio.mothertongues.org/)
   - [L'appli Studio ReadAlong en français](https://readalong-studio.mothertongues.org/fr/)
   - [El Studio de ReadAlong en español](https://readalong-studio.mothertongues.org/es/) (Gracias a Jorge Rosés Labrada)
 - The Command Line Interface app for advanced users:
   - Follow instructions at [Studio CLI](https://github.com/ReadAlongs/Studio)
 - The [ICLDC Workshop Documentation](https://readalongs.github.io/ICLDC-Docs/) includes useful documentation for how to use the ReadAlong Studio web app.
 - [Recording of the ICLDC workshop](https://www.youtube.com/watch?v=9CwDCtJGl6w) (The presentation is from 0:00 to 40:30, then it's mostly silence while participant are in the break-out rooms, which were not recorded. There is a short wrap-up from 1:14:38, but the language party at the end was not recorded due to data sovereignty and privacy considerations, and the conclusion was not recorded either.)
 - Providing feedback:
   - Contact us by email to provide your feature requests or bug reports: readalong dot studio à gmail dot com
   - Submit an issue here on GitHub on the relevant repo (make it a [Studio-Web Issue](https://github.com/ReadAlongs/Studio-Web/issues) if you're not sure)
 - Related publications:
   - Pine et al., 2023. [ReadAlong-Studio Web Interface for Digital Interactive Storytelling](https://nrc-publications.canada.ca/eng/view/object/?id=316fb811-134a-4b1c-8b04-20b8988da57d). BEA @ACL.
   - Pine et al., 2023. [“Watch me Speak!” interactive storytelling using Read-Along Studio](https://nrc-publications.canada.ca/eng/view/object/?id=fa0863c2-1c95-4156-afa3-064cfea987d6). ICLDC. (This is the workshop mentioned above.)
   - Littell et al., 2022. [ReadAlong studio: Practical zero-shot text-speech alignment for Indigenous language audiobooks](https://nrc-publications.canada.ca/eng/view/object/?id=fad56ec7-77a0-4e64-98e8-c3e36ce5ac1c). SIGUL @LREC.
   - Pine et al., 2022. [Gᵢ2Pᵢ: Rule-based, index-preserving grapheme-to-phoneme transformations](https://nrc-publications.canada.ca/eng/view/object/?id=de4b961d-54bf-4187-a3fc-d875ac285e79). ComputEL.

## Source code organization

 - [Studio-Web](https://github.com/ReadAlongs/Studio-Web) (formerly called Web-Component) is a large monorepo that contains the web app and the embeddable web component.
 - [Studio](https://github.com/ReadAlongs/Studio) is the repo for the CLI interface and the web_api backend used by the web app.
 - [SoundSwallower](https://github.com/ReadAlongs/SoundSwallower) is the speech recognizer used for audio-text aligner, including both a JavaScript version (used by the web app) and a C version with bindings for Python (used by the CLI version).
 - [g2p](https://github.com/roedoejet/g2p) is the grapheme-to-phoneme library used by the ReadAlongs Studio.
 - [ICLDC-Docs](https://github.com/ReadAlongs/ICLDC-Docs) hosts the documentation we provided for the ICLDC8 workshop.
 - [OpenSamples](https://github.com/ReadAlongs/OpenSamples) has public data that can be used for testing.
