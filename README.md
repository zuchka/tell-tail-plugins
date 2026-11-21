# Tell-Tail for Codex

This catalog installs Tell-Tail on an Apple Silicon Mac and makes it available in local Codex chats. The plugin includes the executable. For standalone use, see the [Homebrew and Cargo instructions](https://tell-tail.dev/#install).

## Use in Codex

On your first visit, choose **Copy catalog**, then **Use in Codex** on the [Tell-Tail website](https://tell-tail.dev/#use-in-codex). In Plugins, choose **Add → Add a marketplace**, paste `zuchka/tell-tail-plugins`, and select **Add marketplace**. Codex opens the Tell-Tail catalog. Select **Tell-Tail → Install**. Once the catalog is added, **Use in Codex** opens the listing directly.

Open a new local Codex chat and ask **“Open my Codex logs.”** Tell-Tail opens a local dashboard and follows supported desktop logs for that session.

For ongoing tool-call tracing, ask **“Set up persistent tool-call tracing.”** After you approve setup, restart Codex once. The collector then starts at login. If you enable the collector, ask Codex to uninstall it before removing the plugin.

### Install with the Codex CLI

```sh
codex plugin marketplace add zuchka/tell-tail-plugins
codex plugin add tell-tail@tell-tail-plugins
```

## Package

Plugin 0.3.0 bundles the Tell-Tail 0.5.0 executable for macOS arm64. The [build record](plugins/tell-tail/build.json) identifies the [source commit](https://github.com/zuchka/tell-tail/tree/2f2eb2c373e63d18b18272640ba63777d0ecf08b) and executable checksum.

[Privacy policy](https://tell-tail.dev/privacy) · [Report an issue](https://github.com/zuchka/tell-tail/issues) · [License](plugins/tell-tail/LICENSE)
