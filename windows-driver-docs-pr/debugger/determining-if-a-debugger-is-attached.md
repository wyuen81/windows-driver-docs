---
title: Determining if a Debugger is Attached
description: Determining if a Debugger is Attached
ms.assetid: 78f7d90a-459c-4967-a980-3f8d6339eb77
keywords: ["determining if a debugger is attached", "KdRefreshDebuggerNotPresent function", "KD_DEBUGGER_ENABLED global variable", "KD_DEBUGGER_NOT_PRESENT global variable"]
ms.date: 07/20/2020
ms.localizationpriority: medium
---

# Determining if a Debugger is Attached

Kernel-mode code can determine the status of kernel debugging by using the following variables and routines:

- The [**KD\_DEBUGGER\_ENABLED**](https://docs.microsoft.com/previous-versions/ff548118(v=vs.85)) global kernel variable indicates whether kernel debugging is enabled.

- The [**KD\_DEBUGGER\_NOT\_PRESENT**](https://docs.microsoft.com/previous-versions/ff548125(v=vs.85)) global kernel variable indicates whether a kernel debugger is currently attached.

- The [**KdRefreshDebuggerNotPresent**](https://docs.microsoft.com/windows-hardware/drivers/ddi/wdm/nf-wdm-kdrefreshdebuggernotpresent) routine refreshes the value of KD\_DEBUGGER\_NOT\_PRESENT.
