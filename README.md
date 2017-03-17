# Mergado API Python Client

- [Mergado Apps Docs](http://mergado.github.io/docs/)
- [API docs](http://docs.mergado.apiary.io/)

## Usage

```python

from mergadoapiclient import client

# Prepare config with a OAuth2 credentials.
credentials = {
    'client_id': '<client ID>',
    'client_secret': '<client secret key>',
    'grant_type': 'client_credentials',
}

# Build API client instance.
api = client.build(credentials)

# Request Access Token.
api.request_token()

# Get an Eshop with ID = 1.
api.get('shops/1')
```