<h1>coolMail Documentation</h1>
This package enables vRealize Orchestratior (vRO) to send HTML formatted emails via SMTP.<p><span style="color: rgb(94, 125, 156); font-size: 18px; font-weight: bold; ">Highlights</span><br></p><ul><li>Use preformatted HTML or plaintext email Templates<br></li><li>Replace {tags} in the Mail template with vRO values<br></li><li>Repeats HTML structures and fills them either with values from arrays or from properties.<br></li><li>Use a configuration to centrally store your mail settings<br></li></ul><h3>Description<span style="color: rgb(46, 61, 76);"><br></span></h3><p>The coolMail subsystem works by substituting a tag with an vRO value. A coolMail tag can be freely defined and must have { } winged brackets around it. For example {vm.name} or {userName}.<br></p><p>The User just prepares a HTML template (e.g. using&nbsp;<a href="https://html-online.com" target="_blank">html-online.com</a>) and inserts tags where later values from vRO should be displayed. This enables one for example to create very nice looking HTML email that can be used with vRealize Automation (vRA).</p><p>
</p>[collage_base]






















<p><br></p><h3>Varibales</h3><p> The input to CoolMail is a property which is defined as:
<br></p><table class="MsoNormalTable" border="1" cellspacing="0" cellpadding="0" title="" summary="">
 <tbody><tr>
  <td width="131" valign="top" style="width: 98.15pt; border-top-color: rgb(163, 163, 163); border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; background-color: rgb(217, 217, 217); padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><b><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">Property Key Name</span></b></p>
  </td>
  <td width="322" valign="top" style="width: 241.15pt; border-top-color: rgb(163, 163, 163); border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-style: none; background-color: rgb(217, 217, 217); padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><b><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">Type</span></b></p>
  </td>
  <td width="1" valign="top" style="width: 1pt; border-top-color: rgb(163, 163, 163); border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-style: none; background-color: rgb(217, 217, 217); padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><b><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">Required</span></b></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">mailTo</span></p>
  </td>
  <td width="322" valign="top" style="width: 241.15pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">string</span></p>
  </td>
  <td width="1" rowspan="3" valign="top" style="width: 1pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p align="center" style="text-align: center; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">one of them</span></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">mailCC</span></p>
  </td>
  <td width="322" valign="top" style="width: 241.15pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">string</span></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">mailBCC</span></p>
  </td>
  <td width="322" valign="top" style="width: 241.15pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">string</span></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">subject</span></p>
  </td>
  <td width="322" valign="top" style="width: 241.15pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">String (can contain {tags} )</span></p>
  </td>
  <td width="1" valign="top" style="width: 1pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p align="center" style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; text-align: center; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">yes</span></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">mailTemplate</span></p>
  </td>
  <td width="322" valign="top" style="width: 241.15pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">Resource Element</span></p>
  </td>
  <td width="1" valign="top" style="width: 1pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p align="center" style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; text-align: center; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">yes</span></p>
  </td>
 </tr>
 <tr>
  <td width="131" valign="top" style="width: 98.15pt; border-right-color: rgb(163, 163, 163); border-bottom-color: rgb(163, 163, 163); border-left-color: rgb(163, 163, 163); border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">mailReplacements</span></p>
  </td>
  <td width="322" valign="top" style="width: 241.15pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
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
    <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">subName</span></p>
    </td>
    <td width="76" valign="top" style="width: 57.1pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
    <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">subValue</span></p>
    </td>
    <td width="59" valign="top" style="width: 44pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 4pt; padding-right: 4pt; padding-bottom: 4pt; padding-left: 4pt; ">
    <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">yes</span></p>
    </td>
   </tr>
  </tbody></table>
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 41.4pt; margin-bottom: 0.0001pt; ">&nbsp;</p>
  <p style="margin-top: 0cm; margin-right: 0cm; margin-left: 14.4pt; margin-bottom: 0.0001pt; "><b><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">subValue</span></b><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">: </span></p>
  <ul type="disc">
   <li class="MsoNormal" style="vertical-align: middle; "><span lang="EN-GB">String</span></li>
   <li class="MsoNormal" style="vertical-align: middle; "><span lang="EN-GB">Array
       of String</span></li>
   <li class="MsoNormal" style="vertical-align: middle; "><span lang="EN-GB">Property
       (Strings)</span></li>
  </ul>
  </td>
  <td width="1" valign="top" style="width: 1pt; border-top-style: none; border-left-style: none; border-bottom-color: rgb(163, 163, 163); border-bottom-width: 1pt; border-right-color: rgb(163, 163, 163); border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p align="center" style="margin-top: 0cm; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; text-align: center; "><span lang="EN-GB" style="font-size: 11pt; font-family: Calibri, sans-serif; ">no</span></p>
  </td>
 </tr>
