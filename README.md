## Experiment 5 - Create IPAddress Kind enum to represent IPv4, IPv6 addresses and create IP Address structure with IP Address Kind as a member and use this structure in the application.

<H3>NAME: Santhosh G</H3>  
<H3>REGISTER NO: 212223240152</H3>  
 
<H3>DATE: 30/10/2025</H3>  


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
// Rust program to demonstrate Enum and Struct for IPAddress

enum IPAddressKind {
    IPv4,
    IPv6,
}

struct IPAddress {
    kind: IPAddressKind,
    address: String,
}

impl IPAddress {
    fn display(&self) {
        match self.kind {
            IPAddressKind::IPv4 => println!("IPv4 Address: {}", self.address),
            IPAddressKind::IPv6 => println!("IPv6 Address: {}", self.address),
        }
    }
}

fn main() {
    let home = IPAddress {
        kind: IPAddressKind::IPv4,
        address: String::from("192.168.1.1"),
    };

    let loopback = IPAddress {
        kind: IPAddressKind::IPv6,
        address: String::from("::1"),
    };

    home.display();
    loopback.display();
}

```
## OUTPUT:
<img width="1502" height="1031" alt="image" src="https://github.com/user-attachments/assets/1fc8c30e-4949-4917-ba60-995c85e0a810" />


## RESULT:
Thus, the Rust program for creating an Enum IPAddressKind and a Struct IPAddress was successfully implemented and executed.
