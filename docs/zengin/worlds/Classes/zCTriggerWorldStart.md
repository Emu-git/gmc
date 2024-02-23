# zCTriggerWorldStart

!!! abstract inline end "Quick Infos"
    **Class Name:** `zCTriggerWorldStart`<br/>
    **Version Identifiers:**<br />
    — Gothic I: `52224`<br/>
    — Gothic II: `52224`<br/>
    **Sources:**<br/>
    — [spacerhilfedatei.sph](https://wiki.worldofgothic.de/doku.php?id=spacer:hilfedatei)<br/>
    — [zk.gothickit.dev](https://zk.gothickit.dev/engine/objects/zCTriggerWorldStart/)

A special trigger which fires an `OnTrigger` event to its [target](#triggertarget) when the world is loaded and started.

## Class members

=== "Gothic 1"

    - [zCVob](zCVob.md)
      {: .sp-class}
    - zCTriggerWorldStart
      {: .sp-class}
        - [triggerTarget](#triggertarget) = ""
          {: .sp-string}
        - [fireOnlyFirstTime](#fireonlyfirsttime) = FALSE
          {: .sp-bool}

=== "Gothic 2"

    - [zCVob](zCVob.md)
      {: .sp-class}
    - zCTriggerWorldStart
      {: .sp-class}
        - [triggerTarget](#triggertarget) = ""
          {: .sp-string}
        - [fireOnlyFirstTime](#fireonlyfirsttime) = FALSE
          {: .sp-bool}

=== "Gothic 1 (Save)"

    - [zCVob](zCVob.md)
      {: .sp-class}
    - zCTriggerWorldStart
      {: .sp-class}
        - [triggerTarget](#triggertarget) = ""
          {: .sp-string}
        - [fireOnlyFirstTime](#fireonlyfirsttime) = FALSE
          {: .sp-bool}

=== "Gothic 2 (Save)"

    - [zCVob](zCVob.md)
      {: .sp-class}
    - zCTriggerWorldStart
      {: .sp-class}
        - [triggerTarget](#triggertarget) = ""
          {: .sp-string}
        - [fireOnlyFirstTime](#fireonlyfirsttime) = FALSE
          {: .sp-bool}

## Class member overview

### `triggerTarget` {: .sp-string}

The name of VObject to send an `OnTrigger` event to when the world is loaded and started.

### `fireOnlyFirstTime` {: .sp-bool}

Determines whether to fire the `OnTrigger` event only the first time the world is loaded.

**Accepted values:**

* `TRUE` — Only fire the event if this is the first time the world is loaded.
* `FALSE` — Fire the event every time the world is loaded.