</tbody></table><br><p>The variable <span style="font-weight: bold;">subject</span> can also contain {tags} to be replaced.<br></p><h3>HowTo<br></h3><h4>Installation and configuration</h4><ol><li>Import the vRO package into your vRO appliance</li><li>Run the workflow&nbsp;<span style="font-weight: bold; ">configure CoolMail</span></li></ol><p>The configuration program will ask for all the required information to establish a SMTP connection between vRO and a Mail server. The configuration is saved in a Configuration file and a test email can be sent to check if the SMTP configuration is working.</p><p>The example will ask for your name, some other input as well as an array of Strings. It will then use an example mail template to send an email.</p><h4>Basic Usage</h4><p class="MsoListParagraph" style="text-indent: -18pt; padding-left: 40px; "><!--[if !supportLists]--><span lang="EN-GB">1.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><!--&#91;endif&#93;--><span lang="EN-GB">Create a HTML email template
(see example beneath)</span></p>

<table class="MsoTableGrid" border="1" cellspacing="0" cellpadding="0">
 <tbody><tr>
  <td width="604" valign="top" style="width: 453.1pt; border-top-color: windowtext; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">&lt;html&gt;<br></span>this is a test {vm.name}.<br>&lt;table&gt;<br>&lt;tr&gt;&lt;td&gt;Name&lt;/td&gt;&lt;td&gt;{vm.name}&lt;/td&gt;&lt;/tr&gt;<br>&lt;tr&gt;&lt;td&gt;IP&lt;/td&gt;&lt;td&gt;{vm.ip}&lt;/td&gt;&lt;/tr&gt;<br>&lt;tr&gt;&lt;td&gt;Mac&lt;/td&gt;&lt;td&gt;{vm.mac}&lt;/td&gt;&lt;/tr&gt;<br>&lt;/table&gt;<br>&lt;/html&gt;<br><br></p>
  </td>
 </tr>
</tbody></table>

<p>&nbsp; &nbsp;&nbsp;<span lang="EN-GB">2.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><span lang="EN-GB">Save the HTML email as a text file and upload it into
vRO as an resource element</span></p>

<p class="MsoListParagraphCxSpMiddle" style="text-indent: -18pt; padding-left: 40px; "><!--[if !supportLists]--><span lang="EN-GB">3.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><!--&#91;endif&#93;--><span lang="EN-GB">Create a new workflow</span></p>

<p class="MsoListParagraphCxSpMiddle" style="text-indent: -18pt; padding-left: 40px; "><!--[if !supportLists]--><span lang="EN-GB">4. &nbsp; &nbsp; &nbsp; A</span><span lang="EN-GB">dd the <span style="font-weight: bold;">coolMail Subsystem</span> workflow</span></p>

<p class="MsoListParagraphCxSpMiddle" style="text-indent: -18pt; padding-left: 40px; "><!--[if !supportLists]--><span lang="EN-GB">5. &nbsp; &nbsp; &nbsp; C</span><span lang="EN-GB">reate an attribute of type
ResoruceElement and link it to the mail template you have uploaded</span></p>

<p class="MsoListParagraphCxSpMiddle" style="text-indent: -18pt; padding-left: 40px; "><!--[if !supportLists]--><span lang="EN-GB">6. &nbsp; &nbsp; &nbsp; U</span><span lang="EN-GB">se a Scriptable task with an OUT-attribute
of type Properties, called </span><span lang="EN-GB">mailPayload</span><span lang="EN-GB">.</span></p>

<p class="MsoListParagraphCxSpLast" style="text-indent: -18pt; padding-left: 40px; "><!--[if !supportLists]--><span lang="EN-GB">7.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><!--&#91;endif&#93;--><span lang="EN-GB">In the scriptable task define the </span><span lang="EN-GB">mailPayload (see example beneath)</span></p>

