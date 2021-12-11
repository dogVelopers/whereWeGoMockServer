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
