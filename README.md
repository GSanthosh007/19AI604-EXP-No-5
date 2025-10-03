## Experiment 5 - Create IPAddress Kind enum to represent IPv4, IPv6 addresses and create IP Address structure with IP Address Kind as a member and use this structure in the application.

<H3>ENTER YOUR NAME:</H3>  
<H3>ENTER YOUR REGISTER NO:</H3>  
<H3>EX.NO.5</H3>  
<H3>DATE:</H3>  

<H1 ALIGN =CENTER> Create IPAddressKind Enum and IPAddress Structure in Rust </H1>  

## AIM:  
To create an enum IPAddressKind in Rust that represents IPv4 and IPv6 addresses, define a struct IPAddress with IPAddressKind as a member, and use it in a Rust application.  

## EQUIPMENTS REQUIRED:  
- Hardware – PCs  
- Software – Visual Studio Code (Version 1.104.0)  
- Rust Installation  

## RELATED THEORETICAL CONCEPT:  

*Enums in Rust:*  
Enums allow defining a type by enumerating its possible values (variants). For example, `IPAddressKind` can be either `IPv4` or `IPv6`.  

*Structs with Enums:*  
A struct can include an enum as a field, combining descriptive data with categorization.  

*Need for Enum + Struct:*  
- Better organization of related data.  
- Clean representation of IP address types.  
- Provides clear method-based operations.  

## ALGORITHM:  
STEP 1: Define an enum **IPAddressKind** with variants `IPv4` and `IPv6`. <BR>  
STEP 2: Define a struct **IPAddress** with two fields:  
- `kind: IPAddressKind`  
- `address: String` <BR>  
STEP 3: Implement a `display` method to print details of the IP address. <BR>  
STEP 4: In the `main` function:  
- Create IPv4 and IPv6 instances.  
- Call the `display` method on them.  

## PROGRAM:  
```

//Type Your Code


```
## OUTPUT:


## RESULT:
