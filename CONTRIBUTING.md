## Contributing to Web3 Public APIs

> Pull requests and community involvement are appreciated. This API list is not a marketing tool, but a tool to help the  
> community build applications and use free, Web3 public APIs quickly and easily. Pull requests that are identified as marketing attempts will not be accepted.
> 
> Please make sure the API you want to add has full, free access or at least a free tier and does not depend on the purchase of a device/service before submitting. 

## Formatting

Current API entry format:

| API | Description | Auth | HTTPS | CORS | Links |
| --- | --- | --- | --- | --- | --- |
| API Title(Link to API documentation) | Description of API | Does this API require authentication? \* | Does the API support HTTPS? | Does the API support [CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS)? \* | Useful links to Docs, and Official resources |

Example entry:

```plaintext
| [Rarible](https://docs.rarible.org) | NFT data, collections and offers | Yes | Yes | Yes | [SDK](https://github.com/rarible/sdk)
```

\* Currently, the only accepted inputs for the `Auth` field are as follows:

*   `OAuth` - _the API supports OAuth_
*   `apiKey` - _the API uses a private key string/token for authentication - try and use the correct parameter_
*   `X-Mashape-Key` - _the name of the header which may need to be sent_
*   `No` - _the API requires no authentication to run_
*   `User-Agent` - _the name of the header to be sent with requests to the API_

\* Currently, the only accepted inputs for the `CORS` field are as follows:

*   `Yes` - _the API supports CORS_
*   `No` - _the API does not support CORS_
*   `Unknown` - _it is unknown if the API supports CORS_

_Without proper_ [_CORS configuration_](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS) _an API will only be usable server side._

After you've created a branch on your fork with your changes, it's time to [make a pull request](https://help.github.com/articles/creating-a-pull-request/).

_Please follow the guidelines given below while making a Pull Request to the Web3 Public APIs_

## Pull Request Guidelines

*   Never put an update/new version of an API that is already listed, the old version of the API gets deprecated.
*   Continue to follow the alphabetical ordering that is in place per section.
*   Each table column should be padded with one space on either side.
*   The Description should not exceed 100 characters.
*   Add one link per Pull Request.
*   Make sure the PR title is in the format of `Add Api-name API` _for e.g._: `Add Blockchain API`
*   Use a short descriptive commit message. _for e.g._: ❌`Update Readme.md` ✔ `Add Blockchain API to Cryptocurrency`
*   Search previous Pull Requests or Issues before making a new one, as yours may be a duplicate.
*   Don't mention the TLD(Top Level Domain) in the name of the API. _for e.g._: ❌Gmail.com ✔Gmail
*   Please make sure the API name does not end with `API`. _for e.g._: ❌Gmail API ✔Gmail
*   Please make sure the API has proper documentation.
*   Please make sure you squash all commits together before opening a pull request. If your pull request requires changes upon review, please be sure to squash all additional commits as well. [This wiki page](https://github.com/todotxt/todo.txt-android/wiki/Squash-All-Commits-Related-to-a-Single-Issue-into-a-Single-Commit) outlines the squash process.
*   Target your Pull Request to the `master` branch of the web3-public-apis
*   API must be providing services or data related to the blockchain, and web3 space ( web2 apps will be rejected )

Once you’ve submitted a pull request, the collaborators can review your proposed changes and decide whether or not to incorporate (pull in) your changes.

_Thanks for being a part of this project, and we look forward to hearing from you soon!_