# Comparing `tmp/convomeld-0.1.3.tar.gz` & `tmp/convomeld-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convomeld-0.1.3.tar", max compression
+gzip compressed data, was "convomeld-0.1.4.tar", max compression
```

## Comparing `convomeld-0.1.3.tar` & `convomeld-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0    34336 2023-07-31 16:58:18.192409 convomeld-0.1.3/LICENSE.md
--rw-r--r--   0        0        0      226 2023-07-31 16:58:18.196410 convomeld-0.1.3/README.md
--rw-r--r--   0        0        0      834 2023-07-31 17:15:07.998709 convomeld-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       27 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/__init__.py
--rw-r--r--   0        0        0       36 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/__main__.py
--rw-r--r--   0        0        0     5408 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/api.py
--rw-r--r--   0        0        0     1223 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/cli.py
--rw-r--r--   0        0        0      102 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/constants.py
--rw-r--r--   0        0        0     1761 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/convocat.py
--rw-r--r--   0        0        0     1575 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/convoparse.py
--rw-r--r--   0        0        0     6868 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/data_factory.py
--rw-r--r--   0        0        0     2602 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/df_to_convograph.py
--rw-r--r--   0        0        0    17528 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/graph.py
--rw-r--r--   0        0        0     1268 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/matchers.py
--rw-r--r--   0        0        0    10570 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/merge.py
--rw-r--r--   0        0        0     2512 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/parsers.py
--rw-r--r--   0        0        0     2905 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/sorters.py
--rw-r--r--   0        0        0     8061 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/state.py
--rw-r--r--   0        0        0     5182 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/states.py
--rw-r--r--   0        0        0     6960 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/thread.py
--rw-r--r--   0        0        0     1278 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/utils.py
--rw-r--r--   0        0        0     8730 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/validators.py
--rw-r--r--   0        0        0     4239 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/xlsx_csv_parsers.py
--rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 convomeld-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    34996 2023-07-03 13:09:55.682872 convomeld-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0      898 2023-08-07 18:20:39.545698 convomeld-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      230 2023-07-03 13:09:55.682872 convomeld-0.1.4/README.md
+-rw-r--r--   0        0        0       27 2023-07-25 09:48:26.346603 convomeld-0.1.4/src/convomeld/__init__.py
+-rw-r--r--   0        0        0       38 2023-07-05 17:08:03.113682 convomeld-0.1.4/src/convomeld/__main__.py
+-rw-r--r--   0        0        0     5932 2023-08-07 18:17:19.721485 convomeld-0.1.4/src/convomeld/api.py
+-rw-r--r--   0        0        0     1257 2023-07-25 09:48:26.347601 convomeld-0.1.4/src/convomeld/cli.py
+-rw-r--r--   0        0        0      106 2023-08-07 18:16:49.294135 convomeld-0.1.4/src/convomeld/constants.py
+-rw-r--r--   0        0        0    17285 2023-08-07 18:17:03.894406 convomeld-0.1.4/src/convomeld/converters.py
+-rw-r--r--   0        0        0     1820 2023-08-07 18:16:49.296087 convomeld-0.1.4/src/convomeld/convocat.py
+-rw-r--r--   0        0        0     1627 2023-08-07 18:16:49.296087 convomeld-0.1.4/src/convomeld/convoparse.py
+-rw-r--r--   0        0        0     7097 2023-08-07 18:16:49.297063 convomeld-0.1.4/src/convomeld/data_factory.py
+-rw-r--r--   0        0        0     2682 2023-08-07 18:16:49.298039 convomeld-0.1.4/src/convomeld/df_to_convograph.py
+-rw-r--r--   0        0        0    20064 2023-08-07 18:17:19.721485 convomeld-0.1.4/src/convomeld/graph.py
+-rw-r--r--   0        0        0     1308 2023-07-31 17:24:49.411221 convomeld-0.1.4/src/convomeld/matchers.py
+-rw-r--r--   0        0        0    10787 2023-07-31 17:24:49.412352 convomeld-0.1.4/src/convomeld/merge.py
+-rw-r--r--   0        0        0     2580 2023-07-05 17:08:03.123387 convomeld-0.1.4/src/convomeld/parsers.py
+-rw-r--r--   0        0        0     3004 2023-08-07 18:16:49.299015 convomeld-0.1.4/src/convomeld/sorters.py
+-rw-r--r--   0        0        0     8368 2023-08-07 18:17:19.722461 convomeld-0.1.4/src/convomeld/state.py
+-rw-r--r--   0        0        0     5353 2023-08-07 18:16:49.299991 convomeld-0.1.4/src/convomeld/states.py
+-rw-r--r--   0        0        0     7153 2023-07-31 17:24:49.415602 convomeld-0.1.4/src/convomeld/thread.py
+-rw-r--r--   0        0        0     1320 2023-08-07 18:16:49.299991 convomeld-0.1.4/src/convomeld/utils.py
+-rw-r--r--   0        0        0     8934 2023-07-20 13:31:56.961911 convomeld-0.1.4/src/convomeld/validators.py
+-rw-r--r--   0        0        0     4363 2023-08-07 18:16:49.300967 convomeld-0.1.4/src/convomeld/xlsx_csv_parsers.py
+-rw-r--r--   0        0        0      902 1970-01-01 00:00:00.000000 convomeld-0.1.4/PKG-INFO
```

### Comparing `convomeld-0.1.3/LICENSE.md` & `convomeld-0.1.4/LICENSE.md`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,660 +1,660 @@
-### GNU AFFERO GENERAL PUBLIC LICENSE
-
-Version 3, 19 November 2007
-
-Copyright (C) 2007 Free Software Foundation, Inc.
-<https://fsf.org/>
-
-Everyone is permitted to copy and distribute verbatim copies of this
-license document, but changing it is not allowed.
-
-### Preamble
-
-The GNU Affero General Public License is a free, copyleft license for
-software and other kinds of works, specifically designed to ensure
-cooperation with the community in the case of network server software.
-
-The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works. By contrast,
-our General Public Licenses are intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains
-free software for all its users.
-
-When we speak of free software, we are referring to freedom, not
-price. Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-Developers that use our General Public Licenses protect your rights
-with two steps: (1) assert copyright on the software, and (2) offer
-you this License which gives you legal permission to copy, distribute
-and/or modify the software.
-
-A secondary benefit of defending all users' freedom is that
-improvements made in alternate versions of the program, if they
-receive widespread use, become available for other developers to
-incorporate. Many developers of free software are heartened and
-encouraged by the resulting cooperation. However, in the case of
-software used on network servers, this result may fail to come about.
-The GNU General Public License permits making a modified version and
-letting the public access it on a server without ever releasing its
-source code to the public.
-
-The GNU Affero General Public License is designed specifically to
-ensure that, in such cases, the modified source code becomes available
-to the community. It requires the operator of a network server to
-provide the source code of the modified version running there to the
-users of that server. Therefore, public use of a modified version, on
-a publicly accessible server, gives the public access to the source
-code of the modified version.
-
-An older license, called the Affero General Public License and
-published by Affero, was designed to accomplish similar goals. This is
-a different license, not a version of the Affero GPL, but Affero has
-released a new version of the Affero GPL which permits relicensing
-under this license.
-
-The precise terms and conditions for copying, distribution and
-modification follow.
-
-### TERMS AND CONDITIONS
-
-#### 0. Definitions.
-
-"This License" refers to version 3 of the GNU Affero General Public
-License.
-
-"Copyright" also means copyright-like laws that apply to other kinds
-of works, such as semiconductor masks.
-
-"The Program" refers to any copyrightable work licensed under this
-License. Each licensee is addressed as "you". "Licensees" and
-"recipients" may be individuals or organizations.
-
-To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of
-an exact copy. The resulting work is called a "modified version" of
-the earlier work or a work "based on" the earlier work.
-
-A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy. Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies. Mere interaction with a user
-through a computer network, with no transfer of a copy, is not
-conveying.
-
-An interactive user interface displays "Appropriate Legal Notices" to
-the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License. If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-#### 1. Source Code.
-
-The "source code" for a work means the preferred form of the work for
-making modifications to it. "Object code" means any non-source form of
-a work.
-
-A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form. A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities. However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work. For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-The Corresponding Source need not include anything that users can
-regenerate automatically from other parts of the Corresponding Source.
-
-The Corresponding Source for a work in source code form is that same
-work.
-
-#### 2. Basic Permissions.
-
-All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met. This License explicitly affirms your unlimited
-permission to run the unmodified Program. The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work. This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-You may make, run and propagate covered works that you do not convey,
-without conditions so long as your license otherwise remains in force.
-You may convey covered works to others for the sole purpose of having
-them make modifications exclusively for you, or provide you with
-facilities for running those works, provided that you comply with the
-terms of this License in conveying all material for which you do not
-control copyright. Those thus making or running the covered works for
-you must do so exclusively on your behalf, under your direction and
-control, on terms that prohibit them from making any copies of your
-copyrighted material outside their relationship with you.
-
-Conveying under any other circumstances is permitted solely under the
-conditions stated below. Sublicensing is not allowed; section 10 makes
-it unnecessary.
-
-#### 3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such
-circumvention is effected by exercising rights under this License with
-respect to the covered work, and you disclaim any intention to limit
-operation or modification of the work as a means of enforcing, against
-the work's users, your or third parties' legal rights to forbid
-circumvention of technological measures.
-
-#### 4. Conveying Verbatim Copies.
-
-You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-#### 5. Conveying Modified Source Versions.
-
-You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these
-conditions:
-
--   a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
--   b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under
-    section 7. This requirement modifies the requirement in section 4
-    to "keep intact all notices".
--   c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy. This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged. This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
--   d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit. Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-#### 6. Conveying Non-Source Forms.
-
-You may convey a covered work in object code form under the terms of
-sections 4 and 5, provided that you also convey the machine-readable
-Corresponding Source under the terms of this License, in one of these
-ways:
-
--   a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
--   b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the Corresponding
-    Source from a network server at no charge.
--   c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source. This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
--   d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge. You need not require recipients to copy the
-    Corresponding Source along with the object code. If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source. Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
--   e) Convey the object code using peer-to-peer transmission,
-    provided you inform other peers where the object code and
-    Corresponding Source of the work are being offered to the general
-    public at no charge under subsection 6d.
-
-A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal,
-family, or household purposes, or (2) anything designed or sold for
-incorporation into a dwelling. In determining whether a product is a
-consumer product, doubtful cases shall be resolved in favor of
-coverage. For a particular product received by a particular user,
-"normally used" refers to a typical or common use of that class of
-product, regardless of the status of the particular user or of the way
-in which the particular user actually uses, or expects or is expected
-to use, the product. A product is a consumer product regardless of
-whether the product has substantial commercial, industrial or
-non-consumer uses, unless such uses represent the only significant
-mode of use of the product.
-
-"Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to
-install and execute modified versions of a covered work in that User
-Product from a modified version of its Corresponding Source. The
-information must suffice to ensure that the continued functioning of
-the modified object code is in no case prevented or interfered with
-solely because modification has been made.
-
-If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information. But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or
-updates for a work that has been modified or installed by the
-recipient, or for the User Product in which it has been modified or
-installed. Access to a network may be denied when the modification
-itself materially and adversely affects the operation of the network
-or violates the rules and protocols for communication across the
-network.
-
-Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-#### 7. Additional Terms.
-
-"Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law. If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it. (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.) You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders
-of that material) supplement the terms of this License with terms:
-
--   a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
--   b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
--   c) Prohibiting misrepresentation of the origin of that material,
-    or requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
--   d) Limiting the use for publicity purposes of names of licensors
-    or authors of the material; or
--   e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
--   f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions
-    of it) with contractual assumptions of liability to the recipient,
-    for any liability that these contractual assumptions directly
-    impose on those licensors and authors.
-
-All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10. If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term. If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions; the
-above requirements apply either way.
-
-#### 8. Termination.
-
-You may not propagate or modify a covered work except as expressly
-provided under this License. Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-However, if you cease all violation of this License, then your license
-from a particular copyright holder is reinstated (a) provisionally,
-unless and until the copyright holder explicitly and finally
-terminates your license, and (b) permanently, if the copyright holder
-fails to notify you of the violation by some reasonable means prior to
-60 days after the cessation.
-
-Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License. If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-#### 9. Acceptance Not Required for Having Copies.
-
-You are not required to accept this License in order to receive or run
-a copy of the Program. Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance. However,
-nothing other than this License grants you permission to propagate or
-modify any covered work. These actions infringe copyright if you do
-not accept this License. Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-#### 10. Automatic Licensing of Downstream Recipients.
-
-Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License. You are not responsible
-for enforcing compliance by third parties with this License.
-
-An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations. If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License. For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-#### 11. Patents.
-
-A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based. The
-work thus licensed is called the contributor's "contributor version".
-
-A contributor's "essential patent claims" are all patent claims owned
-or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version. For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement). To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients. "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-A patent license is "discriminatory" if it does not include within the
-scope of its coverage, prohibits the exercise of, or is conditioned on
-the non-exercise of one or more of the rights that are specifically
-granted under this License. You may not convey a covered work if you
-are a party to an arrangement with a third party that is in the
-business of distributing software, under which you make payment to the
-third party based on the extent of your activity of conveying the
-work, and under which the third party grants, to any of the parties
-who would receive the covered work from you, a discriminatory patent
-license (a) in connection with copies of the covered work conveyed by
-you (or copies made from those copies), or (b) primarily for and in
-connection with specific products or compilations that contain the
-covered work, unless you entered into that arrangement, or that patent
-license was granted, prior to 28 March 2007.
-
-Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-#### 12. No Surrender of Others' Freedom.
-
-If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License. If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under
-this License and any other pertinent obligations, then as a
-consequence you may not convey it at all. For example, if you agree to
-terms that obligate you to collect a royalty for further conveying
-from those to whom you convey the Program, the only way you could
-satisfy both those terms and this License would be to refrain entirely
-from conveying the Program.
-
-#### 13. Remote Network Interaction; Use with the GNU General Public License.
-
-Notwithstanding any other provision of this License, if you modify the
-Program, your modified version must prominently offer all users
-interacting with it remotely through a computer network (if your
-version supports such interaction) an opportunity to receive the
-Corresponding Source of your version by providing access to the
-Corresponding Source from a network server at no charge, through some
-standard or customary means of facilitating copying of software. This
-Corresponding Source shall include the Corresponding Source for any
-work covered by version 3 of the GNU General Public License that is
-incorporated pursuant to the following paragraph.
-
-Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU General Public License into a single
-combined work, and to convey the resulting work. The terms of this
-License will continue to apply to the part which is the covered work,
-but the work with which it is combined will remain governed by version
-3 of the GNU General Public License.
-
-#### 14. Revised Versions of this License.
-
-The Free Software Foundation may publish revised and/or new versions
-of the GNU Affero General Public License from time to time. Such new
-versions will be similar in spirit to the present version, but may
-differ in detail to address new problems or concerns.
-
-Each version is given a distinguishing version number. If the Program
-specifies that a certain numbered version of the GNU Affero General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation. If the Program does not specify a version number of the
-GNU Affero General Public License, you may choose any version ever
-published by the Free Software Foundation.
-
-If the Program specifies that a proxy can decide which future versions
-of the GNU Affero General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-Later license versions may give you additional or different
-permissions. However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-#### 15. Disclaimer of Warranty.
-
-THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT
-WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT
-LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
-A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND
-PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE
-DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR
-CORRECTION.
-
-#### 16. Limitation of Liability.
-
-IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR
-CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES,
-INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES
-ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT
-NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR
-LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM
-TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER
-PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
-
-#### 17. Interpretation of Sections 15 and 16.
-
-If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-END OF TERMS AND CONDITIONS
-
-### How to Apply These Terms to Your New Programs
-
-If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these
-terms.
-
-To do so, attach the following notices to the program. It is safest to
-attach them to the start of each source file to most effectively state
-the exclusion of warranty; and each file should have at least the
-"copyright" line and a pointer to where the full notice is found.
-
-        Mathactive - K-12 student can learn math from a chatbot that helps them actively solve math problems suitable to their skill level.
-        Copyright (C) 2023  Tangible AI
-
-        This program is free software: you can redistribute it and/or modify
-        it under the terms of the GNU Affero General Public License as
-        published by the Free Software Foundation, either version 3 of the
-        License, or (at your option) any later version.
-
-        This program is distributed in the hope that it will be useful,
-        but WITHOUT ANY WARRANTY; without even the implied warranty of
-        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-        GNU Affero General Public License for more details.
-
-        You should have received a copy of the GNU Affero General Public License
-        along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper
-mail.
-
-If your software can interact with users remotely through a computer
-network, you should also make sure that it provides a way for users to
-get its source. For example, if your program is a web application, its
-interface could display a "Source" link that leads users to an archive
-of the code. There are many ways you could offer source, and different
-solutions will be better for different programs; see section 13 for
-the specific requirements.
-
-You should also get your employer (if you work as a programmer) or
-school, if any, to sign a "copyright disclaimer" for the program, if
-necessary. For more information on this, and how to apply and follow
-the GNU AGPL, see <https://www.gnu.org/licenses/>.
+### GNU AFFERO GENERAL PUBLIC LICENSE
+
+Version 3, 19 November 2007
+
+Copyright (C) 2007 Free Software Foundation, Inc.
+<https://fsf.org/>
+
+Everyone is permitted to copy and distribute verbatim copies of this
+license document, but changing it is not allowed.
+
+### Preamble
+
+The GNU Affero General Public License is a free, copyleft license for
+software and other kinds of works, specifically designed to ensure
+cooperation with the community in the case of network server software.
+
+The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works. By contrast,
+our General Public Licenses are intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains
+free software for all its users.
+
+When we speak of free software, we are referring to freedom, not
+price. Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+Developers that use our General Public Licenses protect your rights
+with two steps: (1) assert copyright on the software, and (2) offer
+you this License which gives you legal permission to copy, distribute
+and/or modify the software.
+
+A secondary benefit of defending all users' freedom is that
+improvements made in alternate versions of the program, if they
+receive widespread use, become available for other developers to
+incorporate. Many developers of free software are heartened and
+encouraged by the resulting cooperation. However, in the case of
+software used on network servers, this result may fail to come about.
+The GNU General Public License permits making a modified version and
+letting the public access it on a server without ever releasing its
+source code to the public.
+
+The GNU Affero General Public License is designed specifically to
+ensure that, in such cases, the modified source code becomes available
+to the community. It requires the operator of a network server to
+provide the source code of the modified version running there to the
+users of that server. Therefore, public use of a modified version, on
+a publicly accessible server, gives the public access to the source
+code of the modified version.
+
+An older license, called the Affero General Public License and
+published by Affero, was designed to accomplish similar goals. This is
+a different license, not a version of the Affero GPL, but Affero has
+released a new version of the Affero GPL which permits relicensing
+under this license.
+
+The precise terms and conditions for copying, distribution and
+modification follow.
+
+### TERMS AND CONDITIONS
+
+#### 0. Definitions.
+
+"This License" refers to version 3 of the GNU Affero General Public
+License.
+
+"Copyright" also means copyright-like laws that apply to other kinds
+of works, such as semiconductor masks.
+
+"The Program" refers to any copyrightable work licensed under this
+License. Each licensee is addressed as "you". "Licensees" and
+"recipients" may be individuals or organizations.
+
+To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of
+an exact copy. The resulting work is called a "modified version" of
+the earlier work or a work "based on" the earlier work.
+
+A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy. Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies. Mere interaction with a user
+through a computer network, with no transfer of a copy, is not
+conveying.
+
+An interactive user interface displays "Appropriate Legal Notices" to
+the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License. If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+#### 1. Source Code.
+
+The "source code" for a work means the preferred form of the work for
+making modifications to it. "Object code" means any non-source form of
+a work.
+
+A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form. A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities. However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work. For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+The Corresponding Source need not include anything that users can
+regenerate automatically from other parts of the Corresponding Source.
+
+The Corresponding Source for a work in source code form is that same
+work.
+
+#### 2. Basic Permissions.
+
+All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met. This License explicitly affirms your unlimited
+permission to run the unmodified Program. The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work. This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+You may make, run and propagate covered works that you do not convey,
+without conditions so long as your license otherwise remains in force.
+You may convey covered works to others for the sole purpose of having
+them make modifications exclusively for you, or provide you with
+facilities for running those works, provided that you comply with the
+terms of this License in conveying all material for which you do not
+control copyright. Those thus making or running the covered works for
+you must do so exclusively on your behalf, under your direction and
+control, on terms that prohibit them from making any copies of your
+copyrighted material outside their relationship with you.
+
+Conveying under any other circumstances is permitted solely under the
+conditions stated below. Sublicensing is not allowed; section 10 makes
+it unnecessary.
+
+#### 3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such
+circumvention is effected by exercising rights under this License with
+respect to the covered work, and you disclaim any intention to limit
+operation or modification of the work as a means of enforcing, against
+the work's users, your or third parties' legal rights to forbid
+circumvention of technological measures.
+
+#### 4. Conveying Verbatim Copies.
+
+You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+#### 5. Conveying Modified Source Versions.
+
+You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these
+conditions:
+
+-   a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+-   b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under
+    section 7. This requirement modifies the requirement in section 4
+    to "keep intact all notices".
+-   c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy. This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged. This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+-   d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit. Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+#### 6. Conveying Non-Source Forms.
+
+You may convey a covered work in object code form under the terms of
+sections 4 and 5, provided that you also convey the machine-readable
+Corresponding Source under the terms of this License, in one of these
+ways:
+
+-   a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+-   b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the Corresponding
+    Source from a network server at no charge.
+-   c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source. This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+-   d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge. You need not require recipients to copy the
+    Corresponding Source along with the object code. If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source. Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+-   e) Convey the object code using peer-to-peer transmission,
+    provided you inform other peers where the object code and
+    Corresponding Source of the work are being offered to the general
+    public at no charge under subsection 6d.
+
+A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal,
+family, or household purposes, or (2) anything designed or sold for
+incorporation into a dwelling. In determining whether a product is a
+consumer product, doubtful cases shall be resolved in favor of
+coverage. For a particular product received by a particular user,
+"normally used" refers to a typical or common use of that class of
+product, regardless of the status of the particular user or of the way
+in which the particular user actually uses, or expects or is expected
+to use, the product. A product is a consumer product regardless of
+whether the product has substantial commercial, industrial or
+non-consumer uses, unless such uses represent the only significant
+mode of use of the product.
+
+"Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to
+install and execute modified versions of a covered work in that User
+Product from a modified version of its Corresponding Source. The
+information must suffice to ensure that the continued functioning of
+the modified object code is in no case prevented or interfered with
+solely because modification has been made.
+
+If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information. But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or
+updates for a work that has been modified or installed by the
+recipient, or for the User Product in which it has been modified or
+installed. Access to a network may be denied when the modification
+itself materially and adversely affects the operation of the network
+or violates the rules and protocols for communication across the
+network.
+
+Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+#### 7. Additional Terms.
+
+"Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law. If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it. (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.) You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders
+of that material) supplement the terms of this License with terms:
+
+-   a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+-   b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+-   c) Prohibiting misrepresentation of the origin of that material,
+    or requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+-   d) Limiting the use for publicity purposes of names of licensors
+    or authors of the material; or
+-   e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+-   f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions
+    of it) with contractual assumptions of liability to the recipient,
+    for any liability that these contractual assumptions directly
+    impose on those licensors and authors.
+
+All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10. If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term. If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions; the
+above requirements apply either way.
+
+#### 8. Termination.
+
+You may not propagate or modify a covered work except as expressly
+provided under this License. Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+However, if you cease all violation of this License, then your license
+from a particular copyright holder is reinstated (a) provisionally,
+unless and until the copyright holder explicitly and finally
+terminates your license, and (b) permanently, if the copyright holder
+fails to notify you of the violation by some reasonable means prior to
+60 days after the cessation.
+
+Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License. If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+#### 9. Acceptance Not Required for Having Copies.
+
+You are not required to accept this License in order to receive or run
+a copy of the Program. Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance. However,
+nothing other than this License grants you permission to propagate or
+modify any covered work. These actions infringe copyright if you do
+not accept this License. Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+#### 10. Automatic Licensing of Downstream Recipients.
+
+Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License. You are not responsible
+for enforcing compliance by third parties with this License.
+
+An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations. If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License. For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+#### 11. Patents.
+
+A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based. The
+work thus licensed is called the contributor's "contributor version".
+
+A contributor's "essential patent claims" are all patent claims owned
+or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version. For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement). To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients. "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+A patent license is "discriminatory" if it does not include within the
+scope of its coverage, prohibits the exercise of, or is conditioned on
+the non-exercise of one or more of the rights that are specifically
+granted under this License. You may not convey a covered work if you
+are a party to an arrangement with a third party that is in the
+business of distributing software, under which you make payment to the
+third party based on the extent of your activity of conveying the
+work, and under which the third party grants, to any of the parties
+who would receive the covered work from you, a discriminatory patent
+license (a) in connection with copies of the covered work conveyed by
+you (or copies made from those copies), or (b) primarily for and in
+connection with specific products or compilations that contain the
+covered work, unless you entered into that arrangement, or that patent
+license was granted, prior to 28 March 2007.
+
+Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+#### 12. No Surrender of Others' Freedom.
+
+If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License. If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under
+this License and any other pertinent obligations, then as a
+consequence you may not convey it at all. For example, if you agree to
+terms that obligate you to collect a royalty for further conveying
+from those to whom you convey the Program, the only way you could
+satisfy both those terms and this License would be to refrain entirely
+from conveying the Program.
+
+#### 13. Remote Network Interaction; Use with the GNU General Public License.
+
+Notwithstanding any other provision of this License, if you modify the
+Program, your modified version must prominently offer all users
+interacting with it remotely through a computer network (if your
+version supports such interaction) an opportunity to receive the
+Corresponding Source of your version by providing access to the
+Corresponding Source from a network server at no charge, through some
+standard or customary means of facilitating copying of software. This
+Corresponding Source shall include the Corresponding Source for any
+work covered by version 3 of the GNU General Public License that is
+incorporated pursuant to the following paragraph.
+
+Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU General Public License into a single
+combined work, and to convey the resulting work. The terms of this
+License will continue to apply to the part which is the covered work,
+but the work with which it is combined will remain governed by version
+3 of the GNU General Public License.
+
+#### 14. Revised Versions of this License.
+
+The Free Software Foundation may publish revised and/or new versions
+of the GNU Affero General Public License from time to time. Such new
+versions will be similar in spirit to the present version, but may
+differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Program
+specifies that a certain numbered version of the GNU Affero General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation. If the Program does not specify a version number of the
+GNU Affero General Public License, you may choose any version ever
+published by the Free Software Foundation.
+
+If the Program specifies that a proxy can decide which future versions
+of the GNU Affero General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+Later license versions may give you additional or different
+permissions. However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+#### 15. Disclaimer of Warranty.
+
+THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT
+WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT
+LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
+A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND
+PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE
+DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR
+CORRECTION.
+
+#### 16. Limitation of Liability.
+
+IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR
+CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES,
+INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES
+ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT
+NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR
+LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM
+TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER
+PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
+
+#### 17. Interpretation of Sections 15 and 16.
+
+If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+END OF TERMS AND CONDITIONS
+
+### How to Apply These Terms to Your New Programs
+
+If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these
+terms.
+
+To do so, attach the following notices to the program. It is safest to
+attach them to the start of each source file to most effectively state
+the exclusion of warranty; and each file should have at least the
+"copyright" line and a pointer to where the full notice is found.
+
+        Mathactive - K-12 student can learn math from a chatbot that helps them actively solve math problems suitable to their skill level.
+        Copyright (C) 2023  Tangible AI
+
+        This program is free software: you can redistribute it and/or modify
+        it under the terms of the GNU Affero General Public License as
+        published by the Free Software Foundation, either version 3 of the
+        License, or (at your option) any later version.
+
+        This program is distributed in the hope that it will be useful,
+        but WITHOUT ANY WARRANTY; without even the implied warranty of
+        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+        GNU Affero General Public License for more details.
+
+        You should have received a copy of the GNU Affero General Public License
+        along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper
+mail.
+
+If your software can interact with users remotely through a computer
+network, you should also make sure that it provides a way for users to
+get its source. For example, if your program is a web application, its
+interface could display a "Source" link that leads users to an archive
+of the code. There are many ways you could offer source, and different
+solutions will be better for different programs; see section 13 for
+the specific requirements.
+
+You should also get your employer (if you work as a programmer) or
+school, if any, to sign a "copyright disclaimer" for the program, if
+necessary. For more information on this, and how to apply and follow
+the GNU AGPL, see <https://www.gnu.org/licenses/>.
```

