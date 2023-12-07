# Example curl commands for testing your server

Replace the IP address in the examples with the IP address of your **load balancer, not your servers!**

My **load balancer** address 64.225.91.41.

Run these commands from your host machine, not your server.

## Testing your frontend

```bash
curl http://64.225.91.41/
```

## Testing your backend

```bash
curl http://64.225.91.41/hey
```

```bash
curl -X POST -H "Content-Type: application/json" \
  -d '{"message": "Hello from your server"}' \
  http://64.225.91.41/echo
```
