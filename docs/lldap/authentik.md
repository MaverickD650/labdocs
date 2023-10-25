---
sidebar_position: 3
---
# Authentik Setup

Authentik is a much more user friendly version of Authelia due to the UI that is a key strength when managing less tech savy users. However another one of it's key strengths is the ability to integrate with other directories and federate logins making in even easier to integrate an easy to use login system into the home lab.

## LLDAP

The above feeds nicely into LLDAP as we can maintain a low footprint user database to sit in the background that Authentik can sync changes to and from. This allows us to easily have additional redundancy and switch instances and login technologies at a whim without affecting the end user too much.

The relevant article for this is [here](https://goauthentik.io/integrations/sources/ldap/).

While Authentik has an LDAP outpost using LLDAP instead allows for maximum redudancy and flexibility in deploying a self-hosted authentication framework.
