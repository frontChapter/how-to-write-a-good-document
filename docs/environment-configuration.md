## Environment Configuration

Create a `.env` file in the root directory and add the following:

```bash
VITE_REDIRECT_URL=http://localhost:3000
VITE_BASE_URL=https://api.example.com
VITE_IS_DEV=true
# ------------------------ #
#          AUTH0           #
# ------------------------ #
# The domain of our Auth0 tenant
VITE_AUTH0_DOMAIN=https://auth.example.com
# The Client ID of our Auth0 application
VITE_AUTH0_CLIENT_ID=XXXXXXXXXXX
# ------------------------ #
#         FIREBASE         #
# ------------------------ #
VITE_FIREBASE_API_KEY=XXXXXXXXXXX
VITE_FIREBASE_AUTH_DOMAIN=XXX.firebaseapp.com
VITE_FIREBASE_PROJECT_ID=XXXXXXXXXXX
# ------------------------ #
#         OPEN_API         #
# ------------------------ #
OPENAPI_URL=https://api.example.com/openapi.json
OPENAPI_USERNAME=XXXX
OPENAPI_PASSWORD=XXXX
```

---

[Go back to Readme](../README.md)
