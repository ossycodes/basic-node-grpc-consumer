# A basic gRPC Producer

please ensure you have a copy of the [Protobuffer](https://github.com/ossycodes/basic-node-proto-buffer) and [producer](https://github.com/ossycodes/basic-node-grpc-producer)


## usage
`node folderyouclonedproducerinto/producer-grpc.js` ##terminal 1

`node folderyouclonedconsumerinto/consumer-grpc.js` #terminal 2

`curl http://localhost:3000/` #terminal 3

you should get a reponse like this

```json
{
    "consumer_id": 2000,
    "producer_data": { "pid": "xxxx"},
    "recipe": {
        "id": 42, "name": "xxxx",
        "steps: "xxxxx",
        "ingredients": [
            {
                "id": 1,
                "name": "xxxx",
                "quantity" "xxxx"
            },
            {
                "id": 2,
                "name": "xxxx",
                "quantity" "xxxx"
            },
        ]
    }
}
```