![Header](https://github.com/emotitron/Simple-Network-Sync/blob/master/Docs/SNS_DocumentHeader.jpg?raw=true)
# Simple Network Sync
This project is an Beta of the Asset Store replacement library for Network Sync Transform, which is becoming very old and hard to maintain. The components used in this are more in line with the determinstic server authority networking library I am working on, so they will be supported and worked on regulary. Once out of Alpha the components will be for charge on the Asset Store, but anyone helping with the testing I will just let have them, as well as access to fixes and such.

All components on a networked gameobject are bitpacked and serialized with circular frameids into one highly compressed byte[].

- This should work extremely well for networking projects that simulate using fixedUpdate.
- This is less than ideal for objects controlled in Update(), but will likely work better than PUN2/UNET/Mirror built in sync components
- Because of the unified tick and ring buffers, Transform and Animator syncs should be syncronized across an object, keeping Animator and Transform actions coordinated.

Please give these a try and let me know how you are able to break them, so I can make them indestructible.

[**Download Current Beta** - Unity Package Download](https://github.com/emotitron/Simple-Network-Sync/releases)

There are two primary components currently and some support components.

## SimpleSyncTransform
A replacement for NetworkTransform or PhotonTransformView. Use as you would NetworkTransform.
![SyncTransform](https://github.com/emotitron/Simple-Network-Sync/blob/master/Docs/Unity_2019-05-19_00-33-06.png?raw=truee)

## SimpleSyncAnimator
A replacement for NetworkAnimator or PhotonAnimatorView. Drag it on to a gameobject where an Animator exists, similar to how you use NetworkAnimator. More instructions to come.

![SyncAnimator](https://github.com/emotitron/Simple-Network-Sync/blob/master/Docs/Unity_2019-05-19_00-31-58.png?raw=true)


## NetMaster
Added to the scene automatically at startup, and is the timing singleton for all of Simple Network Sync. If you don't add one to your first scene, one will be created with the default setting of Send Every X being set to 1.

![NetMaster](https://github.com/emotitron/Simple-Network-Sync/blob/master/Docs/NetMaster.png?raw=true)

## Bug Reports
Let me know how these break for you. I am emotitron on Discord, or email me at davincarten@gmail.com.

I would like it to be able to handle all edge cases, so the more ways you can break it... the better. I'm making note of people who give me feedback for future inclusion in vouchers and git access after it is released.
