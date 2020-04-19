## Project
Blockchain to learn basic concepts for fun

## Installation
python 3.7+

```bash
python3 -m venv dev
source dev/bin/activate
pip3 install -r requirements.txt
```

## Usage locally
```bash
python api.py
```

## REST

### GET

Retrieve blocks in chain

http://localhost:5000/chain

Resolve conflict between nodes in network (call this endpoint on everynode to make sure each of them has authoritative chain)

http://localhost:5000/nodes/resolve

### POST 

Add new transaction in future block

http://localhost:5000/transactions/new

```json
{
	"sender":"testSender",
	"recipient":"testRecipient",
	"amount":5
}
```

Add new node to network

http://localhost:5000/nodes/register

```json
{
	"sender":["http://127.0.0.1:5001"]
}
```




## API Reference

## Tests

None now

## Contributors
Alexson Pel

## License

