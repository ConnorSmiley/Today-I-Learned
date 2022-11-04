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

-`TACACS+` = Terminal Access Controller Access Control System (auth, authenticate, accounting) // Cisco

-`RADIUS` = Remote Authentication Dial-In User Service 

-`Kerberos` = network authentication protocol design // windows

-`Challenge-Handshake Authentication Protocol` = Authenticate user



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

-`MFA` = Multi Factor Authentication

-`UEFI` = Unified Extensible Firmware Interface (replaces BIOS)

-`SAE` = Simulation Authentication Equals

-`x.509` = cert for SSL/TLS



__Remote Desktop Protocol__

-`RDP` = Remote Desktop Protocol

-`VNC` = Virtual Network Computing

-`SSH` = Secure Shell

-`MSP` = Managed Service Provider

-`RMM` = Remote Monitor Management

-`MSRA` = Microsoft Remote Assistance

-`VNC` = Virtual network computing // screen share Mac and Linux

-`RDP` = Remote Desktop Protocol 

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

-`0.0.0.0 - 126.255.255.255` = Class A (public)

-`10.0.0.0 - 10.255.255.255` = Class A (private)

-`10.189.1.0` = Class A (private) example

-`123.15.1.0` = Class A (public) example

-`127.0.0.1` = Loopback

-`128.0.0.0 - 191.255.255.255` = Class B (public)

-`129.50.6.1` = Class B (public) example

-`169.254.1.1` = APIPA2

-`169.254.30.21` = APIPA

-`172.16.0.0 - 172.31.255.255` = Class B (private)

-`172.30.5.12` = Class B (private) example

-`192.0.0.0 - 223.255.255.255` = Class C (public)

-`192.15.1.0` = Class C (public) example

-`192.168.15.2/32` = Class C (private, CIDR format)

-`192.168.0.0 - 192.168.255.255` = Class C (private)

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

-`802.11q` = 



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


__Link Aggregation__
IEEE 802.3ad = combines multiple connections to one connection


__POE__
802.3af = 15.4 watts
802.1x =


__POE+__
802.at = 25.5 watts


__Spanning Tree Protocol__
802.1d = prevents switching loops


__Osi Model___
7. Application layer
6. Presentation layer
5. Session layer
4. Transport layer
3. Network layer
2. Data link layer
1. Physical layer


__VLAN__
-`802.1af` - Power over ethernet
-`802.1d` - spanning tree protocol
-`802.1x` - Network authentication protocol
-`802.1q` - Multi switches for communication


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

-`802.3d` - Spanning Tree Protocol

-`802.3x` - Network Authentication Protocol / Radius



__Protocols__

-`ARP` - Local Address Resolution Protocol

-`RTP` - Real-time Transport Protocol ?

-`NTP` -  Network Time Protocol / Interior

-`STP` - Spanning Tree Protocol / Interior

-`BGP` - Border Gateway Protocol / autonomous systems/ Exterior

-`RIP` - Routing Information Protocol / Interior Gateway Protocol / Autonomous System (AS)

-`EIGRP` - Enhanced Interior Gateway Routing Protocol / Exterior

-`OSPF` - Open Shortest Path First / Interior

-`RIPv2` - classless, distance vector routing protocol that will include the subnet mask with the network addresses 


__APIPA__

-`169.254.0.1 - 169.254.255.254` - Range

-`169.254.1.0 - 169.254.254.255` - Range


__Private IP__

-`10.0.0.0 - 10.255.255.255` - Range

-`172.16.0.0 - 172.31.255.255` - Range

-`192.168.0.0 - 192.168.255.255` - Range


__Ports__

-`20, 21` = File Transfer Protocol. Not secure

-`22` = SSH FTP, encrypted and uses firewall // SSH, SCP, SFTP

-`23` = Telnet, unsecure

-`25` = Simple Mail Transfer protocol, only for sending

-`53` = DNS

-`67, 68` = DHCP uses UDP ports // Dynamic hosting protocol

-`80` = HTTP

-`110` = POP3 (post office protocol 3)

-`139` = Server Message Block

-`143` = Internet Message Access Protocol

-`161` = Simple Network Management Protocol. Managing Network Connected Devices

-`162` = SNMP // Simple Network Management Protocol

-`389` = Lightweight Directory Access Protocol // LDAP

-`443` = SSH

-`445` = Server Message Block Protocol // Client Server Communication

-`636` = LDAP-ssh

-`990` = FTPS. Secure

-`993` = IMAP-ssh

-`995` = POP3-ssh

-`1433` = Microsoft SQL

-`1521` = SQLnet

-`1812` = RADIUS (authentication)

-`3306` = MySQL

-`3389` = RDP (remote desktop protocol)

-`5060 / 5061` = Session Initiation Protocol


Classful vs Classless ipv4 ??


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



























































