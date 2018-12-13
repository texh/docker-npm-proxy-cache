## Usage

Run the container

```
docker run --net=host -p 9876:9876 -t nahanil/npm-proxy-cache
```

Use it with `npm`, replacing the npm-proxy-cache hostname below with the ip or hostname you have the container above running at.

```
npm --proxy http://npm-proxy-cache:9876 --https-proxy http://npm-proxy-cache:9876 --strict-ssl false install
```
