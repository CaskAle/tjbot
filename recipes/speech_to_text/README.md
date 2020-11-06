# Speech to Text
> Control TJBot's LED with your voice!

This recipe uses the [Speech to Text](https://www.ibm.com/watson/services/speech-to-text/) service to let you control the color of TJBot's LED with your voice. For example, if you say "turn the light green," TJBot will change the color of the LED to green.

## Hardware
This recipe requires a TJBot with a microphone and an LED.

## Build and Run
First, make sure you have configured your Raspberry Pi for TJBot by following the [bootstrap instructions](https://github.com/ibmtjbot/tjbot/tree/master/bootstrap).

Next, go to the `recipes/speech_to_text` folder and install the dependencies.

    $ cd tjbot/recipes/speech_to_text
    $ npm install

Create an instance of the [Speech to Text](https://www.ibm.com/watson/services/speech-to-text/) service and download the authentication credentials file. Ensure this file is named `ibm-credentials.env` and place it in the `tjbot/recipes/speech_to_text` folder.

Run!

    $ sudo node stt.js

> Note the `sudo` command. Root user access is required to run TJBot recipes.

Now, speak into TJBot's microphone to change the color of the LED. Say "turn the light blue" to change the light to blue or "turn the light purple" to change it to purle. You can try other colors as well, such as yellow, green, orange, purple, magenta, red, blue, aqua, and white. You can also say "turn the light on" or "turn the light off".

## Customize
We have hidden a disco party for you. Find the code for disco party in `stt.js` and uncomment the code (hint: there are two places that need to be uncommented). Now you can ask TJ to show you the disco lights by saying "Let's have a disco party"!

## Troubleshoot
If you are having difficulties in making this recipe work, please see the [troubleshooting guide](../../TROUBLESHOOTING.md).

# AI Services
- [Speech to Text](https://www.ibm.com/watson/services/speech-to-text/)

# License
This project is licensed under Apache 2.0. Full license text is available in [LICENSE](../../LICENSE).

# Contributing
See [CONTRIBUTING.md](../../CONTRIBUTING.md).
