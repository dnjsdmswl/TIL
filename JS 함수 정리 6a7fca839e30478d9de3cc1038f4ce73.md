# JS 함수 정리

---

# join()

arr.join(separator)

배열 → 문자열

원본 배열은 변화 X.

```jsx
> let RV = ["I", "S", "W", "J", "Y"];
< undefined
> RV.join()
< "I, S, W, J, Y"
> RV
< (5) ["I", "S", "W", "J", "Y"]
```

# split()

str.split(separator)

문자열 → 배열

원본 문자열은 변화 X.

```jsx
> let RV = "I, S, W, J, Y";
< undefined
> RV.split(",");
< (5) ["I", "S", "W", "J", "Y"]
> RV
< "I, S, W, J, Y"
```

# reverse()

arr.reverse()

배열 순서 뒤집기

```jsx
> const array = [1, 2, 3, 4, 5, 6];
< undefined
> array.reverse();
< (6) [6, 5, 4, 3, 2, 1]
> array
< (6) [6, 5, 4, 3, 2, 1]
```

# splice()

arr.splice(시작인덱스, 삭제할 요소의 수)

지정된 부분을 삭제해줌

배열 자체를 수정

```jsx
> let arr = [1, 2, 3, 4, 5, 6, 7];
< undefined
> arr.splice(3, 2);
< (2) [4, 5]
> arr
< (5) [1, 2, 3, 6, 7]
```

# slice()

arr.slice(시작인덱스, 끝 인덱스)

*끝 인덱스 : 지정할 마지막 인덱스 +1

지정된 부분으로 새로운 배열을 만듦

원본 배열 변경 X

```jsx
> let arr = [1, 2, 3, 4, 5, 6, 7];
< undefined
> arr.slice(2, 5)
< (3) [3, 4, 5]
> arr
< (7) [1, 2, 3, 4, 5, 6, 7]
```

# find()

arr.find(콜백 함수)

콜백함수에 true하는 요소 리턴

없을시 undefined 리턴

```jsx
> let arr = [21, 22, 23, 24, 25, 26];
< undefined
> arr.find(value => value % 5 === 0)
< 25
```

# filter()

arr.filter(콜백 함수)

콜백함수에 true하는 요소 새로운 배열로 리턴

원본 배열 변경 X

```jsx
> let arr = [100, 101, 102, 103, 104, 105];
< undefined
> const evenArr = arr.filter(value => value % 2 === 0);
< undefined
> evenArr
< (3) [100, 102, 104]
> arr
< (6) [100, 101, 102, 103, 104, 105]
```

# map()

arr.map(콜백 함수)

배열 요소 하나하나에 콜백함수 실행 → 콜백함수로 가공된 요소들을 새로운 배열로 리턴

원본 배열 변경 X

```jsx
> const arrScoreSum = [478, 499, 398, 494, 432];
< undefined
> const scoreAverage = arrScoreSum.map(sum => sum / 5);
< undefined
> scoreAverage
< (5) [95.6, 99.8, 79.6, 98.8, 86.4]
> arrScoreSum
< (5) [478, 499, 398, 494, 432]
```

# some()

arr.some(콜백 함수)

콜백함수의 조건을 충족하는 요소가 하나라도 있는지 검사

리턴값은 boolean (true, false)

```jsx
> const arrScoreSum = [478, 499, 398, 494, 432];
< undefined
> arrScoreSum.some(sum => sum > 490);
< true
```

# every()

arr.every(콜백 함수)

모든 배열의 요소가 콜백함수의 조건을 충족하는지 검사

리턴값은 boolean (true, false)

```jsx
> const arrScoreSum = [478, 499, 398, 494, 432];
< undefined
> arrScoreSum.every(sum => sum > 490);
< false
```

# reduce()

arr.reduce(콜백 함수)

배열 모든 요소에 콜백함수 실행 → 누적된 값 리턴

return값을 정해주지 않으면 undefined 반환

```jsx
> const scores = [90, 88, 98, 100, 78];
< undefined
> const scoreSum = scores.reduce((sum, score) => {return sum + score}, 0);
< undefined
> scoreSum
< 454
```

# reduceRight()

arr.reduceRight(콜백 함수)

배열 모든 요소에 콜백함수 실행 (뒤 → 앞) → 누적된 값 리턴

원본 배열 변경 X

```jsx
> const scores = [90, 88, 98, 100, 78];
< undefined
> const scoreSumRight = scores.reduceRight(function(sum, score) 
  {return sum + score;}, 0);
< undefined
> scoreSumRight
< 454
> scores
< (5) [90, 88, 98, 100, 78]
```

# sort()

배열을 오름차순 || 내림차순으로 정렬

 오름차순

arr.sort((a, b) ⇒ a - b);

 내림차순

arr.sort((a, b) ⇒ b - a);

```jsx
> const scores = [90, 88, 98, 100, 78];
< undefined
> const asceding = scores.sort((a, b) => a - b);
< undefined
> asceding
< (5) [78, 88, 90, 98, 100]
> const descending = scores.sort((a, b) => b - a);
< undefined
> descending
< (5) [100, 98, 90, 88, 78]
```