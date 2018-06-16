---
title: Windows Event Log Functions
description: Windows Event Log defines the following functions that you can use to get events from a channel or event log and to get the metadata for a provider and the events that it generates.
ms.assetid: 0bc008e4-c01c-482b-b910-49de3de22fab
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Windows Event Log Functions

Windows Event Log defines the following functions that you can use to get events from a channel or event log and to get the metadata for a provider and the events that it generates.



| Function                                                                   | Description                                                                                                                                                                                                       |
|----------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**EVT\_SUBSCRIBE\_CALLBACK**](https://msdn.microsoft.com/en-us/library/Aa385577(v=VS.85).aspx)                 | Implement this callback if you call the [**EvtSubscribe**](/windows/desktop/api/WinEvt/nf-winevt-evtsubscribe) function to receive events that match your query.                                                                                    |
| [**EvtArchiveExportedLog**](/windows/desktop/api/WinEvt/nf-winevt-evtarchiveexportedlog)                     | Adds localized strings to the events in the specified log file.                                                                                                                                                   |
| [**EvtCancel**](/windows/desktop/api/WinEvt/nf-winevt-evtcancel)                                             | Cancels all pending operations on a handle.                                                                                                                                                                       |
| [**EvtClearLog**](/windows/desktop/api/WinEvt/nf-winevt-evtclearlog)                                         | Removes all events from the specified channel and writes them to the target log file.                                                                                                                             |
| [**EvtClose**](/windows/desktop/api/WinEvt/nf-winevt-evtclose)                                               | Closes an open handle.                                                                                                                                                                                            |
| [**EvtCreateBookmark**](/windows/desktop/api/WinEvt/nf-winevt-evtcreatebookmark)                             | Creates a bookmark that identifies an event in a channel.                                                                                                                                                         |
| [**EvtCreateRenderContext**](/windows/desktop/api/WinEvt/nf-winevt-evtcreaterendercontext)                   | Creates a context that specifies the information in the event that you want to render.                                                                                                                            |
| [**EvtExportLog**](/windows/desktop/api/WinEvt/nf-winevt-evtexportlog)                                       | Copies events from the specified channel or log file and writes them to the target log file.                                                                                                                      |
| [**EvtFormatMessage**](/windows/desktop/api/WinEvt/nf-winevt-evtformatmessage)                               | Formats a message string.                                                                                                                                                                                         |
| [**EvtGetChannelConfigProperty**](/windows/desktop/api/WinEvt/nf-winevt-evtgetchannelconfigproperty)         | Gets the specified channel configuration property.                                                                                                                                                                |
| [**EvtGetEventInfo**](/windows/desktop/api/WinEvt/nf-winevt-evtgeteventinfo)                                 | Gets information that identifies the structured XML query that selected the event and the channel or log file from which it came.                                                                                 |
| [**EvtGetEventMetadataProperty**](/windows/desktop/api/WinEvt/nf-winevt-evtgeteventmetadataproperty)         | Gets the specified event metadata property.                                                                                                                                                                       |
| [**EvtGetExtendedStatus**](/windows/desktop/api/WinEvt/nf-winevt-evtgetextendedstatus)                       | Gets a text message that contains the extended error information for the current error.                                                                                                                           |
| [**EvtGetLogInfo**](/windows/desktop/api/WinEvt/nf-winevt-evtgetloginfo)                                     | Gets information about a channel or log file.                                                                                                                                                                     |
| [**EvtGetObjectArrayProperty**](/windows/desktop/api/WinEvt/nf-winevt-evtgetobjectarrayproperty)             | Gets a provider metadata property from the specified object in the array.                                                                                                                                         |
| [**EvtGetObjectArraySize**](/windows/desktop/api/WinEvt/nf-winevt-evtgetobjectarraysize)                     | Gets the number of elements in the array of objects.                                                                                                                                                              |
| [**EvtGetPublisherMetadataProperty**](/windows/desktop/api/WinEvt/nf-winevt-evtgetpublishermetadataproperty) | Gets the specified provider metadata property.                                                                                                                                                                    |
| [**EvtGetQueryInfo**](/windows/desktop/api/WinEvt/nf-winevt-evtgetqueryinfo)                                 | Gets information about a query that you ran that identifies the list of channels or log files that the query attempted to access and a list of return codes that indicates the success or failure of each access. |
| [**EvtNext**](/windows/desktop/api/WinEvt/nf-winevt-evtnext)                                                 | Gets the next event from the query or subscription results.                                                                                                                                                       |
| [**EvtNextChannelPath**](/windows/desktop/api/WinEvt/nf-winevt-evtnextchannelpath)                           | Gets a channel name from the enumerator.                                                                                                                                                                          |
| [**EvtNextEventMetadata**](/windows/desktop/api/WinEvt/nf-winevt-evtnexteventmetadata)                       | Gets an event definition from the enumerator.                                                                                                                                                                     |
| [**EvtNextPublisherId**](/windows/desktop/api/WinEvt/nf-winevt-evtnextpublisherid)                           | Gets the identifier of a provider from the enumerator.                                                                                                                                                            |
| [**EvtOpenChannelConfig**](/windows/desktop/api/WinEvt/nf-winevt-evtopenchannelconfig)                       | Gets a handle that you use to read or modify a channel's configuration property.                                                                                                                                  |
| [**EvtOpenChannelEnum**](/windows/desktop/api/WinEvt/nf-winevt-evtopenchannelenum)                           | Gets a handle that you use to enumerate the list of channels that are registered on the computer.                                                                                                                 |
| [**EvtOpenEventMetadataEnum**](/windows/desktop/api/WinEvt/nf-winevt-evtopeneventmetadataenum)               | Gets a handle that you use to enumerate the list of events that the provider defines.                                                                                                                             |
| [**EvtOpenLog**](/windows/desktop/api/WinEvt/nf-winevt-evtopenlog)                                           | Gets a handle to a channel or log file that you can then use to get information about the channel or log file.                                                                                                    |
| [**EvtOpenPublisherEnum**](/windows/desktop/api/WinEvt/nf-winevt-evtopenpublisherenum)                       | Gets a handle that you use to enumerate the list of registered providers on the computer.                                                                                                                         |
| [**EvtOpenPublisherMetadata**](/windows/desktop/api/WinEvt/nf-winevt-evtopenpublishermetadata)               | Gets a handle that you use to read the specified provider's metadata.                                                                                                                                             |
| [**EvtOpenSession**](/windows/desktop/api/WinEvt/nf-winevt-evtopensession)                                   | Establishes a connection to a remote computer that you can use when calling the other Windows Event Log functions.                                                                                                |
| [**EvtQuery**](/windows/desktop/api/WinEvt/nf-winevt-evtquery)                                               | Runs a query to retrieve events from a channel or log file that match the specified query criteria.                                                                                                               |
| [**EvtRender**](/windows/desktop/api/WinEvt/nf-winevt-evtrender)                                             | Renders an XML fragment based on the rendering context that you specify.                                                                                                                                          |
| [**EvtSaveChannelConfig**](/windows/desktop/api/WinEvt/nf-winevt-evtsavechannelconfig)                       | Saves the changes made to a channel's configuration.                                                                                                                                                              |
| [**EvtSeek**](/windows/desktop/api/WinEvt/nf-winevt-evtseek)                                                 | Seeks to a specific event in a query result set.                                                                                                                                                                  |
| [**EvtSetChannelConfigProperty**](/windows/desktop/api/WinEvt/nf-winevt-evtsetchannelconfigproperty)         | Sets the specified configuration property of a channel.                                                                                                                                                           |
| [**EvtSubscribe**](/windows/desktop/api/WinEvt/nf-winevt-evtsubscribe)                                       | Creates a subscription that will receive current and future events from a channel or log file that match the specified query criteria.                                                                            |
| [**EvtUpdateBookmark**](/windows/desktop/api/WinEvt/nf-winevt-evtupdatebookmark)                             | Updates the bookmark with information that identifies the specified event.                                                                                                                                        |



 

 

 