<table class="MsoTableGrid" border="1" cellspacing="0" cellpadding="0">
 <tbody><tr>
  <td width="604" valign="top" style="width: 453.1pt; border-top-color: windowtext; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">var mailPayload= new Properties();<br></span>mailPayload.put("mailTo","info@langenhan.info");<br>mailPayload.put("subject","Test email
  für {vm.name}");<br>mailPayload.put("mailTemplate",resourceElement);<br>var mailReplacements= new Properties();<br>mailReplacements.put("vm.name","myVM");<br>mailReplacements.put("vm.ip","192.168.220.10");<br>mailReplacements.put("vm.mac","
  0A:0B:0C:0D:0E:0F");<br>mailPayload.put("mailReplacements",mailReplacements);<br><br></p>
  </td>
 </tr>
</tbody></table>

<p class="MsoListParagraph" style="text-indent: -18pt; padding-left: 40px; "><!--[if !supportLists]--><span lang="EN-GB">8.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><!--&#91;endif&#93;--><span lang="EN-GB">Pass the mailPayload to the </span><span lang="EN-GB"><span style="font-weight: bold;">coolMail
Subsystem</span> workflow</span></p><p class="MsoListParagraph" style="text-indent: -18pt; padding-left: 40px; ">8.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Run the workflow<span lang="EN-GB"><br></span></p>

<h4><b><span lang="EN-GB">Repeat
lines</span></b></h4>

<p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">You can use arrays or properties to repeat HTML code.
You need to encase the structure you would like to repeat with the &nbsp;HTML comment
<br><span style="font-weight: bold;">&lt;!--{<span style="font-style: italic;">TAG</span>.start}--&gt;</span> and
<span style="font-weight: bold;">&lt;!--{<span style="font-style: italic;">TAG</span>.end} --&gt; </span><br>where <b style="font-style: italic;">TAG</b> is the replacement tag name you
want to use.</span></p>

<p class="MsoNormal"><span lang="EN-GB">For Arrays you can use <span style="font-weight: bold;">{<span style="font-style: italic;">TAG</span>.counter} </span>to display the counter
(starting at 0) and <span style="font-weight: bold;">{<span style="font-style: italic;">TAG</span>.value}</span> will contain the value of the array for the
given counter. If you use&nbsp;<span style="font-weight: bold;">{<span style="font-style: italic;">TAG</span>.counter1}</span> instead the counting will start at 1. Mixing the Tags will result in nonsence output.</span></p>

<p class="MsoNormal"><span lang="EN-GB">For Properties you can use<span style="font-weight: bold;"> {<span style="font-style: italic;">TAG</span>.name} </span>to display the Property key
and <span style="font-weight: bold;">{<span style="font-style: italic;">TAG</span>.value}</span> to display the
Property value of a given key. Both Tags must be strings.</span></p>

<p class="MsoNormal"><i><span lang="EN-GB">Examples</span></i><span lang="EN-GB">:</span></p><table class="MsoTableGrid" border="1" cellspacing="0" cellpadding="0">
 <tbody><tr>
  <td width="16" valign="top" style="width: 11.8pt; border-top-color: windowtext; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; background-color: rgb(217, 217, 217); padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><b></b></p><p><b>&nbsp;</b></p>
  </td>
  <td width="278" valign="top" style="width: 208.7pt; border-top-color: windowtext; border-right-color: windowtext; border-bottom-color: windowtext; border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-style: none; background-color: rgb(217, 217, 217); padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><b><span lang="EN-GB">Array</span></b></p>
  </td>
  <td width="310" valign="top" style="width: 232.6pt; border-top-color: windowtext; border-right-color: windowtext; border-bottom-color: windowtext; border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-style: none; background-color: rgb(217, 217, 217); padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><b><span lang="EN-GB">Properties</span></b></p>
  </td>
 </tr>
 <tr>
  <td width="16" valign="top" style="width: 11.8pt; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-weight: bold;">HTML Source Code</span></p>
  </td>
  <td width="278" valign="top" style="width: 208.7pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">&lt;!--{repeat.start}--&gt;<br></span>&lt;tr&gt;<br>&lt;td&gt;{repeat.counter}&lt;/td&gt;<br>&lt;td&gt;{repeat.value}&lt;/td&gt;<br>&lt;/tr&gt;<br>&lt;!--{repeat.end}--&gt;</p>
  </td>
  <td width="310" valign="top" style="width: 232.6pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">&lt;!--{plugins.start}--&gt;<br></span>&lt;tr&gt;<br>&lt;td&gt;{plugins.name}&lt;/td&gt;<br>&lt;td&gt;{plugins.value}&lt;/td&gt;<br>&lt;/tr&gt;<br>&lt;!--{plugins.end}--&gt;</p>
  </td>
 </tr>
 <tr>
  <td width="16" valign="top" style="width: 11.8pt; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 10pt; font-family: Arial, sans-serif; font-weight: bold;">vRO code</span></p>
  </td>
  <td width="278" valign="top" style="width: 208.7pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 10pt; font-family: Arial, sans-serif; ">var repeatArray=new Array();</span><span lang="EN-GB" style="font-size: 10pt; font-family: Arial, sans-serif; "><br>
  repeatArray.push("VM 1");<br>
  repeatArray.push("VM 2");<br>
  repeatArray.push("VM 3");<br>
  mailReplacements.put("repeat",repeatArray);</span></p>
  </td>
  <td width="310" valign="top" style="width: 232.6pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">var propertyValues=new Properties();<br></span>propertyValues.put(“VM 1”,”vCenter”);<br>propertyValues.put(“VM 2”,”vRO”);<br>propertyValues.put(“VM 3”,”vRA”);<br>mailReplacements.put("plugins",propertyValues);</p>
  </td>
 </tr>
 <tr>
  <td width="16" valign="top" style="width: 11.8pt; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 10pt; font-family: Arial, sans-serif; font-weight: bold;">HTML output</span></p>
  </td>
  <td width="278" valign="top" style="width: 208.7pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">&lt;tr&gt;<br></span>&lt;td&gt;0&lt;/td&gt;<br>&lt;td&gt;VM 1&lt;/td&gt;<br>&lt;/tr&gt;<br>&lt;tr&gt;<br>&lt;td&gt;1&lt;/td&gt;<br>&lt;td&gt; VM 2&lt;/td&gt;<br>&lt;/tr&gt;<br>&lt;tr&gt;<br>&lt;td&gt;2&lt;/td&gt;<br>&lt;td&gt; VM 3&lt;/td&gt;<br>&lt;/tr&gt;</p>
  
  </td>
  <td width="310" valign="top" style="width: 232.6pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">&lt;tr&gt;<br></span>&lt;td&gt;VM 1&lt;/td&gt;<br>&lt;td&gt;vCenter&lt;/td&gt;<br>&lt;/tr&gt;<br>&lt;tr&gt;<br>&lt;td&gt;VM 2&lt;/td&gt;<br>&lt;td&gt;vRO&lt;/td&gt;<br>&lt;/tr&gt;<br>&lt;tr&gt;<br>&lt;td&gt;VM 3&lt;/td&gt;<br>&lt;td&gt;vRA&lt;/td&gt;<br>&lt;/tr&gt;</p>
  
  </td>
 </tr>
</tbody></table><h4><b><span lang="EN-GB">Replace images</span></b></h4><p class="MsoNormal">You can also use Cool mail to replace images. You do that by exchanging the content of the HTML &lt;img&gt; tag with a image location.</p><table class="MsoNormalTable" border="1" cellspacing="0" cellpadding="0" width="679">
 <tbody><tr>
  <td width="140" valign="top" style="width: 105.1pt; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; background-color: rgb(191, 191, 191); padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-top: 9pt; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><b><span lang="EN-GB" style="font-size: 10pt; font-family: Arial, sans-serif; ">HTML Source Code</span></b></p>
  </td>
  <td width="539" valign="top" style="width: 403.95pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-top: 9pt; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 10pt; font-family: Arial, sans-serif; ">&lt;img src="{ImageSource}"
  /&gt;</span></p>
  </td>
 </tr>
 <tr>
  <td width="140" valign="top" style="width: 105.1pt; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; background-color: rgb(191, 191, 191); padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-top: 9pt; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><b><span lang="EN-GB" style="font-size: 10pt; font-family: Arial, sans-serif; ">vRO code</span></b></p>
  </td>
  <td width="539" valign="top" style="width: 403.95pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-top: 9pt; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 10pt; font-family: Arial, sans-serif; ">mailReplacements.put("</span><span lang="EN-GB" style="font-size: 10pt; font-family: Arial, sans-serif; ">ImageSource</span><span lang="EN-GB" style="font-size: 10pt; font-family: Arial, sans-serif; ">",”</span><span lang="EN-GB" style="font-size: 10pt; font-family: Arial, sans-serif; ">http://langenhan.info/images/object0.png”);</span></p>
  </td>
 </tr>
 <tr>
  <td width="140" valign="top" style="width: 105.1pt; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; background-color: rgb(191, 191, 191); padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-top: 9pt; margin-right: 0cm; margin-left: 0cm; margin-bottom: 0.0001pt; "><b><span lang="EN-GB" style="font-size: 10pt; font-family: Arial, sans-serif; ">HTML output</span></b></p>
  </td>
  <td width="539" style="width: 403.95pt; border-top-style: none; border-left-style: none; border-bottom-style: inset; border-bottom-width: 1pt; border-right-style: inset; border-right-width: 1pt; padding-top: 0cm; padding-right: 0cm; padding-bottom: 0cm; padding-left: 0cm; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span style="font-size: 10pt; font-family: 'Times New Roman', serif; ">&lt;img src="http://langenhan.info/images/object0.png" /&gt;</span></p>
  </td>
 </tr>
</tbody></table>

<p><span style="color: rgb(94, 125, 156); font-size: 18px; font-weight: bold; ">Package content</span><br></p><p class="MsoNormal"><span lang="EN-GB">This Package contains three workflows:</span></p><ul><li><span style="color: rgb(15, 20, 25); text-indent: -24px; ">The CoolMail Subsystem workflow</span><br></li><li><span style="color: rgb(15, 20, 25); text-indent: -24px; ">The CoolMail configuration workflow</span></li><li><span style="color: rgb(15, 20, 25); text-indent: -24px; ">and an example workflow</span></li></ul>
