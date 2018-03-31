boost-bot
=========

Mastodon bot that boosts all local toots with a chosen hashtag.

1. Clone the repository (`git clone https://github.com/Gargron/boost-bot.git`)
2. Install the dependencies (`yarn install`).
3. Fill out the `.env` file with `ACCESS_TOKEN`, `API_HOST`, and `HASHTAG`
4. Launch the bot with `yarn start`.

|Variable      |Description                                                                                                                                                                              |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|`ACCESS_TOKEN`|From the Mastodon account for the bot, go to Preferences, then Development. Create a new application with read and write access. Once it's created, click on it to see your access token.|
|`API_HOST`    |For example: `mastodon.social`                                                                                                                                                           |
|`HASHTAG`     |For example: `catsofmastodon`                                                                                                                                                            |

The bot uses the streaming API to receive toots. It does not catch up on toots that happened while it was not connected.

#### License (MIT)

Copyright 2018 Eugen Rochko

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.