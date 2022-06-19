# Today I Learned
> A library of my TIL

---


-[Chrome](#Chrome)

-[Dev-Tools](#Dev-Tools)

-[JavaScript](#JavaScript)

-[GitHub](#GitHub)

-[Iterm](#Iterm)

-[Mac](#Mac)

-[Postgresql](#Postgresql)

-[Premiere](#Premiere)

-[React](#React)

-[React-StyleComponents](#React-StyleComponents)

-[Sublime-Text](#Sublime-Text)

-[TailWindCSS](#TailWindCSS)

-[ThinkScript](#ThinkScript)

-[Icons](#Icons)

-[Vim](#Vim)

-[Volta](#Volta)



---

## Chrome
 __Disable Google Helper__  
 `chrome://settings/content/unsandboxedPlugins`

## Dev-Tools
__Copy & Paste__
```javascript
copy(Array.from(
    document.querySelectorAll(
        'CLASS-NAME UL LI').map(x =>
            x.innerText)))
```

## JavaScript
 

## GitHub
__Line Break__  
`Double Spaces for line break`  
`</br>`

## Iterm
__Clear History__  
`rm $HISTFILE`

## Mac
__SMC__  
 `shift + ctrl + option + power`

__PRAM__  
 `cmd + option + r + p`

__Disable Mac Chime__  
`sudo nvram StartupMute=%01`

__Quit Finder__  
`defaults write com.apple.finder` <br>
`QuitMenuItem -bool true;`     
`killall Finder`

## Postgresql
__Start / Stop server__  
`brew services start postgresql`  
`brew services stop postgresql`



## Premiere
` \ ` = Show Timeline

## React

___slice and map___
```javascript
array = []

{array.slice(startIndex: number, endIndex: number).map(x => {
 return <Component>{x}</Component>
})}
```


## React-StyleComponents
__Passing Props__
```
${props => props.NAME ? NAME : NAME}  
```

## Sublime-Text
 __Alias File__   
`/Users/UserName/.zshrc`  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•Primary Mac?

## TailWindCss  
__Center__  
`inset-x-0`

## ThinkScript

## Vim
__Save and Write__  
`:q` close      
`:w`        write/saves   
`:wa[!]`   write/save all windows [force]  
`:x`        save and quit, same as wq  
`:q!`      force close's non-saved files with changes

## Volta
__Steps to Enable__  
`⌘+R turn on your Mac`  
`csrutil enable --without kext`  
`csrutil disable`

---

## Icons
➕❌💥✨❓❕🚫✖️➖&nbsp;



