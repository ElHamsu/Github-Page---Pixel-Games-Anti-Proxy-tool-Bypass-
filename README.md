readme.md;

# Understanding

Firstly for you to understand Proxy Check tool generally works by checking parameters (such as screen resulation your location your fps etc.) Theres 130 parameters like that, 

Today we will limit access to those parameters get by site and randomize left overs, and add some of extra stuff and tips so you dont get detected ;)

## Needed AddOns/Extension's;
`Tuxler (as residental proxy, you can use another residental proxy)`
https://addons.mozilla.org/en-US/firefox/addon/free-residential-tuxler-vpn/

`Trace (to limit and randomize parameters and bypass Loc/Header proxy test)`
https://addons.mozilla.org/en-US/firefox/addon/absolutedouble-trace/

`CanvasBlocker (to limit and randomize parameters also making chaptcha easier)`
https://addons.mozilla.org/en-US/firefox/addon/canvasblocker/

`μblockOrigin (some extra stuff to avoid detection :) and limit parameters)`
https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/

## Extension's/AddOns settings:

paste into my filters μblockorigin:
||ipinfo.io^$important
||browserleaks.com/webrtc$script

Enable following settings in Trace/AdvancedProtections;
UserAgentRandomizer
ProxyIpHeaderSpoofing
ClientRectsProtection

Enable FakeMinimalScreenSize from CanvasBlocker/Apis

#### Closing GeoLocation;
write about:config on browser
screach geo
make geo.enabled False

#### Creating profiles:
Make 2 .bat Txt files and copy paste to first one;

`@echo off
echo Profiles creating`

`start "" /WRITE ROOT FILE OF BROWSER HERE\zen.exe" -CreateProfile "proxy1"`
`start "" /WRITE ROOT FILE OF BROWSER HERE\zen.exe" -CreateProfile "proxy2"`

`echo All profiles created
pause`

#### to second .bat file;

`@echo off
echo Opening profiles`

`start "" "/WRITE ROOT FILE OF BROWSER HERE\zen.exe" -P "proxy1" -no-remote
timeout /t 1 >nul
start "" "/WRITE ROOT FILE OF BROWSER HERE\zen.exe" -P "proxy2" -no-remote
timeout /t 1 >nul`

`echo All profiles started
pause`

The first .bat file creates profiles, the second one opens them, those profiles works like vurtial PC but for browser, you will have to do everything that i said above for every browser profile ! Those work by running


#### Remember!
Admins does Check your Email, Password, Username, if those are similar to each other they may tag you as proxy

#### Remember!
Admins can check Previous IP Address, if you connected to 1 account with 2 different proxies in different times(1 from amerika 1 from Spain) admins can easly spot you as proxy (obviously you cant be teleporting to spain and amerika in 5 second)
So if you use wrong proxy on wrong account guranteed ban.

#### Remember!
Most of users get banned for sharing how to proxy, using bad paintbots and being active for 7/24 with proxy, So dont act like a proxy bot :)

#### Remember! 
most of PixelGames uses Proxycheck.io as their Anti-Proxy service so you can check your proxies

### Remember! 
Always use residantal proxy
Remember Those!

## If there is enough demand, the same bypass tool will come for Chromium, currently Firefox Zen is used for this bypass tool. If you use another browser, replace zen.exe in the .bat file
