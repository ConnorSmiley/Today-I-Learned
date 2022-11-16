# Today I Learned
> A library of my TIL

---

-[Cookies](#Cookies)

-[Chrome](#Chrome)

-[CSS](#CSS)

-[Dev-Tools](#Dev-Tools)

-[JavaScript](#JavaScript)

-[GitHub](#GitHub)

-[Iterm](#Iterm)

-[Linux-Commands](#Linux-Commands)

-[Linux-Features](#Linux-Features)

-[LocalStorage](#LocalStorage)

-[Mac](#Mac)

-[Markdown](#Markdown)

-[Network](#Network)

-[Cidr-Block-Notation](#Cidr-Block-Notation)

-[Nextjs](#Nextjs)

-[Postgresql](#Postgresql)

-[Premiere](#Premiere)

-[React](#React)

-[React-StyleComponents](#React-StyleComponents)

-[Redux](#Redux)

-[ReduxToolKid](#ReduxToolKit)

-[Security](#Security)

-[Sublime-Text](#Sublime-Text)

-[TailWindCSS](#TailWindCSS)

-[ThinkScript](#ThinkScript)

-[Icons](#Icons)

-[Vim](#Vim)

-[Volta](#Volta)

-[WindowsCommands](#WindowsCommands)

-[ShortCutUpdates](#ShortCutUpdates)


***

>## CSS

__User Select None__
```css
user-select: auto|none|text|all;
```


>## Cookies


>## Chrome
__Disable Google Helper__  
-`chrome://settings/content/unsandboxedPlugins`


>## Dev-Tools
__Copy & Paste__
```javascript
copy(Array.from(document.querySelectorAll('.DIVNAME li a')).map(x => x.innerText))
```

>## JavaScript
__KeyboardEvent.code vs keydown__  
-Represents a physical key on a keyboard vs the UTF-8 generated
```javascript
KeyboardEvent.code vs

useEffect(() => {
    document.addEventListener("keydown", handleKeyboard)

return () => {
     document.removeEventListener("keydown", handleKeybaord)
}
 }, [handleKeyboard])
```

__Looping Backwards is faster__
Only by a margin


__New Date__
```javascript
{new Date(props.prop).toLocaleTimeString({hour: "numeric", minute: "numeric"})}
```

__Set Interval__
```javascript
setInterval(() => {setState(prev => prev), 1000})
```

>## GitHub
__Line Break__  
-`Double Spaces for line break`  
-`</br>`
<br>
</br>
### Branches

__Create new branch__  
-`git checkout [BRANCH]`  

__List all branches__  
-`git branch -a`  

__Delete branch__  
-`git branch -d [BRANCH]`  

__Create and move to branch__  
-`git checkout -b [BRANCH]`  

__Abort Merge__    
-`git merge --abort`


>## Iterm
__Clear History__  
-`rm $HISTFILE`


>## Linux-Commands

[Link to Linux Commands](Linux-Commands/comptia-a+/linux-commands.md)


>## Linux-Features
 
[Link to Linux Features](Linux-Features/Linus-Features.md)


>## LocalStorage


>## Mac
__SMC__  
-`shift + ctrl + option + power`

__PRAM__  
-`cmd + option + r + p`

__Disable Mac Chime__  
-`sudo nvram StartupMute=%01`

__Quit Finder__  
-`defaults write com.apple.finder` <br>
-`QuitMenuItem -bool true;`     
-`killall Finder`

>## Markdown
__Line Break__  
-`&nbsp;`


>## Network 
__Acronym_

[`Comptia A+ acronyms`](Comptia-a-plus-acronym/acronyms.md)











__Protocols__

-`SNMP` - Simple Network Management Protocol
-Port 161
-SNMP Traps sends error messages - Port 162


__Protocols__

-`SysLog` - Needs lots of storage


__Protocols__

-`ARP` - Local Address Resolution Protocol
-`RTP` - Real-Time Transport Protocol ?
-`NTP` -  Network Time Protocol / Interior
-`STP` - Spanning Tree Protocol / Interior
-`TCP` - Transmission Control Protocol
-`UDP` - User Diagram Protocol
-`BGP` - Border Gateway Protocol / autonomous systems/ Exterior
-`RIP` - Routing Information Protocol / Interior Gateway Protocol / Autonomous System (AS)
-`EIGRP` - Enhanced Interior Gateway Routing Protocol / Exterior
-`OSPF` - Open Shortest Path First / Interior
-`RIPv2` - classless, distance vector routing protocol that will include the subnet mask with the network addresses
-`LACP` - Link Aggregation Control Protocol. Will increase bandwidth between switches
-`NS` - Neighbor Solicitation
-IPv6 instead of IPv4 w/ ARP


__VLAN Protocols__

-`GRE` - Generic Routing Encapsulation // IPsec uses 1-1 or 1-multiple
-`PPTP` - Point to Point Tunneling Protocol 
-VPN but not secure until Microsoft added GRE
-`TLS` - Transport Layer Security


__MPLS Multiprotocol Label Switching__

-`TLS` - Transport Layer Security
-Any connection and any protocol
-Uses labels


__NDP (Neighbor Discovery Protocol)__
-Replaces IPv4 & ARP
-Uses ICMPv6

-`SLAAC` - Stateless Address Autoconfiguration
-Auto assigns IP address w/o DHCP 
-DAD (Duplicate Address Detection) is needed to prevent duplicates

-`RS` - Router Solicitation => Send

-`RA` - Router Advertisement <= Receive


__Authentication Methods__

-`TACACS+` = Terminal Access Controller Access Control System (auth, authenticate, accounting) // Cisco
-`RADIUS` = Remote Authentication Dial-In User Service 
-`Kerberos` = network authentication protocol design // windows
-`Challenge-Handshake Authentication Protocol` = Authenticate user


__Tunneling Methods__

-`Teredo` = IPv6 => IPv4 // Windows
-`Miredo` = IPv6 => IPv4 // Linus Mac OSX
-`Dual Stack Routing` = IPv6 & IPv4 


__Phone__

-`PRI` = Preferred Roaming Index
-`PRL` = Preferred Roaming List


__IP Addresses__

-`10.0.0.0 - 10.255.255.255` = Class A private IP's
-`127.0.0.1` = Loopback for IPv4 //Local-host
-`172.16.0.0 - 172.31.255.255` = Class B private
-`192.168.0.0 - 192.168.255.255` = Class C private
-`169.254.0.0 - 169.254.255.255` = Automatic Private IP Addressing/link-local


__802.11__

-`a` = 5ghz
-`b` = 2.4ghz
-`g` = 2.4ghz
-`n (WiFi 4)` =
-`ac (WiFi 5)` = 2.4/5ghz
-`ax (WiFi 6)` =


__Authentication Methods__

-`RADIUS` = Remote Authentication Dial-In Service
-`TACACS` = Terminal Access Controller Access-Control System
-Common with CISCO
-`KERBEROS` = Network Auth Protocol
-Common with windows
-`SSO` = Single Sign On
-`MFA` = Multi-Factor Authentication
-`UEFI` = Unified Extensible Firmware Interface (replaces BIOS)
-`SAE` = Simulation Authentication Equals
-`x.509` = cert for SSL/TLS


__Remote Desktop Protocol__

-`RDP` = Remote Desktop Protocol
-`MSP` = Managed Service Provider
-`RMM` = Remote Monitor Management
-`MSRA` = Microsoft Remote Assistance
-`TelNet` = Teletype Network. Clear text, no encrypt


__Wifi Protocol__

-`WEP` = Wired Equivalent Privacy // Old
-`WPA` = used for WLAN
-`WPA2` = Microsoft Remote Assistance
-`WPA3` = Uses preshared keys
-`WINS` = Windows Internet Name Service


__Documentation__

-`Knowledge based articals` = KB


__IP Addresses__

-`10.0.0.0 - 10.255.255.255` = Class A (private)
-`172.16.0.0 - 172.31.255.255` = Class B (private)
-`192.168.0.0 - 192.168.255.255` = Class C (private)

-`0.0.0.0 - 126.255.255.255` = Class A (public)
-`123.15.1.0` = Class A (public) example

-`127.0.0.1` = Loopback

-`128.0.0.0 - 191.255.255.255` = Class B (public)
-`129.50.6.1` = Class B (public) example

-`169.254.1.1` = APIPA2
-`169.254.30.21` = APIPA

-`192.0.0.0 - 223.255.255.255` = Class C (public)
-`192.15.1.0` = Class C (public) example

-`240.0.0.0 - 254.255.255.255` = Class E (public, reserved)
-`224.0.0.0 - 239.255.255` = Class D (public, multicast)

-`fe80::/10` = Link Unique Local Unicast
-`::1/128` = Loopback6
-`2000::/3` = Global Unicast
-`fc00::/7` = Unique Local Unicast
-`ff00::/8` = Multicast


__Cables__

-`802.3af` = POE // 15.4 w over 100m
-`802.3at` = POE // 25w over 100m
-`802.11s` = wireless
-`802.11ac` = 2.4ghz // 3.4 gbps
-`802.11ax` = 2.4ghz // 5ghz


__Wifi__

-`802.11a` = 5 ghz - 54 mbit/s | 54 mbit/s | 20 MHz
-`802.11b` = 2.4 ghz - 11 mbit/s | 11 mbit/s | 24 MHz
-`802.11g` = 2.4 ghz - 54 mbit/s | 54 mbit/s | 20 MHz
-`802.11n` = 5 / 2.4 ghz - 4xMIMO 150 mbit/s | 600 mbit/s | 20, 40, 80 MHz
-`802.11ac` = 5 ghz - 8x DL MU-MIMO 867 mbit/s | 6.9 gbit/s | 20, 40, 80+80, 160 MHz
-`802.11ax` = 5 / 2.4 ghz - 8x DL & UL MU-MIMO 1,201 mbit/s | 9.6 gbit/s | OFDMA
-`802.11q` = Standard protocol for trunking


__Ethernet Cables__

-`T568A` = 
-green/white
-green
-orange/white
-blue
-blue/white
-orange
-brown/white
-brown

-`T568B` =
-orange/white
-orange
-green/white
-blue
-blue/white
-green
-brown/white
-brown


__Ethernet__

-`WDM` = Wavelength Division Multiplexing
-`CWDM` = Course Wavelength Division Multiplexing
-`DWDM` = Dense Wavelength Division Multiplexing


__Link Aggregation__
IEEE 802.3ad = combines multiple connections to one connection


__POE__
802.3af = 15.4 watts
802.1x =


__POE+__
802.at = 25.5 watts


__Spanning Tree Protocol__
802.1d = prevents switching loops


__Osi Model__

7. Application layer
-Protocols and Requests

6. Presentation layer
-Encrypting between Networks
-Application Encryption
-SSL // TLS

5. Session layer
-Setups communication channel
-Protocols

4. Transport layer
-TCP / UDP
-Sends packets of information

3. Network layer
-IPsec // Authentic Header (AH) // Encapsulating Security Payload (ESP)
-Routers
-Packets
-ICMP
-Multi-Layer Switch
-Internet Protocol
-IP address
-IPsec

2. Data link layer
-Switches & Bridges
-WAP (Wireless Access Points)
-Sending / Receiving
-NIC for MAC
-MAC
-Ethernet

1. Physical layer
-Physical and Cables
-Modem & Hubs
-Punchdown
-Media Converter


__Encapsulation / Decapsulation__

-Layer 5,6,7 = Application Data
-Layer 4 = TCP // Application Data
-Layer 3 = IP Header // TCP // Application Data
-Layer 2 = Frame Header // IP Header // TCP // Application Data // Frame Header


__TCP Flags__

-`SYN` - Synchronize sequence numbers
-`PSH` - Push data to app w/o buffer
-`RST` - Reset Connection
-`FIN` - Last Packet from sender


__vLAN__
-`802.1af` - Power over ethernet
-`802.1d` - spanning tree protocol
-`802.1x` - Network authentication protocol
-`802.1q` - Multi switches for communication

-`NFV` - Network Function Virtualization
-Virtual Servers


__Severity Level Range__

-`0` - Emergency
-`1` - Immediately
-`2` - Critical Condition
-`3` - Error Condition
-`4` - Warning Conditions
-`5` - Unusual Conditions
-`6` - Normal Operating Conditions
-`7` - Debugging


__IEEE Standard__

-`802.3ad` - Link Aggregation Control Protocol
-`802.3af` - POE
-`802.3at` - POE
-`802.3d` - Spanning Tree Protocol
-`802.3x` - Network Authentication Protocol / Radius


__APIPA__

-`169.254.0.1 - 169.254.255.254` - Range
-`169.254.1.0 - 169.254.254.255` - Range


__Private IP__

-`10.0.0.0 - 10.255.255.255` - Range
-`172.16.0.0 - 172.31.255.255` - Range
-`192.168.0.0 - 192.168.255.255` - Range


__Internet Protocol Security__

-`IPsec` = Layer 3 OSI
-`AH` = Authentication Protocol
-Sends Hash Packets for Security
-`ESP` = Encapsulation Security Payload
-Encrypts packets


__Ports__

-`20, 21` = File Transfer Protocol. Not secure
-`22` = SSH FTP, encrypted and uses firewall // SSH, SCP, SFTP
-`23` = Telnet, unsecure
-`25` = Simple Mail Transfer protocol, only for sending
-`53` = DNS
-`67, 68` = DHCP uses UDP ports // Dynamic hosting protocol
-`80` = HTTP
-`110` = POP3 (post office protocol 3)
-`123` = NTP (Network Time Protocol)
-`139` = SMB // Server Message Block
-`143` = Internet Message Access Protocol
-`161` = SNMP // Simple Network Management Protocol. Managing Network Connected Devices
-`162` = SNMP // Simple Network Management Protocol
-`389` = LDAP // Lightweight Directory Access Protocol
-`443` = SSH
-`445` = SMB // Server Message Block // Client Server Communication
-`514` = SysLog
-`636` = LDAP-ssh
-`990` = FTPS. Secure
-`993` = IMAP-ssh
-`995` = POP3-ssh
-`1433` = Microsoft SQL
-`1521` = SQLnet
-`1812` = RADIUS (authentication)
-`3306` = MySQL
-`3389` = RDP (remote desktop protocol)
-`5060 / 5061` = Session Initiation Protocol // VoIP


__WLAN Concepts__

-`IBSS` = Independent Basic Service Set 
-`BSS` = Basic Service Set
-`ESS` = Extended Service Set


__SD-WAN__

-`SD WAN` = Software Defined Network
-Built in the cloud


__Encryption Basics__

-`PSK` = Pre-Shared key
-`PKI` = Public Key Infrastructure
-`Kerberos` = Uses TCP & UDP - port 88
-Key Distribution Center as main component
-Has two parts - AS (authentication Server) & TGS (Ticket Granting Service)


__Encryption Basics__

-`SSID` = Service Set Identifier


_CSMA_

-`CSMA/CD` = Carrier Sense Multiple Access w/ Collision Detection
-Better for high speed and throughput networks // 802.3

-`CSMA/CA` = Carrier Sense Multiple Access w/ Collision Avoidance 
-Uses RST (request to send) packets
-If RST is clear, then a (CTS) clear to send packet is sent
-Better for lower speeds and lower throughput
-Not used if higher chance of data collision
-OFDM = Multi carrier signal channels // prevents lose of attenuation 
-DSSS = Spread spectrum tech


__Documents__

-`MOU` = Memorandum of Understanding
-`SOW` = Statement of work
-`MLA` = Master Licenses agreement
-`SLA` = Service Level Agreement


_DNS Records_

-`A` = IPv4 address
-`AAAA` = IPv6 address
-`CNAME` = Name Alias
-`PTR` = Points to CNAME
-`MX` = Maps email server to specific domain


__Network Address Translation__

-`SNAT` = Static NAT
-`DNAT` = Dynamic NAT
-`PAT` = Public Address Translation
-Increase scalability of NAT 
-Adds a port number to the end of IP address


__Public Switch Telephone Network__

-`PSTN` = Public Switch Telephone Network
-Telephone line
-`ISDN` = Integrated Service Digital Network
-`BRI` = Basic Rate Interface // B channel & D channel
-Alternative to DSL but not better


1 | 2 | 4 | 8 | 16 | 32 | 64 | 128 | 256
256 | 128 | 64 | 32 | 16 | 8 | 4 | 2 |1
24 | 25 | 26 | 27 | 28 | 29 | 30 | 31 | 32

128 | 64 | 32 | 16 | 8 | 4 | 2 | 1
















>## Cidr Block Notation

[Cidr-Block-Notation](cird/cird.md)


>## Nextjs
__Install TW__  
-`npm install -D tailwindcss postcss autoprefixer`  
-`npx tailwindcss init -p`


>## Postgresql
__Start / Stop server__  
-`brew services start postgresql`  
-`brew services stop postgresql`

>## Premiere
__Show Timeline__  
-` \ `


>## React
__Slice and Map__
```javascript
array = []

{array.slice(startIndex: number, endIndex: number).map(x => {
 return <Component>{x}</Component>
})}
```


__KeyStroke Text__
```javascript
    const [text, setText] = useState("")

    function handleChange(e) {
        const {value} = e.target
        setText(value)
    }

return (
         <div 
                 onChange={handleChange}
                 value={text}
         />
```

__Count Words__
```javascript
const [text, setText] = useState("")

function handleChange(e) {
 const {value} = e.target
 setText(value)
}

function calculateWordCount(text) {
 const wordsArr = text.trim().split(" ")
 const filteredWords = wordsArr.filter(word => word !== "")
 return filteredWords.length
}
    
    return (
        <div>
         <TextBox
                 onChange={handleChange}
                 value={text}
         />
         <button onClick={()=> calculateWordCount(text)} />
         </div>
    )

```

__Timer == setTimeRemaining__
```javascript
const [timeRemaining, setTimeRemaining] = useState(5)


    useEffect(() => {
 setTimeout(() => {
  if (timeRemaining === 0) return
  setTimeRemaining(time => time - 1)
 }, 1000)
}, [timeRemaining])

or

useEffect(() => {
 if(timeRemaining > 0) {
  setTimeout(() => {
   setTimeRemaining(time => time - 1)
  }, 1000)
 }
}, [timeRemaining])
```

__UseEffect Return__
```javascript
    useEffect(() => {
 const intervalId = setInterval(() => {
  setCount(prevCount => prevCount + 1)
 }, 1000)
 setColor(randomcolor())
 return () => clearInterval(intervalId)
}, [count])
```
__Button Disable__
```javascript
const [timeRunning, setTimeRunning] = useState(5)

        return(
<Button 
    disable={timeRunning}/>)
```


_Disable Input_
```javascript
<button disabled={!text}>CLICK</button>

```

>## React-StyleComponents
__Passing Props__  
-`${props => props.NAME ? NAME : NAME}`  

>## Redux  

```javascript

import { createSlice } from '@reduxjs/toolkit'

const initialState = [{

}]

export const $VAR$ = createSlice({
 name: '',
 initialState,
 reducers: {

 },
})

export const ??? = (state) => state.???
export const {} = $VAR$.actions
export default $VAR$.reducer
```


>## Security
 
`ACL` - Access Control List 



>## Sublime-Text
__Alias File__    
-`/Users/UserName/.zshrc`  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•Primary Mac?

>## TailWindCss  
__Center Absolute__  
-`inset-x-0`

__Render Conditions__
```javascript
const handleTail = (small ? "bg-black" : med ? "bg-white" : large ? "bg-red-500" : "bg-green-500")

<div className={handleTail}>Blah</div>
```

>## ThinkScript
__Input Toggle Switching__
```javascript
def VARIABLE_NAME;
    switch (mode) {
    case VARIABLE_NAME:
        something = define logic;

    case VARIABLE_NAME:
        something = define logic;
}
```

>## Vim
__Save and Write__  
-`:q` close      
-`:w`        write/saves   
-`:wa[!]`   write/save all windows [force]  
-`:x`        save and quit, same as wq  
-`:q!`      force close's non-saved files with changes

>## Volta
__Steps to Enable__  
-`⌘+R turn on your Mac`  
-`csrutil enable --without kext`  
-`csrutil disable`


>## WindowsCommands
 
__Navigation__

`cd` = change directory

`dir` = list current dir (similar to ls)

`md` = make dir

`mkdir` = make dir

`chdir` = change dir

`rd` = remove dir

`rmdir` = remove dir

`cls` = clear screen


__Command Line Tools__


`[command name] /?` = Show help command (similar to man)
`help` = help

`chkdsk` = check for disk errors
-`/f` = fixes logical file system errors on disk
-`/r` = locates bad sectors and recovers readable information

`format` = format drive

`xcopy` = copies full directory and files
-`/s` = & copies sub-directories

`copy` = copy `file-name` `rename-copy-file`
-`/v` = verifies that new files are written correctly
-`/y` = suppresses prompt to confirm over-write file message

`robocopy` = more robust copy method to xcopy

`gpupdate` = updates group policy
-`/force` = everything is updated

`gpresult` = shows current group policy update
-`/r` = shows all current active dir policy settings

`shutdown` = shutdown computer
-`/s /t nn` = shutdown timer
-`/r /t nn` = restart timer
-`/a` = abort shutdown

`sfc` = checks and repairs windows system files
-`/scannow` = checks disk

`diskpart` = makes disk partitions

`winver` = shows which version


__Network Command Line Tools__

`ipconfig` = displays TCP/IP, DHCP and DNS
-`/all` = more details on ipconfig

`ping` = Verifies connection with ICMP request.

`pathping` = show path route and network information / tracert + ping

`hostname` = Displays host name

`netstat` = Displays TCP connections, ports, Ethernet, IP routing table, IPv4 and IPv6 stats
-`/a` = show all active connection
-`/b` = show all binaries
-`/n` = do no resolve names

`nslookup` = Name server lookup

`net` = used to connect to, remove, and configure connections with shared resources

`net user` = shows user privileges

`net use` = shows network connections

`tracert` = Determine package route to destination

`nslookup` = look up DNS, names and IP



>## ShortCutUpdates
__Arrow__
ar
`= () => {
$End$
}`


---

## Icons
➕❌💥✨❓❕🚫✖️➖&nbsp;
























































