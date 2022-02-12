# 워들에 사용할 수 있는 한국어 명사 목록

이것은 워들 제작 등에 사용할 수 있도록 정리한 Node 라이브러리입니다.

## 저작권

이 자료 저작권은 [https://github.com/korean-word-game/db]의 것을 포함하고 있으며 해당 저장소에서
설명한 바에 따르면 다음과 같습니다.

> 본래 [저작권법 제24조의2]에 의하면 국가에 의해 작성되어 공표된 저작물은 허락 없이 이용할 수 있어야
> 하지만, 표준국어대사전의 경우에는 국립국어원이 저작재산권 전부를 보유하고 있지 않으므로 저작권
> 등록물에 해당됩니다. 그러나 단순히 낱말과 품사를 수집한 것은 한국어 자체로써 저작권 보호를 받을 수
> 없는 자료이므로 자유로운 2차 가공 및 배포가 가능합니다. 마찬가지로 해당 DB에도 저작권이 없습니다.

국립국어원에서 배포한 [한국어 학습용 어휘 목록]도 포함하고 있습니다.

## 제약 사항

- 한글 조합 방식에 따라 사용하는 단어의 글자수가 바뀌는 한국어 워들들의 특징에 따라, 1글자~3글자
  명사들을 모았습니다.

## 설치

```sh
# NPM
npm install pd-korean-noun-list-for-wordles

# Yarn
yarn add pd-korean-noun-list-for-wordles
```

## 사용

두 목록을 제공하며, `ALL_NOUNS`은 제출 답안 검사용으로 쓸 수 있도록 2018년 11월 13일 수집된
표준국어대사전의 명사를 담고 있습니다. `COMMON_NOUNS`의 경우 문제 출제용으로 쓸 수 있도록 [한국어
학습용 어휘 목록] 2019년 5월 30일 수정본의 명사를 담고 있습니다.

```javascript
const KoreanNounList = require('pd-korean-noun-list-for-wordles');
console.log(KoreanNounList.ALL_NOUNS.length());
console.log(KoreanNounList.COMMON_NOUNS[0]);
```

```typescript
import * as KoreanNounList from 'pd-korean-noun-list-for-wordles';
console.log(KoreanNounList.ALL_NOUNS.length());
console.log(KoreanNounList.COMMON_NOUNS[0]);
```

[https://github.com/korean-word-game/db]: https://github.com/korean-word-game/db
[저작권법 제24조의2]: http://www.law.go.kr/%EB%B2%95%EB%A0%B9/%EC%A0%80%EC%9E%91%EA%B6%8C%EB%B2%95/%EC%A0%9C24%EC%A1%B0%EC%9D%982
[한국어 학습용 어휘 목록]: https://www.korean.go.kr/front/etcData/etcDataView.do?mn_id=46&etc_seq=70&pageIndex=44