### Comparing `convomeld-0.1.3/pyproject.toml` & `convomeld-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-[tool.poetry]
-name = "convomeld"
-version = "0.1.3"
-description = "Parse text scripts or chatbot message logs and merge conversation graphs (Convographs)"
-authors = [
-    "Ruslan Borysov <borysov.ruslan98@gmail.com>",
-    "Hobson Lane <hobson@tangibleai.com>",
-    "Vlad Snisar <vlad@tangibleai.com>",
-    "Cetin Czeckr <cetin@tangibleai.com>",
-]
-license = "AGPL-3.0-or-later"
-readme = "README.md"
-packages = [
-    {include="convomeld", from="src"},
-]
-
-[tool.poetry.dependencies]
-python = "^3.9"
-PyYAML = ">=6.0"
-openpyxl = "*"
-
-[tool.poetry.group.dev.dependencies]
-pytest = ">=7.4.0"
-build = "*"
-pip = "*"
-wheel = "*"
-poetry = "*"
-virtualenv = "*"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.poetry.scripts]
-convocat = "convomeld.convocat:main"
-convoparse = "convomeld.convoparse:main"
+[tool.poetry]
+name = "convomeld"
+version = "0.1.4"
+description = "Parse text scripts or chatbot message logs and merge conversation graphs (Convographs)"
+authors = [
+    "Ruslan Borysov <borysov.ruslan98@gmail.com>",
+    "Hobson Lane <hobson@tangibleai.com>",
+    "Vlad Snisar <vlad@tangibleai.com>",
+    "Cetin Czeckr <cetin@tangibleai.com>",
+]
+license = "AGPL-3.0-or-later"
+readme = "README.md"
+packages = [
+    {include="convomeld", from="src"},
+]
+
+[tool.poetry.dependencies]
+python = ">=3.9"
+PyYAML = ">=6.0"
+openpyxl = "*"
+pandas = "*"
+
+[tool.poetry.group.dev.dependencies]
+pytest = ">=7.4.0"
+build = "*"
+pip = "*"
+wheel = "*"
+poetry = "*"
+virtualenv = "*"
+twine = "*"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+convocat = "convomeld.convocat:main"
+convoparse = "convomeld.convoparse:main"
```

### Comparing `convomeld-0.1.3/src/convomeld/cli.py` & `convomeld-0.1.4/src/convomeld/cli.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import argparse
-import convomeld.graph
-
-
-def cli():
-    parser = argparse.ArgumentParser(
-        prog='ConvoMerge',
-        description='Allows to merge multiptle linear conversation files into single conversation tree'
-    )
-    parser.add_argument('inputs', nargs='+', help='Path(s) to input .txt or .yml linear conversation files')
-    parser.add_argument('-o', '--output', help='Path to output .yml to store the result', required=True)
-    parser.add_argument('-n', '--convo-name')
-    parser.add_argument('-d', '--convo-description')
-    parser.add_argument('-a', '--base-author', default='teacher')
-    args = parser.parse_args()
-    
-    script_files = args.inputs
-    output_file = args.output
-    convo_name = args.convo_name
-    convo_description = args.convo_description
-    base_author = args.base_author
-
-    base_graph = None
-
-    for script_file in script_files:
-        graph = convomeld.graph.ConvoGraph.from_file(script_file, convo_name=convo_name, convo_description=convo_description, base_author=base_author, use_uuid=True)
-
-        if base_graph is None:
-            base_graph = graph
-        else:
-            base_graph = base_graph.merge_graph(graph)
-        
-    base_graph.to_yaml(output_file)
-
+import argparse
+import convomeld.graph
+
+
+def cli():
+    parser = argparse.ArgumentParser(
+        prog='ConvoMerge',
+        description='Allows to merge multiptle linear conversation files into single conversation tree'
+    )
+    parser.add_argument('inputs', nargs='+', help='Path(s) to input .txt or .yml linear conversation files')
+    parser.add_argument('-o', '--output', help='Path to output .yml to store the result', required=True)
+    parser.add_argument('-n', '--convo-name')
+    parser.add_argument('-d', '--convo-description')
+    parser.add_argument('-a', '--base-author', default='teacher')
+    args = parser.parse_args()
+    
+    script_files = args.inputs
+    output_file = args.output
+    convo_name = args.convo_name
+    convo_description = args.convo_description
+    base_author = args.base_author
+
+    base_graph = None
+
+    for script_file in script_files:
+        graph = convomeld.graph.ConvoGraph.from_file(script_file, convo_name=convo_name, convo_description=convo_description, base_author=base_author, use_uuid=True)
+
+        if base_graph is None:
+            base_graph = graph
+        else:
+            base_graph = base_graph.merge_graph(graph)
+        
+    base_graph.to_yaml(output_file)
+
```

### Comparing `convomeld-0.1.3/src/convomeld/convocat.py` & `convomeld-0.1.4/src/convomeld/convocat.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import argparse
-import os
-
-from convomeld.df_to_convograph import (
-    yml_parse_create_single_convograph,
-)
-from convomeld.xlsx_csv_parsers import YAMLFileNamesParser
-from convomeld.utils import YAMLWriter
-from convomeld.sorters import YAMLFileNamesSorter
-
-
-def main():
-    parser = argparse.ArgumentParser(
-        description="Concatenate YAML files in a folder."
-    )
-    parser.add_argument(
-        "file_paths",
-        nargs="+",
-        help="Paths to the YAML files or folders containing YAML files.",
-    )
-    parser.add_argument(
-        "--dest_folder",
-        "-d",
-        help="Path to the destination folder where concatenated YAML file will be created.",
-    )
-    args = parser.parse_args()
-
-    files_names_parser = YAMLFileNamesParser()
-    file_names_file_paths = files_names_parser.parse(args.file_paths)
-
-    if not file_names_file_paths:
-        print("No valid YAML files found in the provided paths.")
-        return
-
-    files_names_sorter = YAMLFileNamesSorter()
-    sorted_file_names = files_names_sorter.sort(file_names_file_paths.keys())
-
-    start_convograph = yml_parse_create_single_convograph(
-        file_path=file_names_file_paths[sorted_file_names[0]]
-    )
-
-    for file_name in sorted_file_names[1:]:
-        next_convograph = yml_parse_create_single_convograph(
-            file_path=file_names_file_paths[file_name]
-        )
-        start_convograph += next_convograph
-
-    if args.dest_folder:
-        YAMLWriter.write_convograph_to_yaml_file(
-            start_convograph.to_list_of_dicts(), file_path=args.dest_folder
-        )
-    else:
-        YAMLWriter.write_convograph_to_yaml_file(
-            start_convograph.to_list_of_dicts(), file_path=os.getcwd()
-        )
-
-
-if __name__ == "__main__":
-    main()
+import argparse
+import os
+
+from convomeld.df_to_convograph import (
+    yml_parse_create_single_convograph,
+)
+from convomeld.xlsx_csv_parsers import YAMLFileNamesParser
+from convomeld.utils import YAMLWriter
+from convomeld.sorters import YAMLFileNamesSorter
+
+
+def main():
+    parser = argparse.ArgumentParser(
+        description="Concatenate YAML files in a folder."
+    )
+    parser.add_argument(
+        "file_paths",
+        nargs="+",
+        help="Paths to the YAML files or folders containing YAML files.",
+    )
+    parser.add_argument(
+        "--dest_folder",
+        "-d",
+        help="Path to the destination folder where concatenated YAML file will be created.",
+    )
+    args = parser.parse_args()
+
+    files_names_parser = YAMLFileNamesParser()
+    file_names_file_paths = files_names_parser.parse(args.file_paths)
+
+    if not file_names_file_paths:
+        print("No valid YAML files found in the provided paths.")
+        return
+
+    files_names_sorter = YAMLFileNamesSorter()
+    sorted_file_names = files_names_sorter.sort(file_names_file_paths.keys())
+
+    start_convograph = yml_parse_create_single_convograph(
+        file_path=file_names_file_paths[sorted_file_names[0]]
+    )
+
+    for file_name in sorted_file_names[1:]:
+        next_convograph = yml_parse_create_single_convograph(
+            file_path=file_names_file_paths[file_name]
+        )
+        start_convograph += next_convograph
+
+    if args.dest_folder:
+        YAMLWriter.write_convograph_to_yaml_file(
+            start_convograph.to_list_of_dicts(), file_path=args.dest_folder
+        )
+    else:
+        YAMLWriter.write_convograph_to_yaml_file(
+            start_convograph.to_list_of_dicts(), file_path=os.getcwd()
+        )
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `convomeld-0.1.3/src/convomeld/convoparse.py` & `convomeld-0.1.4/src/convomeld/convoparse.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import argparse
-import os
-
-from convomeld.df_to_convograph import create_convograph
-from convomeld.xlsx_csv_parsers import ConvoDataParser
-from convomeld.utils import YAMLWriter
-
-
-def main():
-    parser = argparse.ArgumentParser(
-        description="Parse XLSX and CSV files in a folder, create convo_graphs and convert them to YAML files."
-    )
-    parser.add_argument(
-        "file_paths",
-        nargs="+",
-        help="Paths to the XLSX or CSV files containing convo_graph specific format data",
-    )
-    parser.add_argument(
-        "--dest_folder",
-        "-d",
-        help="Path to the destination folder where YAML files will be created.",
-    )
-
-    args = parser.parse_args()
-
-    parsed_dfs = []
-    parsed_worksheet_names = []
-    parser = ConvoDataParser()
-
-    for file_path in args.file_paths:
-        dfs, worksheet_names = parser.parse(file_path=file_path)
-        parsed_dfs.extend(dfs)
-        parsed_worksheet_names.extend(worksheet_names)
-
-    worksheet_names_dfs = dict(zip(parsed_worksheet_names, parsed_dfs))
-
-    for worksheet_name in worksheet_names_dfs.keys():
-        convo_graph = create_convograph(
-            worksheet_names_dfs[worksheet_name], worksheet_name
-        )
-        if args.dest_folder:
-            YAMLWriter.write_convograph_to_yaml_file(
-                convo_graph.to_list_of_dicts(), file_path=args.dest_folder
-            )
-        else:
-            YAMLWriter.write_convograph_to_yaml_file(
-                convo_graph.to_list_of_dicts(), file_path=os.getcwd()
-            )
-
-
-if __name__ == "__main__":
-    main()
+import argparse
+import os
+
+from convomeld.df_to_convograph import create_convograph
+from convomeld.xlsx_csv_parsers import ConvoDataParser
+from convomeld.utils import YAMLWriter
+
+
+def main():
+    parser = argparse.ArgumentParser(
+        description="Parse XLSX and CSV files in a folder, create convo_graphs and convert them to YAML files."
+    )
+    parser.add_argument(
+        "file_paths",
+        nargs="+",
+        help="Paths to the XLSX or CSV files containing convo_graph specific format data",
+    )
+    parser.add_argument(
+        "--dest_folder",
+        "-d",
+        help="Path to the destination folder where YAML files will be created.",
+    )
+
+    args = parser.parse_args()
+
+    parsed_dfs = []
+    parsed_worksheet_names = []
+    parser = ConvoDataParser()
+
+    for file_path in args.file_paths:
+        dfs, worksheet_names = parser.parse(file_path=file_path)
+        parsed_dfs.extend(dfs)
+        parsed_worksheet_names.extend(worksheet_names)
+
+    worksheet_names_dfs = dict(zip(parsed_worksheet_names, parsed_dfs))
+
+    for worksheet_name in worksheet_names_dfs.keys():
+        convo_graph = create_convograph(
+            worksheet_names_dfs[worksheet_name], worksheet_name
+        )
+        if args.dest_folder:
+            YAMLWriter.write_convograph_to_yaml_file(
+                convo_graph.to_list_of_dicts(), file_path=args.dest_folder
+            )
+        else:
+            YAMLWriter.write_convograph_to_yaml_file(
+                convo_graph.to_list_of_dicts(), file_path=os.getcwd()
+            )
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `convomeld-0.1.3/src/convomeld/data_factory.py` & `convomeld-0.1.4/src/convomeld/data_factory.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,229 +1,229 @@
-from typing import Union
-
-from convomeld.states import (
-    ConvoStartState,
-    ConvoStopState,
-    ConvoAnswerState,
-    ConvoQuestionState,
-    ConvoInstructionState,
-    ConvoIntroductionState,
-)
-
-
-def create_convo_start_state(
-    worksheet_name: str, convo_description: str
-) -> ConvoStartState:
-    """Creates structure of the first block of convo which has 'start' state.
-    Accepting already parsed worksheets and descriptions of microlessons.
-
-    Args:
-        sheet_names_sorted (list): Sequence of worksheets after sorting process
-        microlesson_convo_descriptions (list): Sequence of microlessons descriptions
-
-    Returns:
-        list: Sequence of dict which has predefined structure of convo start block.
-        I used list here because later I am smashing lists of different elements together including this one
-    """
-
-    name = "start"
-    convo_name = f"{worksheet_name}"
-    convo_description = f"{convo_description.lower()}"
-    nlp = "case_insensitive"
-    actions = {"en": [convo_description.capitalize()]}
-    triggers = {
-        "en": {
-            "__next__": f"{worksheet_name}-introduction",
-        }
-    }
-
-    return ConvoStartState(
-        name=name,
-        convo_name=convo_name,
-        convo_description=convo_description,
-        nlp=nlp,
-        actions=actions,
-        triggers=triggers,
-    )
-
-
-def create_convo_introduction_state(
-    microlesson_introduction_data: list, worksheet_name: str
-) -> ConvoIntroductionState:
-    """Creates microlesspn-introduction structure for single microlesson
-
-    Args:
-        microlesson_introduction_data (list): Data from first row in microlesson worksheet
-        worksheet_name (str): Name of worksheet
-
-    Returns:
-        Union[dict, None]: Dictionary of prefedined keys:values.
-        If there is no welcome_message in microlesson worksheet than block is redundant
-    """
-
-    introduction_message = microlesson_introduction_data[1]
-
-    name = f"{worksheet_name}-introduction"
-    level = 0
-    actions = {"en": [introduction_message.strip()]}
-    triggers = {
-        "en": {
-            "__next__": f"{worksheet_name}-instruction",
-        }
-    }
-
-    return ConvoIntroductionState(
-        name=name,
-        level=level,
-        actions=actions,
-        triggers=triggers,
-    )
-
-
-def create_convo_instruction_state(
-    microlesson_instruction_data: list, worksheet_name: str
-) -> ConvoInstructionState:
-    """Creates microlesson-instruction  structure for single microlesson
-
-    Args:
-        microlesson_instruction_data (list): Data from first row in microlesson worksheet
-        worksheet_name (str): Name of worksheet
-
-    Returns:
-        Union[dict, None]: Dictionary of prefedined keys:values.
-        If there is no instruction message in microlesson worksheet than block is redundant
-    """
-
-    instruction_message = microlesson_instruction_data[3]
-
-    name = f"{worksheet_name}-instruction"
-    level = 0
-    actions = {"en": [instruction_message]}
-    buttons = {"en": {"OK": f"{worksheet_name}/q1"}}
-    triggers = {
-        "en": {
-            str(
-                microlesson_instruction_data[4]
-            ).title(): f"{worksheet_name}/{microlesson_instruction_data[2].lower()}",
-            "__default__": name,
-        }
-    }
-
-    return ConvoInstructionState(
-        name=name,
-        level=level,
-        actions=actions,
-        buttons=buttons,
-        triggers=triggers,
-    )
-
-
-def create_convo_question(
-    question_raw_data: list, statenum: int, worksheet_name: str
-) -> ConvoQuestionState:
-    """Creates microlesson question worksheet_data structure
-
-    Args:
-      question_raw_data (list): Question data from microlesson worksheet
-      statenum (int): Order number in sequence of questions
-      worksheet_name (str): Name of microlesson's worksheet
-
-    Returns:
-      dict: Predefined keys:values for microlesson's single question worksheet_data
-    """
-
-    # Represent pictures with chosen format.Link should be on column #8
-    actions_data = [question_raw_data[3]]
-    if question_raw_data[7] and question_raw_data[7] != "-":
-        question_image = f"[Image]({question_raw_data[7]})"
-        actions_data.append(question_image)
-
-    name = f"{worksheet_name}/q{statenum}"
-    level = statenum
-    actions = {"en": actions_data}
-    buttons = {"en": {"OK": f"{worksheet_name}/q{statenum}"}}
-    triggers = {
-        "en": {
-            str(question_raw_data[4])
-            .title()
-            .strip(): f"correct-answer-{worksheet_name}/q{statenum}",
-            "__default__": f"wrong-answer-{worksheet_name}/q{statenum}",
-        }
-    }
-
-    return ConvoQuestionState(
-        name=name,
-        level=level,
-        actions=actions,
-        buttons=buttons,
-        triggers=triggers,
-    )
-
-
-def create_convo_wrong_answer_state(
-    statenum: int, worksheet_name: str
-) -> ConvoAnswerState:
-    """Creates microlesson's question wrong answer structure
-
-    Args:
-        statenum (int): Order number in sequence of questions
-        worksheet_name (str): Name of microlesson's worksheet
-
-    Returns:
-        dict: Predefined keys:values for microlesson's single question wrong answer
-    """
-
-    name = f"wrong-answer-{worksheet_name}/q{statenum}"
-    actions = {"en": ["Oops! That's not correct. Let's try again."]}
-    triggers = {"en": {"__next__": f"{worksheet_name}/q{statenum}"}}
-
-    return ConvoAnswerState(
-        name=name,
-        actions=actions,
-        triggers=triggers,
-    )
-
-
-def create_convo_correct_answer_state(
-    statenum: int,
-    worksheet_name: str,
-    stop_state_next: Union[bool, None] = False,
-) -> ConvoAnswerState:
-    """Creates microlesson's question correct answer structure
-
-    Args:
-        statenum (int): Order number in sequence of questions
-        worksheet_name (str): Name of microlesson's worksheet
-        stop_state_next (Union[bool, None], optional): Defines end question of particular microlesson. Defaults to False.
-
-    Returns:
-        dict: Predefined keys:values for microlesson's single question correct answer
-    """
-
-    name = f"correct-answer-{worksheet_name}/q{statenum}"
-    actions = {"en": ["Perfect!"]}
-    triggers = {
-        "en": {
-            "__next__": f"{worksheet_name}/q{statenum + 1}"
-            if not stop_state_next
-            else f"stop"
-        }
-    }
-
-    return ConvoAnswerState(
-        name=name,
-        actions=actions,
-        triggers=triggers,
-    )
-
-
-def create_convo_stop_state(convo_name: str) -> ConvoStopState:
-    triggers = {"en": {"__default__": "start"}}
-    actions = {
-        "en": [
-            f"Congratulations, you have completed the {convo_name} micro-lesson."
-            f"You can start over or choose another practice. Click 'Repeat' to complete {convo_name} "
-            f"micro-lesson one more time"
-        ]
-    }
-
-    return ConvoStopState(triggers=triggers, actions=actions)
+from typing import Union
+
+from convomeld.states import (
+    ConvoStartState,
+    ConvoStopState,
+    ConvoAnswerState,
+    ConvoQuestionState,
+    ConvoInstructionState,
+    ConvoIntroductionState,
+)
+
+
+def create_convo_start_state(
+    worksheet_name: str, convo_description: str
+) -> ConvoStartState:
+    """Creates structure of the first block of convo which has 'start' state.
+    Accepting already parsed worksheets and descriptions of microlessons.
+
+    Args:
+        sheet_names_sorted (list): Sequence of worksheets after sorting process
+        microlesson_convo_descriptions (list): Sequence of microlessons descriptions
+
+    Returns:
+        list: Sequence of dict which has predefined structure of convo start block.
+        I used list here because later I am smashing lists of different elements together including this one
+    """
+
+    name = "start"
+    convo_name = f"{worksheet_name}"
+    convo_description = f"{convo_description.lower()}"
+    nlp = "case_insensitive"
+    actions = {"en": [convo_description.capitalize()]}
+    triggers = {
+        "en": {
+            "__next__": f"{worksheet_name}-introduction",
+        }
+    }
+
+    return ConvoStartState(
+        name=name,
+        convo_name=convo_name,
+        convo_description=convo_description,
+        nlp=nlp,
+        actions=actions,
+        triggers=triggers,
+    )
+
+
+def create_convo_introduction_state(
+    microlesson_introduction_data: list, worksheet_name: str
+) -> ConvoIntroductionState:
+    """Creates microlesspn-introduction structure for single microlesson
+
+    Args:
+        microlesson_introduction_data (list): Data from first row in microlesson worksheet
+        worksheet_name (str): Name of worksheet
+
+    Returns:
+        Union[dict, None]: Dictionary of prefedined keys:values.
+        If there is no welcome_message in microlesson worksheet than block is redundant
+    """
+
+    introduction_message = microlesson_introduction_data[1]
+
+    name = f"{worksheet_name}-introduction"
+    level = 0
+    actions = {"en": [introduction_message.strip()]}
+    triggers = {
+        "en": {
+            "__next__": f"{worksheet_name}-instruction",
+        }
+    }
+
+    return ConvoIntroductionState(
+        name=name,
+        level=level,
+        actions=actions,
+        triggers=triggers,
+    )
+
+
+def create_convo_instruction_state(
+    microlesson_instruction_data: list, worksheet_name: str
+) -> ConvoInstructionState:
+    """Creates microlesson-instruction  structure for single microlesson
+
+    Args:
+        microlesson_instruction_data (list): Data from first row in microlesson worksheet
+        worksheet_name (str): Name of worksheet
+
+    Returns:
+        Union[dict, None]: Dictionary of prefedined keys:values.
+        If there is no instruction message in microlesson worksheet than block is redundant
+    """
+
+    instruction_message = microlesson_instruction_data[3]
+
+    name = f"{worksheet_name}-instruction"
+    level = 0
+    actions = {"en": [instruction_message]}
+    buttons = {"en": {"OK": f"{worksheet_name}/q1"}}
+    triggers = {
+        "en": {
+            str(
+                microlesson_instruction_data[4]
+            ).title(): f"{worksheet_name}/{microlesson_instruction_data[2].lower()}",
+            "__default__": name,
+        }
+    }
+
+    return ConvoInstructionState(
+        name=name,
+        level=level,
+        actions=actions,
+        buttons=buttons,
+        triggers=triggers,
+    )
+
+
+def create_convo_question(
+    question_raw_data: list, statenum: int, worksheet_name: str
+) -> ConvoQuestionState:
+    """Creates microlesson question worksheet_data structure
+
+    Args:
+      question_raw_data (list): Question data from microlesson worksheet
+      statenum (int): Order number in sequence of questions
+      worksheet_name (str): Name of microlesson's worksheet
+
+    Returns:
+      dict: Predefined keys:values for microlesson's single question worksheet_data
+    """
+
+    # Represent pictures with chosen format.Link should be on column #8
+    actions_data = [question_raw_data[3]]
+    if question_raw_data[7] and question_raw_data[7] != "-":
+        question_image = f"[Image]({question_raw_data[7]})"
+        actions_data.append(question_image)
+
+    name = f"{worksheet_name}/q{statenum}"
+    level = statenum
+    actions = {"en": actions_data}
+    buttons = {"en": {"OK": f"{worksheet_name}/q{statenum}"}}
+    triggers = {
+        "en": {
+            str(question_raw_data[4])
+            .title()
+            .strip(): f"correct-answer-{worksheet_name}/q{statenum}",
+            "__default__": f"wrong-answer-{worksheet_name}/q{statenum}",
+        }
+    }
+
+    return ConvoQuestionState(
+        name=name,
+        level=level,
+        actions=actions,
+        buttons=buttons,
+        triggers=triggers,
+    )
+
+
+def create_convo_wrong_answer_state(
+    statenum: int, worksheet_name: str
+) -> ConvoAnswerState:
+    """Creates microlesson's question wrong answer structure
+
+    Args:
+        statenum (int): Order number in sequence of questions
+        worksheet_name (str): Name of microlesson's worksheet
+
+    Returns:
+        dict: Predefined keys:values for microlesson's single question wrong answer
+    """
+
+    name = f"wrong-answer-{worksheet_name}/q{statenum}"
+    actions = {"en": ["Oops! That's not correct. Let's try again."]}
+    triggers = {"en": {"__next__": f"{worksheet_name}/q{statenum}"}}
+
+    return ConvoAnswerState(
+        name=name,
+        actions=actions,
+        triggers=triggers,
+    )
+
+
+def create_convo_correct_answer_state(
+    statenum: int,
+    worksheet_name: str,
+    stop_state_next: Union[bool, None] = False,
+) -> ConvoAnswerState:
+    """Creates microlesson's question correct answer structure
+
+    Args:
+        statenum (int): Order number in sequence of questions
+        worksheet_name (str): Name of microlesson's worksheet
+        stop_state_next (Union[bool, None], optional): Defines end question of particular microlesson. Defaults to False.
+
+    Returns:
+        dict: Predefined keys:values for microlesson's single question correct answer
+    """
+
+    name = f"correct-answer-{worksheet_name}/q{statenum}"
+    actions = {"en": ["Perfect!"]}
+    triggers = {
+        "en": {
+            "__next__": f"{worksheet_name}/q{statenum + 1}"
+            if not stop_state_next
+            else f"stop"
+        }
+    }
+
+    return ConvoAnswerState(
+        name=name,
+        actions=actions,
+        triggers=triggers,
+    )
+
+
+def create_convo_stop_state(convo_name: str) -> ConvoStopState:
+    triggers = {"en": {"__default__": "start"}}
+    actions = {
+        "en": [
+            f"Congratulations, you have completed the {convo_name} micro-lesson."
+            f"You can start over or choose another practice. Click 'Repeat' to complete {convo_name} "
+            f"micro-lesson one more time"
+        ]
+    }
+
+    return ConvoStopState(triggers=triggers, actions=actions)
```

### Comparing `convomeld-0.1.3/src/convomeld/df_to_convograph.py` & `convomeld-0.1.4/src/convomeld/df_to_convograph.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-from pandas import DataFrame
-
-from convomeld.xlsx_csv_parsers import ConvoDataParser
-from convomeld.states import ConvoGraph
-from convomeld.data_factory import (
-    create_convo_stop_state,
-    create_convo_start_state,
-    create_convo_question,
-    create_convo_instruction_state,
-    create_convo_introduction_state,
-    create_convo_correct_answer_state,
-    create_convo_wrong_answer_state,
-)
-
-
-def create_convograph(df: DataFrame, worksheet_name: str) -> ConvoGraph:
-    data_from_df = df.values.tolist()
-    convo_graph = ConvoGraph(worksheet_name_source_data=worksheet_name)
-    convo_graph.add_state(
-        create_convo_start_state(
-            worksheet_name=worksheet_name,
-            convo_description=f"A lesson about {data_from_df[0][0].lower()}",
-        )
-    )
-
-    microlesson_welcome_data: list[str] = data_from_df[0]
-    convo_graph.add_state(
-        create_convo_introduction_state(
-            microlesson_welcome_data, worksheet_name=worksheet_name
-        )
-    )
-    convo_graph.add_state(
-        create_convo_instruction_state(
-            microlesson_welcome_data, worksheet_name=worksheet_name
-        )
-    )
-
-    for statenum, question_state in enumerate(data_from_df[1:], 1):
-        convo_graph.add_state(
-            create_convo_question(
-                question_raw_data=question_state,
-                statenum=statenum,
-                worksheet_name=worksheet_name,
-            )
-        )
-        convo_graph.add_state(
-            create_convo_wrong_answer_state(
-                statenum=statenum, worksheet_name=worksheet_name
-            )
-        )
-        if statenum == len(data_from_df) - 1:
-            convo_graph.add_state(
-                create_convo_correct_answer_state(
-                    statenum=statenum,
-                    worksheet_name=worksheet_name,
-                    stop_state_next=True,
-                )
-            )
-        else:
-            convo_graph.add_state(
-                create_convo_correct_answer_state(
-                    statenum=statenum, worksheet_name=worksheet_name
-                )
-            )
-    microlesson_name = data_from_df[0][0]
-    convo_graph.add_state(create_convo_stop_state(microlesson_name))
-    return convo_graph
-
-
-def yml_parse_create_single_convograph(file_path: str) -> ConvoGraph:
-    parser = ConvoDataParser()
-    dfs, worksheet_names = parser.parse(file_path=file_path)
-
-    for index, df in enumerate(dfs):
-        convo_graph = ConvoGraph(
-            worksheet_name_source_data=worksheet_names[index]
-        )
-        convo_graph.populate_convo(df)
-
-    return convo_graph
+from pandas import DataFrame
+
+from convomeld.xlsx_csv_parsers import ConvoDataParser
+from convomeld.states import ConvoGraph
+from convomeld.data_factory import (
+    create_convo_stop_state,
+    create_convo_start_state,
+    create_convo_question,
+    create_convo_instruction_state,
+    create_convo_introduction_state,
+    create_convo_correct_answer_state,
+    create_convo_wrong_answer_state,
+)
+
+
+def create_convograph(df: DataFrame, worksheet_name: str) -> ConvoGraph:
+    data_from_df = df.values.tolist()
+    convo_graph = ConvoGraph(worksheet_name_source_data=worksheet_name)
+    convo_graph.add_state(
+        create_convo_start_state(
+            worksheet_name=worksheet_name,
+            convo_description=f"A lesson about {data_from_df[0][0].lower()}",
+        )
+    )
+
+    microlesson_welcome_data: list[str] = data_from_df[0]
+    convo_graph.add_state(
+        create_convo_introduction_state(
+            microlesson_welcome_data, worksheet_name=worksheet_name
+        )
+    )
+    convo_graph.add_state(
+        create_convo_instruction_state(
+            microlesson_welcome_data, worksheet_name=worksheet_name
+        )
+    )
+
+    for statenum, question_state in enumerate(data_from_df[1:], 1):
+        convo_graph.add_state(
+            create_convo_question(
+                question_raw_data=question_state,
+                statenum=statenum,
+                worksheet_name=worksheet_name,
+            )
+        )
+        convo_graph.add_state(
+            create_convo_wrong_answer_state(
+                statenum=statenum, worksheet_name=worksheet_name
+            )
+        )
+        if statenum == len(data_from_df) - 1:
+            convo_graph.add_state(
+                create_convo_correct_answer_state(
+                    statenum=statenum,
+                    worksheet_name=worksheet_name,
+                    stop_state_next=True,
+                )
+            )
+        else:
+            convo_graph.add_state(
+                create_convo_correct_answer_state(
+                    statenum=statenum, worksheet_name=worksheet_name
+                )
+            )
+    microlesson_name = data_from_df[0][0]
+    convo_graph.add_state(create_convo_stop_state(microlesson_name))
+    return convo_graph
+
+
+def yml_parse_create_single_convograph(file_path: str) -> ConvoGraph:
+    parser = ConvoDataParser()
+    dfs, worksheet_names = parser.parse(file_path=file_path)
+
+    for index, df in enumerate(dfs):
+        convo_graph = ConvoGraph(
+            worksheet_name_source_data=worksheet_names[index]
+        )
+        convo_graph.populate_convo(df)
+
+    return convo_graph
```

### Comparing `convomeld-0.1.3/src/convomeld/sorters.py` & `convomeld-0.1.4/src/convomeld/sorters.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-import re
-from abc import ABC, abstractmethod
-
-
-class Sorter(ABC):
-    @abstractmethod
-    def sort(self, input_data: list[str]):
-        pass
-
-
-class WorkSheetsSorter(Sorter):
-    def sort(self, worksheets) -> list:
-        """Sorts worksheets in provided workbook with predefined lesson order logic
-
-        Args:
-            workbook (openpyxl.Workbook): Loaded .xlsx file
-
-        Returns:
-            None: Blank return
-        """
-
-        pattern = r"G(\d+)[._](\w+)[._](\d+)[._](\d+)[._](\d+)"
-
-        grouped_lessons = {}
-
-        for sheet_name in worksheets:
-            match = re.search(pattern, sheet_name)
-            if match:
-                grade = int(match.group(1))
-                domain = match.group(2)
-                n1 = int(match.group(3))
-                n2 = int(match.group(4))
-                n3 = int(match.group(5))
-
-                if domain not in grouped_lessons:
-                    grouped_lessons[domain] = []
-
-                grouped_lessons[domain].append((sheet_name, grade, n1, n2, n3))
-
-        sorted_worksheets = []
-
-        for _, lessons in sorted(grouped_lessons.items()):
-            sorted_lessons = sorted(
-                lessons, key=lambda x: (x[1], x[2], x[3], x[4])
-            )
-            sorted_worksheets.extend(
-                [sheet_name for sheet_name, _, _, _, _ in sorted_lessons]
-            )
-
-        return sorted_worksheets
-
-
-class YAMLFileNamesSorter(Sorter):
-    def sort(self, file_names) -> list:
-        """Sorts list of .yml file_names in predefined order logic
-
-        Args:
-            file_names (list): Unsorted list of file_names
-
-        Returns:
-            list: Sorted list of file_names
-        """
-
-        pattern = r"G(\d+)[._](\w+)[._](\d+)[._](\d+)[._](\d+)"
-
-        grouped_file_names = {}
-
-        other_file_names_different_format = []
-
-        for file_name in file_names:
-            match = re.search(pattern, file_name)
-            if match:
-                grade = int(match.group(1))
-                domain = match.group(2)
-                n1 = int(match.group(3))
-                n2 = int(match.group(4))
-                n3 = int(match.group(5))
-
-                if domain not in grouped_file_names:
-                    grouped_file_names[domain] = []
-
-                grouped_file_names[domain].append(
-                    (file_name, grade, n1, n2, n3)
-                )
-            else:
-                other_file_names_different_format.append(file_name)
-        sorted_file_names = []
-
-        for _, lessons in sorted(grouped_file_names.items()):
-            sorted_lessons = sorted(
-                lessons, key=lambda x: (x[1], x[2], x[3], x[4])
-            )
-            sorted_file_names.extend(
-                [sheet_name for sheet_name, _, _, _, _ in sorted_lessons]
-            )
-
-        sorted_file_names.extend(other_file_names_different_format)
-
-        return sorted_file_names
+import re
+from abc import ABC, abstractmethod
+
+
+class Sorter(ABC):
+    @abstractmethod
+    def sort(self, input_data: list[str]):
+        pass
+
+
+class WorkSheetsSorter(Sorter):
+    def sort(self, worksheets) -> list:
+        """Sorts worksheets in provided workbook with predefined lesson order logic
+
+        Args:
+            workbook (openpyxl.Workbook): Loaded .xlsx file
+
+        Returns:
+            None: Blank return
+        """
+
+        pattern = r"G(\d+)[._](\w+)[._](\d+)[._](\d+)[._](\d+)"
+
+        grouped_lessons = {}
+
+        for sheet_name in worksheets:
+            match = re.search(pattern, sheet_name)
+            if match:
+                grade = int(match.group(1))
+                domain = match.group(2)
+                n1 = int(match.group(3))
+                n2 = int(match.group(4))
+                n3 = int(match.group(5))
+
+                if domain not in grouped_lessons:
+                    grouped_lessons[domain] = []
+
+                grouped_lessons[domain].append((sheet_name, grade, n1, n2, n3))
+
+        sorted_worksheets = []
+
+        for _, lessons in sorted(grouped_lessons.items()):
+            sorted_lessons = sorted(
+                lessons, key=lambda x: (x[1], x[2], x[3], x[4])
+            )
+            sorted_worksheets.extend(
+                [sheet_name for sheet_name, _, _, _, _ in sorted_lessons]
+            )
+
+        return sorted_worksheets
+
+
+class YAMLFileNamesSorter(Sorter):
+    def sort(self, file_names) -> list:
+        """Sorts list of .yml file_names in predefined order logic
+
+        Args:
+            file_names (list): Unsorted list of file_names
+
+        Returns:
+            list: Sorted list of file_names
+        """
+
+        pattern = r"G(\d+)[._](\w+)[._](\d+)[._](\d+)[._](\d+)"
+
+        grouped_file_names = {}
+
+        other_file_names_different_format = []
+
+        for file_name in file_names:
+            match = re.search(pattern, file_name)
+            if match:
+                grade = int(match.group(1))
+                domain = match.group(2)
+                n1 = int(match.group(3))
+                n2 = int(match.group(4))
+                n3 = int(match.group(5))
+
+                if domain not in grouped_file_names:
+                    grouped_file_names[domain] = []
+
+                grouped_file_names[domain].append(
+                    (file_name, grade, n1, n2, n3)
+                )
+            else:
+                other_file_names_different_format.append(file_name)
+        sorted_file_names = []
+
+        for _, lessons in sorted(grouped_file_names.items()):
+            sorted_lessons = sorted(
+                lessons, key=lambda x: (x[1], x[2], x[3], x[4])
+            )
+            sorted_file_names.extend(
+                [sheet_name for sheet_name, _, _, _, _ in sorted_lessons]
+            )
+
+        sorted_file_names.extend(other_file_names_different_format)
+
+        return sorted_file_names
```

### Comparing `convomeld-0.1.3/src/convomeld/states.py` & `convomeld-0.1.4/src/convomeld/states.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-class ToDictMixin:
-    def to_dict(self):
-        return self.__dict__
-
-
-class ConvoStartState(ToDictMixin):
-    """Conversation Start State."""
-
-    def __init__(
-        self,
-        convo_name: str,
-        convo_description: str,
-        nlp: str,
-        actions: dict[str, list[str]],
-        triggers: dict[str, dict[str, str]],
-        name: str = "start",
-    ):
-        self.name = name
-        self.convo_name = convo_name
-        self.convo_description = convo_description
-        self.nlp = nlp
-        self.actions = actions
-        self.triggers = triggers
-
-
-class ConvoStopState(ToDictMixin):
-    """Conversation Stop State."""
-
-    def __init__(
-        self,
-        actions: dict,
-        triggers: dict[str, dict[str, str]],
-        name: str = "stop",
-    ):
-        self.name = name
-        self.actions = actions
-        self.triggers = triggers
-
-
-class ConvoIntroductionState(ToDictMixin):
-    def __init__(
-        self,
-        name: str,
-        level: int,
-        actions: dict[str, dict[str, str]],
-        triggers: dict[str, dict[str, str]],
-    ):
-        self.name = name
-        self.level = level
-        self.actions = actions
-        self.triggers = triggers
-
-
-class ConvoInstructionState(ToDictMixin):
-    def __init__(
-        self,
-        name: str,
-        level: int,
-        actions: dict[str, dict[str, str]],
-        buttons: dict[str, dict[str, str]],
-        triggers: dict[str, dict[str, str]],
-    ):
-        self.name = name
-        self.level = level
-        self.actions = actions
-        self.buttons = buttons
-        self.triggers = triggers
-
-
-class ConvoQuestionState(ToDictMixin):
-    def __init__(
-        self,
-        name: str,
-        actions: dict[str, list],
-        level: int = 0,
-        buttons: dict[str, dict[str, str]] = {},
-        triggers: dict[str, dict[str, str]] = {},
-    ):
-        self.name = name
-        self.level = level
-        self.actions = actions
-        if buttons:
-            self.buttons = buttons
-        if triggers:
-            self.triggers = triggers
-
-
-class ConvoAnswerState(ToDictMixin):
-    def __init__(
-        self,
-        name: str,
-        actions: dict[str, list[str]],
-        triggers: dict[str, dict[str, str]],
-    ):
-        self.name = name
-        self.actions = actions
-        self.triggers = triggers
-
-
-class ConvoGraph:
-    def __init__(self, worksheet_name_source_data: str):
-        self.__states = []
-        self.__current_convo_name = worksheet_name_source_data
-
-    def add_state(self, state):
-        self.__states.append(state)
-
-    def __add__(self, other_convo_graph):
-        if not isinstance(other_convo_graph, ConvoGraph):
-            raise ValueError("You can concatenate only ConvoGraph objects")
-
-        def update_start_state():
-            other_convo_start_state = other_convo_graph.__states[0]
-            self.__states[0].convo_description += (
-                "/" + other_convo_start_state.convo_description
-            )
-            self.__states[0].convo_name += (
-                "__" + other_convo_start_state.convo_name
-            )
-
-        def update_stop_state():
-            self.__states[-1].name = f"stop-{self.__current_convo_name}"
-
-            # Handle function for state before StopState
-            if "__next__" in self.__states[-2].triggers["en"]:
-                self.__states[-2].triggers["en"]["__next__"] = self.__states[
-                    -1
-                ].name
-            else:
-                for key, value in self.__states[-2].triggers["en"].items():
-                    if (
-                        key not in ["__default__", "__next__"]
-                        and self.__states[-2].triggers["en"][key] == "stop"
-                    ):
-                        self.__states[-2].triggers["en"][key] = self.__states[
-                            -1
-                        ].name
-            self.__states[-1].triggers["en"][
-                "__default__"
-            ] = f"{other_convo_graph.__states[0].convo_name}-introduction"
-
-        def concatenate_states():
-            # Exclude start state of other Convo
-            states_copy = other_convo_graph.__states[1:]
-            self.__states.extend(states_copy)
-
-        update_start_state()
-        update_stop_state()
-        concatenate_states()
-
-        self.__current_convo_name = other_convo_graph.__current_convo_name
-
-        return self
-
-    def to_list_of_dicts(self):
-        return [state.to_dict() for state in self.__states]
-
-    def populate_convo(self, data: list):
-        for state in data:
-            if "start" in state["name"]:
-                self.__states.append(ConvoStartState(**state))
-            elif "introduction" in state["name"]:
-                self.__states.append(ConvoIntroductionState(**state))
-            elif "instruction" in state["name"]:
-                self.__states.append(ConvoInstructionState(**state))
-            elif "answer" in state["name"]:
-                self.__states.append(ConvoAnswerState(**state))
-            elif "stop" in state["name"]:
-                self.__states.append(ConvoStopState(**state))
-            else:
-                self.__states.append(ConvoQuestionState(**state))
+class ToDictMixin:
+    def to_dict(self):
+        return self.__dict__
+
+
+class ConvoStartState(ToDictMixin):
+    """Conversation Start State."""
+
+    def __init__(
+        self,
+        convo_name: str,
+        convo_description: str,
+        nlp: str,
+        actions: dict[str, list[str]],
+        triggers: dict[str, dict[str, str]],
+        name: str = "start",
+    ):
+        self.name = name
+        self.convo_name = convo_name
+        self.convo_description = convo_description
+        self.nlp = nlp
+        self.actions = actions
+        self.triggers = triggers
+
+
+class ConvoStopState(ToDictMixin):
+    """Conversation Stop State."""
+
+    def __init__(
+        self,
+        actions: dict,
+        triggers: dict[str, dict[str, str]],
+        name: str = "stop",
+    ):
+        self.name = name
+        self.actions = actions
+        self.triggers = triggers
+
+
+class ConvoIntroductionState(ToDictMixin):
+    def __init__(
+        self,
+        name: str,
+        level: int,
+        actions: dict[str, dict[str, str]],
+        triggers: dict[str, dict[str, str]],
+    ):
+        self.name = name
+        self.level = level
+        self.actions = actions
+        self.triggers = triggers
+
+
+class ConvoInstructionState(ToDictMixin):
+    def __init__(
+        self,
+        name: str,
+        level: int,
+        actions: dict[str, dict[str, str]],
+        buttons: dict[str, dict[str, str]],
+        triggers: dict[str, dict[str, str]],
+    ):
+        self.name = name
+        self.level = level
+        self.actions = actions
+        self.buttons = buttons
+        self.triggers = triggers
+
+
+class ConvoQuestionState(ToDictMixin):
+    def __init__(
+        self,
+        name: str,
+        actions: dict[str, list],
+        level: int = 0,
+        buttons: dict[str, dict[str, str]] = {},
+        triggers: dict[str, dict[str, str]] = {},
+    ):
+        self.name = name
+        self.level = level
+        self.actions = actions
+        if buttons:
+            self.buttons = buttons
+        if triggers:
+            self.triggers = triggers
+
+
+class ConvoAnswerState(ToDictMixin):
+    def __init__(
+        self,
+        name: str,
+        actions: dict[str, list[str]],
+        triggers: dict[str, dict[str, str]],
+    ):
+        self.name = name
+        self.actions = actions
+        self.triggers = triggers
+
+
+class ConvoGraph:
+    def __init__(self, worksheet_name_source_data: str):
+        self.__states = []
+        self.__current_convo_name = worksheet_name_source_data
+
+    def add_state(self, state):
+        self.__states.append(state)
+
+    def __add__(self, other_convo_graph):
+        if not isinstance(other_convo_graph, ConvoGraph):
+            raise ValueError("You can concatenate only ConvoGraph objects")
+
+        def update_start_state():
+            other_convo_start_state = other_convo_graph.__states[0]
+            self.__states[0].convo_description += (
+                "/" + other_convo_start_state.convo_description
+            )
+            self.__states[0].convo_name += (
+                "__" + other_convo_start_state.convo_name
+            )
+
+        def update_stop_state():
+            self.__states[-1].name = f"stop-{self.__current_convo_name}"
+
+            # Handle function for state before StopState
+            if "__next__" in self.__states[-2].triggers["en"]:
+                self.__states[-2].triggers["en"]["__next__"] = self.__states[
+                    -1
+                ].name
+            else:
+                for key, value in self.__states[-2].triggers["en"].items():
+                    if (
+                        key not in ["__default__", "__next__"]
+                        and self.__states[-2].triggers["en"][key] == "stop"
+                    ):
+                        self.__states[-2].triggers["en"][key] = self.__states[
+                            -1
+                        ].name
+            self.__states[-1].triggers["en"][
+                "__default__"
+            ] = f"{other_convo_graph.__states[0].convo_name}-introduction"
+
+        def concatenate_states():
+            # Exclude start state of other Convo
+            states_copy = other_convo_graph.__states[1:]
+            self.__states.extend(states_copy)
+
+        update_start_state()
+        update_stop_state()
+        concatenate_states()
+
+        self.__current_convo_name = other_convo_graph.__current_convo_name
+
+        return self
+
+    def to_list_of_dicts(self):
+        return [state.to_dict() for state in self.__states]
+
+    def populate_convo(self, data: list):
+        for state in data:
+            if "start" in state["name"]:
+                self.__states.append(ConvoStartState(**state))
+            elif "introduction" in state["name"]:
+                self.__states.append(ConvoIntroductionState(**state))
+            elif "instruction" in state["name"]:
+                self.__states.append(ConvoInstructionState(**state))
+            elif "answer" in state["name"]:
+                self.__states.append(ConvoAnswerState(**state))
+            elif "stop" in state["name"]:
+                self.__states.append(ConvoStopState(**state))
+            else:
+                self.__states.append(ConvoQuestionState(**state))
```

### Comparing `convomeld-0.1.3/src/convomeld/thread.py` & `convomeld-0.1.4/src/convomeld/thread.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,194 +1,194 @@
-from __future__ import annotations
-from typing import Iterator, Optional, Union
-from collections.abc import Iterator
-from convomeld.state import Action, State, Trigger, TriggerPlaceholder
-from uuid import uuid4
-
-
-class ConvoThread:
-    def __init__(self) -> None:
-        self._states: dict[str, State] = {}
-        self._uuid = uuid4().hex[-6:]
-        self._first_state = None
-        self._last_state = None
-        self._state_count = 0
-
-    def __repr__(self) -> str:
-        return f'ConvoThread(states={repr(self._states)}, first_state_name={repr(self._first_state and self._first_state.name)})'
-    
-    def __str__(self) -> str:
-        res = ''
-
-        for state in self.iter_states():
-            trigger_str =  f'--{state.triggers[0].value}-->' if len(state.triggers) == 1 else ''
-            res += f'{str(state)} {trigger_str} '
-
-        return res
-
-    def iter_states(self, with_prev_trigger: bool = False) -> ConvoThreadIterator:
-        self.validate()
-        return ConvoThreadIterator(self._states, self._first_state and self._first_state.name, with_prev_trigger=with_prev_trigger)
-
-    def copy(self):
-        self.validate()
-        copy = ConvoThread()
-        
-        for state, prev_trigger in self.iter_states(with_prev_trigger=True):
-            if prev_trigger is None:
-                tp = TriggerPlaceholder.empty()
-            else:
-                tp = TriggerPlaceholder.from_trigger(prev_trigger)
-                
-            copy = copy.append_state(state.actions, tp, **state.attrs)
-
-        return copy
-        
-    # Utils section
-
-    def num_states(self) -> int:
-        self.validate()
-        return len(self._states)
-    
-    def num_triggers(self) -> int:
-        self.validate()
-        return max(len(self._states) - 1, 0)
-    
-    def get_first_state(self) -> Optional[State]:
-        self.validate()
-        return self._first_state and self._first_state.copy()
-
-    def get_last_state(self) -> Optional[State]:
-        self.validate()
-        return self._last_state and self._last_state.copy()
-    
-    def append_state(self, actions: Union[Action, list[Action]], tp: TriggerPlaceholder, **state_attrs) -> ConvoThread:
-        self.validate()
-        if isinstance(actions, Action):
-            actions = [actions]
-
-        self._state_count += 1
-        new_state = State(f'path_{self._uuid}/state_{self._state_count}', actions, **state_attrs)
-        self._states[new_state.name] = new_state
-
-        if len(self._states) == 1:
-            self._first_state = new_state
-            self._last_state = new_state
-            self.validate()
-            return self
-        
-        prev_trigger = tp.create_trigger(new_state.name)
-        self._last_state.triggers.append(prev_trigger)
-        self._last_state = new_state
-        self.validate()
-        return self
-    
-    def prepend_state(self, actions: Union[Action, list[Action]], tp: TriggerPlaceholder, **state_attrs) -> ConvoThread:
-        self.validate()
-        if isinstance(actions, Action):
-            actions = [actions]
-
-        self._state_count += 1
-        new_state = State(f'path_{self._uuid}/state_{self._state_count}', actions, **state_attrs)
-        self._states[new_state.name] = new_state
-
-        if len(self._states) == 1:
-            self._first_state = new_state
-            self._last_state = new_state
-            self.validate()
-            return self
-
-        new_trigger = tp.create_trigger(self._first_state.name)
-        new_state.triggers.append(new_trigger)
-        self._first_state = new_state
-        self.validate()
-        return self
-    
-    def pop_first_state(self) -> Optional[State]:
-        self.validate()
-
-        if len(self._states) == 0:
-            return None
-        elif len(self._states) == 1:
-            state = self._states.pop(self._first_state.name)
-            self._first_state = None
-            self._last_state = None
-            return state.copy()
-        else:
-            state = self._states.pop(self._first_state.name)
-            self._first_state = self._states[state.triggers[0].state_name]
-            return state.copy()
-    
-    # Validation section
-
-    def validate(self) -> None:
-        self._validate_state_names()
-        self._validate_linear()
-
-    def _validate_state_names(self) -> None:
-        for state_name, state in self._states.items():
-            if state_name != state.name:
-                raise RuntimeError('State names constraint of ConvoThread violated')
-            
-            for trigger in state.triggers:
-                if trigger.state_name not in self._states:
-                    raise RuntimeError('State names constraint of ConvoThread violated')
-    
-    def _validate_linear(self) -> None:
-        if len(self._states) == 0:
-            return
-
-        current_state = self._first_state
-        num_states = 0
-
-        while current_state is not None and num_states <= len(self._states) + 1:
-            if len(current_state.triggers) == 0:
-                # Reached end
-                current_state = None
-            elif len(current_state.triggers) == 1:
-                next_state_name = current_state.triggers[0].state_name
-                current_state = self._states[next_state_name]
-            else:
-                raise RuntimeError('Linearity constraint of ConvoThread violated')
-
-            num_states += 1
-
-        if num_states != len(self._states):
-            # print(self)
-            raise RuntimeError('Linearity constraint of ConvoThread violated')
-
-
-class ConvoThreadIterator(Iterator[Union[State, tuple[State, Trigger]]]):
-        def __init__(self, states: dict[str, State], first_state_name: Optional[str], with_prev_trigger: bool) -> None:
-            self._states = {state_name: state.copy() for state_name, state in states.items()}
-            self._first_state = self._states.get(first_state_name, None)
-            self._with_prev_trigger = with_prev_trigger
-
-            self._current_state = self._first_state
-            self._current_trigger = TriggerPlaceholder.none().create_trigger(self._current_state.name)
-
-        def __next__(self) -> State:
-            if self._current_state is None:
-                raise StopIteration()
-            
-            current_state = self._current_state
-            current_trigger = self._current_trigger
-
-            if len(self._current_state.triggers) == 0:
-                # Reached end
-                next_state = None
-                next_trigger = None
-            else:
-                next_trigger = self._current_state.triggers[0]
-                next_state = self._states[next_trigger.state_name]
-
-            # Prepare next iterator state
-            self._current_state = next_state
-            self._current_trigger = next_trigger
-
-            # Collect result
-            if self._with_prev_trigger:
-                result = (current_state, current_trigger)
-            else:
-                result = current_state
-
+from __future__ import annotations
+from typing import Iterator, Optional, Union
+from collections.abc import Iterator
+from convomeld.state import Action, State, Trigger, TriggerPlaceholder
+from uuid import uuid4
+
+
+class ConvoThread:
+    def __init__(self) -> None:
+        self._states: dict[str, State] = {}
+        self._uuid = uuid4().hex[-6:]
+        self._first_state = None
+        self._last_state = None
+        self._state_count = 0
+
+    def __repr__(self) -> str:
+        return f'ConvoThread(states={repr(self._states)}, first_state_name={repr(self._first_state and self._first_state.name)})'
+    
+    def __str__(self) -> str:
+        res = ''
+
+        for state in self.iter_states():
+            trigger_str =  f'--{state.triggers[0].value}-->' if len(state.triggers) == 1 else ''
+            res += f'{str(state)} {trigger_str} '
+
+        return res
+
+    def iter_states(self, with_prev_trigger: bool = False) -> ConvoThreadIterator:
+        self.validate()
+        return ConvoThreadIterator(self._states, self._first_state and self._first_state.name, with_prev_trigger=with_prev_trigger)
+
+    def copy(self):
+        self.validate()
+        copy = ConvoThread()
+        
+        for state, prev_trigger in self.iter_states(with_prev_trigger=True):
+            if prev_trigger is None:
+                tp = TriggerPlaceholder.empty()
+            else:
+                tp = TriggerPlaceholder.from_trigger(prev_trigger)
+                
+            copy = copy.append_state(state.actions, tp, **state.attrs)
+
+        return copy
+        
+    # Utils section
+
+    def num_states(self) -> int:
+        self.validate()
+        return len(self._states)
+    
+    def num_triggers(self) -> int:
+        self.validate()
+        return max(len(self._states) - 1, 0)
+    
+    def get_first_state(self) -> Optional[State]:
+        self.validate()
+        return self._first_state and self._first_state.copy()
+
+    def get_last_state(self) -> Optional[State]:
+        self.validate()
+        return self._last_state and self._last_state.copy()
+    
+    def append_state(self, actions: Union[Action, list[Action]], tp: TriggerPlaceholder, **state_attrs) -> ConvoThread:
+        self.validate()
+        if isinstance(actions, Action):
+            actions = [actions]
+
+        self._state_count += 1
+        new_state = State(f'path_{self._uuid}/state_{self._state_count}', actions, **state_attrs)
+        self._states[new_state.name] = new_state
+
+        if len(self._states) == 1:
+            self._first_state = new_state
+            self._last_state = new_state
+            self.validate()
+            return self
+        
+        prev_trigger = tp.create_trigger(new_state.name)
+        self._last_state.triggers.append(prev_trigger)
+        self._last_state = new_state
+        self.validate()
+        return self
+    
+    def prepend_state(self, actions: Union[Action, list[Action]], tp: TriggerPlaceholder, **state_attrs) -> ConvoThread:
+        self.validate()
+        if isinstance(actions, Action):
+            actions = [actions]
+
+        self._state_count += 1
+        new_state = State(f'path_{self._uuid}/state_{self._state_count}', actions, **state_attrs)
+        self._states[new_state.name] = new_state
+
+        if len(self._states) == 1:
+            self._first_state = new_state
+            self._last_state = new_state
+            self.validate()
+            return self
+
+        new_trigger = tp.create_trigger(self._first_state.name)
+        new_state.triggers.append(new_trigger)
+        self._first_state = new_state
+        self.validate()
+        return self
+    
+    def pop_first_state(self) -> Optional[State]:
+        self.validate()
+
+        if len(self._states) == 0:
+            return None
+        elif len(self._states) == 1:
+            state = self._states.pop(self._first_state.name)
+            self._first_state = None
+            self._last_state = None
+            return state.copy()
+        else:
+            state = self._states.pop(self._first_state.name)
+            self._first_state = self._states[state.triggers[0].state_name]
+            return state.copy()
+    
+    # Validation section
+
+    def validate(self) -> None:
+        self._validate_state_names()
+        self._validate_linear()
+
+    def _validate_state_names(self) -> None:
+        for state_name, state in self._states.items():
+            if state_name != state.name:
+                raise RuntimeError('State names constraint of ConvoThread violated')
+            
+            for trigger in state.triggers:
+                if trigger.state_name not in self._states:
+                    raise RuntimeError('State names constraint of ConvoThread violated')
+    
+    def _validate_linear(self) -> None:
+        if len(self._states) == 0:
+            return
+
+        current_state = self._first_state
+        num_states = 0
+
+        while current_state is not None and num_states <= len(self._states) + 1:
+            if len(current_state.triggers) == 0:
+                # Reached end
+                current_state = None
+            elif len(current_state.triggers) == 1:
+                next_state_name = current_state.triggers[0].state_name
+                current_state = self._states[next_state_name]
+            else:
+                raise RuntimeError('Linearity constraint of ConvoThread violated')
+
+            num_states += 1
+
+        if num_states != len(self._states):
+            # print(self)
+            raise RuntimeError('Linearity constraint of ConvoThread violated')
+
+
+class ConvoThreadIterator(Iterator[Union[State, tuple[State, Trigger]]]):
+        def __init__(self, states: dict[str, State], first_state_name: Optional[str], with_prev_trigger: bool) -> None:
+            self._states = {state_name: state.copy() for state_name, state in states.items()}
+            self._first_state = self._states.get(first_state_name, None)
+            self._with_prev_trigger = with_prev_trigger
+
+            self._current_state = self._first_state
+            self._current_trigger = TriggerPlaceholder.none().create_trigger(self._current_state.name)
+
+        def __next__(self) -> State:
+            if self._current_state is None:
+                raise StopIteration()
+            
+            current_state = self._current_state
+            current_trigger = self._current_trigger
+
+            if len(self._current_state.triggers) == 0:
+                # Reached end
+                next_state = None
+                next_trigger = None
+            else:
+                next_trigger = self._current_state.triggers[0]
+                next_state = self._states[next_trigger.state_name]
+
+            # Prepare next iterator state
+            self._current_state = next_state
+            self._current_trigger = next_trigger
+
+            # Collect result
+            if self._with_prev_trigger:
+                result = (current_state, current_trigger)
+            else:
+                result = current_state
+
             return result
