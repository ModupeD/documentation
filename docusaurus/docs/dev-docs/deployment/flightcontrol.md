---
title: AWS via Flightcontrol
description: Learn in this guide how to deploy your Strapi application on Flightcontrol.
displayed_sidebar: devDocsSidebar

---

# Deploy to AWS via Flightcontrol

The purpose of this guide is to allow users to deploy Strapi applications to AWS via [Flightcontrol](https://www.flightcontrol.dev/?ref=strapi). There are other options for how to deploy software to Flightcontrol available in our [documentation](https://www.flightcontrol.dev/docs?ref=strapi).

:::prerequisites

* A [Strapi project](/dev-docs/quick-start).
* Read through Strapi's [configuration documentation](/dev-docs/deployment#application-configuration).
* A [Flightcontrol account](https://app.flightcontrol.dev/signup?ref=strapi)
* An [AWS account](https://signin.aws.amazon.com/signin?redirect_uri=https%3A%2F%2Fus-east-1.console.aws.amazon.com%2Fbilling%2Fhome%3Fregion%3Dus-east-1%26state%3DhashArgs%2523%252Faccount%253Fnc2%253Dh_m_ma%26isauthcode%3Dtrue&client_id=arn%3Aaws%3Aiam%3A%3A934814114565%3Auser%2Fportal-aws-auth&forceMobileApp=0&code_challenge=hV6nNzYNHmki5JweiiVQcoLxr0WxjqXpVF4Lsh2NXxM&code_challenge_method=SHA-256)
* A [Git version control](https://docs.github.com/en/get-started/quickstart/set-up-git)

:::

## How to Deploy

1. Go to [app.flightcontrol.dev/projects/new/1](https://app.flightcontrol.dev/projects/new/1?ref=strapi)
2. Connect your GitHub account and select your repo
3. Select your desired Config Type:
    - `GUI` (all config managed through Flightcontrol dashboard)
    - `flightcontrol.json` ("Infrastructure as Code" option where all config is in your repo)
4. Strapi requires that the following environment variables be set on Flightcontrol for the remote instance:

- `NODE_ENV`,
- `MY_HEROKU_URL`,
- `JWT_SECRET`,
- `ADMIN_JWT_SECRET`,
- `API_TOKEN_SALT`,
- `APP_KEYS`.

5. Adjust configuration as needed
6. Click "Create Project" and complete any required steps (like linking your AWS account).
