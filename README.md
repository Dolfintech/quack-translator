# Quack Translator

Quack Translator is an experimental web page that listens for the MicroDuck ducks’ tone words and shows each recognized word in toki pona and English. It recognizes eight words. Unmatched detected notes show as unknown.

Audio and translations stay on your phone. Once the page is open, it processes microphone input and audio files locally and keeps translations in memory until you clear them or close the page.

## Open in Safari on iPhone

1. Open the translator’s HTTPS page in Safari.
2. Tap **Share**, choose **Add to Home Screen**, then tap **Add**.
3. Open Quack Translator. Tap **Start listening** and allow microphone access, or tap **Choose audio** to open a recording. The audio picker may offer recording on iOS.

Microphone access, the audio picker and Home Screen launch remain untested on an iPhone. Offline relaunch is unverified.

## Simulated recording tests

All tests used simulated recordings. The table pools the two duck voices. Each result gives correct, unknown and wrong counts in that order.

| Input | Takes | Web translator | Python reference |
| --- | ---: | ---: | ---: |
| Clean WAVs | 10 | 10 / 0 / 0 | 10 / 0 / 0 |
| Clean paired replay | 48 | 48 / 0 / 0 | 48 / 0 / 0 |
| Simulated room noise, 25 dB SNR | 240 | 240 / 0 / 0 | 240 / 0 / 0 |
| Simulated room noise, 12 dB SNR | 240 | 240 / 0 / 0 | 240 / 0 / 0 |
| Simulated room noise, 3 dB SNR | 240 | 221 / 19 / 0 | 1 / 232 / 7 |
