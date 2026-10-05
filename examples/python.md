# Python example

```python
import os
import requests

response = requests.post(
    "https://genory.dev/api/profile",
    headers={
        "Authorization": f"Bearer {os.environ['GENORY_API_KEY']}",
        "Content-Type": "application/json",
    },
    json={
        "country": "DE",
        "amount": 1,
        "fields": ["firstName", "lastName", "email"],
    },
    timeout=30,
)

response.raise_for_status()
print(response.json())
```

Keep API keys out of source control and check https://genory.dev/docs for the current API reference.
