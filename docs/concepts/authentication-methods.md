---
title: 'Authentication methods'
subtitle: 'Understand and select your preferred authentication method in PlanetScale.'
date: '2022-08-01'
---

## Overview

There are three ways to authenticate with PlanetScale: _email address and password_, _single sign-on_, and _OAuth via GitHub_.

Let's break down how each of these work.

## Email address and password

This is the only authentication mechanism where PlanetScale maintains user credentials.

Additionally, users can opt to configure [two-factor authentication (2FA)](/docs/concepts/mfa). This option requires **something you know** _(i.e. your password)_ and **something you have** _(i.e. recovery codes)_.

## Single sign-on

Users can authenticate with their chosen corporate identity provider _(i.e. Okta)_ instead of maintaining passwords with PlanetScale.

Once [SSO](/docs/concepts/sso) is enabled for an `organization`, all members are redirected through that identity provider's authentication flow. Moving forward, they must pass through SSO to access their PlanetScale account.

## OAuth via GitHub

Users can authenticate with PlanetScale using their GitHub account.

{% callout type="warning" %} PlanetScale doesn't maintain the passwords for these accounts. Losing access to your GitHub account prevents accessing your PlanetScale account. {% /callout %}

{% callout %} Enabling SSO removes OAuth access for all members of your _organization_, meaning they will no longer be able to sign in with their GitHub credentials. {% /callout %}

{% callout title="Next steps" %}

- [Multi-factor authentication](/docs/concepts/mfa)

{% /callout %}
