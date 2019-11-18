Getting Started with Common Extensibility Platform (CEP)
==============

This page provides the resources you need to get started in order to create extensions for Adobe Creative Cloud applications, using the new HTML5/JavaScript interface model. The Flash/ActionScript interface model for extensions is deprecated in Creative Cloud releases; Support has already been removed from CC2014 and later releases.

* Creative Cloud 2019 products include CEP 9 for developing extensions and add-ons. Refer to the [table](https://github.com/Adobe-CEP/CEP-Resources/blob/master/CEP_9.x/Documentation/CEP%209.0%20HTML%20Extension%20Cookbook.md#applications-integrated-with-cep) for 2019 products integration with CEP 9.

* Creative Cloud 2018 products include CEP 8 for developing extensions and add-ons. Refer to the [table](https://github.com/Adobe-CEP/CEP-Resources/blob/master/CEP_8.x/Documentation/CEP%208.0%20HTML%20Extension%20Cookbook.md#applications-integrated-with-cep) for 2018 product integration with CEP 8.

* In the Creative Cloud 2015.x release in June 2016, Photoshop and Illustrator use CEP 7 while other applications still use CEP 6.1. Extensions and add-ons must be built on at least CEP 6 infrastructure.

* In the Creative Cloud 2015 release, extensions and add-ons must be built on the CEP 6 infrastructure.

* In the Creative Cloud 2014 release, extensions and add-ons must be built on the CEP 5 infrastructure and loaded with Extension Manager. The current releases either do not now or soon will not support CEP 4 and Flash/ActionScript extensions.

* The Creative Suite 6 and the Creative Cloud 2013 releases of Adobe desktop applications support CEP 4, which allows you to build extensions using the older Flash/ActionScript interface model. However, the new HTML5/JavaScript model is preferred. It is recommended that you port existing Flash/ActionScript extensions to the new model.

This SDK provides the low-level tools that you need to build extensions. Extensions that you build using these tools must be packaged as ZXP files in order to be seen and loaded by Extension Manager. You can offer extensions as free or paid products through our marketing portals (Adobe Exchange, the Add-ins website, the Creative Cloud desktop app). When you do this, you upload the extension to Adobe as a single ZXP file.

Resources you will need include:
* CEP JavaScript libraries for communicating with the operating system and Extension Manager and for communicating with the host application and other extensions.
* Sample code for how to use these libraries
* The ZXP packager, a command-line utility

---

For developing CEP 9.0 HTML/JavaScript extensions for CC 2019.x host applications

**Documentation**
* [CEP 9.0 HTML Extension Cookbook](https://github.com/Adobe-CEP/CEP-Resources/blob/master/CEP_9.x/Documentation/CEP%209.0%20HTML%20Extension%20Cookbook.md)
* [CEP 9 runtime](https://github.com/Adobe-CEP/CEP-Resources/blob/master/CEP_9.x/Documentation/CEP%209.0%20HTML%20Extension%20Cookbook.md#chromium-embedded-framework-cef) 

For CEP 8,
* [CEP 8.0 HTML Extension Cookbook](https://github.com/Adobe-CEP/CEP-Resources/blob/master/CEP_8.x/Documentation/CEP%208.0%20HTML%20Extension%20Cookbook.md)
* [CEP 8 runtime](https://github.com/Adobe-CEP/CEP-Resources/blob/master/CEP_8.x/Documentation/CEP%208.0%20HTML%20Extension%20Cookbook.md#chromium-embedded-framework-cef) 

**APIs** 
CEP 9 APIs: https://github.com/Adobe-CEP/CEP-Resources/tree/master/CEP_9.x
* Include these files in your extension project if you need to use the APIs.
  * CSInterface.js
  * Vulcan.js
* Do NOT include this file in your extension project. It is already integrated into CEP.
  * CEPEngine_extensions.js

**Samples**
* [Sample extensions](https://github.com/Adobe-CEP/Samples)

**Packaging and Signing Tool (ZXPSignCMD)**
* Tool: [ZXPSignCMD](https://github.com/Adobe-CEP/CEP-Resources/tree/master/ZXPSignCMD)
* Document: [Packaging and Signing Adobe Extensions](http://wwwimages.adobe.com/content/dam/Adobe/en/devnet/creativesuite/pdfs/SigningTechNote_CC.pdf) 

**Extension Installation Tools**
* Extension Manager Command Line Tool
  * [Announcement: Extension Manager End of Life](https://www.adobeexchange.com/resources/27)
  * [ExMan Command Line Tool](https://www.adobeexchange.com/resources/28)
  * [ExMan Command Line Tool's Error Codes](http://www.adobeexchange.com/resources/19#errors)
* [A Python script to install & manage extensions](https://github.com/adobe-photoshop/generator-panels/blob/master/installPanels.py) (by John Peterson)
* Other Tools
  * http://zxpinstaller.com/
  * http://install.anastasiy.com/

---

For developing CEP 7.0 HTML/JavaScript extensions for CC 2015.x host applications

**Documentation**
* [CEP 7.0 HTML Extension Cookbook for 2015.x in June 2016](https://github.com/Adobe-CEP/CEP-Resources/blob/master/CEP_7.x/CEP_7.0_HTML_Extension_Cookbook.pdf)
* [CEP 7 Feature List](https://github.com/Adobe-CEP/CEP-Resources/blob/master/CEP_7.x/CEP_7_Feature_List.pdf)

**APIs** (https://github.com/Adobe-CEP/CEP-Resources/tree/master/CEP_7.x)
* Include these files in your extension project if you need to use the APIs.
  * AgoraLib.js
  * CSInterface.js
  * Vulcan.js
* Do NOT include this file in your extension project. It is already integrated into CEP.
  * CEPEngine_extensions.js
* Extension Manifest
  * ExtensionManifest_v_7_0.xsd

**Samples**
* [Sample extensions](https://github.com/Adobe-CEP/Samples)

**Packaging and Signing Tool (ZXPSignCMD)**
* Tool: [ZXPSignCMD](https://github.com/Adobe-CEP/CEP-Resources/tree/master/ZXPSignCMD)
* Document: [Packaging and Signing Adobe Extensions](http://wwwimages.adobe.com/content/dam/Adobe/en/devnet/creativesuite/pdfs/SigningTechNote_CC.pdf) (NOTE:  For CEP 4.0 but valid for CEP 7.x)

**Extension Installation Tools**
* Extension Manager Command Line Tool
  * [Announcement: Extension Manager End of Life](https://www.adobeexchange.com/resources/27)
  * [ExMan Command Line Tool](https://www.adobeexchange.com/resources/28)
  * [ExMan Command Line Tool's Error Codes](http://www.adobeexchange.com/resources/19#errors)
* [A Python script to install & manage extensions](https://github.com/adobe-photoshop/generator-panels/blob/master/installPanels.py) (by John Peterson)
* Other Tools
  * http://zxpinstaller.com/
  * http://install.anastasiy.com/

----

For developing CEP 6.1 HTML/JavaScript extensions for CC2015.1 host applications

**Documentation**
* [CEP 6.1 HTML Extension Cookbook for CC 2015.1](https://github.com/Adobe-CEP/CEP-Resources/blob/master/CEP_6.x/CEP_6.1_HTML_Extension_Cookbook.pdf)
* [CEP 6 Feature List](https://github.com/Adobe-CEP/CEP-Resources/blob/master/CEP_6.x/CEP_6_Feature_List.pdf)

**APIs** (https://github.com/Adobe-CEP/CEP-Resources/tree/master/CEP_6.x)
* Include these files in your extension project if you need to use the APIs.
  * AgoraLib.js
  * CSInterface.js
  * Vulcan.js
* Do NOT include this file in your extension project. It is already integrated into CEP.
  * CEPEngine_extensions.js
* Extension Manifest
  * ExtensionManifest_v_6_0.xsd

**Samples**
* [Sample extensions](https://github.com/Adobe-CEP/Samples)

**Packaging and Signing Tool (ZXPSignCMD)**
* [Packaging and Signing Adobe Extensions](http://wwwimages.adobe.com/content/dam/Adobe/en/devnet/creativesuite/pdfs/SigningTechNote_CC.pdf) (NOTE:  For CEP 4.0 but valid for CEP 6.x)

**Extension Installation Tools**
* Extension Manager Command Line Tool
  * [Announcement: Extension Manager End of Life](https://www.adobeexchange.com/resources/27)
  * [ExMan Command Line Tool](https://www.adobeexchange.com/resources/28)
  * [ExMan Command Line Tool's Error Codes](http://www.adobeexchange.com/resources/19#errors)
* [A Python script to install & manage extensions](https://github.com/adobe-photoshop/generator-panels/blob/master/installPanels.py) (by John Peterson)
* Other Tools
  * http://zxpinstaller.com/
  * http://install.anastasiy.com/

----

For developing CEP 6.0 HTML/JavaScript extensions for CC2015 host applications

**Documentation**
* [CEP 6.0 HTML Extension Cookbook for CC 2015](https://github.com/Adobe-CEP/CEP-Resources/wiki/CEP-6-HTML-Extension-Cookbook-for-CC-2015)

**APIs** (https://github.com/Adobe-CEP/CEP-Resources/tree/master/CEP_6.x)
* Include these files in your extension project if you need to use the APIs.
  * AgoraLib.js
  * CSInterface.js
  * Vulcan.js
* Do NOT include this file in your extension project. It is already integrated into CEP.
  * CEPEngine_extensions.js
* Extension Manifest (unchanged in CEP 6.0)
  * ExtensionManifest_v_5_0.xsd

**Samples**
* [Sample extensions](https://github.com/Adobe-CEP/Samples)

**Packaging and Signing Tool (ZXPSignCMD)**
* [Packaging and Signing Adobe Extensions](http://wwwimages.adobe.com/content/dam/Adobe/en/devnet/creativesuite/pdfs/SigningTechNote_CC.pdf) (NOTE:  For CEP 4.0 but valid for CEP 6)

**Extension Installation Tools**
* Extension Manager Command Line Tool
  * [Announcement: Extension Manager End of Life](https://www.adobeexchange.com/resources/27)
  * [ExMan Command Line Tool](https://www.adobeexchange.com/resources/28)
  * [ExMan Command Line Tool's Error Codes](http://www.adobeexchange.com/resources/19#errors)
* [A Python script to install & manage extensions](https://github.com/adobe-photoshop/generator-panels/blob/master/installPanels.py) (by John Peterson)
* Other Tools
  * http://zxpinstaller.com/
  * http://install.anastasiy.com/

----

For developing CEP 5.x HTML/JavaScript extensions for CC2014 host applications

**Documentation**
* [Offical Adobe Extension SDK Documentation for CC 2014](http://adobe.ly/1rin38t)
* [CEP 5 HTML Extension Cookbook for CC 2014](https://github.com/Adobe-CEP/CEP-Resources/wiki/CEP-5-HTML-Extension-Cookbook-for-CC-2014)
* [CEP 5 Flash Extension Cookbook for CC 2014](https://github.com/Adobe-CEP/CEP-Resources/wiki/CEP-5-Flash-Extension-Cookbook-for-CC-2014)

**APIs** (https://github.com/Adobe-CEP/CEP-Resources/tree/master/CEP_5.x)
* Include these files in your extension project if you need to use the APIs.
  * AgoraLib.js
  * CSInterface.js
  * Vulcan.js
* Do NOT include this file in your extension project. It is already integrated into CEP.
  * CEPEngine_extensions.js
* Extension Manifest
  * ExtensionManifest_v_5_0.xsd
* PlugPlugExternalObject
  * [PlugPlugExternalObject for InDesign CC 2014](http://bit.ly/1qlnKOb)

**Samples**
* [Sample extensions](https://github.com/Adobe-CEP/Samples)

**Other Documents**
* [CEP for the InDesign Developer](http://adobe.ly/1xXkviH)
* [Extending Adobe CC 2014 apps using Node.js](http://bit.ly/1yAR0T9)
* [A short guide to HTML5 extensions](http://adobe.ly/Nk1EK7)
   (NOTE:  For CEP 4.0 but still mostly relevant)
* [Guide to signing extensions](http://adobe.ly/1oiS4FE)
   (NOTE:  For CEP 4.0 but valid for CEP 5)

----

For developing CEP 4.x and extensions for CS6/CC host applications

**Documentation**
* [Documentation for CEP 4.2](http://adobe.ly/1cWBggl)
* [Tutorial](http://bit.ly/1nNLqH4)
   (NOTE: A bit old)

**APIs** (https://github.com/Adobe-CEP/CEP-Resources/tree/master/CEP_4.x)
* Include these files in your extension project if you need to use the APIs.
  * CSInterface.js
  * Vulcan.js
* Do NOT include this file in your extension project. It is already integrated into CEP.
  * CEPEngine_extensions.js
* Extension Manifest
  * ExtensionManifest_v_4_0.xsd

**Tooling**
* [Extension Builder 3 Preview](http://adobe.ly/1pho2QU)
* [Extension Builder 3 forums - get help from the developer community](http://adobe.ly/1mgZ2xe)
   (NOTE: EB3 is compatible with CEP 4.x only. You can [tweak it](http://adobe.ly/1v3wgiq) so that it supports CC 2014 (with limitations))

----

Miscellaneous help
* [Getting Started Guides](https://github.com/Adobe-CEP/Getting-Started-guides)
* [CS SDK Blog](https://blogs.adobe.com/cssdk/)
* [Andy Hall's Super Mega Guide (English)] (http://bit.ly/XQn9IV) [ (Japanese)] (http://bit.ly/XQnB9P)
* [Davide Barranca’s blog](http://www.davidebarranca.com/) and [HTML Panels Development Course](http://htmlpanelsbook.com/)
* [David Deraedt’s plugin for Adobe Brackets](http://bit.ly/QKWWYL)
* [Olav Martin Kvern's article on extensibility and InDesign](http://bit.ly/1zEa9Ef)
* [The other API (Article on Medium)](http://bit.ly/1hIFZay)
* [Adobe Exchange](http://bit.ly/1mHVksI)
* [Photoshop CC 2014 CEP samples by John Peterson](http://bit.ly/1nGAWYN)

----

    Apache License
                           Version 2.0, January 2004
                        https://www.apache.org/licenses/

   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION

   1. Definitions.

      "License" shall mean the terms and conditions for use, reproduction,
      and distribution as defined by Sections 1 through 9 of this document.

      "Licensor" shall mean the copyright owner or entity authorized by
      the copyright owner that is granting the License.

      "Legal Entity" shall mean the union of the acting entity and all
      other entities that control, are controlled by, or are under common
      control with that entity. For the purposes of this definition,
      "control" means (i) the power, direct or indirect, to cause the
      direction or management of such entity, whether by contract or
      otherwise, or (ii) ownership of fifty percent (50%) or more of the
      outstanding shares, or (iii) beneficial ownership of such entity.

      "You" (or "Your") shall mean an individual or Legal Entity
      exercising permissions granted by this License.

      "Source" form shall mean the preferred form for making modifications,
      including but not limited to software source code, documentation
      source, and configuration files.

      "Object" form shall mean any form resulting from mechanical
      transformation or translation of a Source form, including but
      not limited to compiled object code, generated documentation,
      and conversions to other media types.

      "Work" shall mean the work of authorship, whether in Source or
      Object form, made available under the License, as indicated by a
      copyright notice that is included in or attached to the work
      (an example is provided in the Appendix below).

      "Derivative Works" shall mean any work, whether in Source or Object
      form, that is based on (or derived from) the Work and for which the
      editorial revisions, annotations, elaborations, or other modifications
      represent, as a whole, an original work of authorship. For the purposes
      of this License, Derivative Works shall not include works that remain
      separable from, or merely link (or bind by name) to the interfaces of,
      the Work and Derivative Works thereof.

      "Contribution" shall mean any work of authorship, including
      the original version of the Work and any modifications or additions
      to that Work or Derivative Works thereof, that is intentionally
      submitted to Licensor for inclusion in the Work by the copyright owner
      or by an individual or Legal Entity authorized to submit on behalf of
      the copyright owner. For the purposes of this definition, "submitted"
      means any form of electronic, verbal, or written communication sent
      to the Licensor or its representatives, including but not limited to
      communication on electronic mailing lists, source code control systems,
      and issue tracking systems that are managed by, or on behalf of, the
      Licensor for the purpose of discussing and improving the Work, but
      excluding communication that is conspicuously marked or otherwise
      designated in writing by the copyright owner as "Not a Contribution."

      "Contributor" shall mean Licensor and any individual or Legal Entity
      on behalf of whom a Contribution has been received by Licensor and
      subsequently incorporated within the Work.

   2. Grant of Copyright License. Subject to the terms and conditions of
      this License, each Contributor hereby grants to You a perpetual,
      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
      copyright license to reproduce, prepare Derivative Works of,
      publicly display, publicly perform, sublicense, and distribute the
      Work and such Derivative Works in Source or Object form.

   3. Grant of Patent License. Subject to the terms and conditions of
      this License, each Contributor hereby grants to You a perpetual,
      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
      (except as stated in this section) patent license to make, have made,
      use, offer to sell, sell, import, and otherwise transfer the Work,
      where such license applies only to those patent claims licensable
      by such Contributor that are necessarily infringed by their
      Contribution(s) alone or by combination of their Contribution(s)
      with the Work to which such Contribution(s) was submitted. If You
      institute patent litigation against any entity (including a
      cross-claim or counterclaim in a lawsuit) alleging that the Work
      or a Contribution incorporated within the Work constitutes direct
      or contributory patent infringement, then any patent licenses
      granted to You under this License for that Work shall terminate
      as of the date such litigation is filed.

   4. Redistribution. You may reproduce and distribute copies of the
      Work or Derivative Works thereof in any medium, with or without
      modifications, and in Source or Object form, provided that You
      meet the following conditions:

      (a) You must give any other recipients of the Work or
          Derivative Works a copy of this License; and

      (b) You must cause any modified files to carry prominent notices
          stating that You changed the files; and

      (c) You must retain, in the Source form of any Derivative Works
          that You distribute, all copyright, patent, trademark, and
          attribution notices from the Source form of the Work,
          excluding those notices that do not pertain to any part of
          the Derivative Works; and

      (d) If the Work includes a "NOTICE" text file as part of its
          distribution, then any Derivative Works that You distribute must
          include a readable copy of the attribution notices contained
          within such NOTICE file, excluding those notices that do not
          pertain to any part of the Derivative Works, in at least one
          of the following places: within a NOTICE text file distributed
          as part of the Derivative Works; within the Source form or
          documentation, if provided along with the Derivative Works; or,
          within a display generated by the Derivative Works, if and
          wherever such third-party notices normally appear. The contents
          of the NOTICE file are for informational purposes only and
          do not modify the License. You may add Your own attribution
          notices within Derivative Works that You distribute, alongside
          or as an addendum to the NOTICE text from the Work, provided
          that such additional attribution notices cannot be construed
          as modifying the License.

      You may add Your own copyright statement to Your modifications and
      may provide additional or different license terms and conditions
      for use, reproduction, or distribution of Your modifications, or
      for any such Derivative Works as a whole, provided Your use,
      reproduction, and distribution of the Work otherwise complies with
      the conditions stated in this License.

   5. Submission of Contributions. Unless You explicitly state otherwise,
      any Contribution intentionally submitted for inclusion in the Work
      by You to the Licensor shall be under the terms and conditions of
      this License, without any additional terms or conditions.
      Notwithstanding the above, nothing herein shall supersede or modify
      the terms of any separate license agreement you may have executed
      with Licensor regarding such Contributions.

   6. Trademarks. This License does not grant permission to use the trade
      names, trademarks, service marks, or product names of the Licensor,
      except as required for reasonable and customary use in describing the
      origin of the Work and reproducing the content of the NOTICE file.

   7. Disclaimer of Warranty. Unless required by applicable law or
      agreed to in writing, Licensor provides the Work (and each
      Contributor provides its Contributions) on an "AS IS" BASIS,
      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
      implied, including, without limitation, any warranties or conditions
      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
      PARTICULAR PURPOSE. You are solely responsible for determining the
      appropriateness of using or redistributing the Work and assume any
      risks associated with Your exercise of permissions under this License.

   8. Limitation of Liability. In no event and under no legal theory,
      whether in tort (including negligence), contract, or otherwise,
      unless required by applicable law (such as deliberate and grossly
      negligent acts) or agreed to in writing, shall any Contributor be
      liable to You for damages, including any direct, indirect, special,
      incidental, or consequential damages of any character arising as a
      result of this License or out of the use or inability to use the
      Work (including but not limited to damages for loss of goodwill,
      work stoppage, computer failure or malfunction, or any and all
      other commercial damages or losses), even if such Contributor
      has been advised of the possibility of such damages.

   9. Accepting Warranty or Additional Liability. While redistributing
      the Work or Derivative Works thereof, You may choose to offer,
      and charge a fee for, acceptance of support, warranty, indemnity,
      or other liability obligations and/or rights consistent with this
      License. However, in accepting such obligations, You may act only
      on Your own behalf and on Your sole responsibility, not on behalf
      of any other Contributor, and only if You agree to indemnify,
      defend, and hold each Contributor harmless for any liability
      incurred by, or claims asserted against, such Contributor by reason
      of your accepting any such warranty or additional liability.

   END OF TERMS AND CONDITIONS

   APPENDIX: How to apply the Apache License to your work.

      To apply the Apache License to your work, attach the following
      boilerplate notice, with the fields enclosed by brackets "[]"
      replaced with your own identifying information. (Don't include
      the brackets!)  The text should be enclosed in the appropriate
      comment syntax for the file format. We also recommend that a
      file or class name and description of purpose be included on the
      same "printed page" as the copyright notice for easier
      identification within third-party archives.

   Copyright 2019 Rolando Gopez Lacuata

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       https://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.


