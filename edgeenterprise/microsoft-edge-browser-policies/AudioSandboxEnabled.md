---
title: "Microsoft Edge Browser Policy Documentation AudioSandboxEnabled"
ms.author: jalam
author: vmliramichael
manager: nuyunzhang
ms.date: 04/22/2025
audience: ITPro
ms.topic: reference
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
ms.custom:
description: "Windows and Mac documentation for supported Microsoft Edge Browser policy: Allow the audio sandbox to run"
---

# AudioSandboxEnabled

## Allow the audio sandbox to run


## Supported versions

- On Windows and macOS since 81 or later

## Description

This policy controls the audio process sandbox.

If you enable this policy, the audio process will run sandboxed.

If you disable this policy, the audio process will run unsandboxed and the WebRTC audio-processing module will run in the renderer process.
This leaves users open to security risks related to running the audio subsystem unsandboxed.

If you don't configure this policy, the default configuration for the audio sandbox will be used, which might differ based on the platform.

This policy is intended to give enterprises flexibility to disable the audio sandbox if they use security software setups that interfere with the sandbox.

## Supported features

- Can be mandatory: No
- Can be recommended: No
- Dynamic Policy Refresh: No - Requires browser restart
- Per Profile: No
- Applies to a profile that is signed in with a Microsoft account: Yes

## Data type

- Boolean

## Windows information and settings

### Group Policy (ADMX) info

- GP unique name: AudioSandboxEnabled
- GP name: Allow the audio sandbox to run
- GP path (Mandatory): N/A
- GP path (Recommended): N/A
- GP ADMX file name: MSEdge.admx

#### Example value

```
Enabled
```

### Registry settings

- Path (Mandatory): N/A
- Path (Recommended): N/A
- Value name: AudioSandboxEnabled
- Value type: REG_DWORD

#### Example value

```
0x00000001
```


## Mac information and settings

- Preference Key name: AudioSandboxEnabled
- Example value:

```xml
<true/>
```

## See also
- [Microsoft Edge - Policies](../microsoft-edge-policies.md)
