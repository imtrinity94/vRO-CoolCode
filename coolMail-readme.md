<h1>coolRun Documentation</h1>
This package enables&nbsp;vRealize Orchestratior (vRO) to run scripts of various types inside a VM using VMware tools.<p><span style="color: rgb(94, 125, 156); font-size: 18px; font-weight: bold;">Highlights</span><br></p><ul><li>Easy to use script ruinning engine<br></li><li>Replace {tags} in the script template with values from vRO<br></li><li>Can use Windows, Linux, (virtual) ESXi and Photon OS &nbsp;</li><li>Runs Linux&nbsp;Bash, Linux PHP, Linux Python, Linux Perl, Windows DOS, Windows PowerShell, Windows Diskpart</li><li>Can be easily addapted to run other OSs or Script types</li><li>Stores Configuration centraly and differentiates between Linux and Windows login credentials</li></ul><h3>Description<br></h3><p>CoolRun enables you to run scripts inside a VM without caring to much about copy, run, check etc. Using {tags} in the script you can replace these tags with any value from vRO. The workflow has the correct script exection setting for Linux Bash, Linux PHP, Linux Python, Linux Perl, Windows DOS, Windows PowerShell, Windows Diskpart build in. This for example allows a user to create a workflow that would add a new Disk to a Windows VM and then runs Windows Diskpart to create a partition, formatting it and assign a lab to it.</p><p>CoolRun is also built in such a way that it can be easily adapted to other script languages as well as OSs. &nbsp;&nbsp;<span style="color: rgb(46, 61, 76); "><br></span></p>[collage_base1]






















