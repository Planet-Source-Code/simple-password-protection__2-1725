<div align="center">

## Simple Password Protection


</div>

### Description

Posted by Unknown (emerald.bbs@bbs.cs.nthu.edu.tw)

to newsgroup tw.bbs.comp.www (30 September, 1998)

Description: A simple script that allows only users who know a fixed password to visit your pages. The password is part of the HTML source, so this script provides only basic security. (The password of the demo page is 12345).

Instructions
 
### More Info
 
1. Copy Part 1 from the sample page below into the HRAD of your page

2. Set the variables password and protected_page


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[N/A](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/empty.md)
**Level**          |Unknown
**User Rating**    |5.0 (25 globes from 5 users)
**Compatibility**  |
**Category**       |[Security](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/security__2-74.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/simple-password-protection__2-1725/archive/master.zip)





### Source Code

```
<!----------------------------------------Simple Password ProtectionJavaScript archived by JavaScript Cornerhttp://pbc.bhcom1.com-------------------------------------------->
<head>
<!------------------------------------------########## Script Part 1 ###################Copy this part into the HEAD of your page------------------------------------------->
<script language="JavaScript">
var password ="12345"; //set this to the desired string
var protected_page ="../common/2ndwindow.htm"; //set this to the destination URL
var pd="";
pd=prompt("You are about to enter a restricted zone. Password:","");
if(pd!=password)
{
alert("Invalid password");
history.back();
}
else
{
alert("Password accepted");
window.location.href=protected_page;
}
</script>
<!------------------------------------------########## End of Script Part 1 ############------------------------------------------->
<title>Simple Password Protection</title>
</head>
<body bgcolor="#000000" text="#FFFF00" link="#00FFFF" vlink="#C0C0C0">
<p align="center"><img src="../../bitmaps/jsbanner.gif" width="500" height="25"></p>
<h2 align="center">Simple Password Protection</h2>
</body>
</html>
```

