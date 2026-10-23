# Codlet GUI

Official Codlet plugin for graphical plugin and runtime management

Plugin ID: `codlet-gui` · Version: `1.0.0-rc.5`

## Install and update

In Codlet, choose **Add → Import plugin → GitHub**, then paste:

https://github.com/baoabaob/codlet-gui

Use the plugin ZIP from [Releases](https://github.com/baoabaob/codlet-gui/releases), not GitHub's generated source-code archive. Codlet reads this plugin's signed update manifest and verifies direct-file downloads with the publisher key recorded in the installed package. The first remote update of a preinstalled package asks you to review its adoption; local author folders are never enrolled automatically. Private repositories and draft releases are not available to the current unauthenticated importer.

Dependencies: Core only. Codlet Core 1 supplies the standard UI/Desktop SDK; separate Adapter installation is not required.

Permissions: `ui.dom`, `runtime.manage`

## Development

This repository is generated from [codlet-plugins](https://github.com/baoabaob/codlet-plugins). Make changes and report issues in that development repository; edits here are not automatically merged back.

The source snapshot and pinned build dependencies are included. To rebuild this plugin:

```text
npm ci --prefix frontend
node frontend/build.mjs
```

Core's runtime SDK is supplied by Codlet. The source revision and exact files are recorded in `.codlet-distribution.json`. Reviewed client profiles and actual native acceptance boundaries are documented in the [development repository's known issues](https://github.com/baoabaob/codlet-plugins/blob/main/docs/known-issues.md).

## License

Original Codlet code is licensed under [Apache-2.0](LICENSE); see [NOTICE](NOTICE). Third-party dependencies retain their own licenses and notices. Independently developed Codlet plugins may choose their own licenses.

## Remove

Uninstall from the Codlet GUI or CLI. Uninstall removes the installed copy and clears configuration, data, cache and credentials. When installing over an existing ID, Update preserves data and Replace starts empty. These installation features require Codlet Core 1.0.0-rc.5 or later.