<p><br></p><h3>Varibales</h3><p>The input variable for CoolRun is a property and is defined as:</p><table class="MsoNormalTable" border="1" cellspacing="0" cellpadding="0">
 <tbody><tr>
  <td width="131" valign="top" style="width: 98.15pt; border-top-color: rgb(163, 163, 163); border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; background-color: rgb(217, 217, 217); padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><b><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">Property Key Name</span></b></p>
  </td>
  <td width="322" valign="top" style="width: 241.15pt; border-top-color: rgb(163, 163, 163); border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-style: none; background-color: rgb(217, 217, 217); padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><b><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">Type</span></b></p>
  </td>
  <td width="57" valign="top" style="width: 42.6pt; border-top-color: rgb(163, 163, 163); border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-style: none; background-color: rgb(217, 217, 217); padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><b><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">Required</span></b></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">vm</span></p>
  </td>
  <td width="322" valign="top" style="width: 241.15pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">VC:VirtualMachine</span></p>
  </td>
  <td width="57" valign="top" style="width: 42.6pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p align="center" style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; text-align: center; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">yes</span></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">script</span></p>
  </td>
  <td width="322" valign="top" style="width: 241.15pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">Resource Element</span></p>
  </td>
  <td width="57" valign="top" style="width: 42.6pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p align="center" style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; text-align: center; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">yes</span></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">wrapper</span></p>
  </td>
  <td width="322" valign="top" style="width: 241.15pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">String<br>
  </span>[dos | bash | php | perl | python | powershell | diskpart]</p>
  </td>
  <td width="57" valign="top" style="width: 42.6pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p align="center" style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; text-align: center; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">yes</span></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">vmUsername</span></p>
  </td>
  <td width="322" valign="top" style="width: 241.15pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">String&nbsp;</span></p>
  </td>
  <td width="57" valign="top" style="width: 42.6pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p align="center" style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; text-align: center; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">No</span></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">vmPassword</span></p>
  </td>
  <td width="322" valign="top" style="width: 241.15pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">Secure String</span></p>
  </td>
  <td width="57" valign="top" style="width: 42.6pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p align="center" style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; text-align: center; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">No</span></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">timeout</span></p>
  </td>
  <td width="322" valign="top" style="width: 241.15pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">number</span></p>
  </td>
  <td width="57" valign="top" style="width: 42.6pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p align="center" style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; text-align: center; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">No</span></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">waitTime</span></p>
  </td>
  <td width="322" valign="top" style="width: 241.15pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">number</span></p>
  </td>
  <td width="57" valign="top" style="width: 42.6pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p class="MsoNormal" align="center" style="text-align: center; "><span lang="EN-GB">No</span></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">delGuestFile</span></p>
  </td>
  <td width="322" valign="top" style="width: 241.15pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">Boolean</span></p>
  </td>
  <td width="57" valign="top" style="width: 42.6pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p class="MsoNormal" align="center" style="text-align: center; "><span lang="EN-GB">No</span></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">environment</span></p>
  </td>
  <td width="322" valign="top" style="width: 241.15pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">array of string</span></p>
  </td>
  <td width="57" valign="top" style="width: 42.6pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p class="MsoNormal" align="center" style="text-align: center; "><span lang="EN-GB">No</span></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; ">workingDirectory</p>
  </td>
  <td width="322" valign="top" style="width: 241.15pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">string</span></p>
  </td>
  <td width="57" valign="top" style="width: 42.6pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p class="MsoNormal" align="center" style="text-align: center; "><span lang="EN-GB">No</span></p>
  </td>
 </tr>
 <tr style="height: 59.9pt; ">
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; height: 59.9pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; ">scriptVariables</p>
  </td>
  <td width="322" valign="top" style="width: 241.15pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; height: 59.9pt; ">
  <table class="MsoNormalTable" border="1" cellspacing="0" cellpadding="0" title="" summary="">
   <tbody><tr>
    <td width="140" valign="top" style="width: 104.85pt; border-top-color: rgb(163, 163, 163); border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; background-color: rgb(217, 217, 217); padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
    <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><b><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">Property Key Name</span></b></p>
    </td>
    <td width="74" valign="top" style="width: 55.65pt; border-top-color: rgb(163, 163, 163); border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-style: none; background-color: rgb(217, 217, 217); padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
    <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><b><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">Type</span></b></p>
    </td>
    <td width="69" valign="top" style="width: 51.5pt; border-top-color: rgb(163, 163, 163); border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-style: none; background-color: rgb(217, 217, 217); padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
    <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><b><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">Required</span></b></p>
    </td>
   </tr>
   <tr>
    <td width="138" valign="top" style="width: 103.45pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
    <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">script Tag</span></p>
    </td>
    <td width="76" valign="top" style="width: 57.1pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
    <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">String</span></p>
    </td>
    <td width="59" valign="top" style="width: 44pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
    <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">yes</span></p>
    </td>
   </tr>
  </tbody></table>
  </td>
  <td width="57" valign="top" style="width: 42.6pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; height: 59.9pt; ">
  <p class="MsoNormal" align="center" style="text-align: center; "><span lang="EN-GB">No</span></p>
  </td>
 </tr>
</tbody></table><br><p>All variables that are not required can be used optionally to overwrite the existing values defined in the configuration element.</p><table class="MsoNormalTable" border="1" cellspacing="0" cellpadding="0">
 <tbody><tr>
  <td width="131" valign="top" style="width: 98.15pt; border-top-color: rgb(163, 163, 163); border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; background-color: rgb(217, 217, 217); padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><b><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">Optional function</span></b></p>
  </td>
  <td width="426" valign="top" style="width: 319.55pt; border-top-color: rgb(163, 163, 163); border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-style: none; background-color: rgb(217, 217, 217); padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><b><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">Usage</span></b></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">vmUsername</span></p>
  </td>
  <td width="426" valign="top" style="width: 319.55pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">Overwrites the configured Linux or Windows username</span></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">vmPassword</span></p>
  </td>
  <td width="426" valign="top" style="width: 319.55pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">Overwrites the configured Linux or Windows password</span></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">timeout</span></p>
  </td>
  <td width="426" valign="top" style="width: 319.55pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">maximal time in seconds CoolRun is waiting until it kills the script
  process. If set to 0 timeout is disabled. Default: 0.</span></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">waitTime</span></p>
  </td>
  <td width="426" valign="top" style="width: 319.55pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">time in seconds to wait before each check if the script has finished. Default:
  5</span></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">delGuestFile</span></p>
  </td>
  <td width="426" valign="top" style="width: 319.55pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">should the script file in the guest VM be deleted after it has been executed?</span></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">environment</span></p>
  </td>
  <td width="426" valign="top" style="width: 319.55pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">Overwrites the configured Linux or Windows environment variables</span></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">workingDirectory</span></p>
  </td>
  <td width="426" valign="top" style="width: 319.55pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">in what directory should the script be executed. <br>
  Default Windows: c:\ Default Linux: /tmp/</span></p>
  </td>
 </tr>
