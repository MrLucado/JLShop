# Athena - Fortnite-API.com

Athena is a utility which generates the current Fortnite Item Shop into a stylized image and shares it on Twitter.

# Versions

[FortniteAPI.io](https://github.com/Liimiitz/Athena-FNAPI.io)

[Fortnite-API.com](https://github.com/Liimiitz/Athena-FNAPI.com)

[FNBR.co](https://github.com/Liimiitz/Athena-FNBR.co) (Forked from Liimiitz)

# Image Example

<p align="center"><img src="./itemshop.jpeg" width="650px" draggable="false"></p>

## Requirements

- [Python 3.7](https://www.python.org/downloads/)
- [Requests](http://docs.python-requests.org/en/master/user/install/)
- [coloredlogs](https://pypi.org/project/coloredlogs/)
- [Pillow](https://pillow.readthedocs.io/en/stable/installation.html#basic-installation)
- [python-twitter](https://github.com/bear/python-twitter#installing)

A [Fortnite-API API Key](https://fortnite-api.com/profile) is not required to obtain the Item Shop data, [Twitter API credentials](https://developer.twitter.com/en/apps) are required to Tweet the image.

## Usage

Open `configuration_example.json` in your preferred text editor, fill the configurable values. Once finished, save and rename the file to `configuration.json`.

- `language`: Set the language for the Item Shop data ([Supported Languages](https://fortnite-api.com/documentation))
- `supportACreator`: Leave blank to omit the Support-A-Creator tag section of the Tweet
- `twitter`: Set `enabled` to `false` if you wish for `itemshop.png` to not be Tweeted

Edit the images found in `assets/images/` to your liking, avoid changing image dimensions for optimal results.

Athena is designed to be ran using a scheduler, such as [cron](https://en.wikipedia.org/wiki/Cron).

Start the bot by opening Command Prompt and entering the following command below.

```
python itemshop.py
```

## Credits


- Item Shop data provided by [Fortnite-API](https://fortnite-api.com/)
- Original Creator: [EthanC](https://github.com/EthanC/Athena)
