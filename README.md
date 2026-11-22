<!-- Generated distribution; edit the canonical repository. -->
# swift-ai-tencent 1.0.1

Independent Swift-native port of Vercel AI SDK. Source and upstream dispositions are in PROVENANCE.json and Porting/.

## Distribution manifest

Add this package to your SwiftPM dependencies:

```swift
.package(url: "https://github.com/SwiftAISDK/swift-ai-tencent.git", from: "1.0.1")
```

Products: `SwiftAITencent`.
Contribute and report issues in the canonical SwiftAISDK repository.

## Authored usage guide

# Tencent (TokenHub and Cloud VOD) for Swift

`SwiftAITencent` adds Tencent (TokenHub and Cloud VOD) to [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK), an independent Swift port of the Vercel AI SDK. It ports `@ai-sdk/tencent` and supports text generation and video generation.

Provider guide with models, options, streaming and errors:

- [Tencent (TokenHub and Cloud VOD)](https://swiftaisdk.github.io/SwiftAISDK/providers/tencent/)

## Usage

Add the `SwiftAI` product from `swift-ai-core` and the `SwiftAITencent` product from this package to your target, then create the provider:

```swift
import SwiftAI
import SwiftAITencent

let provider = try AIProviders.tencent(configuration: TencentProviderSettings())
```

By default the provider reads `TENCENT_TOKENHUB_API_KEY`, `TENCENTCLOUD_SECRET_ID`, `TENCENTCLOUD_SECRET_KEY`, `TENCENTCLOUD_VOD_SUB_APP_ID` and `TENCENTCLOUD_SESSION_TOKEN` from the environment; values set in `TencentProviderSettings` take precedence.

To use every provider through one dependency, add the complete [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) package instead; see [Install](https://swiftaisdk.github.io/SwiftAISDK/getting-started/install/).

## Contributing

This package is exported from `Packages/swift-ai-tencent` in the canonical [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) repository. Open issues and pull requests there.
