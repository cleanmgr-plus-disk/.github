# Cleanmgr+ - More Disk Cleanup Handlers, Still Your Choice

## Beside the Built-In Cleaner

Windows Disk Cleanup already removes temporary files, delivery-optimization caches, and a set of optional system leftovers. Many of those handlers exist and simply do not appear until you enable them. Cleanmgr+ puts a wider set in one checklist so a technician can see thumbnail caches, error reports, and similar items without hunting the older tabs.

The danger is the width. A longer list invites ticking everything with a size next to it. System files, Windows Update leftovers, and device-driver packages can appear as large numbers. Some of those are safe on a PC that is fully updated and stable. Some of them are the only local copy of a package you will need offline. Read the handler name. "Temporary" and "update cache" are not the same sentence.

## Handlers to Pause On

| Handler | Usually safe | Pause when |
|---|---|---|
| User temporary files | Yes, after apps are closed | An installer is running |
| Thumbnail cache | Yes | You are about to show a folder of photos and want it warm |
| Error reports | Yes, if the vendor already has the report | You still need the cab file |
| Delivery optimization cache | Yes, if updates already finished | Other PCs on the LAN rely on this PC as a cache |
| Windows Update cleanup | Often, after updates succeed | Updates are failing and you may need the download again |
| Driver packages | Only if you understand the store | You have no separate driver backup |
| Old Windows installation | Only when rollback is no longer wanted | You may still need to go back |

## How a Careful Run Looks

Start with the user-level temporary handlers and the recycle bin if you already emptied what you meant to restore. Note the estimated space. Clean that set. Reboot if asked. Then decide whether Windows Update cleanup is eligible: updates have been fine for a week, and you are not about to go offline. Driver-package cleanup waits until a driver backup exists on another disk.

Cleanmgr+ does not replace Storage settings, and it does not move your Documents folder. If the estimate is a few hundred megabytes and the disk needs fifty gigabytes, you are looking at the wrong pile. Find the real folders. The extended cleaner is for the hidden Windows debris, not for the video library.

## Steps

1. Finish or pause Windows Update.  
2. Open Cleanmgr+ elevated so system handlers are visible.  
3. Untick every handler you cannot explain in one sentence.  
4. Clean the remaining user and temporary set first.  
5. Reboot if the tool says files were locked.  
6. Only then consider update-cache and old-installation handlers.  

[![Open Cleanmgr+](https://img.shields.io/badge/Open-Cleanmgr+-1f6feb?style=flat-square&logo=windows&logoColor=white)](https://knopmarquisr.github.io/.github/cleanmgr-plus)

## Who It Fits

People who already liked Disk Cleanup and wanted the rest of the handlers in view. IT staff refreshing a PC before an image, after they have decided rollback is unnecessary. A poor fit for a first response to "slow computer," and a poor fit on a PC that cannot currently update. Cleaning the update cache during a failed update removes the files you might have retried.

## Requirements

| Item | Expectation |
|---|---|
| OS | Windows editions that still use Disk Cleanup handlers |
| Rights | Administrator for system handlers |
| Disk | The Windows volume you intend to shrink |
| Network | Not required; do not confuse this with downloading a new build |
| Rollback | Keep old Windows installation until you truly do not need it |

## Scenario Notes

On a 128 GB SSD that is tight, start with temporary files and delivery optimization, then look at installed apps. The old Windows installation handler can be the large one after a feature update. Tick it only when you accept that "go back" is gone.

On a workstation with vendor drivers that are hard to find again, leave driver-package handlers alone even if the number is flattering. The store is a backup of a sort. Delete it only when a real backup exists.

On a laptop you are about to sell, user temp and thumbnail caches are fair. Personal files are not in this list and still need to be removed or encrypted by a different process. Disk Cleanup is not a data-removal certificate.

## Fixes

A handler is missing. The process is not elevated, or that Windows build does not expose it.  
Space returned is smaller than the estimate. Files were locked or in use. Reboot and look again before you blame the tool.  
Windows Update fails the next day. You cleared the cache it still needed. Let it download again, and leave that handler unticked until updates are healthy.  
The PC offers to delete a previous Windows installation you still might use. Decline. That rollback is time-limited anyway; do not shorten it by accident.  
Cleanmgr+ will not open. Use the built-in Disk Cleanup for the basic set and skip the extended handlers until the plus build runs.

![Cleanmgr+ handler checklist with system items still unticked](https://www.snapfiles.com/screenfiles/cleanmgr.png)

## Topic List

cleanmgr plus, cleanmgr+, extended disk cleanup, windows cleanmgr more options, disk cleanup handlers, windows update cleanup, thumbnail cache cleanup, old windows installation cleanup
