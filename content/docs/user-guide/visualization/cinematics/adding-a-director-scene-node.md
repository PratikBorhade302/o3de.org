---
description: ' Add a Director (Scene) node in the <guilabel>Track View</guilabel> editor in Open 3D Engine. '
title: Adding a Director (Scene) Node
---

{{< preview-migrated >}}

To determine what camera you want your sequence to use, you must add a [Director (Scene) Node](/docs/user-guide/visualization/cinematics/track-view/nodes-director.md).

**To add a Director node in the Track View**

1. In O3DE Editor, choose **Tools**, **Track View**.

1. In the Track View, select or create a sequence.

1. Do one of the following:
   + Right-click your sequence and choose **Add Director (Scene) Node**.
   + Click the **Add Director Node** icon.
![\[Add the Director node in the Track View to manage your track view sequence.\]](/images/user-guide/cinematics/cinematics-track-view-editor-adding-director-node-1.png)

By default, the **Camera** track appears on the **Director (Scene) Node** to control which camera is active for the sequence. This is the only track that is needed to assign and switch between cameras.

For more information about other tracks that you can add, see the [Director (Scene) Node](/docs/user-guide/visualization/cinematics/track-view/nodes-director.md).

![\[Add the Camera track in the Track View\]](/images/user-guide/cinematics/cinematics-track-view-editor-adding-director-node-2.png)

When you add an animation key on the **Camera** track, you can select the key and assign which camera should be active from the **Key Properties** pane. When a camera is set, you can see the name of the camera on the track.

![\[Add keyframes for the Director node in the Track View to manage your camera.\]](/images/user-guide/cinematics/cinematics-track-view-editor-adding-director-node-3.png)

To create a series of jump cuts from one camera to another camera in a sequence, add animation keys on the **Camera** track for the **Director** node. The **Director** node uses the key properties set for the **Camera** track to determine which camera to switch.
