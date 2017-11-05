<h1>logAllProps</h1>
This workflow allows you to completely read out a property in all its details using vRealize Orchestratior (vRO). The output will be displayed into the logs of the workflow. This workflow is extremly useful for vRealize Automation (vRA)<h3><span lang="EN-GB">Highlights</span></h3><ul><li>Recursive logging of properties within properties</li><li>displaying the variable type</li><li>showing the content of arrays</li></ul><p><span style="color: rgb(94, 125, 156); font-size: 18px; font-weight: bold; ">Description</span><br></p><p>This workflow will log the content of a property into the logs (System.log). The property can consists of multiple properties in properties as well as arrays. 
The workflow will also log all system context variables (mostly used with vRA).

The input variable debugFlag can be null. If set to false the workflow is not executed. This can be used to make sure that the logging will only work in a debug situtation. <br></p>[collage_coolRunLog]
















<p><span style="color: rgb(94, 125, 156); font-size: 18px; font-weight: bold; ">Variables</span><br></p><p>The input variables are:<br></p><table class="MsoTableGrid" border="1" cellspacing="0" cellpadding="0">
 <tbody><tr>
  <td width="104" valign="top" style="width: 77.75pt; border-top-color: windowtext; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; background-color: rgb(217, 217, 217); padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><b><span lang="EN-GB">Name</span></b></p>
  </td>
  <td width="85" valign="top" style="width: 64.1pt; border-top-color: windowtext; border-right-color: windowtext; border-bottom-color: windowtext; border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-style: none; background-color: rgb(217, 217, 217); padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><b><span lang="EN-GB">Type</span></b></p>
  </td>
  <td width="415" valign="top" style="width: 311.25pt; border-top-color: windowtext; border-right-color: windowtext; border-bottom-color: windowtext; border-top-width: 1pt; border-right-width: 1pt; border-bottom-width: 1pt; border-left-style: none; background-color: rgb(217, 217, 217); padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><b><span lang="EN-GB">Usage</span></b></p>
  </td>
 </tr>
 <tr>
  <td width="104" valign="top" style="width: 77.75pt; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">payload</span></p>
  </td>
  <td width="85" valign="top" style="width: 64.1pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">property</span></p>
  </td>
  <td width="415" valign="top" style="width: 311.25pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">property to log</span></p>
  </td>
 </tr>
 <tr>
  <td width="104" valign="top" style="width: 77.75pt; border-right-color: windowtext; border-bottom-color: windowtext; border-left-color: windowtext; border-right-width: 1pt; border-bottom-width: 1pt; border-left-width: 1pt; border-top-style: none; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">debugFlag</span></p>
  </td>
  <td width="85" valign="top" style="width: 64.1pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB">boolean</span></p>
  </td>
  <td width="415" valign="top" style="width: 311.25pt; border-top-style: none; border-left-style: none; border-bottom-color: windowtext; border-bottom-width: 1pt; border-right-color: windowtext; border-right-width: 1pt; padding-top: 0cm; padding-right: 5.4pt; padding-bottom: 0cm; padding-left: 5.4pt; ">
  <p class="MsoNormal" style="margin-bottom: 0.0001pt; "><span lang="EN-GB" style="font-size: 10pt; font-family: Arial, sans-serif; ">(optional) If set to false the
  workflow will exit without doing anything. This property can be null which is
  the same as true.&nbsp;</span></p>
  </td>
 </tr>
</tbody></table><p><br></p><h3>Usage</h3><h4>Installation and configuration</h4><ol><li>Import the vRO package into your vRO appliance</li></ol><h4>Basic Usage</h4><p>Just insert the workflow logAllProps into your existing workflow and add the property you would like to log to it. As an example use a vRA EventManager subscription linked to a workflow in vRO. Insert into this workflow the logAllProperty and add the property that the vRA Event Manager provides to logAllProps. &nbsp; &nbsp;<br></p><h3>Package content</h3><p class="MsoNormal"><span lang="EN-GB">This Package contains three workflows:</span></p><ul><li><span style="color: rgb(15, 20, 25); text-indent: -24px; ">The logAllProbs core workflow</span><br></li><li><span style="color: rgb(15, 20, 25); text-indent: -24px; ">The logAllProps program that reads out a VCAC:VirtualMachine and displays its properties as well as its Entities</span><br></li><li><span style="text-indent: -24px; color: rgb(15, 20, 25); ">The logAllProps program that reads out a VCAC:VirtualMachine and displays its properties as well as its Entities</span><br></li><li><span style="color: rgb(15, 20, 25); text-indent: -24px; ">and an example workflow</span></li></ul>
