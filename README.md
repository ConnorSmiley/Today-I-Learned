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


__Documents__

-`Scope` = defines area, number, size or scale of change

-`Purpose` = defines why the change/installation will occur

-`Risk analysis` = Provides risk levels or why a change is needed

-`Plan` = How the change will occur. (Who, what when, where why and how)



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

-`990` = FTPS. Secure

-`1812` = RADIUS (authentication)

-`3389` = RDP (remote desktop protocol)



__Protocols__

-`TACACS+` = Terminal Access Controller Access Control System (auth, authenticate, accounting)

-`RADIUS` = Remote Authentication Dial-In User Service

-`Kerberos` = network authentication protocol design // windows

-`Challenge-Handshake Authentication Protocol` = Authenticate user


__Phone__

-`PRI` = Preferred Roaming Index

-`PRL` = Preferred Roaming List



__Words__

-`PXE` = Preboot eXecution environment. Allows remote workstation to boot remote

-`UPnP` = Universal plugin and play

-`MDM` = mobile device management

-`DHCP` = protocol for IP address

-`NAT` = network service provider

-`MMC` = microsoft management console. Performance operations panel

-`RDS` = remote desktop services

-`UAC` = user account control. Prevent unauthorized installs

-`PerfMon` = Performance monitoring

-`COPE` = Company Owned/personally enabled

-`CYOD` = Choose your own device

-`BSOD` = Blue screen of death

-`POST` = Power on self test

-`MSDS` = Material Safety Data Sheet

-`SOP` = Standard Operating Proceedure

-`SOW` = statement of work

-`MSDS` = material safety data sheet

-`TPM` = Trust Platform Module

-`PAM` = Pluggable Authentication Module

-`FDE` = Full disk encrypt

-`AES` = Advance Encryption System





__Malware Removal Steps__


1. Investigate and verify malware symptoms

2. Quarantine the infected systems

3. Disable System Restore in Windows

4. Remediate the infected systems, update anti-malware software, scan the system, and use removal techniques (e.g., safe mode, pre-installation environment)

5. Schedule scans and run updates

6. Enable System Restore and create a restore point in Windows

7. Educate the end user



__Install__

-`Clean` = Fresh install

-`Upgrade` = Overwrite current OS

-`Unattended` = Large Company??

-`Repair` = Repair OS, can change default settings

-`In place Install` = Overwrite current OS

-`Refresh` = re-installs OS




__Backups__

-`grandfather-father-son` = grandfather/monthly, father/weekly, son/daily

-`3-2-1` = 3) primary backup & 2 copies. 2)save back to 2 different media. 1) one backup off-site

-`Tower of Hanoi` = rotates backups to prevent wear

-`FIFO Backup` = First in, first out. Overwrites the oldest drive

-`Synthetic backup` = Merging past and earlier parts to create a backup

-`Differential backup` = Uses last modified and adds to last modified. Then merges with full backup

-`Incremental backup` = Makes new backup after every change, then adds many backups to the full backup


__Scripts__

-`.bat` = Batch files
-Windows file systems

-`.ps1` = Windows powershell files
-Windows file systems

-`cmdlets` = command-lets

-`.vbs` = Visual basic. Used for administrative tasks
-Windows file systems

-`.js` = javascript

-`.py` = python

-`.sh` = shell. Scripts for automating tasks
-Unix/Linux




__Partitions__

-`Primary Partitions` = Only 4 with MBR

-`Extended Partitions` = Only 4 with MBR

-`Swap Partitions` = Linux, can add extra V-memory if needed

-`Logical Partitions` = Can add to Extended Part to make 23



__IP Addresses__

-`10.0.0.0 - 10.255.255.255` = Class A private IP's

-`127.0.0.1` = Loopback for IPv4 //Local-host

-`172.16.0.0 - 172.31.255.255` = Class B private

-`192.168.0.0 - 192.168.255.255` = Class C private

-`169.254.0.0 - 169.254.255.255` = Automatic Private IP Addressing/link-local


__802.11__

-`a` =
-`b` =
-`g` =
-`n (WiFi 4)` =
-`ac (WiFi 5)` =
-`ax (WiFi 6)` =


__File Systems__

-`Fat32` = 32-bit file support for Windows, Mac and Linux

-`exFAT` = Both Mac and Microsoft supported

-`UDF` = Universal Disk Format

-`NTFS` = Windows 64-bit address space 

-`CDFS` = CD File System


__Network Attacks__

-`Whaling` = Targeting high profile figures

-`Spear Fishing` = Targets specific groups

-`Vishing` = Voice and Fishing

-`XSS` = Cross Site Scripting

-`CSRF` = Cross Site Request Forgery. User performs actions

-`Root Kit` = Controls computer without detection



__Wireless Encryption__

-`WPA2` = CCMP and CBC-MAC (Counter mode with cipher block chaining / Counter CBC-MAC protocol)

-`WPA3` = GCMP, GMAC and SAE (Galois/Counter Mode Protocol)
–Includes mutual authentication
–Creates a shared session key without sending key across network
–No more four-way handshakes, no hashes, no brute force attacks
–Adds perfect forward secrecy

-`AES` = Advance Encryption Standard

-`PSK` = Pre Shared Keys

-`SAE` = Simultaneous Authentication of Equals
-Diffie-Hellman derived key exchange
– Everyone uses different session keys, even with same PSK
– An IEEE standard - the dragonfly handshake


__Network Security__

-`On Path Network Attack` = aka Man in the middle

-`SOE` = Standard Operation Environment




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



__Distribution Denial of Service__

-`UEFI` = Unified Extensible Firmware Interface (replaces BIOS)


__Windows Boot Errors__

-`bootrec /rebuildbcd` = BCD / Boot Configuration Database. Add missing files

-`bootrec /fixboot` = fix boot sector

-`bootrec /fixmbr` = fix master boot sector

-`SFC` = System File Checker
-/scannow = begins system scan



__Privacy & Licenses__

-`PCI DSS` = Payment Card Industry Data Security Standard

-`PII` = Personally Identifiable Information

-`GDPR` = General Data Protection Regulation
-EU protection

-`PHI` = Protected Health Information

-`IP` = Intellectual property

-`CUI` = Controlled Unclassified Information

-`HIPAA` = Health Insurance Portability and Accountability of 1996  



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


__Beeps__

-`1 long beep, 1 short beep` = Bad Motherboard

-`1 long beep, 3 short beep` = Video CGA Display

-`1 long beep, 2 short beep` = Video EGA Display

-`No Beep` = Power supply

-`1 long beep, 8 short beep` = Bad Video Card

-`7 short beeps` = Bad Cpu

-`1 short beeps` = POST passed

-`3 short beeps` = Bad Ram

-`3 long beeps` = Bad Keyboard



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



__Comptia Troubleshooting__

-Identify the problem

-Establish a theory on probable cause

-Test theory

-Create plan of action to resolve the problem

-Verify and implement preventative measures

-Document findings



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



__Ethernet Cables__

-`T568A` = 

-`T568B` =



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



























































