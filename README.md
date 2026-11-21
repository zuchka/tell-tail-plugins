# Tell-Tail for Codex

This catalog installs Tell-Tail on an Apple Silicon Mac and makes it available in local Codex chats. The plugin includes the executable. For standalone use, see the [Homebrew and Cargo instructions](https://tell-tail.dev/#install).

## Use in Codex

Select **Use in Codex** on the [Tell-Tail website](https://tell-tail.dev/#use-in-codex). On your first visit, Codex opens Plugins. Choose **Add → Add a marketplace**, enter `zuchka/tell-tail-plugins`, and select **Add marketplace**. The website button now opens the Tell-Tail listing, where you can click **Install**.

Open a new local Codex chat and ask **“Open my Codex logs.”** Tell-Tail opens a local dashboard and follows supported desktop logs for that session.

For ongoing tool-call tracing, ask **“Set up persistent tool-call tracing.”** After you approve setup, restart Codex once. The collector then starts at login. If you enable the collector, ask Codex to uninstall it before removing the plugin.

### Install with the Codex CLI

```sh
codex plugin marketplace add zuchka/tell-tail-plugins
codex plugin add tell-tail@tell-tail-plugins
```

## Package

Plugin 0.2.1 bundles the Tell-Tail 0.4.0 executable for macOS arm64. The [build record](plugins/tell-tail/build.json) identifies the [source commit](https://github.com/zuchka/tell-tail/tree/6992db1ac7f2a0da515bc218a0f0202887d8baa6) and executable checksum.

[Privacy policy](https://tell-tail.dev/privacy) · [Report an issue](https://github.com/zuchka/tell-tail/issues) · [License](plugins/tell-tail/LICENSE)