</tbody></table><p><span style="color: rgb(94, 125, 156); font-size: 18px; font-weight: bold; ">HowTo</span><br></p><h4>Installation and configuration</h4><ol><li>Import the vRO package into your vRO appliance</li><li>run the workflow <span style="font-weight: bold;">configure CoolRun</span></li></ol><p>The configuration program will ask for all the required information to run a script inside a VM. The configuration is saved in a Configuration file and a DOS or BASH Test can be run.</p><p>The example will ask for for a VM your name as well as a working directory. The advanced feature lets you define different credentials.</p><h4>Basic Usage</h4><p class="MsoListParagraph" style="padding-left: 40px; text-indent: -18pt; ">&nbsp;1<span lang="EN-GB">.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span lang="EN-GB">Create a scipt &nbsp;(see bash/dos example beneath)</span></p><table class="MsoTableGrid" border="1" cellspacing="0" cellpadding="0"><tbody><tr><td width="604" valign="top" style="padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-color: windowtext; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; width: 453.1pt; "><p class="MsoNormal" style="margin-bottom: 0.0001pt; ">echo "Hello {user.name}, have fun with coolRun" &gt; {user.dir}text.txt<br><br></p></td></tr></tbody></table><p>&nbsp; &nbsp;&nbsp;<span lang="EN-GB">2.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span lang="EN-GB">Save the script as a Text file and upload it into vRO as an resource element</span></p><p class="MsoListParagraphCxSpMiddle" style="padding-left: 40px; text-indent: -18pt; "><span lang="EN-GB">3.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span lang="EN-GB">Create a new workflow</span></p><p class="MsoListParagraphCxSpMiddle" style="padding-left: 40px; text-indent: -18pt; "><span lang="EN-GB">4. &nbsp; &nbsp; &nbsp; A</span><span lang="EN-GB">dd the<span style="font-weight: bold;"> coolRun SubSystem</span> workflow</span></p><p class="MsoListParagraphCxSpMiddle" style="padding-left: 40px; text-indent: -18pt; "><span lang="EN-GB">5. &nbsp; &nbsp; &nbsp; C</span><span lang="EN-GB">reate an attribute of type ResoruceElement and link it to the script you uploaded</span></p><p class="MsoListParagraphCxSpMiddle" style="padding-left: 40px; text-indent: -18pt; "><span lang="EN-GB">6. &nbsp; &nbsp; &nbsp; U</span><span lang="EN-GB">se a Scriptable task with an OUT-attribute of type Properties, called&nbsp;</span><span lang="EN-GB">payload</span><span lang="EN-GB">.</span></p><p class="MsoListParagraphCxSpMiddle" style="padding-left: 40px; text-indent: -18pt; ">7. &nbsp; &nbsp; &nbsp;&nbsp;Define the following workflow input variable:</p><table class="MsoTableGrid" border="1" cellspacing="0" cellpadding="0">
 <tbody><tr>
  <td width="132" valign="top" style="width: 99pt; border-top-color: windowtext; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; background-color: rgb(217, 217, 217); padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><b><span lang="EN-GB">Name</span></b></p>
  </td>
  <td width="132" valign="top" style="width: 99.2pt; border-top-color: windowtext; border-right-color: windowtext; border-bottom-color: windowtext; border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-style: none; background-color: rgb(217, 217, 217); padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><b><span lang="EN-GB">Type</span></b></p>
  </td>
  <td width="340" valign="top" style="width: 254.9pt; border-top-color: windowtext; border-right-color: windowtext; border-bottom-color: windowtext; border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-style: none; background-color: rgb(217, 217, 217); padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><b><span lang="EN-GB">Usage</span></b></p>
  </td>
 </tr>
 <tr>
  <td width="132" valign="top" style="width: 99pt; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">vm</span></p>
  </td>
  <td width="132" valign="top" style="width: 99.2pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">VC:VirtualMachine</span></p>
  </td>
  <td width="340" valign="top" style="width: 254.9pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">VM on which to execute</span></p>
  </td>
 </tr>
 <tr>
  <td width="132" valign="top" style="width: 99pt; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">name</span></p>
  </td>
  <td width="132" valign="top" style="width: 99.2pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">string</span></p>
  </td>
  <td width="340" valign="top" style="width: 254.9pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">your name</span></p>
  </td>
 </tr>
 <tr>
  <td width="132" valign="top" style="width: 99pt; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">workingDirectory</span></p>
  </td>
  <td width="132" valign="top" style="width: 99.2pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">string</span></p>
  </td>
  <td width="340" valign="top" style="width: 254.9pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">directory where the output should be stored</span></p>
  </td>
 </tr>
