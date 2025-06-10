# 🧩 SSO Foundations and Attack Simulations

## 🔐 Purpose
This repo offers a comprehensive view of how Single Sign-On (SSO) works via OAuth 2.0, OIDC, and SAML — and how to attack or misconfigure these systems.

## 📚 Sections

### Basics
- `oauth_flow_demo.py`: Authorization Code Flow example
- `oidc_id_token_demo.py`: OpenID Connect login and ID token processing
- `sso_provider_sim.py`: Simulates an Identity Provider (IdP)
- `client_app.py`: Relying party demo for consuming identity tokens

### Advanced
- `pkce_demo.py`: Demonstrates PKCE protection against code interception
- `token_replay_attack.py`: Shows how stolen access tokens can be reused
- `id_token_misuse.py`: Tests audience/issuer confusion
- `saml_response_lab.py`: Highlights SAML parsing weaknesses and signature skipping

## 🔧 Tech Stack
- FastAPI (can be added for API interfaces)
- JWT handling: `pyjwt`, `cryptography`
- Optional: Flask for client UI, XML for SAML demos

## 🔍 Security Topics Covered
- OAuth 2.0 vs OpenID Connect
- ID token verification
- Access token leakage
- SAML response spoofing
- Token audience validation
- Token expiration and scope enforcement

## 🧠 Bonus
- Add diagrams for flow visualization
- Add detection logic (e.g., for ID token misuse)
- Extend to include OIDC hybrid flow

## 🚀 Getting Started
```bash
# Clone the repo
$ git clone https://github.com/yourusername/sso-foundations-and-attacks.git
$ cd sso-foundations-and-attacks

# Create and activate virtual env
$ python3 -m venv venv && source venv/bin/activate
$ pip install -r requirements.txt

# Run selected demo
$ python basics/oauth_flow_demo.py
```

## ✅ To Do
- [ ] Add real IdP integration (Auth0, Okta)
- [ ] Write token parser for all formats (JWT, SAML)
- [ ] Add flow toggles in a unified web dashboard
- [ ] Add coverage for logout flows and refresh tokens

## 📄 License
MIT
