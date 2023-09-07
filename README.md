<div align="center">

<a href="https://tezos.com/unity/"><img height="200x" src="https://tezos.com/tez/tez-banner.jpg" /></a>

  <h1>Tezos Market SDK</h1>

  <p>
    <strong>Unity SDK to interact with marketplace on Tezos</strong>
  </p>

  <p>
    <a href="https://github.com/mismirnov/tezos-market-sdk/issues"><img alt="Issues" src="https://img.shields.io/github/issues/baking-bad/tezos-market-sdk" /></a>
    <a href="https://opensource.org/licenses/MIT"><img alt="License" src="https://img.shields.io/github/license/baking-bad/tezos-market-sdk" /></a>
  </p>
</div>

The Tezos Market SDK invites developers to discover the future of Web3 gaming with a complete kit that empowers game
developers with the ability to:

- Connect to a Tezos wallet
- Utilize data on the blockchain
- Call smart contracts
- True ownership of in-game assets

The Tezos SDK supports Desktop, Android, iOS, and browsers. Beyond allowing game developers to interact with the Tezos
blockchain, this SDK is a helpful resource for developing any Tezos decentralized application (dApp).

### Installation pre-requirements

This package is depend on [tezos-unity-sdk](https://github.com/trilitech/tezos-unity-sdk) Unity package. To be able to work it is
necessary to add `com.trilitech` scope to your project
[manifest file](https://docs.unity3d.com/Manual/upm-manifestPrj.html). To do this, add `scopedRegistries` section as
shown in the example below to your project `manifest.json` file.
 
```json
{
  "scopedRegistries": [{
    "name": "npmjs",
    "url": "https://registry.npmjs.org/",
    "scopes": [
      "com.trilitech"
    ]
  }]
}
```

### Install from unitypackage file

You can install TezosMarketSdk via `.unitypackage` file. To load a package from a unitypackage file:

* Go to [Releases](https://github.com/mismirnov/tezos-market-sdk/releases) page and download the
  latest `TezosMarketSdk.unitypackage`.
* Open your project in Unity Editor.
* Double-click the `TezosMarketSdk.unitypackage` file to import it into the current project.

### Install from a Git URL

You can install the UPM package via directly Git URL. To load a package from a Git URL:

* Open [Unity Package Manager](https://docs.unity3d.com/Manual/upm-ui.html) window.
* Click the add **+** button in the status bar.
* The options for adding packages appear.
* Select Add package from git URL from the add menu. A text box and an Add button appear.
* Enter the `https://github.com/mismirnov/tezos-market-sdk.git` Git URL in the text box and click Add.
* You may also install a specific package version by using the URL with the specified version.
    * `https://github.com/mismirnov/tezos-market-sdk.git#X.Y.Z`
    * Please note that the version `X.Y.Z` stated here is to be replaced with the version you would like to get.
    * You can find all the available releases [here](https://github.com/mismirnov/tezos-market-sdk/releases).
    * The latest available release version
      is [![Last Release](https://img.shields.io/github/v/release/mismirnov/tezos-market-sdk)](https://github.com/baking-bad/tezos-market-sdk/releases/latest)

For more information about what protocols Unity supports, see [Git URLs](https://docs.unity3d.com/Manual/upm-git.html).

### Install from NPM

* Navigate to the `Packages` directory of your project.
* Adjust the [project manifest file](https://docs.unity3d.com/Manual/upm-manifestPrj.html) `manifest.json` in a text
  editor.
* Ensure `https://registry.npmjs.org/` is part of `scopedRegistries`.
    * Ensure `com.baking-bad` is part of `scopes`.
    * Add `com.baking-bad.tezos-market-sdk` to the `dependencies`, stating the latest version.

A minimal example ends up looking like this. Please note that the version `X.Y.Z` stated here is to be replaced
with [the latest released version](https://www.npmjs.com/package/com.baking-bad.tezos-market-sdk), which is
currently [![NPM Package](https://img.shields.io/npm/v/com.baking-bad.tezos-market-sdk?color=blue)](https://www.npmjs.com/package/com.baking-bad.tezos-market-sdk).

```json
{
  "scopedRegistries": [
    {
      "name": "npmjs",
      "url": "https://registry.npmjs.org/",
      "scopes": [
        "com.baking-bad"
      ]
    }
  ],
  "dependencies": {
    "com.baking-bad.tezos-market-sdk": "X.Y.Z",
    ...
  }
}
```

* Switch back to the Unity Editor and wait for it to finish importing the added package.