```

### Comparing `convomeld-0.1.3/src/convomeld/utils.py` & `convomeld-0.1.4/src/convomeld/utils.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import yaml
-
-
-class YAMLWriter:
-    @staticmethod
-    def write_convograph_to_yaml_file(
-        convograph_data: list, file_path: str
-    ) -> None:
-        """Write down prepared sequence of microlessons structures to YAML file
-
-        Args:
-            convograph_data (list): Contains sequence of proccessed complete microlessons structures
-            file_path (str): filepath of destination YAML file
-
-        Returns:
-            None: Blank return
-        """
-        file_name = (
-            convograph_data[0]["convo_name"]
-            if len(convograph_data[0]["convo_name"]) < 110
-            else "merged_convographs"
-        )
-        yaml_file_path = f"{file_path}/{file_name}.yml"
-
-        with open(yaml_file_path, "w") as file:
-
-            class MyDumper(yaml.SafeDumper):
-                """Class that helps put space between blocks in YML file"""
-
-                def write_line_break(self, data=None):
-                    super().write_line_break(data)
-
-                    if len(self.indents) == 1:
-                        super().write_line_break()
-
-            yaml.dump(
-                convograph_data,
-                file,
-                default_flow_style=False,
-                sort_keys=False,
-                Dumper=MyDumper,
-            )
+import yaml
+
+
+class YAMLWriter:
+    @staticmethod
+    def write_convograph_to_yaml_file(
+        convograph_data: list, file_path: str
+    ) -> None:
+        """Write down prepared sequence of microlessons structures to YAML file
+
+        Args:
+            convograph_data (list): Contains sequence of proccessed complete microlessons structures
+            file_path (str): filepath of destination YAML file
+
+        Returns:
+            None: Blank return
+        """
+        file_name = (
+            convograph_data[0]["convo_name"]
+            if len(convograph_data[0]["convo_name"]) < 110
+            else "merged_convographs"
+        )
+        yaml_file_path = f"{file_path}/{file_name}.yml"
+
+        with open(yaml_file_path, "w") as file:
+
+            class MyDumper(yaml.SafeDumper):
+                """Class that helps put space between blocks in YML file"""
+
+                def write_line_break(self, data=None):
+                    super().write_line_break(data)
+
+                    if len(self.indents) == 1:
+                        super().write_line_break()
+
+            yaml.dump(
+                convograph_data,
+                file,
+                default_flow_style=False,
+                sort_keys=False,
+                Dumper=MyDumper,
+            )
```

### Comparing `convomeld-0.1.3/src/convomeld/validators.py` & `convomeld-0.1.4/src/convomeld/validators.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,204 +1,204 @@
-import re
-
-
-class ConvographValidationError(Exception):
-    """ Exception processing the Convograph grammar (syntax)
-    
-    We do not currently use the error_codes feature.
-
-    From https://stackoverflow.com/a/1319675
-    """
-    error_codes = {}
-
-    def __init__(self, message, error_codes={}):
-        """ error_codes can be used as shorthand for error messages """             
-        super().__init__(message)    
-        self.error_codes.update(error_codes)
-
-
-class ConvographValidator:
-    def __init__(self, file_content):
-        self.convograph = file_content
-
-    def is_document_structure_valid(self):
-        if not isinstance(self.convograph, list):
-            return ConvographValidationError(
-                f"A Convograph is a list of dictionaries and should have type `list` but yours is type {type(self.convograph)}. "
-                "Perhaps you forgot to put leading '-' before one of your states in the YAML file."
-            )
-        for state in self.convograph:
-            if not isinstance(state, dict):
-                return ConvographValidationError(
-                    f"The '{state}' state object is of type `{type(state)}` but should be `dict`. "
-                    "Perhaps your state name doesn't have a leading '-' character or a trailing ':' character in the YAML file."
-                )
-        return True
-
-    def are_states_fulfilled(self):
-        for state in self.convograph:
-            if "name" not in state:
-                return ConvographValidationError(f'"{state}" state doesn\'t have "name" keyword.')
-            for key in ("actions", "triggers"):
-                if key not in state:
-                    return ConvographValidationError(
-                        f'"{state["name"]}" state doesn\'t have "{key}" keyword.'
-                    )
-        return True
-
-    def are_names_valid(self):
-        for s in self.convograph:
-            if not self.is_name_valid(s["name"]):
-                return ConvographValidationError(
-                    f'"{s["name"]}" isn\'t valid name for state. It should contain alphanumerical, "_" or "/" characters.'
-                )
-        return True
-
-    @staticmethod
-    def is_name_valid(state_name):
-        """ State names must be lowercase alphanumeric and be valid python module paths.
-        They must contain no whitespace or punctuation except "/" and "_".
-    
-        >>> ConvographValidator.is_name_valid('Hello')
-        False
-        >>> ConvographValidator.is_name_valid('hello_earth/from_mars')
-        True
-        """
-        return bool(re.match('[a-z0-9_/]+', state_name))
-
-    def is_start_state_exist(self):
-        for state in self.convograph:
-            if state["name"] == "start":
-                return True
-        return ConvographValidationError('No "start" state was found.')
-
-    def is_start_state_valid(self):
-        for state in self.convograph:
-            if state["name"] == "start":
-                if "convo_name" not in state:
-                    return ConvographValidationError('"start" state doesn\'t have "convo_name" attribute.')
-                if not self.is_name_valid(state["convo_name"]):
-                    return ConvographValidationError(
-                        f'"{state["convo_name"]}" isn\'t valid convo_name for state. It should contain alphanumerical, "_" or "/" symbols.'
-                    )
-                if "convo_description" not in state:
-                    return ConvographValidationError(
-                        '"start" state doesn\'t have "convo_description" attribute.'
-                    )
-                if not self.is_name_valid(state["convo_description"]):
-                    return ConvographValidationError(
-                        f'"{state["convo_description"]}" isn\'t valid convo_description for state. It should contain alphanumerical, "_" or "/" symbols.'
-                    )
-        return True
-
-    def are_names_unique(self):
-        state_names = []
-        for state in self.convograph:
-            state_names.append(state["name"])
-        for s in state_names:
-            if state_names.count(s) > 1:
-                return ConvographValidationError(f'"{s}" state occurs more than once.')
-        return True
-
-    def are_actions_valid(self):
-        for state in self.convograph:
-            if not isinstance(state["actions"], dict):
-                return ConvographValidationError(
-                    f'"{state}" state has wrong value specified for "actions". It should be a dict type.'
-                )
-            for lang_a, v in state["actions"].items():
-                if not isinstance(v, list):
-                    return ConvographValidationError(
-                        f'"{state}" state has wrong value specified for "{lang_a}" actions. It should be a list type.'
-                    )
-                if not len(v):
-                    return ConvographValidationError(f'"{lang_a}" actions are empty for "{state}" state.')
-        return True
-
-    def are_triggers_valid(self):
-        for state in self.convograph:
-            if not isinstance(state["triggers"], dict):
-                return ConvographValidationError(
-                    f'"{state}" state has wrong value specified for "tiggers". It should be a dict type.'
-                )
-            for lang_t, v in state["triggers"].items():
-                if not isinstance(v, dict):
-                    return ConvographValidationError(
-                        f'"{state}" state has wrong value specified for "{lang_t}" triggers. It should be a dict type.'
-                    )
-                if not len(v):
-                    return ConvographValidationError(f'"{lang_t}" triggers are empty for "{state}" state.')
-        return True
-
-    def do_all_triggers_have_essential(self):
-        for state in self.convograph:
-            for lang_triggers in state["triggers"].values():
-                if not all(
-                    (
-                        isinstance(self.is_dunder_trigger_valid(t, "__default__"), bool)
-                        or isinstance(self.is_dunder_trigger_valid(t, "__next__"), bool)
-                        for t in lang_triggers
-                    )
-                ):
-                    return ConvographValidationError(
-                        f'Neither "__default__ " nor "__next__" trigger was found for "{state}" state. Please, check spell.'
-                    )
-        return True
-
-    @staticmethod
-    def is_dunder_trigger_valid(trigger, mandatory_trigger):
-        return trigger.strip().strip("_").strip().lower() == mandatory_trigger.strip(
-            "__"
-        )
-
-    def are_target_states_exist(self):
-        pointed_states = []
-        target_states = []
-        for state in self.convograph:
-            target_states.append(state["name"])
-            for lang_triggers in state["triggers"].values():
-                for target_state in lang_triggers.values():
-                    pointed_states.append(target_state)
-
-        pointed_states = tuple(set(pointed_states))
-        target_states = tuple(set(target_states))
-        for s in pointed_states:
-            if s not in target_states:
-                return ConvographValidationError(f'"{s}" state doesn\'t exist!')
-        return True
-
-    def are_key_lengths_allowed(self):
-        for state in self.convograph:
-            for lang_a, v in state["actions"].items():
-                if not all((len(a) <= 1024 for a in v)):
-                    return ConvographValidationError(
-                        f'Some of "{lang_a}" actions inside "{state}" state exceeded max length of 1024 characters.'
-                    )
-            for lang_t, v in state["triggers"].items():
-                if not all((len(t) <= 1024 for t in v)):
-                    return ConvographValidationError(
-                        f'Some of "{lang_t}" triggers inside "{state}" state exceeded max length of 1024 characters.'
-                    )
-        return True
-
-    def is_valid(self, convograph=None):
-        if convograph is not None:
-            self.convograph = convograph
-
-        checks_to_pass = [
-            self.is_document_structure_valid,
-            self.are_states_fulfilled,
-            self.are_names_valid,
-            self.is_start_state_exist,
-            self.is_start_state_valid,
-            self.are_names_unique,
-            self.are_actions_valid,
-            self.are_triggers_valid,
-            self.do_all_triggers_have_essential,
-            self.are_target_states_exist,
-            self.are_key_lengths_allowed,
-        ]
-        for check in checks_to_pass:
-            invoked_check = check()
-            if not isinstance(invoked_check, bool):
-                raise invoked_check
-        return True
+import re
+
+
+class ConvographValidationError(Exception):
+    """ Exception processing the Convograph grammar (syntax)
+    
+    We do not currently use the error_codes feature.
+
+    From https://stackoverflow.com/a/1319675
+    """
+    error_codes = {}
+
+    def __init__(self, message, error_codes={}):
+        """ error_codes can be used as shorthand for error messages """             
+        super().__init__(message)    
+        self.error_codes.update(error_codes)
+
+
+class ConvographValidator:
+    def __init__(self, file_content):
+        self.convograph = file_content
+
+    def is_document_structure_valid(self):
+        if not isinstance(self.convograph, list):
+            return ConvographValidationError(
+                f"A Convograph is a list of dictionaries and should have type `list` but yours is type {type(self.convograph)}. "
+                "Perhaps you forgot to put leading '-' before one of your states in the YAML file."
+            )
+        for state in self.convograph:
+            if not isinstance(state, dict):
+                return ConvographValidationError(
+                    f"The '{state}' state object is of type `{type(state)}` but should be `dict`. "
+                    "Perhaps your state name doesn't have a leading '-' character or a trailing ':' character in the YAML file."
+                )
+        return True
+
+    def are_states_fulfilled(self):
+        for state in self.convograph:
+            if "name" not in state:
+                return ConvographValidationError(f'"{state}" state doesn\'t have "name" keyword.')
+            for key in ("actions", "triggers"):
+                if key not in state:
+                    return ConvographValidationError(
+                        f'"{state["name"]}" state doesn\'t have "{key}" keyword.'
+                    )
+        return True
+
+    def are_names_valid(self):
+        for s in self.convograph:
+            if not self.is_name_valid(s["name"]):
+                return ConvographValidationError(
+                    f'"{s["name"]}" isn\'t valid name for state. It should contain alphanumerical, "_" or "/" characters.'
+                )
+        return True
+
+    @staticmethod
+    def is_name_valid(state_name):
+        """ State names must be lowercase alphanumeric and be valid python module paths.
+        They must contain no whitespace or punctuation except "/" and "_".
+    
+        >>> ConvographValidator.is_name_valid('Hello')
+        False
+        >>> ConvographValidator.is_name_valid('hello_earth/from_mars')
+        True
+        """
+        return bool(re.match('[a-z0-9_/]+', state_name))
+
+    def is_start_state_exist(self):
+        for state in self.convograph:
+            if state["name"] == "start":
+                return True
+        return ConvographValidationError('No "start" state was found.')
+
+    def is_start_state_valid(self):
+        for state in self.convograph:
+            if state["name"] == "start":
+                if "convo_name" not in state:
+                    return ConvographValidationError('"start" state doesn\'t have "convo_name" attribute.')
+                if not self.is_name_valid(state["convo_name"]):
+                    return ConvographValidationError(
+                        f'"{state["convo_name"]}" isn\'t valid convo_name for state. It should contain alphanumerical, "_" or "/" symbols.'
+                    )
+                if "convo_description" not in state:
+                    return ConvographValidationError(
+                        '"start" state doesn\'t have "convo_description" attribute.'
+                    )
+                if not self.is_name_valid(state["convo_description"]):
+                    return ConvographValidationError(
+                        f'"{state["convo_description"]}" isn\'t valid convo_description for state. It should contain alphanumerical, "_" or "/" symbols.'
+                    )
+        return True
+
+    def are_names_unique(self):
+        state_names = []
+        for state in self.convograph:
+            state_names.append(state["name"])
+        for s in state_names:
+            if state_names.count(s) > 1:
+                return ConvographValidationError(f'"{s}" state occurs more than once.')
+        return True
+
+    def are_actions_valid(self):
+        for state in self.convograph:
+            if not isinstance(state["actions"], dict):
+                return ConvographValidationError(
+                    f'"{state}" state has wrong value specified for "actions". It should be a dict type.'
+                )
+            for lang_a, v in state["actions"].items():
+                if not isinstance(v, list):
+                    return ConvographValidationError(
+                        f'"{state}" state has wrong value specified for "{lang_a}" actions. It should be a list type.'
+                    )
+                if not len(v):
+                    return ConvographValidationError(f'"{lang_a}" actions are empty for "{state}" state.')
+        return True
+
+    def are_triggers_valid(self):
+        for state in self.convograph:
+            if not isinstance(state["triggers"], dict):
+                return ConvographValidationError(
+                    f'"{state}" state has wrong value specified for "tiggers". It should be a dict type.'
+                )
+            for lang_t, v in state["triggers"].items():
+                if not isinstance(v, dict):
+                    return ConvographValidationError(
+                        f'"{state}" state has wrong value specified for "{lang_t}" triggers. It should be a dict type.'
+                    )
+                if not len(v):
+                    return ConvographValidationError(f'"{lang_t}" triggers are empty for "{state}" state.')
+        return True
+
+    def do_all_triggers_have_essential(self):
+        for state in self.convograph:
+            for lang_triggers in state["triggers"].values():
+                if not all(
+                    (
+                        isinstance(self.is_dunder_trigger_valid(t, "__default__"), bool)
+                        or isinstance(self.is_dunder_trigger_valid(t, "__next__"), bool)
+                        for t in lang_triggers
+                    )
+                ):
+                    return ConvographValidationError(
+                        f'Neither "__default__ " nor "__next__" trigger was found for "{state}" state. Please, check spell.'
+                    )
+        return True
+
+    @staticmethod
+    def is_dunder_trigger_valid(trigger, mandatory_trigger):
+        return trigger.strip().strip("_").strip().lower() == mandatory_trigger.strip(
+            "__"
+        )
+
+    def are_target_states_exist(self):
+        pointed_states = []
+        target_states = []
+        for state in self.convograph:
+            target_states.append(state["name"])
+            for lang_triggers in state["triggers"].values():
+                for target_state in lang_triggers.values():
+                    pointed_states.append(target_state)
+
+        pointed_states = tuple(set(pointed_states))
+        target_states = tuple(set(target_states))
+        for s in pointed_states:
+            if s not in target_states:
+                return ConvographValidationError(f'"{s}" state doesn\'t exist!')
+        return True
+
+    def are_key_lengths_allowed(self):
+        for state in self.convograph:
+            for lang_a, v in state["actions"].items():
+                if not all((len(a) <= 1024 for a in v)):
+                    return ConvographValidationError(
+                        f'Some of "{lang_a}" actions inside "{state}" state exceeded max length of 1024 characters.'
+                    )
+            for lang_t, v in state["triggers"].items():
+                if not all((len(t) <= 1024 for t in v)):
+                    return ConvographValidationError(
+                        f'Some of "{lang_t}" triggers inside "{state}" state exceeded max length of 1024 characters.'
+                    )
+        return True
+
+    def is_valid(self, convograph=None):
+        if convograph is not None:
+            self.convograph = convograph
+
+        checks_to_pass = [
+            self.is_document_structure_valid,
+            self.are_states_fulfilled,
+            self.are_names_valid,
+            self.is_start_state_exist,
+            self.is_start_state_valid,
+            self.are_names_unique,
+            self.are_actions_valid,
+            self.are_triggers_valid,
+            self.do_all_triggers_have_essential,
+            self.are_target_states_exist,
+            self.are_key_lengths_allowed,
+        ]
+        for check in checks_to_pass:
+            invoked_check = check()
+            if not isinstance(invoked_check, bool):
+                raise invoked_check
+        return True
```

### Comparing `convomeld-0.1.3/src/convomeld/xlsx_csv_parsers.py` & `convomeld-0.1.4/src/convomeld/xlsx_csv_parsers.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-import datetime
-from abc import ABC, abstractmethod
-from pathlib import Path
-from typing import List, Tuple, Union
-import os
-import pandas as pd
-import yaml
-
-
-class Parser(ABC):
-    @abstractmethod
-    def parse(self, path: str):
-        pass
-
-
-class ConvoDataParser(Parser):
-    """Class that provides methods to parse different file formats"""
-
-    @staticmethod
-    def __parse_csv(file_path: str) -> Tuple[List[pd.DataFrame], List[str]]:
-        try:
-            file_name = os.path.basename(file_path).split(".")[0]
-
-            data = pd.read_csv(file_path, dtype="str")
-            data = data.dropna(how="all")
-            data = [data.columns.tolist()] + data.values.tolist()
-            df = pd.DataFrame(data)
-
-            return [df], [file_name]
-        except Exception as e:
-            print(f"Error parsing CSV: {e}")
-            return []
-
-    @staticmethod
-    def __parse_xlsx(file_path: str) -> Tuple[List[pd.DataFrame], List[str]]:
-        def convert_to_fraction(value):
-            if isinstance(value, datetime.datetime):
-                value = value.strftime("%-d/%-m")
-                return value
-            return value
-
-        try:
-            dfs_xlsx_file = []
-
-            xlsx_file = pd.ExcelFile(file_path)
-            worksheet_names = xlsx_file.sheet_names
-
-            for sheet_name in worksheet_names:
-                df = pd.read_excel(
-                    xlsx_file, sheet_name=sheet_name, header=None
-                )
-                df[4] = df[4].apply(convert_to_fraction)
-                sheet_data = df.dropna(how="any")
-
-                dfs_xlsx_file.append(sheet_data)
-            return dfs_xlsx_file, worksheet_names
-        except Exception as e:
-            print(f"Error parsing Excel file: {e}")
-            return []
-
-    @staticmethod
-    def __parse_yml(file_path: str) -> Tuple[List[List], List[str]]:
-        file_name = os.path.basename(file_path).rstrip(".yml")
-
-        with open(file_path, "r") as file:
-            yaml_data = yaml.safe_load(file)
-
-        return [yaml_data], [file_name]
-
-    def parse(
-        self, file_path: Union[str, Path]
-    ) -> Union[
-        Tuple[List[pd.DataFrame], List[str]], Tuple[List[List], List[str]]
-    ]:
-        file_name = os.path.basename(file_path)
-        if file_name.endswith(".csv"):
-            return self.__parse_csv(file_path=file_path)
-        elif file_name.endswith(".xlsx"):
-            return self.__parse_xlsx(file_path=file_path)
-        elif file_name.endswith(".yml"):
-            return self.__parse_yml(file_path=file_path)
-        else:
-            raise ValueError(f"Unsupported file format: {file_name}")
-
-
-class YAMLFileNamesParser(Parser):
-    def parse(self, args_path: list) -> dict:
-        """Parse and return list of filenames which has .yml format"""
-        file_name_file_path = {}
-        for path in args_path:
-            if os.path.isfile(path) and path.lower().endswith(".yml"):
-                file_name_file_path[os.path.basename(path)] = path
-            elif os.path.isdir(path):
-                for root, _, files in os.walk(path):
-                    for file in files:
-                        if file.lower().endswith(".yml"):
-                            file_name_file_path[file] = os.path.join(
-                                root, file
-                            )
-        return file_name_file_path
-
-
-class XLSXFileNamesParser(Parser):
-    def parse(self, folder_path: str) -> list[str]:
-        """Parse folder and return list of filenames which has .xlsx format"""
-        files_list = []
-        for filename in os.listdir(folder_path):
-            if os.path.isfile(
-                os.path.join(folder_path, filename)
-            ) and filename.endswith(".xlsx"):
-                files_list.append(filename)
-        return files_list
-
-
-class CSVFileNamesParser(Parser):
-    def parse(self, folder_path: str) -> list[str]:
-        """Parse folder and return list of filenames which has .csv format"""
-        files_list = []
-        for filename in os.listdir(folder_path):
-            if os.path.isfile(
-                os.path.join(folder_path, filename)
-            ) and filename.endswith(".csv"):
-                files_list.append(filename)
-        return files_list
+import datetime
+from abc import ABC, abstractmethod
+from pathlib import Path
+from typing import List, Tuple, Union
+import os
+import pandas as pd
+import yaml
+
+
+class Parser(ABC):
+    @abstractmethod
+    def parse(self, path: str):
+        pass
+
+
+class ConvoDataParser(Parser):
+    """Class that provides methods to parse different file formats"""
+
+    @staticmethod
+    def __parse_csv(file_path: str) -> Tuple[List[pd.DataFrame], List[str]]:
+        try:
+            file_name = os.path.basename(file_path).split(".")[0]
+
+            data = pd.read_csv(file_path, dtype="str")
+            data = data.dropna(how="all")
+            data = [data.columns.tolist()] + data.values.tolist()
+            df = pd.DataFrame(data)
+
+            return [df], [file_name]
+        except Exception as e:
+            print(f"Error parsing CSV: {e}")
+            return []
+
+    @staticmethod
+    def __parse_xlsx(file_path: str) -> Tuple[List[pd.DataFrame], List[str]]:
+        def convert_to_fraction(value):
+            if isinstance(value, datetime.datetime):
+                value = value.strftime("%-d/%-m")
+                return value
+            return value
+
+        try:
+            dfs_xlsx_file = []
+
+            xlsx_file = pd.ExcelFile(file_path)
+            worksheet_names = xlsx_file.sheet_names
+
+            for sheet_name in worksheet_names:
+                df = pd.read_excel(
+                    xlsx_file, sheet_name=sheet_name, header=None
+                )
+                df[4] = df[4].apply(convert_to_fraction)
+                sheet_data = df.dropna(how="any")
+
+                dfs_xlsx_file.append(sheet_data)
+            return dfs_xlsx_file, worksheet_names
+        except Exception as e:
+            print(f"Error parsing Excel file: {e}")
+            return []
+
+    @staticmethod
+    def __parse_yml(file_path: str) -> Tuple[List[List], List[str]]:
+        file_name = os.path.basename(file_path).rstrip(".yml")
+
+        with open(file_path, "r") as file:
+            yaml_data = yaml.safe_load(file)
+
+        return [yaml_data], [file_name]
+
+    def parse(
+        self, file_path: Union[str, Path]
+    ) -> Union[
+        Tuple[List[pd.DataFrame], List[str]], Tuple[List[List], List[str]]
+    ]:
+        file_name = os.path.basename(file_path)
+        if file_name.endswith(".csv"):
+            return self.__parse_csv(file_path=file_path)
+        elif file_name.endswith(".xlsx"):
+            return self.__parse_xlsx(file_path=file_path)
+        elif file_name.endswith(".yml"):
+            return self.__parse_yml(file_path=file_path)
+        else:
+            raise ValueError(f"Unsupported file format: {file_name}")
+
+
+class YAMLFileNamesParser(Parser):
+    def parse(self, args_path: list) -> dict:
+        """Parse and return list of filenames which has .yml format"""
+        file_name_file_path = {}
+        for path in args_path:
+            if os.path.isfile(path) and path.lower().endswith(".yml"):
+                file_name_file_path[os.path.basename(path)] = path
+            elif os.path.isdir(path):
+                for root, _, files in os.walk(path):
+                    for file in files:
+                        if file.lower().endswith(".yml"):
+                            file_name_file_path[file] = os.path.join(
+                                root, file
+                            )
+        return file_name_file_path
+
+
+class XLSXFileNamesParser(Parser):
+    def parse(self, folder_path: str) -> list[str]:
+        """Parse folder and return list of filenames which has .xlsx format"""
+        files_list = []
+        for filename in os.listdir(folder_path):
+            if os.path.isfile(
+                os.path.join(folder_path, filename)
+            ) and filename.endswith(".xlsx"):
+                files_list.append(filename)
+        return files_list
+
+
+class CSVFileNamesParser(Parser):
+    def parse(self, folder_path: str) -> list[str]:
+        """Parse folder and return list of filenames which has .csv format"""
+        files_list = []
+        for filename in os.listdir(folder_path):
+            if os.path.isfile(
+                os.path.join(folder_path, filename)
+            ) and filename.endswith(".csv"):
+                files_list.append(filename)
+        return files_list
```

### Comparing `convomeld-0.1.3/PKG-INFO` & `convomeld-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: convomeld
-Version: 0.1.3
+Version: 0.1.4
 Summary: Parse text scripts or chatbot message logs and merge conversation graphs (Convographs)
 License: AGPL-3.0-or-later
 Author: Ruslan Borysov
 Author-email: borysov.ruslan98@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0)
 Requires-Dist: openpyxl
+Requires-Dist: pandas
 Description-Content-Type: text/markdown
 
 # Convomeld
 
 Tools for composing, validating, merging and simplifying the graph data structures that define the a conversational agent's behavior - a program that can be run by a conversation manager to interact with humans.
```

