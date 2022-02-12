# PD Korean Noun list for Wordles

This is a node library provides a list of Korean nouns extracted from [Wikidata], under [CC0].

Disclaimers:

- The length of word is up to 3 letters. (e.g. "가나다")
- This list does not guarantee that words are listed in the dictionary.

## Install

```sh
# NPM
npm install TBD

# Yarn
yarn add TBD
```

## Usage

```javascript
const KoreanNounList = require('pd-korean-noun-list-for-wordles');
console.log(KoreanNounList.ALL_NOUNS.length());
```

```typescript
import * as KoreanNounList from 'pd-korean-noun-list-for-wordles';
console.log(KoreanNounList.ALL_NOUNS.length());
```

[wikidata]: https://www.wikidata.org/wiki/Wikidata:Copyright
[cc0]: https://www.wikidata.org/wiki/WD:CC0
[wikidata query service]: https://query.wikidata.org/
