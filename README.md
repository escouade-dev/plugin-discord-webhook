# Discord · plugin for Escouade

Tickets to test and agents waiting, in a Discord channel. No code: two webhooks (`contributes.webhooks`) called on `ticket.column` and `agent.status`, to `discord.com` only.

At install, Escouade asks for the channel’s webhook address (Discord: channel settings › Integrations › Webhooks) and keeps it in the system keychain. The address must be on `discord.com` (Escouade sends a webhook only to a host of `permissions.network`). Both messages carry an empty `allowed_mentions`: an `@everyone` in a ticket’s title (from a public issue, say) shows without notifying the channel.

> Les tickets à tester et les agents qui attendent, dans un salon Discord. Sans code : deux webhooks (`contributes.webhooks`) appelés sur `ticket.column` et `agent.status`, vers `discord.com` seulement.

One of the example plugins of [Escouade](https://escouade.dev) (id `dev.exemple.discord`), published on its store: https://store.escouade.dev. The documentation shows it whole: https://escouade.dev/en/docs/plugins/examples

## Check

```sh
npx -p @escouade-dev/plugin escouade-plugin validate .
```

## Try it in Escouade

Plugins view › “In development”, then this folder; or install it from the store.

## License

MIT (`LICENSE`).
