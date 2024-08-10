![](https://www.teguharief.com/img/teguh-arief.png)

# Chat Server

a real-time chat server using a microservices architecture with Express - Node.js, TypeScript, JWT auth, MongoDB, Socket.IO, and RabbitMQ.

## Installation

Install the app on terminal

```
git clone git@github.com:teguharifudin/Chat-Server.git
```
```
cd Chat-Server
```

### User Service
```
cd user-service
```
```
npm run dev
```

### Client Service
```
cd client-service
```
```
npm run dev
```

### Notification Service
```
cd notification-service
```
```
npm run dev
```

### API Gateway
```
cd gateway
```
```
npm run dev
```

## Usage

POST http://localhost:8080/api/auth/register
- User A
```
{
    "name": "Teguh",
    "email": "teguh@gmail.com",
    "password": "123456"
}
```
- User B
```
{
    "name": "Arief",
    "email": "arief@gmail.com",
    "password": "123456"
}
```

POST http://localhost:8080/api/auth/login
- User A
```
{
    "email": "teguh@gmail.com",
    "password": "123456"
}
```

POST Bearer Authentication http://localhost:8080/api/messages/send
- User A to User B
```
{
    "receiverId": "66b7712ee3ff3b538d066875",
    "message": "Hello there!"
}
```

## Contributing

Please use the [issue tracker](https://github.com/teguharifudin/Chat-Server/issues) to report any bugs or file feature requests.
