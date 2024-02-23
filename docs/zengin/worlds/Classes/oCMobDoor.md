# oCMobDoor

!!! abstract inline end "Quick Infos"
    **Class Name:** `oCMobDoor`<br/>
    **Version Identifiers:**<br />
    — Gothic I: `64513`<br/>
    — Gothic II: `64513`<br/>
    **Sources:**<br/>
    — [gothic-library.ru](http://www.gothic-library.ru/publ/ocmobdoor/1-1-0-510)<br/>
    — [zk.gothickit.dev](https://zk.gothickit.dev/engine/objects/oCMobDoor/)

A VObject representing a door. This is also used for NPCs navigating the waynet.

## Class members

=== "Gothic 1"

    - [zCVob](zCVob.md)
      {: .sp-class}
    - [oCVob](oCVob.md)
      {: .sp-class}
    - [oCMOB](oCMOB.md)
      {: .sp-class}
    - [oCMobInter](oCMobInter.md)
      {: .sp-class}
    - oCMobContainer
      {: .sp-class}
        - Lockable
          {: .sp-folder}
            - [locked](#locked) = FALSE
              {: .sp-bool}
            - [keyInstance](#keyinstance) = ""
              {: .sp-string}
            - [pickLockStr](#picklockstr) = ""
              {: .sp-string}

=== "Gothic 2"

    - [zCVob](zCVob.md)
      {: .sp-class}
    - [oCVob](oCVob.md)
      {: .sp-class}
    - [oCMOB](oCMOB.md)
      {: .sp-class}
    - [oCMobInter](oCMobInter.md)
      {: .sp-class}
    - oCMobContainer
      {: .sp-class}
        - Lockable
          {: .sp-folder}
            - [locked](#locked) = FALSE
              {: .sp-bool}
            - [keyInstance](#keyinstance) = ""
              {: .sp-string}
            - [pickLockStr](#picklockstr) = ""
              {: .sp-string}

=== "Gothic 1 (Save)"

    - [zCVob](zCVob.md)
      {: .sp-class}
    - [oCVob](oCVob.md)
      {: .sp-class}
    - [oCMOB](oCMOB.md)
      {: .sp-class}
    - [oCMobInter](oCMobInter.md)
      {: .sp-class}
    - oCMobContainer
      {: .sp-class}
        - Lockable
          {: .sp-folder}
            - [locked](#locked) = FALSE
              {: .sp-bool}
            - [keyInstance](#keyinstance) = ""
              {: .sp-string}
            - [pickLockStr](#picklockstr) = ""
              {: .sp-string}

=== "Gothic 2 (Save)"

    - [zCVob](zCVob.md)
      {: .sp-class}
    - [oCVob](oCVob.md)
      {: .sp-class}
    - [oCMOB](oCMOB.md)
      {: .sp-class}
    - [oCMobInter](oCMobInter.md)
      {: .sp-class}
    - oCMobContainer
      {: .sp-class}
        - Lockable
          {: .sp-folder}
            - [locked](#locked) = FALSE
              {: .sp-bool}
            - [keyInstance](#keyinstance) = ""
              {: .sp-string}
            - [pickLockStr](#picklockstr) = ""
              {: .sp-string}

## Class member overview

### `locked` {: .sp-bool}

Determines whether the container is locked.

**Accepted values:**

* `TRUE` — The container is locked
* `FALSE` — The container is not locked

### `keyInstance` {: .sp-string}

The name of the item script instance which unlocks the container.

!!! tip
    Only relevant if the container is locked.

### `pickLockStr` {: .sp-string}

The combination which unlocks this container when picking the lock. Each character of the string is either `R` or
`L` where `R` stands for "Right" and `L` stands for "Left". If empty, the lock can not be picked.
<br />Example: `LRRLLRL`.

!!! tip
    Only relevant if the container is locked.
