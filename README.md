# whereWeGoMockServer

mockup server of Where we go

## How to start

```bash
yarn # or
npm install

yarn start # or
npm run start # or
json-server --watch src/db.json --port 3004
```

## Usage

사용하기 전, 위 커맨드를 통해 서버를 실행해주세요.

그 후 `http://localhost:3004/nations`에 REST 요청을 보내면 됩니다.

```bash
# get all
curl http://localhost:3004/nations

# get by id
curl http://localhost:3004/nations/0
```

자세한 사용 방법은 [공식문서](https://github.com/typicode/json-server)를 참고하시면 됩니다.

## 예시

```json
{
  "nations": [
    {
      "id": 0,
      "nation_name": "대한민국",
      "introduce": "세상에서 제일 바쁜 도시 서울을 경험해보세요",
      "quarantine_policy": "백신 접종이 완료된 사람에 한하여, 격리 없이 자유여행 가능합니다.",
      "image_url": "https://images.pexels.com/photos/373290/pexels-photo-373290.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940"
    },
    {
      "id": 1,
      "nation_name": "태국",
      "introduce": "이쁜 자연과 함께 저렴한 물가",
      "quarantine_policy": "백신 접종이 완료된 사람에 한하여, 격리 없이 자유여행 가능합니다.",
      "image_url": "https://images.pexels.com/photos/415708/pexels-photo-415708.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940"
    },
    {
      "id": 2,
      "nation_name": "괌",
      "introduce": "신혼여행의 성지, 광활한 바다를 느껴보세요",
      "quarantine_policy": "쿠브 앱을 통해 백신 증명 가능하며 격리 없이 자유여행 가능합니다.",
      "image_url": "https://images.pexels.com/photos/1645028/pexels-photo-1645028.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940"
    },
    {
      "id": 3,
      "nation_name": "프랑스",
      "introduce": "낭만의 도시, 예술의 도시 파리에 가봐요",
      "quarantine_policy": "프랑스 외교부 사이트에서 접종 증명서 발급 후 자유여행 가능합니다.",
      "image_url": "https://images.pexels.com/photos/2082103/pexels-photo-2082103.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940"
    }
  ]
}
```

`GET` / `http://localhost:3004/nations` 호출 시

```JSON
[
  {
    "id": 0,
    "nation_name": "대한민국",
    "introduce": "세상에서 제일 바쁜 도시 서울을 경험해보세요",
    "quarantine_policy": "백신 접종이 완료된 사람에 한하여, 격리 없이 자유여행 가능합니다.",
    "image_url": "https://images.pexels.com/photos/373290/pexels-photo-373290.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940"
  },
  {
    "id": 1,
    "nation_name": "태국",
    "introduce": "이쁜 자연과 함께 저렴한 물가",
    "quarantine_policy": "백신 접종이 완료된 사람에 한하여, 격리 없이 자유여행 가능합니다.",
    "image_url": "https://images.pexels.com/photos/415708/pexels-photo-415708.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940"
  },
  {
    "id": 2,
    "nation_name": "괌",
    "introduce": "신혼여행의 성지, 광활한 바다를 느껴보세요",
    "quarantine_policy": "쿠브 앱을 통해 백신 증명 가능하며 격리 없이 자유여행 가능합니다.",
    "image_url": "https://images.pexels.com/photos/1645028/pexels-photo-1645028.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940"
  },
  {
    "id": 3,
    "nation_name": "프랑스",
    "introduce": "낭만의 도시, 예술의 도시 파리에 가봐요",
    "quarantine_policy": "프랑스 외교부 사이트에서 접종 증명서 발급 후 자유여행 가능합니다.",
    "image_url": "https://images.pexels.com/photos/2082103/pexels-photo-2082103.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940"
  }
]
```