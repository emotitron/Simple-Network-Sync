![Header](https://github.com/emotitron/Simple-Network-Sync/blob/master/Docs/SNS_DocumentHeader.jpg?raw=true)
# Simple Network Sync
This project is an Alpha of the Asset Store replacement library for Network Sync Transform, which is becoming very old and hard to maintain. The components used in this are more in line with the determinstic server authority networking library I am working on, so they will be supported and worked on regulary. Once out of Alpha the components will be for charge on the Asset Store, but anyone helping with the testing I will just let have them, as well as access to fixes and such.

Please give these a try and let me know how you are able to break them, so I can make them indestructible.

[**Download Current Alpha** - Unity Package Download](https://github.com/emotitron/Simple-Network-Sync/releases/tag/0.2a)

There are two primary components.

**Note: The order of SimpleSyncTransform and SimpleSyncAnimator affect the order in which they are applied, which for objects with root motion can have interesting results if the Animator is before the Transform sync. So in summary, put the SyncTransform above the SyncAnimator in the inspector.**

## SimpleSyncTransform
A replacement for NetworkTransform or PhotonTransformView. Use as you would NetworkTransform.

## SimpleSyncAnimator
A replacement for NetworkAnimator or PhotonAnimatorView. Drag it on to a gameobject where an Animator exists, similar to how you use NetworkAnimator. More instructions to come.

Let me know how these break for you. I would like it to be able to handle all edge cases, so the more ways you can break it... the better.