</tbody></table><p class="MsoListParagraphCxSpMiddle" style="padding-left: 40px; text-indent: -18pt; "><span lang="EN-GB">8.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span lang="EN-GB">In the scriptable task define the&nbsp;</span><span lang="EN-GB">payload (see example beneath, all bold names are vari</span>ables)</p><table class="MsoTableGrid" border="1" cellspacing="0" cellpadding="0"><tbody><tr><td width="604" valign="top" style="padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-color: windowtext; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; width: 453.1pt; "><p class="MsoNormal" style="margin-bottom: 0.0001pt; ">var payload= new Properties();<br>payload.put("vm",vm);
<br>payload.put("wrapper","dos");
<br>payload.put("script",exampleScript);
<br>payload.put("workingDirectory",workingDirectory);&nbsp;<br>var scriptVariables= new Properties();
<br>scriptVariables.put("user.name",name);
<br>scriptVariables.put("user.dir",workingDirectory);
<br>payload.put("scriptVariables",scriptVariables);<br><br></p></td></tr></tbody></table><p class="MsoListParagraph" style="padding-left: 40px; text-indent: -18pt; "><span lang="EN-GB">9.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span lang="EN-GB">Pass the Payload to the&nbsp;</span><span lang="EN-GB"><span style="font-weight: bold;">coolRun Subsystem</span> workflow</span></p><p class="MsoListParagraph" style="padding-left: 40px; text-indent: -18pt; ">10. &nbsp; &nbsp; Run the workflow &nbsp;<span lang="EN-GB"><br></span></p><p><span style="color: rgb(61, 82, 102); font-size: 16px; font-weight: bold; ">Modifications and extentions</span><br></p><p>CoolRun is built so that it can be easily extended to run with other OS types and script types. In order to add a OS or script type, you just need to configure the switch element before either the OS Type or the Script Type.</p><p>For OS the follwing output variables are needed:</p><table class="MsoTableGrid" border="1" cellspacing="0" cellpadding="0">
 <tbody><tr>
  <td width="132" valign="top" style="width: 99pt; border-top-color: windowtext; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; background-color: rgb(217, 217, 217); padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><b><span lang="EN-GB">Name</span></b></p>
  </td>
  <td width="123" valign="top" style="width: 92.15pt; border-top-color: windowtext; border-right-color: windowtext; border-bottom-color: windowtext; border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-style: none; background-color: rgb(217, 217, 217); padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><b><span lang="EN-GB">Type</span></b></p>
  </td>
  <td width="349" valign="top" style="width: 261.95pt; border-top-color: windowtext; border-right-color: windowtext; border-bottom-color: windowtext; border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-style: none; background-color: rgb(217, 217, 217); padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><b><span lang="EN-GB">Usage</span></b></p>
  </td>
 </tr>
 <tr>
  <td width="132" valign="top" style="width: 99pt; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">workingDirectory</span></p>
  </td>
  <td width="123" valign="top" style="width: 92.15pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">string</span></p>
  </td>
  <td width="349" valign="top" style="width: 261.95pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">where should the program run (e.g. c:\ or /tmp/)</span></p>
  </td>
 </tr>
 <tr>
  <td width="132" valign="top" style="width: 99pt; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">vmUsername</span></p>
  </td>
  <td width="123" valign="top" style="width: 92.15pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">string</span></p>
  </td>
  <td width="349" valign="top" style="width: 261.95pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">final username to be used</span></p>
  </td>
 </tr>
 <tr>
  <td width="132" valign="top" style="width: 99pt; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">vmPassword</span></p>
  </td>
  <td width="123" valign="top" style="width: 92.15pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">string</span></p>
  </td>
  <td width="349" valign="top" style="width: 261.95pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">final password to be used</span></p>
  </td>
 </tr>
 <tr>
  <td width="132" valign="top" style="width: 99pt; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">vmEnvironment</span></p>
  </td>
  <td width="123" valign="top" style="width: 92.15pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">array of strings</span></p>
  </td>
  <td width="349" valign="top" style="width: 261.95pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">(can be empty) final Environment variables to be
  used</span></p>
  </td>
 </tr>
