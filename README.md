# Human–Computer Interaction Projects

Coursework covering a quiz application prototype and a dense-interface target-selection experiment.

## Source and credit

This is David Correia's showcase fork of [l28j/IPM](https://github.com/l28j/IPM). The original repository records commits by **jlucas (l28j)** and **Mariana Santana**. This fork preserves that history and does not assert authorship of the original implementation.

## Quiz prototype

[Quizzes Tutor in Figma](https://www.figma.com/proto/qemuJXujJGC2PIpzkWyfwo/Quizzes-Tutor?node-id=50-3&mode=design).

The prototype currently asks visitors to sign in to Figma. Its file owner must change sharing settings or supply exported images/video for a demo accessible without an account.

## Selection-time experiment

Run a static server from the repository root:

```sh
python3 -m http.server 8080 --bind 127.0.0.1
```

Open http://127.0.0.1:8080. The experiment uses p5.js from a CDN, so an internet connection is required. Enter an anonymous participant identifier and display size when prompted, then follow the experiment instructions.

Result recording is disabled by default (`RECORD_TO_FIREBASE = false`). The showcase also removes the original team's Firebase configuration. To collect results in your own project, configure `firebaseConfig` in `index.html`, review your Firebase access rules, and explicitly enable recording in `sketch.js`.
