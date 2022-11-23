# Today I Learned
> A library of my TIL

---

-[A-plus](#A-plus)

-[AWS](#AWS)

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

-[Homelab](#Homelab)

-[Mac](#Mac)

-[Markdown](#Markdown)

-[Cidr-Block-Notation](#Cidr-Block-Notation)

-[Nextjs](#Nextjs)

-[Network-plus](#Network-plus)

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

-[WindowsServer](#WindowsServer)

-[ShortCutUpdates](#ShortCutUpdates)




***


>## A-plus
__Acronym__

[A+ Notes](Comptia-a-plus-acronym/acronyms.md)


>## AWS
__AWS Notes__

[AWS](Aws/Aws.md)


>## Azure
__Azure Notes__

[Azure](Azure/Azure.md)


>## CSS

[CSS](CSS/CSS.md)


>## JavaScript

[JavaScript](JavaScript/JavaScript.md)


>## GitHub

[Github](Github/Github.md)

>## Iterm
__Clear History__  
-`rm $HISTFILE`


>## Linux-Commands

[Link to Linux Commands](Linux-Commands/comptia-a+/linux-commands.md)


>## Linux-Features
 
[Link to Linux Features](Linux-Features/Linus-Features.md)


>## LocalStorage

>## LocalStorage
__Notes for HomeLab__

[HomeLab](Homelab/Homelab.md)


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




>## Network-plus
__Click Below for Notes__

[Network+ Notes](Network+/Network+.md)


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

__React Options Chaining__
```javascript

console.log(maybeNo.Object?)

```


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


>## WindowsCommands
 
__Windows Server__
net user Administrator /passwordreq:yes *


>## ShortCutUpdates
__Arrow__
ar
`= () => {
$End$
}`


---

## Icons
➕❌💥✨❓❕🚫✖️➖&nbsp;
