---
Description: MSFT\_NetAdapter\_ChecksumOffload.
ms.assetid: 1ed880e0-9142-47f3-8f33-921970824027
title: MSFT\_NetAdapterChecksumOffloadCapabilities class
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# MSFT\_NetAdapterChecksumOffloadCapabilities class

MSFT\_NetAdapter\_ChecksumOffload

The following syntax is simplified from Managed Object Format (MOF) code and includes all of the inherited properties.

## Syntax

``` syntax
[Dynamic, Provider("NetAdapterCim")]
class MSFT_NetAdapterChecksumOffloadCapabilities
{
  string  IPv4TransmitEncapsulation;
  boolean IPv4TransmitIpOptionsSupported;
  boolean IPv4TransmitTcpOptionsSupported;
  boolean IPv4TransmitTcpChecksumSupported;
  boolean IPv4TransmitUdpChecksumSupported;
  boolean IPv4TransmitIpChecksumSupported;
  string  IPv4ReceiveEncapsulation;
  boolean IPv4ReceiveIpOptionsSupported;
  boolean IPv4ReceiveTcpOptionsSupported;
  boolean IPv4ReceiveTcpChecksumSupported;
  boolean IPv4ReceiveUdpChecksumSupported;
  boolean IPv4ReceiveIpChecksumSupported;
  string  IPv6TransmitEncapsulation;
  boolean IPv6TransmitIpExtensionHeadersSupported;
  boolean IPv6TransmitTcpOptionsSupported;
  boolean IPv6TransmitTcpChecksumSupported;
  boolean IPv6TransmitUdpChecksumSupported;
  string  IPv6ReceiveEncapsulation;
  boolean IPv6ReceiveIpExtensionHeadersSupported;
  boolean IPv6ReceiveTcpOptionsSupported;
  boolean IPv6ReceiveTcpChecksumSupported;
  boolean IPv6ReceiveUdpChecksumSupported;
};
```

## Members

The **MSFT\_NetAdapterChecksumOffloadCapabilities** class has these types of members:

-   [Properties](#properties)

### Properties

The **MSFT\_NetAdapterChecksumOffloadCapabilities** class has these properties.

<dl> <dt>

**IPv4ReceiveEncapsulation**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Defines the checksum offload encapsulation settings for the Adapter for IPv4 receive packets.

</dd> <dt>

**IPv4ReceiveIpChecksumSupported**
</dt> <dd> <dl> <dt>

Data type: **boolean**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Indicates if the Adapter supports IP checksum validation offload for receive IPv4 packets.

</dd> <dt>

**IPv4ReceiveIpOptionsSupported**
</dt> <dd> <dl> <dt>

Data type: **boolean**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Indicates if the Adapter supports IPv4 options for receive checksum offload.

</dd> <dt>

**IPv4ReceiveTcpChecksumSupported**
</dt> <dd> <dl> <dt>

Data type: **boolean**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Indicates if the Adapter supports TCP checksum validation offload for receive IPv4 packets.

</dd> <dt>

**IPv4ReceiveTcpOptionsSupported**
</dt> <dd> <dl> <dt>

Data type: **boolean**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Indicates if the Adapter supports TCP options for receive checksum offload on IPv4 packets.

</dd> <dt>

**IPv4ReceiveUdpChecksumSupported**
</dt> <dd> <dl> <dt>

Data type: **boolean**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Indicates if the Adapter supports UDP checksum validation offload for receive IPv4 packets.

</dd> <dt>

**IPv4TransmitEncapsulation**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Defines the checksum offload encapsulation settings for the Adapter for IPv4 transmit packets.

</dd> <dt>

**IPv4TransmitIpChecksumSupported**
</dt> <dd> <dl> <dt>

Data type: **boolean**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Indicates if the Adapter supports IP checksum computation offload for transmit IPv4 packets.

</dd> <dt>

**IPv4TransmitIpOptionsSupported**
</dt> <dd> <dl> <dt>

Data type: **boolean**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Indicates if the Adapter supports IPv4 options for transmit checksum offload.

</dd> <dt>

**IPv4TransmitTcpChecksumSupported**
</dt> <dd> <dl> <dt>

Data type: **boolean**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Indicates if the Adapter supports TCP checksum computation offload for transmit IPv4 packets.

</dd> <dt>

**IPv4TransmitTcpOptionsSupported**
</dt> <dd> <dl> <dt>

Data type: **boolean**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Indicates if the Adapter supports TCP options for transmit checksum offload on IPv4 packets.

</dd> <dt>

**IPv4TransmitUdpChecksumSupported**
</dt> <dd> <dl> <dt>

Data type: **boolean**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Indicates if the Adapter supports UDP checksum computation offload for transmit IPv4 packets.

</dd> <dt>

**IPv6ReceiveEncapsulation**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Defines the checksum offload encapsulation settings for the Adapter for IPv6 receive packets.

</dd> <dt>

**IPv6ReceiveIpExtensionHeadersSupported**
</dt> <dd> <dl> <dt>

Data type: **boolean**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Indicates if the Adapter supports IPv6 extension headers for receive checksum offload.

</dd> <dt>

**IPv6ReceiveTcpChecksumSupported**
</dt> <dd> <dl> <dt>

Data type: **boolean**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Indicates if the Adapter supports TCP checksum validation offload for receive IPv6 packets.

</dd> <dt>

**IPv6ReceiveTcpOptionsSupported**
</dt> <dd> <dl> <dt>

Data type: **boolean**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Indicates if the Adapter supports TCP options for receive checksum offload on IPv6 packets.

</dd> <dt>

**IPv6ReceiveUdpChecksumSupported**
</dt> <dd> <dl> <dt>

Data type: **boolean**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Indicates if the Adapter supports UDP checksum validation offload for receive IPv6 packets.

</dd> <dt>

**IPv6TransmitEncapsulation**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Defines the checksum offload encapsulation settings for the Adapter for IPv6 transmit packets.

</dd> <dt>

**IPv6TransmitIpExtensionHeadersSupported**
</dt> <dd> <dl> <dt>

Data type: **boolean**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Indicates if the Adapter supports IPv6 extension headers for transmit checksum offload.

</dd> <dt>

**IPv6TransmitTcpChecksumSupported**
</dt> <dd> <dl> <dt>

Data type: **boolean**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Indicates if the Adapter supports TCP checksum computation offload for transmit IPv6 packets.

</dd> <dt>

**IPv6TransmitTcpOptionsSupported**
</dt> <dd> <dl> <dt>

Data type: **boolean**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Indicates if the Adapter supports TCP options for transmit checksum offload on IPv6 packets.

</dd> <dt>

**IPv6TransmitUdpChecksumSupported**
</dt> <dd> <dl> <dt>

Data type: **boolean**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Indicates if the Adapter supports UDP checksum computation offload for transmit IPv6 packets.

</dd> </dl>

## Requirements



|                                     |                                                                                              |
|-------------------------------------|----------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                                    |
| Minimum supported server<br/> | Windows Server 2012<br/>                                                               |
| Namespace<br/>                | Root\\StandardCimv2<br/>                                                               |
| MOF<br/>                      | <dl> <dt>NetAdapterCim.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>NetAdapterCim.dll</dt> </dl> |



 

 



