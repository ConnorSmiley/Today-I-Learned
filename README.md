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


__Names__

-`Subnet` = File Transfer Protocol. Not secure


__Documents__

-`Scope` = defines area, number, size or scale of change

-`Purpose` = defines why the change/installation will occur

-`Risk analysis` = Provides risk levels or why a change is needed

-`Plan` = How the change will occur. (Who, what when, where why and how)



__Ports__


-`21` = File Transfer Protocol. Not secure

-`22` = Secure FTP, encrypted and uses firewall // SSH, SCP, SFTP

-`23` = Secure FTP, acts like TelNet

-`25` = Simple Mail Transfer protocol

-`53` = DNS

-`67, 68` = DHCP uses UDP ports

-`110` = POP3 (post office protocol 3)

-`139` = Server Message Block

-`143` = Internet Message Access Protocol

-`161` = Simple Network Management Protocol. Managing Network Connected Devices

-`389` = Lightweight Directory Access Protocol // LDAP

-`445` = Server Message Block Protocol // Client Server Communication 

-`990` = FTPS. Secure

-`1812` = RADIUS (authentication)

-`3389` = RDP (remote desktop protocol)



__Protocols__

-`TACACS+` = Terminal Access Controller Access Control System (auth, authenticate, accounting)

-`RADIUS` = Remote Authentication Dial-In User Service

-`Kerberos` = network authentication protocol design

-`Challenge-Handshake Authentication Protocol` = Authenticate user


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

-`Swap Partitions` = Linux, can add extra Vmemory if needed

-`Logical Partitions` = Can add to Extended Part to make 23



__IP Addresses__

-`10.0.0.0 - 10.255.255.255` = Class A private IP's

-`172.16.0.0 - 172.31.255.255` = Class B private

-`192.168.0.0 - 192.168.255.255` = Class C private

-`169.254.0.0 - 169.254.255.255` = APIPA/link-local



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

-`PII` = Personal Identification Information

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