</tbody></table><p>For scipts the folowing output varibales are needed:</p><table class="MsoTableGrid" border="1" cellspacing="0" cellpadding="0">
 <tbody><tr>
  <td width="132" valign="top" style="width: 99pt; border-top-color: windowtext; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; background-color: rgb(217, 217, 217); padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><b><span lang="EN-GB">Name</span></b></p>
  </td>
  <td width="123" valign="top" style="width: 92.15pt; border-top-color: windowtext; border-right-color: windowtext; border-bottom-color: windowtext; border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-style: none; background-color: rgb(217, 217, 217); padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><b><span lang="EN-GB">Type</span></b></p>
  </td>
  <td width="349" valign="top" style="width: 261.95pt; border-top-color: windowtext; border-right-color: windowtext; border-bottom-color: windowtext; border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-style: none; background-color: rgb(217, 217, 217); padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><b><span lang="EN-GB">Usage</span></b></p>
  </td>
 </tr>
 <tr>
  <td width="132" valign="top" style="width: 99pt; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">arguments</span></p>
  </td>
  <td width="123" valign="top" style="width: 92.15pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">string</span></p>
  </td>
  <td width="349" valign="top" style="width: 261.95pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">arguments of the program to be executed (e.g.
  /tmp/script.txt)</span></p>
  </td>
 </tr>
 <tr>
  <td width="132" valign="top" style="width: 99pt; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">guestFilePath</span></p>
  </td>
  <td width="123" valign="top" style="width: 92.15pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">string</span></p>
  </td>
  <td width="349" valign="top" style="width: 261.95pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">where should the program be put on the VM (e.g. /tmp/script.txt)</span></p>
  </td>
 </tr>
 <tr>
  <td width="132" valign="top" style="width: 99pt; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">programPath</span></p>
  </td>
  <td width="123" valign="top" style="width: 92.15pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">string</span></p>
  </td>
  <td width="349" valign="top" style="width: 261.95pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">path of the program to be executes (e.g. /bin/bash)</span></p>
  </td>
 </tr>
 
</tbody></table><p>If you want to overwrite existing settings with user input use the following litte function</p><table class="art-article" style="width: 60%; "><tbody><tr><td style="width: 100%; ">function exists(prop,key,alt){
<br>&nbsp; temp=prop.get(key);
<br>&nbsp; if (temp==null){
<br>&nbsp; &nbsp; return alt;
<br>&nbsp; } else {
<br>&nbsp; &nbsp; return temp;
<br>&nbsp; }
<br>}


<br><br>vmUsername=exists(payload,"vmUsername",WinvmUsername);<br></td></tr></tbody></table><h5><span style="color: rgb(94, 125, 156); font-size: 18px; font-weight: bold; "></span></h5><h3>Package content</h3><p class="MsoNormal"><span lang="EN-GB">This Package contains three workflows:</span></p><ul><li><span style="color: rgb(15, 20, 25); text-indent: -24px;">The CoolRun core workflow</span><br></li><li><span style="color: rgb(15, 20, 25); text-indent: -24px;">The&nbsp;WaitForGuestProcess workflow</span></li><li>a configuration program</li><li>five example workflows that showcase Bash, Dos, PowerShell, python (linux) and Diskpart (Windows)</li><li>a configuration to centrally store login information and settings</li><li>four example scripts</li></ul>
