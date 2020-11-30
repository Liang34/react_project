1、react Objects are not valid as a React child (found: object with keys {})
原因：虽然报错位置在actions中，但是实际上是在HTML中插入了对像，
在这次中不小心打多了个大括号，从而导致报错
2、问题：用require加载图片时，报GET http://localhost:3000/[object%20Module] 404 (Not Found)错误，
解决：require(`../../assets/images/${text}.png`).default,加上default即可。
3、注意websock前后端的版本号要一致
客户端用的是websocket.io-client
服务端用的是websocket.io