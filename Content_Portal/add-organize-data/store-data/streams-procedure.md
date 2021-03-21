---
uid: gpStreams
---

# Add a stream

Sequential Data Store (SDS) stream data are values or events of the same SDS type. SDS stream data are stored in the Sequential Data Store and indexed by one or more properties defined by the stream's SDS type. See the following for more information about streams:

- [About streams](xref:ccStreams)
- [Streams best practices](xref:bpStreams)

## Procedure

1. Click the ![Menu icon](images\menu-icon.png) icon and click **Sequential Data Store** (under Data Management).

1. Click **Streams**. From the **Namespace** drop-down list, select the namespace in which you want the stream created.

1. Click **Add Stream**.

1. In the Add Stream window, enter the following:

   - Stream Id &ndash;   Identifier for referencing the stream
   - Description &ndash; SDS Stream used by OCS Quick Start
   - Type ID &ndash; Sds type identifier of the type used in this stream          

    Note: Leave the Name field blank. By default, it will take the value of the Stream Id.

1. Click **Save**.

1. In the **Search...** field, enter: TypeId:type_ID, where *type_ID* is the value of the TypeID of the stream.

    This searches for streams that use the specified type. 

1. In the left panel, select the newly created stream in the list.

## Add stream tags

1.  In the right panel, select the **Metadata and Tags** tab, and then click **Add Tag**.

1. In the input field, type the name of the metadata tag and click **Enter**. 

    Note: You can click the tag to edit it, or click the *X* to delete it from the stream.

## Add metadata to the stream

1. Click **Add Metadata**.

1. In **Enter Metadata key...**, type , and in in **Enter Metadata value...**, enter *SLTC*. 

    Note: You can click either of these fields to edit them later, click the *X* to delete it from the stream, or click the *i* <!-- add screen capture here --> to see who last changed this metadata key.

1. In the **Search...** field, enter *Site:SLTC*. 

    This searches for streams that have the metadata key *Site* and the value *SLTC*. This search query returns the QuickStart stream. 
   
    Note: Use quotation marks around the value if there are spaces in the text.
    
1. Select the QuickStart.NorthAmerica.SLTC.PumpA stream and click **Manage Data**. 

    This allows you to run queries against the data in the stream and to add, edit, and remove events.

1. Click **Add Event**.

1. In the Add Event window, enter the following: 

   - Status &ndash; Running
   - Value &ndash; 3.14
   - Timestamp &ndash; Leave at default, which should be current time

1. Click **Save**. 

    The event appears as the latest value in the stream.

## Related Links

- [Streams](xref:sdsStreams) API