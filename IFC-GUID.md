# IFC GUID
## Introduction
The IFC specification uses an unique identifier for object instances that follows the universal unique identifier standard UUID with its implementation as a globally unique identifier GUID. The generated GUID is compressed for exchange purpose following a published compression function. The compressed GUID is called "IFC-GUID" here.

## Background Information
A Globally Unique Identifier (GUID) or Universal Unique Identifier (UUID) (as defined by ISO/IEC 11578:1996 Information technology -- Open Systems Interconnection -- Remote Procedure Call (RPC)specification and more recently in ITU-T Rec. X.667 | ISO/IEC 9834-8:2005) provides a way of uniquely identifying an object. GUID generation algorithms have been developed for most software development framework environments and methods exist within these frameworks for persistence.

For file-based data exchange, a methodology was devised to compress these GUIDs to conserve space when physically exchanging IFC models through various media. Given that each IFC object instance required a unique identifier containing a 128-bit number, a base 64 character encoding was devised as shown below:

IFC-GUID Base-64 character encoding mapping: 

**0**123456789**0**123456789**0**123456789**0**123456789**0**123456789**0**1234567890123
0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz_$

The resulting IFC-GUID is a fixed 22 character length string. Software implementations will need to use an algorithm that converts standard GUIDs to and from this encoding for compliance with the IFC specifications.

Note: The compression of the GUID for IFC file based exchange had been introduced back in 1996 for version IFC1.0. At that time data files were still stored on floppy disks with 1,44 MB capacity where every byte counted. Today compression of a GUID would be considered unnecessary but due to backward compatibility issues it is still enforced.

Examples of code to generate compliant GUIDs can be found here https://github.com/IfcOpenShell/IfcOpenShell/blob/master/src/ifcopenshell-python/ifcopenshell/guid.py#L56
 
