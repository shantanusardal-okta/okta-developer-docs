---
title: Overview
---

## What is a refresh token?

A refresh token is a special token that is used to generate additional access tokens. This allows you to have short-lived access tokens without having to collect credentials every single time one expires. You request this token alongside the access and/or ID tokens as part of a user's initial authentication flow.

## Set up your application

Refresh tokens are available for a subset of Okta OAuth 2.0 client applications, specifically web or native applications. For more about creating an OpenID Connect application, see our [OAuth 2.0 and OIDC overview](/docs/concepts/auth-overview/#recommended-flow-by-application-type).

Be sure to specify `refresh_token` as a `data_type` value for the `grant_type` parameter when adding an [OAuth client app](/docs/reference/api/apps/#add-oauth-2-0-client-application) using the `/apps` API. Alternatively, after you set up an application, you can select the **Refresh Token** option for **Allowed grant types** on the **General Settings** tab in the Admin Console.

<NextSectionLink/>
