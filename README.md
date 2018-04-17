# Node.js Scryfall API Client

This package is auto-geneated from the [Scryfall API definition](https://github.com/jdharmon/scryfallapi).

## Getting Started

1. Create a folder for your project

```sh
mkdir MyPackage
cd MyPackage
git init
```

2. Add this repository as a submodule.

```sh
git submodule add https://github.com/jdharmon/scryfallapi-nodejs.git scryfall
```

3. Initialize package, and install dependencies

```sh
npm init
npm install ms-rest
```

5. Edit index.js

```js
const scryfallClient = require('./scryfall/scryfallClient');
const scryfall = new scryfallClient();

scryfall.cards.getRandom((error, card) => {
    if (card != null) {
        console.log(`Got card: ${card.name}`);
        console.log(card);
    }
});
```

6. Run your app

```sh
node index.js
```