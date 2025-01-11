# ic-slidev

`ic-slidev` enables you to create slides in Markdown using [Slidev](https://sli.dev/) and host them on the [Internet Computer](https://internetcomputer.org/).

## Demo

A presentation hosted on the Internet Computer is accessible at [https://kdn3b-iqaaa-aaaao-a3yqq-cai.icp0.io/](https://kdn3b-iqaaa-aaaao-a3yqq-cai.icp0.io/).
The source code is available at [ilbertt/voxxed-days-2025-talk](https://github.com/ilbertt/voxxed-days-2025-talk).

## Getting started

Make sure you have the following tools installed:

- [Node.js](https://nodejs.org/en/download/)
- [pnpm](https://pnpm.io/)
- [dfx](https://internetcomputer.org/docs/current/developer-docs/setup/install)

Then, clone this repo or use it as a template from GitHub directly.

### Install dependencies

```bash
pnpm install
```

### Edit the slides locally

To start the slide show:

- `pnpm dev`
- visit <http://localhost:3030>

Edit the [slides.md](./slides.md) to see the changes.

Learn more about Slidev at the [documentation](https://sli.dev/).

You can also use the [Slidev for VSCode](https://sli.dev/features/vscode-extension) extension to edit the slides locally in your editor. The extension is already added to the recommended extensions for this repo.

### Deploy the slides to the Internet Computer

Once you're done editing the slides, you can deploy them to the Internet Computer:

```bash
dfx deploy --ic --no-wallet
```

> NOTE: Make sure you have some cycles in your dfx account to pay for the deployment. You can check your balance with `dfx cycles balance --ic`.

You now have a presentation that can be accessed at `https://<your-canister-id>.icp0.io/`.

## License

[MIT](./LICENSE)
