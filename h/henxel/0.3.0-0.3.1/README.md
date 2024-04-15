# Comparing `tmp/henxel-0.3.0.tar.gz` & `tmp/henxel-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "henxel-0.3.0.tar", last modified: Wed Nov 22 14:07:54 2023, max compression
+gzip compressed data, was "henxel-0.3.1.tar", last modified: Mon Apr 15 17:33:54 2024, max compression
```

## Comparing `henxel-0.3.0.tar` & `henxel-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-11-22 14:07:54.869806 henxel-0.3.0/
--rw-rw-rw-   0        0        0    35475 2023-10-02 16:39:50.000000 henxel-0.3.0/LICENSE
--rw-rw-rw-   0        0        0       52 2023-10-03 12:54:25.000000 henxel-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7456 2023-11-22 14:07:54.869806 henxel-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     6702 2023-11-22 14:00:11.000000 henxel-0.3.0/README.md
--rw-rw-rw-   0        0        0      104 2023-11-22 13:59:26.000000 henxel-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0      867 2023-11-22 14:07:54.869806 henxel-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-11-22 14:07:54.776077 henxel-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-11-22 14:07:54.838556 henxel-0.3.0/src/henxel/
--rw-rw-rw-   0        0        0   154172 2023-11-22 13:56:48.000000 henxel-0.3.0/src/henxel/__init__.py
--rw-rw-rw-   0        0        0    11224 2023-10-03 12:53:32.000000 henxel-0.3.0/src/henxel/changefont.py
--rw-rw-rw-   0        0        0      359 2023-10-02 16:39:50.000000 henxel-0.3.0/src/henxel/editor.png
--rw-rw-rw-   0        0        0     7869 2023-10-03 12:53:32.000000 henxel-0.3.0/src/henxel/fdialog.py
--rw-rw-rw-   0        0        0     9077 2023-11-22 13:56:48.000000 henxel-0.3.0/src/henxel/help.txt
--rw-rw-rw-   0        0        0     9145 2023-11-22 13:56:48.000000 henxel-0.3.0/src/henxel/help_mac.txt
--rw-rw-rw-   0        0        0     3013 2023-10-02 16:39:50.000000 henxel-0.3.0/src/henxel/wordexpand.py
-drwxrwxrwx   0        0        0        0 2023-11-22 14:07:54.869806 henxel-0.3.0/src/henxel.egg-info/
--rw-rw-rw-   0        0        0     7456 2023-11-22 14:07:54.000000 henxel-0.3.0/src/henxel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-11-22 14:07:54.000000 henxel-0.3.0/src/henxel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-22 14:07:54.000000 henxel-0.3.0/src/henxel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-11-22 14:07:54.000000 henxel-0.3.0/src/henxel.egg-info/top_level.txt
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2024-04-15 17:33:54.893362 henxel-0.3.1/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    34801 2024-03-26 11:13:09.000000 henxel-0.3.1/LICENSE
+-rw-r--r--   0 samuel    (1000) samuel    (1000)       50 2024-03-26 11:13:09.000000 henxel-0.3.1/MANIFEST.in
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     5351 2024-04-15 17:33:54.893362 henxel-0.3.1/PKG-INFO
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     4616 2024-04-15 17:30:33.000000 henxel-0.3.1/README.md
+-rw-r--r--   0 samuel    (1000) samuel    (1000)       98 2024-04-15 17:30:33.000000 henxel-0.3.1/pyproject.toml
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      833 2024-04-15 17:33:54.893362 henxel-0.3.1/setup.cfg
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2024-04-15 17:33:54.869362 henxel-0.3.1/src/
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2024-04-15 17:33:54.893362 henxel-0.3.1/src/henxel/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)   165232 2024-04-15 17:30:33.000000 henxel-0.3.1/src/henxel/__init__.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    10837 2024-03-26 17:17:11.000000 henxel-0.3.1/src/henxel/changefont.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      359 2024-03-26 11:13:09.000000 henxel-0.3.1/src/henxel/editor.png
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     7571 2024-03-26 11:13:09.000000 henxel-0.3.1/src/henxel/fdialog.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     8153 2024-04-15 17:30:33.000000 henxel-0.3.1/src/henxel/help.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     8141 2024-04-15 17:30:33.000000 henxel-0.3.1/src/henxel/help_mac.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     2947 2024-04-15 17:30:33.000000 henxel-0.3.1/src/henxel/wordexpand.py
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2024-04-15 17:33:54.893362 henxel-0.3.1/src/henxel.egg-info/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     5351 2024-04-15 17:33:54.000000 henxel-0.3.1/src/henxel.egg-info/PKG-INFO
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      351 2024-04-15 17:33:54.000000 henxel-0.3.1/src/henxel.egg-info/SOURCES.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)        1 2024-04-15 17:33:54.000000 henxel-0.3.1/src/henxel.egg-info/dependency_links.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)        7 2024-04-15 17:33:54.000000 henxel-0.3.1/src/henxel.egg-info/top_level.txt
```

### Comparing `henxel-0.3.0/LICENSE` & `henxel-0.3.1/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-					GNU GENERAL PUBLIC LICENSE
-					   Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-							Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-					   TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-	a) The work must carry prominent notices stating that you modified
-	it, and giving a relevant date.
-
-	b) The work must carry prominent notices stating that it is
-	released under this License and any conditions added under section
-	7.  This requirement modifies the requirement in section 4 to
-	"keep intact all notices".
-
-	c) You must license the entire work, as a whole, under this
-	License to anyone who comes into possession of a copy.  This
-	License will therefore apply, along with any applicable section 7
-	additional terms, to the whole of the work, and all its parts,
-	regardless of how they are packaged.  This License gives no
-	permission to license the work in any other way, but it does not
-	invalidate such permission if you have separately received it.
-
-	d) If the work has interactive user interfaces, each must display
-	Appropriate Legal Notices; however, if the Program has interactive
-	interfaces that do not display Appropriate Legal Notices, your
-	work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-	a) Convey the object code in, or embodied in, a physical product
-	(including a physical distribution medium), accompanied by the
-	Corresponding Source fixed on a durable physical medium
-	customarily used for software interchange.
-
-	b) Convey the object code in, or embodied in, a physical product
-	(including a physical distribution medium), accompanied by a
-	written offer, valid for at least three years and valid for as
-	long as you offer spare parts or customer support for that product
-	model, to give anyone who possesses the object code either (1) a
-	copy of the Corresponding Source for all the software in the
-	product that is covered by this License, on a durable physical
-	medium customarily used for software interchange, for a price no
-	more than your reasonable cost of physically performing this
-	conveying of source, or (2) access to copy the
-	Corresponding Source from a network server at no charge.
-
-	c) Convey individual copies of the object code with a copy of the
-	written offer to provide the Corresponding Source.  This
-	alternative is allowed only occasionally and noncommercially, and
-	only if you received the object code with such an offer, in accord
-	with subsection 6b.
-
-	d) Convey the object code by offering access from a designated
-	place (gratis or for a charge), and offer equivalent access to the
-	Corresponding Source in the same way through the same place at no
-	further charge.  You need not require recipients to copy the
-	Corresponding Source along with the object code.  If the place to
-	copy the object code is a network server, the Corresponding Source
-	may be on a different server (operated by you or a third party)
-	that supports equivalent copying facilities, provided you maintain
-	clear directions next to the object code saying where to find the
-	Corresponding Source.  Regardless of what server hosts the
-	Corresponding Source, you remain obligated to ensure that it is
-	available for as long as needed to satisfy these requirements.
-
-	e) Convey the object code using peer-to-peer transmission, provided
-	you inform other peers where the object code and Corresponding
-	Source of the work are being offered to the general public at no
-	charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-	a) Disclaiming warranty or limiting liability differently from the
-	terms of sections 15 and 16 of this License; or
-
-	b) Requiring preservation of specified reasonable legal notices or
-	author attributions in that material or in the Appropriate Legal
-	Notices displayed by works containing it; or
-
-	c) Prohibiting misrepresentation of the origin of that material, or
-	requiring that modified versions of such material be marked in
-	reasonable ways as different from the original version; or
-
-	d) Limiting the use for publicity purposes of names of licensors or
-	authors of the material; or
-
-	e) Declining to grant rights under trademark law for use of some
-	trade names, trademarks, or service marks; or
-
-	f) Requiring indemnification of licensors and authors of that
-	material by anyone who conveys the material (or modified versions of
-	it) with contractual assumptions of liability to the recipient, for
-	any liability that these contractual assumptions directly impose on
-	those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-					 END OF TERMS AND CONDITIONS
-
-			How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-	<one line to give the program's name and a brief idea of what it does.>
-	Copyright (C) <year>  <name of author>
-
-	This program is free software: you can redistribute it and/or modify
-	it under the terms of the GNU General Public License as published by
-	the Free Software Foundation, either version 3 of the License, or
-	(at your option) any later version.
-
-	This program is distributed in the hope that it will be useful,
-	but WITHOUT ANY WARRANTY; without even the implied warranty of
-	MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-	GNU General Public License for more details.
-
-	You should have received a copy of the GNU General Public License
-	along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-	<program>  Copyright (C) <year>  <name of author>
-	This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-	This is free software, and you are welcome to redistribute it
-	under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+					GNU GENERAL PUBLIC LICENSE
+					   Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+							Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+					   TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+	a) The work must carry prominent notices stating that you modified
+	it, and giving a relevant date.
+
+	b) The work must carry prominent notices stating that it is
+	released under this License and any conditions added under section
+	7.  This requirement modifies the requirement in section 4 to
+	"keep intact all notices".
+
+	c) You must license the entire work, as a whole, under this
+	License to anyone who comes into possession of a copy.  This
+	License will therefore apply, along with any applicable section 7
+	additional terms, to the whole of the work, and all its parts,
+	regardless of how they are packaged.  This License gives no
+	permission to license the work in any other way, but it does not
+	invalidate such permission if you have separately received it.
+
+	d) If the work has interactive user interfaces, each must display
+	Appropriate Legal Notices; however, if the Program has interactive
+	interfaces that do not display Appropriate Legal Notices, your
+	work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+	a) Convey the object code in, or embodied in, a physical product
+	(including a physical distribution medium), accompanied by the
+	Corresponding Source fixed on a durable physical medium
+	customarily used for software interchange.
+
+	b) Convey the object code in, or embodied in, a physical product
+	(including a physical distribution medium), accompanied by a
+	written offer, valid for at least three years and valid for as
+	long as you offer spare parts or customer support for that product
+	model, to give anyone who possesses the object code either (1) a
+	copy of the Corresponding Source for all the software in the
+	product that is covered by this License, on a durable physical
+	medium customarily used for software interchange, for a price no
+	more than your reasonable cost of physically performing this
+	conveying of source, or (2) access to copy the
+	Corresponding Source from a network server at no charge.
+
+	c) Convey individual copies of the object code with a copy of the
+	written offer to provide the Corresponding Source.  This
+	alternative is allowed only occasionally and noncommercially, and
+	only if you received the object code with such an offer, in accord
+	with subsection 6b.
+
+	d) Convey the object code by offering access from a designated
+	place (gratis or for a charge), and offer equivalent access to the
+	Corresponding Source in the same way through the same place at no
+	further charge.  You need not require recipients to copy the
+	Corresponding Source along with the object code.  If the place to
+	copy the object code is a network server, the Corresponding Source
+	may be on a different server (operated by you or a third party)
+	that supports equivalent copying facilities, provided you maintain
+	clear directions next to the object code saying where to find the
+	Corresponding Source.  Regardless of what server hosts the
+	Corresponding Source, you remain obligated to ensure that it is
+	available for as long as needed to satisfy these requirements.
+
+	e) Convey the object code using peer-to-peer transmission, provided
+	you inform other peers where the object code and Corresponding
+	Source of the work are being offered to the general public at no
+	charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+	a) Disclaiming warranty or limiting liability differently from the
+	terms of sections 15 and 16 of this License; or
+
+	b) Requiring preservation of specified reasonable legal notices or
+	author attributions in that material or in the Appropriate Legal
+	Notices displayed by works containing it; or
+
+	c) Prohibiting misrepresentation of the origin of that material, or
+	requiring that modified versions of such material be marked in
+	reasonable ways as different from the original version; or
+
+	d) Limiting the use for publicity purposes of names of licensors or
+	authors of the material; or
+
+	e) Declining to grant rights under trademark law for use of some
+	trade names, trademarks, or service marks; or
+
+	f) Requiring indemnification of licensors and authors of that
+	material by anyone who conveys the material (or modified versions of
+	it) with contractual assumptions of liability to the recipient, for
+	any liability that these contractual assumptions directly impose on
+	those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+					 END OF TERMS AND CONDITIONS
+
+			How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+	<one line to give the program's name and a brief idea of what it does.>
+	Copyright (C) <year>  <name of author>
+
+	This program is free software: you can redistribute it and/or modify
+	it under the terms of the GNU General Public License as published by
+	the Free Software Foundation, either version 3 of the License, or
+	(at your option) any later version.
+
+	This program is distributed in the hope that it will be useful,
+	but WITHOUT ANY WARRANTY; without even the implied warranty of
+	MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+	GNU General Public License for more details.
+
+	You should have received a copy of the GNU General Public License
+	along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+	<program>  Copyright (C) <year>  <name of author>
+	This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+	This is free software, and you are welcome to redistribute it
+	under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `henxel-0.3.0/README.md` & `henxel-0.3.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,215 +1,185 @@
-# Henxel
-GUI-editor for Python development. Tested to work with Debian 12, Windows 10 and 11 and macOS 12.
-
-
-# Featuring
-* Auto-indent
-* Font Chooser
-* Color Chooser
-* Line numbering
-* Tabbed editing
-* Inspect object
-* Show git-branch
-* Run current file
-* Search - Replace
-* Indent - Unindent
-* Comment - Uncomment
-* Syntax highlighting
-* Click to open errors
-* Parenthesis checking
-* Persistent configuration
-
-# Lacking
-* Auto-completion
-* Hinting
-
-# Prerequisites in Linux
-Python modules required that are sometimes not installed with OS: tkinter. Check in Python-console:
-
-```console
->>> import tkinter
-```
-
-If no error, it is installed. If it throws an error you have to install it from OS-repository. In debian it is: python3-tk
-
-```console
-~$ sudo apt install python3-tk
-```
-
-# About virtual environment, optional but highly recommended
-Consider creating virtual environment for your python-projects and installing python packages like this editor to it. Editor will not save your configuration if it was not launched from virtual environment. In debian you have to first install this package: python3-venv:
-
-```console
-~$ sudo apt install python3-venv
-```
-
-There is a linux-script named 'mkvenv' in /util. Copy it to some place nice like bin-directory in your home-directory and make it executable if it is not already:
-
-```console
-~/bin$ chmod u+x mkvenv
-```
-
-Then make folder for your new project and install venv there and activate it, and show currently installed python-packages in your new virtual environment, and lastly deactivate (quit) environment:
-
-```console
-~$ mkdir myproject
-~$ cd myproject
-~/myproject$ mkvenv env
--------------------------------
-~/myproject$ source env/bin/activate
-(env) ~/myproject$ pip list
------------------------------------
-(env) ~/myproject$ deactivate
-~/myproject$
-```
-
-To remove venv just remove the env-directory and you can start from clean desk making new one with mkvenv later. Optional about virtual environment ends here.
-
-# Prerequisites in Windows and venv-creation
-Python installation should already include tkinter. There is
-mkvenv-install script for Windows in /util. Here is short info about how to
-create a working Python virtual environment in Windows. First open console, like
-PowerShell (in which: ctrl-r to search command history, most useful) or CMD-Terminal and:
-
-```console
-mkdir myproject
-cd myproject
-myproject> py win_install_mkvenv.py
-myproject> mkvenv env
-
-myproject> env\act.bat
-
-If that did not activate venv:
-myproject> env\Scripts\activate
-
-After venv is active upgrade pip and install Henxel:
-(env) myproject> pip install --upgrade pip
-(env) myproject> pip install henxel
-
-Venv is now ready:
-(env) myproject> pip list
-(env) myproject> deactivate
-
-Launch Henxel:
-myproject> env\launch_ed.bat
-```
-
-
-# Prerequisites in macOS and venv-creation
-Python installation (you may need to install newer version of python from python.org)
-should already include tkinter. There currently is no mkvenv script for macOS,
-but making venv is quite same as in Linux. It seems to be enough to make venv
-and then install henxel to it without anything else.
-
-```console
-~$ mkdir myproject
-~$ cd myproject
-~/myproject$ python -m venv env
--------------------------------
-~/myproject$ source env/bin/activate
-(env) ~/myproject$ pip list
------------------------------------
-(env) ~/myproject$ deactivate
-~/myproject$
-```
-
-
-
-# Installing
-```console
-(env) ~/myproject$ pip install henxel
-```
-
-or to install system-wide, not recommended. You need first to install pip from OS-repository:
-
-```console
-~/myproject$ pip install henxel
-```
-
-
-# Running from Python-console:
-
-```console
-~/myproject$ source env/bin/activate
-(env) ~/myproject$ python
---------------------------------------
->>> import henxel
->>> e=henxel.Editor()
-```
-
-# Developing
-
-```console
-~/myproject$ mkvenv env
-~/myproject$ . env/bin/activate
-(env) ~/myproject$ git clone https://github.com/SamuelKos/henxel
-(env) ~/myproject$ cd henxel
-(env) ~/myproject/henxel$ pip install -e .
-```
-
-If you currently have no internet but have previously installed virtual environment which has pip and setuptools and you have downloaded henxel-repository:
-
-```console
-(env) ~/myproject/henxel$ pip install --no-build-isolation -e .
-```
-
-Files are in src/henxel/
-
-
-# More on virtual environments:
-This is now bit more complex, because we are not anymore expecting that we have many older versions of the project left (as packages). But with this lenghty method we can compare to any commit, not just released packages. So this is for you who are packaging Python-project and might want things like side-by-side live-comparison of two different versions, most propably version you are currently developing and some earlier version. I Assume you are the owner of the project so you have the git-history, or else you have done git clone. I use henxel as the project example.
-
-
-First create development-venv for the project, if you haven't already and install current version to it in editable mode:
-
-```console
-~/myproject/henxel$ mkvenv env
-~/myproject/henxel$ . env/bin/activate
-(env) ~/myproject/henxel$ pip install -e .
-```
-
-Then select the git-commit for the reference version. I have interesting commits with message like: version 0.2.0 so to list all such commits:
-
-```console
-~/myproject/henxel$ git log --grep=version
-```
-
-For example to make new branch from version 0.2.0, copy the first letters from the commit-id and:
-
-```console
-~/myproject/henxel$ git branch version020 e4f1f4ab3f
-~/myproject/henxel$ git switch version020
-```
-
-Then create ref-env to some place that is not version-controlled like the parent-folder and install version020 of the project to it with pip, again in editable mode, just in case you want to try something out.
-
-```console
-~/myproject/henxel$ cd ..
-~/myproject$ mkvenv v020
-~/myproject$ . v020/bin/activate
-(v020) ~/myproject$ cd henxel
-(v020) ~/myproject/henxel$ pip list
-(v020) ~/myproject/henxel$ pip install -e .
-(v020) ~/myproject/henxel$ deactivate
-```
-
-Now you are ready to launch both versions of your project and do side-by-side comparison if that is what you want:
-
-```console
-~/myproject/henxel$ . env/bin/activate
-(env) ~/myproject/henxel$ pip list
-```
-
-From other shell-window:
-
-```console
-~/myproject$ . v020/bin/activate
-(v020) ~/myproject$ pip list
-```
-
-
-# More resources
-[Changelog](https://github.com/SamuelKos/henxel/blob/main/CHANGELOG)
-
-# Licence
-This project is licensed under the terms of the GNU General Public License v3.0.
+Metadata-Version: 2.1
+Name: henxel
+Version: 0.3.1
+Summary: GUI-editor for Python development.
+Home-page: https://github.com/SamuelKos/henxel
+Author: SamuelKos
+Author-email: koskinens371@gmail.com
+Project-URL: Bug Tracker, https://github.com/SamuelKos/henxel/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development
+Classifier: Topic :: Text Editors
+Requires-Python: >=3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Henxel
+GUI-editor for Python development. Tested to work with Debian 12, Windows 10 and 11 and macOS 12.
+
+![editor_mac](pics/editor_macOS.png)
+![editor_linux](pics/editor_linux.png)
+
+# Featuring
+* Auto-indent
+* Font Chooser
+* Color Chooser
+* Line numbering
+* Tabbed editing
+* Tab-completion
+* Inspect object
+* Show git-branch
+* Run current file
+* Search - Replace
+* Indent - Unindent
+* Comment - Uncomment
+* Syntax highlighting
+* Click to open errors
+* Parenthesis checking
+* Persistent configuration
+
+
+# Prerequisites in Linux
+Python modules required that are sometimes not installed with OS: tkinter. Check in Python-console:
+
+```console
+>>> import tkinter
+```
+
+If no error, it is installed. If it throws an error you have to install it from OS-repository. In debian it is: python3-tk
+
+```console
+~$ sudo apt install python3-tk
+```
+
+# About virtual environment, optional but highly recommended
+Consider creating virtual environment for your python-projects and installing python packages like this editor to it. Editor will not save your configuration if it was not launched from virtual environment. In debian you have to first install this package: python3-venv:
+
+```console
+~$ sudo apt install python3-venv
+```
+
+There is a linux-script named 'mkvenv' in /util. Copy it to some place nice like bin-directory in your home-directory and make it executable if it is not already:
+
+```console
+~/bin$ chmod u+x mkvenv
+```
+
+Then make folder for your new project and install venv there and activate it, and show currently installed python-packages in your new virtual environment, and lastly deactivate (quit) environment:
+
+```console
+~$ mkdir myproject
+~$ cd myproject
+~/myproject$ mkvenv env
+-------------------------------
+~/myproject$ source env/bin/activate
+(env) ~/myproject$ pip list
+-----------------------------------
+(env) ~/myproject$ deactivate
+~/myproject$
+```
+
+To remove venv just remove the env-directory and you can start from clean desk making new one with mkvenv later. Optional about virtual environment ends here.
+
+# Prerequisites in Windows and venv-creation
+Python installation should already include tkinter. There is
+mkvenv-install script for Windows in /util. Here is short info about how to
+create a working Python virtual environment in Windows. First open console, like
+PowerShell (in which: ctrl-r to search command history, most useful) or CMD-Terminal and:
+
+```console
+mkdir myproject
+cd myproject
+myproject> py win_install_mkvenv.py
+myproject> mkvenv env
+
+myproject> env\act.bat
+
+If that did not activate venv:
+myproject> env\Scripts\activate
+
+After venv is active upgrade pip and install Henxel:
+(env) myproject> pip install --upgrade pip
+(env) myproject> pip install henxel
+
+Venv is now ready:
+(env) myproject> pip list
+(env) myproject> deactivate
+
+Launch Henxel:
+myproject> env\launch_ed.bat
+```
+
+
+# Prerequisites in macOS and venv-creation
+Python installation (you may need to install newer version of python from python.org)
+should already include tkinter. There currently is no mkvenv script for macOS,
+but making venv is quite same as in Linux. It seems to be enough to make venv
+and then install henxel to it without anything else.
+
+```console
+~$ mkdir myproject
+~$ cd myproject
+~/myproject$ python -m venv env
+-------------------------------
+~/myproject$ source env/bin/activate
+(env) ~/myproject$ pip list
+-----------------------------------
+(env) ~/myproject$ deactivate
+~/myproject$
+```
+
+
+
+# Installing
+```console
+(env) ~/myproject$ pip install henxel
+```
+
+or to install system-wide, not recommended. You need first to install pip from OS-repository:
+
+```console
+~/myproject$ pip install henxel
+```
+
+
+# Running from Python-console:
+
+```console
+~/myproject$ source env/bin/activate
+(env) ~/myproject$ python
+--------------------------------------
+>>> import henxel
+>>> e=henxel.Editor()
+```
+
+# Developing
+
+```console
+~/myproject$ mkvenv env
+~/myproject$ . env/bin/activate
+(env) ~/myproject$ git clone https://github.com/SamuelKos/henxel
+(env) ~/myproject$ cd henxel
+(env) ~/myproject/henxel$ pip install -e .
+```
+
+If you currently have no internet but have previously installed virtual environment which has pip and setuptools and you have downloaded henxel-repository:
+
+```console
+(env) ~/myproject/henxel$ pip install --no-build-isolation -e .
+```
+
+Files are in src/henxel/
+
+
+# More resources
+[Tcl/Tk](https://tcl.tk/man/tcl9.0/TkCmd/index.html)
+[Python/Tkinter](https://docs.python.org/3/library/tkinter.html)
+[Changelog](https://github.com/SamuelKos/henxel/blob/main/CHANGELOG)
+
+# Licence
+This project is licensed under the terms of the GNU General Public License v3.0.
```

### Comparing `henxel-0.3.0/setup.cfg` & `henxel-0.3.1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,53 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2068 656e 7865 6c0d 0a76 6572 7369   = henxel..versi
-00000020: 6f6e 203d 2030 2e33 2e30 0d0a 6175 7468  on = 0.3.0..auth
-00000030: 6f72 203d 2053 616d 7565 6c4b 6f73 0d0a  or = SamuelKos..
-00000040: 6175 7468 6f72 5f65 6d61 696c 203d 206b  author_email = k
-00000050: 6f73 6b69 6e65 6e73 3337 3140 676d 6169  oskinens371@gmai
-00000060: 6c2e 636f 6d0d 0a64 6573 6372 6970 7469  l.com..descripti
-00000070: 6f6e 203d 2047 5549 2d65 6469 746f 7220  on = GUI-editor 
-00000080: 666f 7220 5079 7468 6f6e 2064 6576 656c  for Python devel
-00000090: 6f70 6d65 6e74 2e0d 0a6c 6f6e 675f 6465  opment...long_de
-000000a0: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
-000000b0: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
-000000c0: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
-000000d0: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
-000000e0: 742f 6d61 726b 646f 776e 0d0a 7572 6c20  t/markdown..url 
-000000f0: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-00000100: 2e63 6f6d 2f53 616d 7565 6c4b 6f73 2f68  .com/SamuelKos/h
-00000110: 656e 7865 6c0d 0a70 726f 6a65 6374 5f75  enxel..project_u
-00000120: 726c 7320 3d20 0d0a 0942 7567 2054 7261  rls = ...Bug Tra
-00000130: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
-00000140: 6974 6875 622e 636f 6d2f 5361 6d75 656c  ithub.com/Samuel
-00000150: 4b6f 732f 6865 6e78 656c 2f69 7373 7565  Kos/henxel/issue
-00000160: 730d 0a63 6c61 7373 6966 6965 7273 203d  s..classifiers =
-00000170: 200d 0a09 5072 6f67 7261 6d6d 696e 6720   ...Programming 
-00000180: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000190: 6f6e 203a 3a20 330d 0a09 4c69 6365 6e73  on :: 3...Licens
-000001a0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-000001b0: 6420 3a3a 2047 4e55 2047 656e 6572 616c  d :: GNU General
-000001c0: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
-000001d0: 7633 2028 4750 4c76 3329 0d0a 094f 7065  v3 (GPLv3)...Ope
-000001e0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-000001f0: 2050 4f53 4958 203a 3a20 4c69 6e75 780d   POSIX :: Linux.
-00000200: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
-00000210: 656d 203a 3a20 4d69 6372 6f73 6f66 7420  em :: Microsoft 
-00000220: 3a3a 2057 696e 646f 7773 0d0a 094f 7065  :: Windows...Ope
-00000230: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000240: 204d 6163 4f53 0d0a 0949 6e74 656e 6465   MacOS...Intende
-00000250: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
-00000260: 7665 6c6f 7065 7273 0d0a 0954 6f70 6963  velopers...Topic
-00000270: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
-00000280: 656c 6f70 6d65 6e74 0d0a 0954 6f70 6963  elopment...Topic
-00000290: 203a 3a20 5465 7874 2045 6469 746f 7273   :: Text Editors
-000002a0: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
-000002b0: 6163 6b61 6765 5f64 6972 203d 200d 0a09  ackage_dir = ...
-000002c0: 3d20 7372 630d 0a70 6163 6b61 6765 7320  = src..packages 
-000002d0: 3d20 6669 6e64 3a0d 0a69 6e63 6c75 6465  = find:..include
-000002e0: 5f70 6163 6b61 6765 5f64 6174 6120 3d20  _package_data = 
-000002f0: 5472 7565 0d0a 7079 7468 6f6e 5f72 6571  True..python_req
-00000300: 7569 7265 7320 3d20 3e3d 332e 390d 0a0d  uires = >=3.9...
-00000310: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-00000320: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-00000330: 3d20 7372 630d 0a0d 0a5b 6567 675f 696e  = src....[egg_in
-00000340: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-00000350: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-00000360: 0a0d 0a                                  ...
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6865 6e78 656c 0a76 6572 7369 6f6e  = henxel.version
+00000020: 203d 2030 2e33 2e31 0a61 7574 686f 7220   = 0.3.1.author 
+00000030: 3d20 5361 6d75 656c 4b6f 730a 6175 7468  = SamuelKos.auth
+00000040: 6f72 5f65 6d61 696c 203d 206b 6f73 6b69  or_email = koski
+00000050: 6e65 6e73 3337 3140 676d 6169 6c2e 636f  nens371@gmail.co
+00000060: 6d0a 6465 7363 7269 7074 696f 6e20 3d20  m.description = 
+00000070: 4755 492d 6564 6974 6f72 2066 6f72 2050  GUI-editor for P
+00000080: 7974 686f 6e20 6465 7665 6c6f 706d 656e  ython developmen
+00000090: 742e 0a6c 6f6e 675f 6465 7363 7269 7074  t..long_descript
+000000a0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
+000000b0: 4d45 2e6d 640a 6c6f 6e67 5f64 6573 6372  ME.md.long_descr
+000000c0: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
+000000d0: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
+000000e0: 6f77 6e0a 7572 6c20 3d20 6874 7470 733a  own.url = https:
+000000f0: 2f2f 6769 7468 7562 2e63 6f6d 2f53 616d  //github.com/Sam
+00000100: 7565 6c4b 6f73 2f68 656e 7865 6c0a 7072  uelKos/henxel.pr
+00000110: 6f6a 6563 745f 7572 6c73 203d 200a 0942  oject_urls = ..B
+00000120: 7567 2054 7261 636b 6572 203d 2068 7474  ug Tracker = htt
+00000130: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000140: 5361 6d75 656c 4b6f 732f 6865 6e78 656c  SamuelKos/henxel
+00000150: 2f69 7373 7565 730a 636c 6173 7369 6669  /issues.classifi
+00000160: 6572 7320 3d20 0a09 5072 6f67 7261 6d6d  ers = ..Programm
+00000170: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000180: 5079 7468 6f6e 203a 3a20 330a 094c 6963  Python :: 3..Lic
+00000190: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+000001a0: 6f76 6564 203a 3a20 474e 5520 4765 6e65  oved :: GNU Gene
+000001b0: 7261 6c20 5075 626c 6963 204c 6963 656e  ral Public Licen
+000001c0: 7365 2076 3320 2847 504c 7633 290a 094f  se v3 (GPLv3)..O
+000001d0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+000001e0: 3a3a 2050 4f53 4958 203a 3a20 4c69 6e75  :: POSIX :: Linu
+000001f0: 780a 094f 7065 7261 7469 6e67 2053 7973  x..Operating Sys
+00000200: 7465 6d20 3a3a 204d 6963 726f 736f 6674  tem :: Microsoft
+00000210: 203a 3a20 5769 6e64 6f77 730a 094f 7065   :: Windows..Ope
+00000220: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000230: 204d 6163 4f53 0a09 496e 7465 6e64 6564   MacOS..Intended
+00000240: 2041 7564 6965 6e63 6520 3a3a 2044 6576   Audience :: Dev
+00000250: 656c 6f70 6572 730a 0954 6f70 6963 203a  elopers..Topic :
+00000260: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
+00000270: 6f70 6d65 6e74 0a09 546f 7069 6320 3a3a  opment..Topic ::
+00000280: 2054 6578 7420 4564 6974 6f72 730a 0a5b   Text Editors..[
+00000290: 6f70 7469 6f6e 735d 0a70 6163 6b61 6765  options].package
+000002a0: 5f64 6972 203d 200a 093d 2073 7263 0a70  _dir = ..= src.p
+000002b0: 6163 6b61 6765 7320 3d20 6669 6e64 3a0a  ackages = find:.
+000002c0: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
+000002d0: 6461 7461 203d 2054 7275 650a 7079 7468  data = True.pyth
+000002e0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
+000002f0: 332e 3132 0a0a 5b6f 7074 696f 6e73 2e70  3.12..[options.p
+00000300: 6163 6b61 6765 732e 6669 6e64 5d0a 7768  ackages.find].wh
+00000310: 6572 6520 3d20 7372 630a 0a5b 6567 675f  ere = src..[egg_
+00000320: 696e 666f 5d0a 7461 675f 6275 696c 6420  info].tag_build 
+00000330: 3d20 0a74 6167 5f64 6174 6520 3d20 300a  = .tag_date = 0.
+00000340: 0a                                       .
```

### Comparing `henxel-0.3.0/src/henxel/__init__.py` & `henxel-0.3.1/src/henxel/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,5737 +1,6337 @@
-############ Stucture briefing Begin
-
-# Stucture briefing
-# TODO
-# Imports
-# Class Tab
-
-####################
-# Class Editor Begin
-#
-# Constants
-# init etc.
-# Linenumbers
-# Tab Related
-# Configuration Related
-# Syntax highlight
-# Theme Related
-# Run file Related
-# Overrides
-# Utilities
-# Save and Load
-# Gotoline and Help
-# Indent and Comment
-# Search
-# Replace
-#
-# Class Editor End
-
-############ Stucture briefing End
-############ TODO Begin
-
-#
-
-############ TODO End
-############ Imports Begin
-
-# from standard library
-import tkinter.font
-import tkinter
-import pathlib
-import json
-import copy
-
-# used in init
-import importlib.resources
-import importlib.metadata
-import sys
-
-# used in syntax highlight
-import tokenize
-import io
-
-# from current directory
-from . import wordexpand
-from . import changefont
-from . import fdialog
-
-# for executing edited file in the same env than this editor, which is nice:
-# It means you have your installed dependencies available. By self.run()
-import subprocess
-
-# for making paste to work in Windows
-import threading
-		
-############ Imports End
-############ Class Tab Begin
-					
-class Tab:
-	'''	Represents a tab-page of an Editor-instance
-	'''
-	
-	def __init__(self, **entries):
-		self.active = True
-		self.filepath = None
-		self.contents = ''
-		self.oldcontents = ''
-		self.position = '1.0'
-		self.type = 'newtab'
-		
-		self.__dict__.update(entries)
-		
-		
-	def __str__(self):
-		
-		return	'\nfilepath: %s\nactive: %s\ntype: %s\nposition: %s' % (
-				str(self.filepath),
-				str(self.active),
-				self.type,
-				self.position
-				)
-				
-				
-############ Class Tab End
-############ Class Editor Begin
-
-###############################################################################
-# config(**options) Modifies one or more widget options. If no options are
-# given, method returns a dictionary containing all current option values.
-#
-# https://www.tcl.tk/man/tcl8.6/TkCmd/event.htm
-# https://docs.python.org/3/library/tkinter.html
-#
-###############################################################################
-
-############ Constants Begin
-CONFPATH = 'editor.cnf'
-ICONPATH = 'editor.png'
-HELPPATH = 'help.txt'
-HELP_MAC = 'help_mac.txt'
-
-VERSION = importlib.metadata.version(__name__)
-
-
-TAB_WIDTH = 4
-TAB_WIDTH_CHAR = 'A'
-
-SLIDER_MINSIZE = 66
-
-
-GOODFONTS = [
-			'Andale Mono',
-			'Noto Mono',
-			'Bitstream Vera Sans Mono',
-			'Liberation Mono',
-			'DejaVu Sans Mono',
-			'Inconsolata',
-			'Courier 10 Pitch',
-			'Consolas',
-			'Courier New',
-			'Noto Sans Mono',
-			'Courier'
-			]
-			
-############ Constants End
-			
-class Editor(tkinter.Toplevel):
-
-	alive = False
-	
-	pkg_contents = None
-	no_icon = True
-	pic = None
-	helptxt = None
-	
-	root = None
-	
-	mac_term = None
-	win_id = None
-	os_type = None
-	
-	if sys.platform == 'darwin': os_type = 'mac_os'
-	elif sys.platform[:3] == 'win': os_type = 'windows'
-	elif sys.platform.count('linux'): os_type = 'linux'
-	else: os_type = 'linux'
-		
-	
-	if os_type == 'mac_os':
-		# macOS: Get name of terminal App.
-		# Used to give focus back to it when closing editor, in quit_me()
-		
-		# This have to be before tkinter.tk()
-		# or we get 'Python' as appname.
-		try:
-			
-##			# With this method we get appname with single run but is still slower
-##			# than the two run method used earlier and now below:
-##			tmp = ['lsappinfo', 'metainfo']
-##			tmp = subprocess.run(tmp, check=True, capture_output=True).stdout.decode()
-##			# Returns many lines.
-##			# Line of interest is like:
-##			#bringForwardOrder = "Terminal" ASN:0x0-0x1438437:  "Safari" ASN:0x0-0x1447446:  "Python" ASN:0x0-0x1452451:  "Finder" ASN:0x0-0x1436435:
-##
-##			# Get that line
-##			tmp = tmp.partition('bringForwardOrder')[2]
-##			# Get appname from line
-##			mac_term = tmp.split(sep='"', maxsplit=2)[1]
-			
-			
-			tmp = ['lsappinfo', 'front']
-			tmp = subprocess.run(tmp, check=True, capture_output=True).stdout.decode()
-			tmp = tmp[:-1]
-			
-			tmp = ('lsappinfo info -only name %s' % tmp).split()
-			tmp = subprocess.run(tmp, check=True, capture_output=True).stdout.decode()
-			tmp = tmp[:-1]
-			mac_term = tmp.split('=')[1].strip('"')
-			
-			# Get window id in case many windows of app is open
-			tmp = ['osascript', '-e', 'id of window 1 of app "%s"' % mac_term]
-			tmp = subprocess.run(tmp, check=True, capture_output=True).stdout.decode()
-			
-			win_id = tmp[:-1]
-			del tmp
-			
-			#print(win_id)
-			#print('AAAAAAAAA', mac_term)
-		
-		except (FileNotFoundError, subprocess.SubprocessError):
-			pass
-
-	
-	def __new__(cls):
-	
-		if not cls.root:
-			#print('BBBB')
-			# Was earlier v.0.2.2 in init:
-
-			# self.root = tkinter.Tk().withdraw()
-
-			# wich worked in Debian 11, but not in Debian 12,
-			# resulted error msg like: class str has no some attribute etc.
-			# After changing this line in init to:
-
-			# self.root = tkinter.Tk()
-			# self.root.withdraw()
-
-			# Editor would launch, but after closing and reopening in the same python-console-instance,
-			# there would be same kind of messages but about icon, and also fonts would change.
-			# This is why that stuff is now here to keep those references.
-
-			cls.root = tkinter.Tk()
-			cls.root.withdraw()
-
-		
-		if not cls.pkg_contents:
-			cls.pkg_contents = importlib.resources.files(__name__)
-			
-
-		if cls.pkg_contents:
-
-			if cls.no_icon:
-				for item in cls.pkg_contents.iterdir():
-
-					if item.name == ICONPATH:
-						try:
-							cls.pic = tkinter.Image("photo", file=item)
-							cls.no_icon = False
-							break
-
-						except tkinter.TclError as e:
-							print(e)
-
-			if not cls.helptxt:
-				for item in cls.pkg_contents.iterdir():
-					
-					helpfile = HELPPATH
-					if cls.os_type == 'mac_os': helpfile = HELP_MAC
-
-					if item.name == helpfile:
-						try:
-							cls.helptxt = item.read_text()
-							break
-
-						except Exception as e:
-							print(e.__str__())
-
-
-		if cls.no_icon: print('Could not load icon-file.')
-
-
-		if not cls.alive:
-			return super(Editor, cls).__new__(cls)
-			
-		else:
-			print('Instance of ', cls, ' already running!\n')
-			
-			# By raising error the object creation is totally aborted.
-			raise ValueError()
-			
-			
-
-	def __init__(self):
-		
-		self.root = self.__class__.root
-		super().__init__(self.root, class_='Henxel', bd=4)
-		self.protocol("WM_DELETE_WINDOW", self.quit_me)
-		
-		
-		# other widgets
-		self.to_be_closed = list()
-		
-		self.ln_string = ''
-		self.want_ln = True
-		self.syntax = True
-		self.oldconf = None
-		self.tab_char = TAB_WIDTH_CHAR
-			
-		if sys.prefix != sys.base_prefix:
-			self.env = sys.prefix
-		else:
-			self.env = None
-		
-		self.tabs = list()
-		self.tabindex = None
-		self.branch = None
-		self.version = VERSION
-		self.os_type = self.__class__.os_type
-		
-		
-		self.font = tkinter.font.Font(family='TkDefaulFont', size=12, name='textfont')
-		self.menufont = tkinter.font.Font(family='TkDefaulFont', size=10, name='menufont')
-		
-		# get current git-branch
-		try:
-			self.branch = subprocess.run('git branch --show-current'.split(),
-					check=True, capture_output=True).stdout.decode().strip()
-		except Exception as e:
-			pass
-		
-		
-		self.search_idx = ('1.0', '1.0')
-		self.search_matches = 0
-		self.old_word = ''
-		self.new_word = ''
-		
-		self.errlines = list()
-		
-		# When clicked with mouse button 1 while searching
-		# to set cursor position to that position clicked.
-		self.save_pos = None
-		
-		# used in load()
-		self.tracevar_filename = tkinter.StringVar()
-		self.tracefunc_name = None
-		self.lastdir = None
-
-		self.check_pars = False
-		self.par_err = False
-		
-		self.waitvar = tkinter.IntVar()
-		self.state = 'normal'
-		
-		
-		self.helptxt = 'Could not load help-file. Press ESC to return.'
-		
-		if self.__class__.helptxt:
-			self.helptxt = self.__class__.helptxt
-					
-		try:
-			self.tk.call('wm','iconphoto', self._w, self.__class__.pic)
-		except tkinter.TclError as e:
-			print(e)
-		
-		
-		# Initiate widgets
-		####################################
-		self.btn_git = tkinter.Button(self, takefocus=0)
-		
-		if self.branch:
-			branch = self.branch[:5]
-			self.btn_git.config(font=self.menufont, relief='flat', highlightthickness=0,
-						padx=0, text=branch, state='disabled')
-
-			if 'main' in self.branch or 'master' in self.branch:
-				self.btn_git.config(disabledforeground='brown1')
-
-		else:
-			self.btn_git.config(font=self.menufont, relief='flat', highlightthickness=0,
-						padx=0, bitmap='info', state='disabled')
-
-		
-		self.entry = tkinter.Entry(self, bd=4, highlightthickness=0)
-		if self.os_type != 'mac_os': self.entry.config(bg='#d9d9d9')
-		self.entry.bind("<Return>", self.load)
-		
-		self.btn_open=tkinter.Button(self, takefocus=0, text='Open', bd=4, highlightthickness=0, command=self.load)
-		self.btn_save=tkinter.Button(self, takefocus=0, text='Save', bd=4, highlightthickness=0, command=self.save)
-		
-		# Get conf:
-		string_representation = None
-		data = None
-		
-		# Try to apply saved configurations:
-		if self.env:
-			p = pathlib.Path(self.env) / CONFPATH
-		
-		if self.env and p.exists():
-			try:
-				with open(p, 'r', encoding='utf-8') as f:
-					string_representation = f.read()
-					data = json.loads(string_representation)
-						
-			except EnvironmentError as e:
-				print(e.__str__())	# __str__() is for user (print to screen)
-				#print(e.__repr__())	# __repr__() is for developer (log to file)
-				print(f'\n Could not load existing configuration file: {p}')
-			
-		if data:
-			self.oldconf = string_representation
-			self.load_config(data)
-			
-		
-		self.ln_widget = tkinter.Text(self, width=4, padx=10, highlightthickness=0, bd=4, pady=4)
-		self.ln_widget.tag_config('justright', justify=tkinter.RIGHT)
-		
-		# disable copying linenumbers:
-		shortcut = '<Mod1-Key-c>'
-		if self.os_type != 'mac_os': shortcut = '<Control-c>'
-		self.ln_widget.bind(shortcut, self.no_copy_ln)
-		
-		self.contents = tkinter.Text(self, undo=True, maxundo=-1, autoseparators=True, tabstyle='wordprocessor', highlightthickness=0, bd=4, pady=4, padx=10)
-		
-		self.scrollbar = tkinter.Scrollbar(self, orient=tkinter.VERTICAL, highlightthickness=0, bd=0, command = self.contents.yview)
-
-		self.expander = wordexpand.ExpandWord(self.contents)
-		shortcut = "<Alt-e>"
-		if self.os_type == 'mac_os': shortcut = "<eacute>"
-		self.contents.bind( shortcut, self.expander.expand_word_event)
-		
-		
-		# Needed in leave() taglink in: Run file Related
-		self.name_of_cursor_in_text_widget = self.contents['cursor']
-		
-		self.popup = tkinter.Menu(self.contents, tearoff=0, bd=0, activeborderwidth=0)
-		self.popup.bind("<FocusOut>", self.popup_focusOut) # to remove popup when clicked outside
-		self.popup.add_command(label="         run", command=self.run)
-		self.popup.add_command(label="        copy", command=self.copy)
-		self.popup.add_command(label="       paste", command=self.paste)
-		self.popup.add_command(label="##   comment", command=self.comment)
-		self.popup.add_command(label="   uncomment", command=self.uncomment)
-		self.popup.add_command(label="  select all", command=self.select_all)
-		self.popup.add_command(label="     inspect", command=self.insert_inspected)
-		self.popup.add_command(label="      errors", command=self.show_errors)
-		self.popup.add_command(label="        help", command=self.help)
-
-
-		# Win11 ctrl-leftright does not work (as supposed) in tcl 8.6.12 but does in
-		# Debian 12, 8.6.13, and macOS 12, 8.6.12   so:
-		self.tcl_version = self.info_patchlevel()
-		if self.os_type == 'windows':
-			if self.tcl_version.major == 8 and self.tcl_version.minor == 6 and self.tcl_version.micro < 13:
-	
-				# To fix: replace array ::tcl::WordBreakRE contents with newer version, and
-				# replace proc tk::TextNextWord with newer version which was looked in Debian 12 from tcl version 8.6.13.
-				# Need for some reason generate ctrl-leftright before, because array ::tcl::WordBreakRE does not exist yet,
-				# but after this event it does:
-	
-				self.contents.insert(1.0, 'asd')
-				self.contents.event_generate('<<NextWord>>')
-				self.contents.delete('1.0', '1.3')
-	
-				self.tk.eval('set l3 [list previous {\W*(\w+)\W*$} after {\w\W|\W\w} next {\w*\W+\w} end {\W*\w+\W} before {^.*(\w\W|\W\w)}] ')
-				self.tk.eval('array set ::tcl::WordBreakRE $l3 ')
-				self.tk.eval('proc tk::TextNextWord {w start} {TextNextPos $w $start tcl_endOfWord} ')
-
-
-		
-		if data:
-			self.apply_config()
-			
-			# Hide selection in linenumbers
-			self.ln_widget.config( selectbackground=self.bgcolor, selectforeground=self.fgcolor, inactiveselectbackground=self.bgcolor )
-			
-		
-		# Colors Begin #######################
-			
-		red = r'#c01c28'
-		cyan = r'#2aa1b3'
-		magenta = r'#a347ba'
-		green = r'#26a269'
-		orange = r'#e95b38'
-		gray = r'#508490'
-		black = r'#000000'
-		white = r'#d3d7cf'
-		
-		
-		self.default_themes = dict()
-		self.default_themes['day'] = d = dict()
-		self.default_themes['night'] = n = dict()
-		
-		# self.default_themes[self.curtheme][tagname] = [backgroundcolor, foregroundcolor]
-		d['normal_text'] = [white, black]
-		n['normal_text'] = [black, white]
-		
-		# if background is same as sel background, change
-		
-		d['keywords'] = ['', orange]
-		n['keywords'] = ['', 'deep sky blue']
-		d['numbers'] = ['', red]
-		n['numbers'] = ['', red]
-		d['bools'] = ['', magenta]
-		n['bools'] = ['', magenta]
-		d['strings'] = ['', green]
-		n['strings'] = ['', green]
-		d['comments'] = ['', gray]
-		n['comments'] = ['', gray]
-		d['calls'] = ['', cyan]
-		n['calls'] = ['', cyan]
-		d['breaks'] = ['', orange]
-		n['breaks'] = ['', orange]
-		d['selfs'] = ['', gray]
-		n['selfs'] = ['', gray]
-		
-		d['match'] = ['lightyellow', 'black']
-		n['match'] = ['lightyellow', 'black']
-		d['focus'] = ['lightgreen', 'black']
-		n['focus'] = ['lightgreen', 'black']
-		d['replaced'] = ['yellow', 'black']
-		n['replaced'] = ['yellow', 'black']
-		
-		d['mismatch'] = ['brown1', 'white']
-		n['mismatch'] = ['brown1', 'white']
-		
-		d['sel'] = ['#c3c3c3', black]
-		n['sel'] = ['#c3c3c3', black]
-		
-		
-		# if no conf:
-		if self.tabindex == None:
-		
-			self.tabindex = -1
-			self.new_tab()
-			
-			self.curtheme = 'night'
-			self.themes = copy.deepcopy(self.default_themes)
-			
-			for tagname in self.themes[self.curtheme]:
-				bg, fg = self.themes[self.curtheme][tagname][:]
-				self.contents.tag_config(tagname, background=bg, foreground=fg)
-			
-			
-			self.bgcolor, self.fgcolor = self.themes[self.curtheme]['normal_text'][:]
-			
-			
-			# Set Font Begin ##################################################
-			fontname = None
-						
-			fontfamilies = [f for f in tkinter.font.families()]
-			
-			for font in GOODFONTS:
-				if font in fontfamilies:
-					fontname = font
-					break
-					
-			if not fontname:
-				fontname = 'TkDefaulFont'
-				
-			
-			size0, size1 = 12, 10
-			# There is no font-scaling in macOS?
-			if self.os_type == 'mac_os': size0, size1 = 22, 16
-				
-				
-			# Initialize rest of configurables
-			self.font.config(family=fontname, size=size0)
-			self.menufont.config(family=fontname, size=size1)
-			
-			self.scrollbar_width, self.elementborderwidth = 16, 2
-			if self.os_type == 'linux': self.scrollbar_width, self.elementborderwidth = 30, 4
-			
-			self.scrollbar.config(width=self.scrollbar_width)
-			self.scrollbar.config(elementborderwidth=self.elementborderwidth)
-			
-			self.ind_depth = TAB_WIDTH
-			self.tab_width = self.font.measure(self.ind_depth * self.tab_char)
-			
-
-
-			# One char lenght is: self.tab_width // self.ind_depth
-			# Use this in measuring padding
-			pad_x =  self.tab_width // self.ind_depth // 3
-			pad_y = pad_x
-
-
-			self.contents.config(font=self.font, foreground=self.fgcolor,
-				background=self.bgcolor, insertbackground=self.fgcolor,
-				tabs=(self.tab_width, ), padx=pad_x, pady=pad_y)
-				
-			self.entry.config(font=self.menufont)
-			self.btn_open.config(font=self.menufont)
-			self.btn_save.config(font=self.menufont)
-			self.popup.config(font=self.menufont)
-			
-			self.btn_git.config(font=self.menufont)
-			
-			self.ln_widget.config(font=self.font, foreground=self.fgcolor, background=self.bgcolor, selectbackground=self.bgcolor, selectforeground=self.fgcolor, inactiveselectbackground=self.bgcolor, state='disabled', padx=pad_x, pady=pad_y)
-
-		
-		# Widgets are initiated, now more configuration
-		################################################
-		# Needed in update_linenums(), there is more info.
-		self.update_idletasks()
-		# if self.y_extra_offset > 0, it needs attention
-		self.y_extra_offset = self.contents['highlightthickness'] + self.contents['bd'] + self.contents['pady']
-		# Needed in update_linenums() and sbset_override()
-		self.bbox_height = self.contents.bbox('@0,0')[3]
-		self.text_widget_height = self.scrollbar.winfo_height()
-				
-		self.contents['yscrollcommand'] = lambda *args: self.sbset_override(*args)
-		
-		
-		
-		
-		# Bindigs Begin
-		####################################################
-		self.right_mousebutton_num = 3
-		
-		if self.os_type == 'mac_os':
-			self.right_mousebutton_num = 2
-			
-			# Default cmd-q does not trigger quit_me
-			# Override Cmd-Q:
-			# https://www.tcl.tk/man/tcl8.6/TkCmd/tk_mac.html
-			self.root.createcommand("tk::mac::Quit", self.quit_me)
-			#self.root.createcommand("tk::mac::OnHide", self.test_hide)
-				
-		self.contents.bind( "<Button-%i>" % self.right_mousebutton_num, self.raise_popup)
-		
-		
-		if self.os_type == 'windows':
-			# fix copying to clipboard in Windows.
-			self.bind( "<Control-c>", self.copy_windows)
-		
-		
-		if self.os_type == 'linux':
-			self.contents.bind( "<ISO_Left_Tab>", self.unindent)
-		
-		
-		############################################################
-		# In macOS all Alt-shortcuts makes some special symbol.
-		# Have to bind to this symbol-name to get Alt-shorcuts work.
-		# For example binding to Alt-f:
-		# self.contents.bind( "<function>", self.font_choose)
-		
-		# Except that tkinter does not give all symbol names, like
-		# Alt-x or l
-		# which makes these key-combinations quite unbindable.
-		# It would be much easier if one could do bindings normally:
-		# Alt-SomeKey
-		# like in Linux and Windows.
-		
-		# Also binding to combinations which has Command-key (apple-key)
-		# (or Meta-key as reported by events.py)
-		# must use Mod1-Key as modifier name:
-		# Mod1-Key-n == Command-Key-n
-		
-		# fn-key -bindings have to be done by checking the state of the event
-		# in proxy-callback: mac_cmd_overrides
-		
-		# In short, In macOS one can not just bind like:
-		# Command-n
-		# fn-f
-		# Alt-f
-		
-		# This is the reason why below is some extra
-		# and strange looking binding-lines when using macOS.
-		##############################################################
-		if self.os_type != 'mac_os':
-			
-			self.bind( "<Alt-n>", self.new_tab)
-			self.contents.bind( "<Alt-s>", self.color_choose)
-			self.contents.bind( "<Alt-t>", self.toggle_color)
-			
-			self.bind( "<Alt-w>", self.walk_tabs)
-			self.bind( "<Alt-q>", lambda event: self.walk_tabs(event, **{'back':True}) )
-			
-			self.contents.bind( "<Alt-Return>", lambda event: self.btn_open.invoke())
-			self.contents.bind( "<Alt-l>", self.toggle_ln)
-			self.contents.bind( "<Alt-x>", self.toggle_syntax)
-			self.contents.bind( "<Alt-f>", self.font_choose)
-		
-			self.contents.bind( "<Control-v>", self.paste)
-			self.contents.bind( "<Control-y>", self.yank_line)
-			
-			self.contents.bind( "<Control-Left>", self.move_by_words)
-			self.contents.bind( "<Control-Right>", self.move_by_words)
-			self.contents.bind( "<Control-Shift-Left>", self.select_by_words)
-			self.contents.bind( "<Control-Shift-Right>", self.select_by_words)
-			
-			# Used in check_next_event
-			self.bid_left = self.contents.bind("<Left>", self.check_sel)
-			self.contents.bind("<Right>", self.check_sel)
-			self.entry.bind("<Left>", self.check_sel)
-			self.entry.bind("<Right>", self.check_sel)
-		
-		
-		#self.os_type == 'mac_os':
-		else:
-			# Used in check_next_event
-			self.bid_left = self.contents.bind( "<Left>", self.mac_cmd_overrides)# + cmd walk_tab, check_sel
-			
-			self.contents.bind( "<Right>", self.mac_cmd_overrides)	# + cmd walk_tab, check_sel
-			self.entry.bind( "<Right>", self.mac_cmd_overrides)		# + cmd check_sel
-			self.entry.bind( "<Left>", self.mac_cmd_overrides)		# + cmd check_sel
-			
-			
-			self.contents.bind( "<f>", self.mac_cmd_overrides)		# + fn full screen
-			
-			# Have to bind using Mod1 as modifier name if want bind to Command-key,
-			# Last line is the only one working:
-			#self.contents.bind( "<Meta-Key-k>", lambda event, arg=('AAA'): print(arg) )
-			#self.contents.bind( "<Command-Key-k>", lambda event, arg=('AAA'): print(arg) )
-			#self.contents.bind( "<Mod1-Key-k>", lambda event, arg=('AAA'): print(arg) )
-			
-			
-			self.contents.bind( "<Mod1-Key-y>", self.yank_line)
-			self.contents.bind( "<Mod1-Key-n>", self.new_tab)
-			self.contents.bind( "<Mod1-Key-f>", self.search)
-			self.contents.bind( "<Mod1-Key-v>", self.paste)
-			self.contents.bind( "<Mod1-Key-R>", self.replace_all)
-			self.contents.bind( "<Mod1-Key-g>", self.gotoline)
-			self.contents.bind( "<Mod1-Key-r>", self.replace)
-			self.contents.bind( "<Mod1-Key-z>", self.undo_override)
-			self.contents.bind( "<Mod1-Key-Z>", self.redo_override)
-			
-			# Could not get keysym for Alt-l and x, so use ctrl
-			self.contents.bind( "<Control-l>", self.toggle_ln)
-			self.contents.bind( "<Control-x>", self.toggle_syntax)
-			
-			self.contents.bind( "<Shift-Tab>", self.unindent)
-			
-			# have to bind to symbol name to get Alt-shorcuts work in macOS
-			# This is: Alt-f
-			self.contents.bind( "<function>", self.font_choose)		# Alt-f
-			self.contents.bind( "<dagger>", self.toggle_color)		# Alt-t
-			self.contents.bind( "<ssharp>", self.color_choose)		# Alt-s
-			
-			
-		#######################################################
-		
-		
-		self.bind( "<Control-R>", self.replace_all)
-		self.bind( "<Control-g>", self.gotoline)
-		self.bind( "<Control-r>", self.replace)
-
-		self.bind( "<Escape>", self.do_nothing )
-		self.bind( "<Return>", self.do_nothing)
-		self.bind( "<Control-minus>", self.decrease_scrollbar_width)
-		self.bind( "<Control-plus>", self.increase_scrollbar_width)
-		
-		self.contents.bind( "<Control-a>", self.goto_linestart)
-		self.contents.bind( "<Control-e>", self.goto_lineend)
-		self.contents.bind( "<Control-A>", self.goto_linestart)
-		self.contents.bind( "<Control-E>", self.goto_lineend)
-		
-		if self.os_type == 'windows':
-			self.entry.bind( "<Control-E>", lambda event, arg=('<<SelectLineEnd>>'): self.entry.event_generate)
-			self.entry.bind( "<Control-A>", lambda event, arg=('<<SelectLineStart>>'): self.entry.event_generate)
-		
-		
-		self.contents.bind( "<Control-i>", self.move_right)
-		self.contents.bind( "<Control-b>", self.move_left)
-		self.contents.bind( "<Control-n>", self.move_down)
-		self.contents.bind( "<Control-p>", self.move_up)
-		
-		self.contents.bind( "<Control-j>", self.center_view)
-		self.contents.bind( "<Control-u>", lambda event: self.center_view(event, **{'up':True}) )
-		
-		self.contents.bind( "<Return>", self.return_override)
-		
-		self.contents.bind( "<Control-d>", self.del_tab)
-		self.contents.bind( "<Control-q>", lambda event: self.del_tab(event, **{'save':False}) )
-		
-		self.contents.bind( "<Shift-Return>", self.comment)
-		self.contents.bind( "<Shift-BackSpace>", self.uncomment)
-		self.contents.bind( "<Tab>", self.tab_override)
-		
-		self.contents.bind( "<Control-t>", self.tabify_lines)
-		self.contents.bind( "<Control-z>", self.undo_override)
-		self.contents.bind( "<Control-Z>", self.redo_override)
-		self.contents.bind( "<Control-f>", self.search)
-		
-		self.contents.bind( "<BackSpace>", self.backspace_override)
-		self.contents.bind( "<Control-BackSpace>", self.search_next)
-		
-		
-##		# this move_line interferes with search_next,check_nextevent, so not in use
-##		self.contents.bind("<Left>", lambda event: self.move_line(event, **{'direction':'left'} ))
-##		self.contents.bind("<Right>", lambda event: self.move_line(event, **{'direction':'right'} ))
-##
-##		# updown_override not in use
-##		self.contents.bind("<Up>", lambda event: self.updown_override(event, **{'direction':'up'} ))
-##		self.contents.bind("<Down>", lambda event: self.updown_override(event, **{'direction':'down'} ))
-		
-		
-		# Unbind some default bindings
-		# Paragraph-bindings: too easy to press by accident
-		self.contents.unbind_class('Text', '<<NextPara>>')
-		self.contents.unbind_class('Text', '<<PrevPara>>')
-		self.contents.unbind_class('Text', '<<SelectNextPara>>')
-		self.contents.unbind_class('Text', '<<SelectPrevPara>>')
-		
-		# LineStart and -End:
-		# fix goto_linestart-end and
-		# enable tab-walking in mac_os with cmd-left-right
-		self.contents.unbind_class('Text', '<<LineStart>>')
-		self.contents.unbind_class('Text', '<<LineEnd>>')
-		self.contents.unbind_class('Text', '<<SelectLineEnd>>')
-		self.contents.unbind_class('Text', '<<SelectLineStart>>')
-		
-		
-		self.helptxt = f'{self.helptxt}\n\nHenxel v. {self.version}'
-		
-		# Widgets are configured
-		###############################
-		#
-		# Syntax-highlight Begin #################
-		
-		self.keywords = [
-						'self',
-						'False',
-						'True',
-						'None',
-						'break',
-						'for',
-						'not',
-						'class',
-						'from',
-						'or',
-						'continue',
-						'global',
-						'pass',
-						'def',
-						'if',
-						'raise',
-						'and',
-						'del',
-						'import',
-						'return',
-						'as',
-						'elif',
-						'in',
-						'try',
-						'assert',
-						'else',
-						'is',
-						'while',
-						'async',
-						'except',
-						'lambda',
-						'with',
-						'await',
-						'finally',
-						'nonlocal',
-						'yield',
-						'open'
-						]
-						
-		self.bools = [ 'False', 'True', 'None' ]
-		self.breaks = [
-						'break',
-						'return',
-						'continue',
-						'pass',
-						'raise',
-						'assert',
-						'yield'
-						]
-						
-		self.tests = [
-					'not',
-					'or',
-					'and',
-					'in',
-					'as'
-					]
-		
-		self.tagnames = [
-				'keywords',
-				'numbers',
-				'bools',
-				'strings',
-				'comments',
-				'breaks',
-				'calls',
-				'selfs'
-				]
-		
-		
-		self.boldfont = self.font.copy()
-		self.boldfont.config(weight='bold')
-		
-		self.contents.tag_config('keywords', font=self.boldfont)
-		self.contents.tag_config('numbers', font=self.boldfont)
-		self.contents.tag_config('comments', font=self.boldfont)
-		self.contents.tag_config('breaks', font=self.boldfont)
-		self.contents.tag_config('calls', font=self.boldfont)
-
-		# search tags have highest priority
-		self.contents.tag_raise('match')
-		self.contents.tag_raise('replaced')
-		self.contents.tag_raise('focus')
-		
-		
-		self.oldline = ''
-		self.token_err = False
-		self.token_can_update = False
-		self.oldlinenum = self.contents.index(tkinter.INSERT).split('.')[0]
-		
-		self.do_syntax(everything=True)
-			
-		self.contents.bind( "<<WidgetViewSync>>", self.viewsync)
-		# Viewsync-event does not trigger at window size changes,
-		# to get linenumbers right, we bind to this:
-		self.contents.bind("<Configure>", self.handle_configure)
-		
-		
-		####  Syntax-highlight End  ######################################
-		
-		# Layout Begin
-		################################
-		self.rowconfigure(1, weight=1)
-		self.columnconfigure(1, weight=1)
-		
-		# It seems that widget is shown on screen when doing grid_configure
-		self.btn_git.grid_configure(row=0, column = 0, sticky='nsew')
-		self.entry.grid_configure(row=0, column = 1, sticky='nsew')
-		self.btn_open.grid_configure(row=0, column = 2, sticky='nsew')
-		self.btn_save.grid_configure(row=0, column = 3, columnspan=2, sticky='nsew')
-		
-		
-		self.ln_widget.grid_configure(row=1, column = 0, sticky='nswe')
-			
-		# If want linenumbers:
-		if self.want_ln:
-			self.contents.grid_configure(row=1, column=1, columnspan=3, sticky='nswe')
-		
-		else:
-			self.contents.grid_configure(row=1, column=0, columnspan=4, sticky='nswe')
-			self.ln_widget.grid_remove()
-			
-		self.scrollbar.grid_configure(row=1,column=4, sticky='nse')
-
-		
-		# set cursor pos:
-		line = self.tabs[self.tabindex].position
-		
-		if self.os_type == 'windows':
-			self.contents.focus_force()
-		else:
-			self.contents.focus_set()
-		
-		
-		try:
-			self.contents.mark_set('insert', line)
-			self.ensure_idx_visibility(line)
-			
-		except tkinter.TclError:
-			self.contents.mark_set('insert', '1.0')
-			self.tabs[self.tabindex].position = '1.0'
-			self.contents.see('1.0')
-				
-		
-		self.avoid_viewsync_mess()
-		self.update_idletasks()
-		self.viewsync()
-		self.__class__.alive = True
-		self.update_title()
-		
-		############################# init End ##########################
-		
-	
-	def update_title(self, event=None):
-		tail = len(self.tabs) - self.tabindex - 1
-		self.title( f'Henxel {"0"*self.tabindex}@{"0"*(tail)}' )
-		
-	
-	def handle_configure(self, event=None):
-		'''	In case of size change, like maximize etc. viewsync-event is not
-			generated in such situation so need to bind to <Configure>-event.
-		'''
-		self.text_widget_height = self.scrollbar.winfo_height()
-		self.update_linenums()
-		
-	
-	def copy_windows(self, event=None):
-		
-		
-		try:
-			#self.clipboard_clear()
-			tmp = self.selection_get()
-			
-			
-			# https://stackoverflow.com/questions/51921386
-			# pyperclip approach works in windows fine
-			# import clipboard as cb
-			# cb.copy(tmp)
-			
-			# os.system approach also works but freezes editor for a little time
-			
-			
-			d = dict()
-			d['input'] = tmp.encode('ascii')
-			
-			t = threading.Thread( target=subprocess.run, args=('clip',), kwargs=d, daemon=True )
-			#t.setDeamon(True)
-			t.start()
-			
-				
-			#self.clipboard_append(tmp)
-		except tkinter.TclError:
-			# is empty
-			return 'break'
-			
-			
-		#print(#self.clipboard_get())
-		return 'break'
-		
-	
-	def wait_for(self, ms):
-		self.waitvar.set(False)
-		self.after(ms, self.waiter)
-		self.wait_variable(self.waitvar)
-		
-	
-	def waiter(self):
-		self.waitvar.set(True)
-		
-	
-	def do_nothing(self, event=None):
-		self.bell()
-		return 'break'
-		
-	
-	def do_nothing_without_bell(self, event=None):
-		return 'break'
-	
-	
-	def test_bind(self, event=None):
-		print('jou')
-	
-	
-	def skip_bindlevel(self, event=None):
-		return 'continue'
-		
-	
-	def ensure_idx_visibility(self, index, back=None):
-		b=2
-		if back:
-			b=back
-			
-		self.contents.mark_set('insert', index)
-		s = self.contents.bbox('%s - %ilines' % (index,b))
-		e = self.contents.bbox('%s + 4lines' % index)
-		
-		tests = [
-				not s,
-				not e,
-				( s and s[1] < 0 )
-				]
-				
-		if any(tests):
-			self.contents.see('%s - %ilines' % (index,b))
-			self.update_idletasks()
-			self.contents.see('%s + 4lines' % index)
-		
-		
-	def quit_me(self, event=None):
-	
-		self.save(forced=True)
-		self.save_config()
-		
-		# affects color, fontchoose, load:
-		for widget in self.to_be_closed:
-			widget.destroy()
-		
-		self.quit()
-		self.destroy()
-		
-		
-		# Activate terminal
-		if self.os_type == 'mac_os':
-		
-			# This osascript-language is funny
-			# https://ss64.com/osx/osascript.html
-			
-			mac_term = 'Terminal'
-			
-			
-			
-			try:
-				# Giving focus back to python terminal-window is not very simple task in macOS
-				# https://apple.stackexchange.com/questions/421137
-				tmp = None
-				if self.__class__.mac_term and self.__class__.win_id:
-					mac_term = self.__class__.mac_term
-					win_id  = self.__class__.win_id
-
-					
-					if mac_term == 'iTerm2':
-						tmp = [ 'osascript', '-e', 'tell app "%s" to select windows whose id = %s' % (mac_term, win_id), '-e', 'tell app "%s" to activate' % mac_term ]
-						
-					else:
-						tmp = [ 'osascript', '-e', 'tell app "%s" to set frontmost of windows whose id = %s to true' % (mac_term, win_id), '-e', 'tell app "%s" to activate' % mac_term ]
-
-
-
-
-				elif self.__class__.mac_term:
-					mac_term = self.__class__.mac_term
-					tmp = ['osascript', '-e', 'tell app "%s" to activate' % mac_term ]
-
-				else:
-					tmp = ['osascript', '-e', 'tell app "%s" to activate' % mac_term ]
-
-				subprocess.run(tmp)
-
-
-			except (FileNotFoundError, subprocess.SubprocessError):
-				pass
-			
-			# No need to put in thread
-			#t = threading.Thread( target=subprocess.run, args=(tmp,), daemon=True )
-			#t.start()
-			
-		
-		if self.tracefunc_name:
-			self.tracevar_filename.trace_remove('write', self.tracefunc_name)
-		
-		del self.font
-		del self.menufont
-		del self.boldfont
-		
-		# this is maybe not necessary
-		del self.entry
-		del self.btn_open
-		del self.btn_save
-		del self.btn_git
-		del self.contents
-		del self.ln_widget
-		del self.scrollbar
-		del self.popup
-				
-		self.__class__.alive = False
-		
-	
-	def avoid_viewsync_mess(self, event=None):
-		# Avoid viewsync messing when cursor
-		# position is in line with multiline string marker:
-		
-		if self.tabs[self.tabindex].filepath:
-			if self.can_do_syntax():
-				pos = self.tabs[self.tabindex].position
-				lineend = '%s lineend' % pos
-				linestart = '%s linestart' % pos
-				tmp = self.contents.get( linestart, lineend )
-				self.oldline = tmp
-				self.oldlinenum = pos.split('.')[0]
-				self.token_can_update = True
-
-
-	def viewsync(self, event=None):
-		'''	Triggered when event is <<WidgetViewSync>>
-			Used to update linenumbers and syntax highlight.
-		
-			This event itself is generated *after* when inserting, deleting or on screen geometry change, but
-			not when just scrolling (like yview). Almost all font-changes also generates this event.
-		'''
-		
-		# More info in update_linenums()
-		self.bbox_height = self.contents.bbox('@0,0')[3]
-		self.text_widget_height = self.scrollbar.winfo_height()
-		self.update_linenums()
-		
-		if self.tabs[self.tabindex].filepath:
-			if self.can_do_syntax():
-				if self.token_can_update:
-				
-					#  tag alter triggers this event if font changes, like from normal to bold.
-					# --> need to check if line is changed to prevent self-trigger
-					line_idx = self.contents.index( tkinter.INSERT )
-					linenum = line_idx.split('.')[0]
-					#prev_char = self.contents.get( '%s - 1c' % tkinter.INSERT )
-					
-					
-					lineend = '%s lineend' % line_idx
-					linestart = '%s linestart' % line_idx
-					
-					tmp = self.contents.get( linestart, lineend )
-					
-					if self.oldline != tmp or self.oldlinenum != linenum:
-					
-						#print('sync')
-						self.oldline = tmp
-						self.oldlinenum = linenum
-						self.update_tokens(start=linestart, end=lineend, line=tmp)
-				
-
-############## Linenumbers Begin
-
-	def no_copy_ln(self, event=None):
-		return 'break'
-		
-	
-	def toggle_ln(self, event=None):
-		
-		# if dont want linenumbers:
-		if self.want_ln:
-			# remove remembers grid-options
-			self.ln_widget.grid_remove()
-			self.contents.grid_configure(column=0, columnspan=4)
-			self.want_ln = False
-		else:
-			self.contents.grid_configure(column=1, columnspan=3)
-			self.ln_widget.grid()
-			
-			self.want_ln = True
-		
-		return 'break'
-		
-	
-	def get_linenums(self):
-
-		x = 0
-		line = '0'
-		col= ''
-		ln = ''
-
-		# line-height is used as step, it depends on font:
-		step = self.bbox_height
-
-		nl = '\n'
-		lineMask = '%s\n'
-		
-		# @x,y is tkinter text-index -notation:
-		# The character that covers the (x,y) -coordinate within the text's window.
-		indexMask = '@0,%d'
-		
-		# stepping lineheight at time, checking index of each lines first cell, and splitting it.
-		
-		for i in range(0, self.text_widget_height, step):
-
-			ll, cc = self.contents.index( indexMask % i).split('.')
-
-			if line == ll:
-				# is the line wrapping:
-				if col != cc:
-					col = cc
-					ln += nl
-			else:
-				line, col = ll, cc
-				# -5: show up to four smallest number (0-9999)
-				# then starts again from 0 (when actually 10000)
-				ln += (lineMask % line)[-5:]
-				
-		return ln
-
-	
-	def update_linenums(self):
-
-		# self.ln_widget is linenumber-widget,
-		# self.ln_string is string which holds the linenumbers in self.ln_widget
-		tt = self.ln_widget
-		ln = self.get_linenums()
-		
-		if self.ln_string != ln:
-			self.ln_string = ln
-			
-			# 1 - 3 : adjust linenumber-lines with text-lines
-			
-			# 1:
-			# @0,0 is currently visible first character at
-			# x=0 y=0 in text-widget.
-			
-			# 2: bbox returns this kind of tuple: (3, -9, 19, 38)
-			# (bbox is cell that holds a character)
-			# (x-offset, y-offset, width, height) in pixels
-			# Want y-offset of first visible line, and reverse it:
-			
-			y_offset = self.contents.bbox('@0,0')[1]
-			
-			y_offset *= -1
-			
-			#if self.y_extra_offset > 0, we need this:
-			if y_offset != 0:
-				y_offset += self.y_extra_offset
-				
-			tt.config(state='normal')
-			tt.delete('1.0', tkinter.END)
-			tt.insert('1.0', self.ln_string)
-			tt.tag_add('justright', '1.0', tkinter.END)
-			
-			# 3: Then scroll lineswidget same amount to fix offset
-			# compared to text-widget:
-			tt.yview_scroll(y_offset, 'pixels')
-
-			tt.config(state='disabled')
-
-		
-############## Linenumbers End
-############## Tab Related Begin
-
-	
-	def mac_cmd_overrides(self, event=None):
-		
-		
-		# Pressed Cmd + Shift + arrow left or right.
-		# Want: select line from cursor.
-		if event.state == 105:
-		
-			# self.contents or self.entry
-			wid = event.widget
-			
-			# Enable select from in entry
-			if wid == self.entry: return
-			
-			# Enable select from in contents
-			elif wid == self.contents:
-				
-				if event.keysym == 'Right':
-					self.goto_lineend(event=event)
-					
-				elif event.keysym == 'Left':
-					self.goto_linestart(event=event)
-		
-				else:
-					return
-			
-			return 'break'
-		
-		
-		# Pressed Cmd + arrow left or right.
-		elif event.state == 104:
-	
-			if event.keysym == 'Right':
-				self.walk_tabs(event=event)
-				
-			elif event.keysym == 'Left':
-				self.walk_tabs(event=event, **{'back':True})
-	
-			else:
-				return
-			
-			return 'break'
-			
-			
-		# Pressed Alt + arrow left or right.
-		elif event.state == 112:
-			res = self.move_by_words(event=event)
-			return res
-		
-		# disabled as inconsistent
-		# Pressed Alt + Shift + arrow left or right.
-		elif event.state == 113:
-			res = self.select_by_words(event=event)
-			return res
-			
-			
-		# Pressed arrow left or right.
-		# If have selection, put cursor on the wanted side of selection.
-		elif event.state == 96:
-			
-			# self.contents or self.entry
-			wid = event.widget
-			have_selection = False
-
-			if wid == self.entry:
-				have_selection = self.entry.selection_present()
-
-			elif wid == self.contents:
-				have_selection = len(self.contents.tag_ranges('sel')) > 0
-
-			else:
-				return
-
-			if have_selection:
-				if event.keysym == 'Right':
-					self.check_sel(event=event)
-						
-				elif event.keysym == 'Left':
-					self.check_sel(event=event)
-			
-			else:
-				return
-				
-			return 'break'
-			
-		
-		# Pressed Fn
-		elif event.state == 64:
-			
-			# fullscreen
-			if event.keysym == 'f':
-				#pass
-				return 'break'
-
-			# Some shortcuts does not insert.
-			# Like fn-h does not insert h.
-			else:
-				return
-	
-	
-	def new_tab(self, event=None, error=False):
-	
-		# event == None when clicked hyper-link in tag_link()
-		if self.state != 'normal' and event != None:
-			self.bell()
-			return 'break'
-		
-		
-		
-		if len(self.tabs) > 0  and not error:
-			try:
-				pos = self.contents.index(tkinter.INSERT)
-				
-			except tkinter.TclError:
-				pos = '1.0'
-				
-			self.tabs[self.tabindex].position = pos
-			
-			tmp = self.contents.get('1.0', tkinter.END)
-			# [:-1]: remove unwanted extra newline
-			self.tabs[self.tabindex].contents = tmp[:-1]
-			
-			
-		self.contents.delete('1.0', tkinter.END)
-		self.entry.delete(0, tkinter.END)
-		
-		if len(self.tabs) > 0:
-			self.tabs[self.tabindex].active = False
-			
-		newtab = Tab()
-		
-		self.tabindex += 1
-		self.tabs.insert(self.tabindex, newtab)
-		
-		self.contents.focus_set()
-		self.contents.see('1.0')
-		self.contents.mark_set('insert', '1.0')
-		
-		self.contents.edit_reset()
-		self.contents.edit_modified(0)
-		
-		self.update_title()
-		return 'break'
-		
-		
-	def del_tab(self, event=None, save=True):
-
-		if self.state != 'normal':
-			self.bell()
-			return 'break'
-			
-		if ((len(self.tabs) == 1) and self.tabs[self.tabindex].type == 'newtab'):
-			self.contents.delete('1.0', tkinter.END)
-			self.bell()
-			return 'break'
-
-		if self.tabs[self.tabindex].type == 'normal' and save:
-			self.save(activetab=True)
-			
-		self.tabs.pop(self.tabindex)
-			
-		if (len(self.tabs) == 0):
-			newtab = Tab()
-			self.tabs.append(newtab)
-	
-		if self.tabindex > 0:
-			self.tabindex -= 1
-	
-		self.tabs[self.tabindex].active = True
-		self.entry.delete(0, tkinter.END)
-		
-		if self.tabs[self.tabindex].filepath:
-			self.entry.insert(0, self.tabs[self.tabindex].filepath)
-		
-		
-		self.contents.delete('1.0', tkinter.END)
-		self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
-		
-		
-		self.do_syntax(everything=True)
-		
-		# set cursor pos
-		line = self.tabs[self.tabindex].position
-		self.contents.focus_set()
-		
-		try:
-			self.contents.mark_set('insert', line)
-			self.ensure_idx_visibility(line)
-			
-		except tkinter.TclError:
-			self.contents.mark_set('insert', '1.0')
-			self.tabs[self.tabindex].position = '1.0'
-			self.contents.see('1.0')
-		
-			
-		self.contents.edit_reset()
-		self.contents.edit_modified(0)
-		
-		self.avoid_viewsync_mess()
-		self.update_title()
-		
-		return 'break'
-
-		
-	def walk_tabs(self, event=None, back=False):
-	
-		if self.state != 'normal' or len(self.tabs) < 2:
-			self.bell()
-			return "break"
-		
-		
-		self.tabs[self.tabindex].active = False
-		
-		try:
-			pos = self.contents.index(tkinter.INSERT)
-		except tkinter.TclError:
-			pos = '1.0'
-		
-		self.tabs[self.tabindex].position = pos
-			
-		tmp = self.contents.get('1.0', tkinter.END)
-		# [:-1]: remove unwanted extra newline
-		self.tabs[self.tabindex].contents = tmp[:-1]
-			
-		idx = self.tabindex
-		
-		if back:
-			if idx == 0:
-				idx = len(self.tabs)
-			idx -= 1
-			
-		else:
-			if idx == len(self.tabs) - 1:
-				idx = -1
-			idx += 1
-		
-		self.tabindex = idx
-		self.tabs[self.tabindex].active = True
-		self.entry.delete(0, tkinter.END)
-
-
-		if self.tabs[self.tabindex].filepath:
-			self.entry.insert(0, self.tabs[self.tabindex].filepath)
-			
-		
-		self.token_can_update = False
-		self.contents.delete('1.0', tkinter.END)
-		self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
-	
-		if self.tabs[self.tabindex].filepath:
-			if self.can_do_syntax():
-				self.update_tokens(start='1.0', end=tkinter.END, everything=True)
-
-		# set cursor pos
-		line = self.tabs[self.tabindex].position
-		self.contents.focus_set()
-		
-		try:
-			self.contents.mark_set('insert', line)
-			self.ensure_idx_visibility(line)
-			
-		except tkinter.TclError:
-			self.contents.mark_set('insert', '1.0')
-			self.tabs[self.tabindex].position = '1.0'
-			self.contents.see('1.0')
-
-		
-		self.contents.edit_reset()
-		self.contents.edit_modified(0)
-		
-		self.avoid_viewsync_mess()
-		self.update_title()
-		
-		return 'break'
-
-########## Tab Related End
-########## Configuration Related Begin
-
-	def save_config(self, event=None):
-		data = self.get_config()
-		
-		string_representation = json.dumps(data)
-		
-		if string_representation == self.oldconf:
-			return
-			
-		if self.env:
-			p = pathlib.Path(self.env) / CONFPATH
-			try:
-				with open(p, 'w', encoding='utf-8') as f:
-					f.write(string_representation)
-			except EnvironmentError as e:
-				print(e.__str__())
-				print('\nCould not save configuration')
-		else:
-			print('\nNot saving configuration when not in venv.')
-		
-	
-	def load_config(self, data):
-		
-		font, menufont = self.fonts_exists(data)
-		self.set_config(data, font, menufont)
-		
-	
-	def fonts_exists(self, dictionary):
-		
-		res = True
-		fontfamilies = [f for f in tkinter.font.families()]
-		
-		font = dictionary['font']['family']
-		
-		if font not in fontfamilies:
-			print(f'Font {font.upper()} does not exist.')
-			font = False
-		
-		menufont = dictionary['menufont']['family']
-		
-		if dictionary['menufont']['family'] not in fontfamilies:
-			print(f'Font {menufont.upper()} does not exist.')
-			menufont = False
-			
-		return font, menufont
-		
-		
-	def get_config(self):
-		dictionary = dict()
-		dictionary['curtheme'] = self.curtheme
-		dictionary['lastdir'] = self.lastdir.__str__()
-		
-		# Replace possible Tkdefaulfont as family with real name,
-		# if not mac_os, because tkinter.font.Font does not recognise
-		# this: .APPLESYSTEMUIFONT
-
-		if self.os_type == 'mac_os':
-		
-			if self.font.cget('family') == 'TkDefaulFont':
-				dictionary['font'] = self.font.config()
-				
-			else:
-				dictionary['font'] = self.font.actual()
-				
-			if self.menufont.cget('family') == 'TkDefaulFont':
-				dictionary['menufont'] = self.menufont.config()
-				
-			else:
-				dictionary['menufont'] = self.menufont.actual()
-				
-		else:
-			dictionary['font'] = self.font.actual()
-			dictionary['menufont'] = self.menufont.actual()
-
-		
-		dictionary['scrollbar_width'] = self.scrollbar_width
-		dictionary['elementborderwidth'] = self.elementborderwidth
-		dictionary['want_ln'] = self.want_ln
-		dictionary['syntax'] = self.syntax
-		dictionary['ind_depth'] = self.ind_depth
-		dictionary['themes'] = self.themes
-		
-		for tab in self.tabs:
-			tab.contents = ''
-			tab.oldcontents = ''
-			
-			# Convert tab.filepath to string for serialization
-			if tab.filepath:
-				tab.filepath = tab.filepath.__str__()
-		
-		tmplist = [ tab.__dict__ for tab in self.tabs ]
-		dictionary['tabs'] = tmplist
-		
-		return dictionary
-		
-		
-	def set_config(self, dictionary, font, menufont):
-		
-		# Set Font Begin ##############################
-		
-		# Both missing:
-		if not font and not menufont:
-			fontname = None
-			
-			fontfamilies = [f for f in tkinter.font.families()]
-			
-			for font in GOODFONTS:
-				if font in fontfamilies:
-					fontname = font
-					break
-			
-			if not fontname:
-				fontname = 'TkDefaulFont'
-				
-			dictionary['font']['family'] = fontname
-			dictionary['menufont']['family'] = fontname
-		
-		# One missing, copy existing:
-		elif bool(font) ^ bool(menufont):
-			if font:
-				dictionary['menufont']['family'] = font
-			else:
-				dictionary['font']['family'] = menufont
-			
-			
-		self.font.config(**dictionary['font'])
-		self.menufont.config(**dictionary['menufont'])
-		self.scrollbar_width 	= dictionary['scrollbar_width']
-		self.elementborderwidth	= dictionary['elementborderwidth']
-		self.want_ln = dictionary['want_ln']
-		self.syntax = dictionary['syntax']
-		self.ind_depth = dictionary['ind_depth']
-		self.themes = dictionary['themes']
-		self.curtheme = dictionary['curtheme']
-		
-		self.bgcolor, self.fgcolor = self.themes[self.curtheme]['normal_text'][:]
-			
-		self.lastdir = dictionary['lastdir']
-		
-		if self.lastdir != None:
-			self.lastdir = pathlib.Path(dictionary['lastdir'])
-			if not self.lastdir.exists():
-				self.lastdir = None
-		
-		self.tabs = [ Tab(**item) for item in dictionary['tabs'] ]
-		
-		# Have to step backwards here to avoid for-loop breaking
-		# while removing items from the container.
-		
-		for i in range(len(self.tabs)-1, -1, -1):
-			tab = self.tabs[i]
-			
-			if tab.type == 'normal':
-				try:
-					with open(tab.filepath, 'r', encoding='utf-8') as f:
-						tmp = f.read()
-						tab.contents = tmp
-						tab.oldcontents = tab.contents
-						
-					tab.filepath = pathlib.Path(tab.filepath)
-					
-					
-				except (EnvironmentError, UnicodeDecodeError) as e:
-					print(e.__str__())
-					self.tabs.pop(i)
-			else:
-				tab.filepath = None
-				tab.position = '1.0'
-				
-		for i,tab in enumerate(self.tabs):
-			if tab.active == True:
-				self.tabindex = i
-				break
-		
-
-	def apply_config(self):
-		
-		if self.tabindex == None:
-			if len(self.tabs) == 0:
-				self.tabindex = -1
-				self.new_tab()
-			# recently active normal tab is gone:
-			else:
-				self.tabindex = 0
-				self.tabs[self.tabindex].active = True
-		
-
-		self.tab_width = self.font.measure(self.ind_depth * TAB_WIDTH_CHAR)
-		
-		pad_x =  self.tab_width // self.ind_depth // 3
-		pad_y = pad_x
-
-		for tagname in self.themes[self.curtheme]:
-			bg, fg = self.themes[self.curtheme][tagname][:]
-			self.contents.tag_config(tagname, background=bg, foreground=fg)
-		
-		
-		self.contents.config(font=self.font, foreground=self.fgcolor,
-			background=self.bgcolor, insertbackground=self.fgcolor,
-			tabs=(self.tab_width, ), padx=pad_x, pady=pad_y)
-			
-		self.scrollbar.config(width=self.scrollbar_width)
-		self.scrollbar.config(elementborderwidth=self.elementborderwidth)
-		
-		self.ln_widget.config(font=self.font, foreground=self.fgcolor, background=self.bgcolor,
-			padx=pad_x, pady=pad_y)
-			
-		self.entry.config(font=self.menufont)
-		self.btn_open.config(font=self.menufont)
-		self.btn_save.config(font=self.menufont)
-		self.btn_git.config(font=self.menufont)
-		self.popup.config(font=self.menufont)
-		
-		if self.tabs[self.tabindex].type == 'normal':
-			self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
-			self.entry.insert(0, self.tabs[self.tabindex].filepath)
-			
-		self.contents.edit_reset()
-		self.contents.edit_modified(0)
-		
-########## Configuration Related End
-########## Syntax highlight Begin
-	
-	def toggle_syntax(self, event=None):
-		
-		if self.syntax:
-			self.syntax = False
-			self.token_can_update = False
-			
-			for tag in self.tagnames:
-				self.contents.tag_remove( tag, '1.0', tkinter.END )
-				
-			return 'break'
-	
-		else:
-			self.syntax = True
-			self.do_syntax(everything=True)
-			
-			return 'break'
-			
-	
-	def can_do_syntax(self):
-	
-		return '.py' in self.tabs[self.tabindex].filepath.suffix and self.syntax
-		
-		
-	def do_syntax(self, everything=False):
-	
-		if self.tabs[self.tabindex].filepath:
-			if self.can_do_syntax():
-			
-				self.token_err = True
-				content_is_uptodate = everything
-				self.update_tokens(start='1.0', end=tkinter.END, everything=content_is_uptodate)
-				self.token_can_update = True
-				
-			else:
-				self.token_err = False
-				self.token_can_update = False
-			
-		else:
-			self.token_err = False
-			self.token_can_update = False
-			
-	
-	def update_tokens(self, start=None, end=None, line=None, everything=False):
-	
-		start_idx = start
-		end_idx = end
-		linecontents = None
-		
-		if not everything:
-			if line:
-				linecontents = line
-				test1 = [
-					self.token_err,
-					( '"""' in linecontents and '#' in linecontents ),
-					( "'''" in linecontents and '#' in linecontents )
-					]
-			else:
-				test1 = [self.token_err]
-				
-				
-			if any(test1):
-				start_idx = '1.0'
-				end_idx = tkinter.END
-				linecontents = None
-				#print('err')
-		
-			# check if inside multiline string
-			elif 'strings' in self.contents.tag_names(tkinter.INSERT) and \
-					not ( start_idx == '1.0' and end_idx == tkinter.END ):
-				
-				try:
-					s, e = self.contents.tag_prevrange('strings', tkinter.INSERT)
-					l0, l1 = map( lambda x: int( x.split('.')[0] ), [s, e] )
-				
-					if l0 != l1:
-						start_idx, end_idx = (s, e)
-						linecontents = None
-		
-				except ValueError:
-					pass
-			
-			
-			if not linecontents:
-				tmp = self.contents.get( start_idx, end_idx )
-				
-			else:
-				tmp = linecontents
-				
-		else:
-			tmp = self.tabs[self.tabindex].contents
-			
-		
-		
-		prev_char = self.contents.get( '%s - 1c' % tkinter.INSERT, tkinter.INSERT )
-		if prev_char in [ '(', ')', '[', ']' , '{', '}' ]:
-			self.par_err = True
-		
-		linenum = int(start_idx.split('.')[0])
-		flag_err = False
-		#print(self.token_err)
-		
-		
-		try:
-			par_err = None
-			
-			with io.BytesIO( tmp.encode('utf-8') ) as fo:
-			
-				tokens = tokenize.tokenize( fo.readline )
-			
-				# Remove old tags:
-				for tag in self.tagnames:
-					self.contents.tag_remove( tag, start_idx, end_idx )
-					
-				# Retag:
-				idx_start = None
-				for token in tokens:
-					#print(token)
-					
-					# token.line contains line as string which contains token.
-					
-					if token.type == tokenize.NAME or \
-						( token.type in [ tokenize.NUMBER, tokenize.STRING, tokenize.COMMENT] ) or \
-						( token.exact_type == tokenize.LPAR ):
-						
-						# initiate indexes with correct linenum
-						s0, s1 = map(str, [ token.start[0] + linenum - 1, token.start[1] ] )
-						e0, e1 = map(str, [ token.end[0] + linenum - 1, token.end[1] ] )
-						idx_start = s0 + '.' + s1
-						idx_end = e0 + '.' + e1
-						
-							
-						if token.type == tokenize.NAME:
-							
-							#lastoken = token
-							last_idx_start = idx_start
-							last_idx_end = idx_end
-							
-							if token.string in self.keywords:
-							
-								if token.string == 'self':
-									self.contents.tag_add('selfs', idx_start, idx_end)
-								
-								elif token.string in self.bools:
-									self.contents.tag_add('bools', idx_start, idx_end)
-									
-##								elif token.string in self.tests:
-##									self.contents.tag_add('tests', idx_start, idx_end)
-								
-								elif token.string in self.breaks:
-									self.contents.tag_add('breaks', idx_start, idx_end)
-								
-								else:
-									self.contents.tag_add('keywords', idx_start, idx_end)
-								
-						
-						# calls
-						elif token.exact_type == tokenize.LPAR:
-							# Need to know if last char before ( was not empty.
-							# Previously used test was:
-							#if self.contents.get( '%s - 1c' % idx_start, idx_start ).strip():
-							
-							# token.line contains line as string which contains token.
-							prev_char_idx = token.start[1]-1
-							if prev_char_idx > -1 and token.line[prev_char_idx].isalnum():
-								self.contents.tag_add('calls', last_idx_start, last_idx_end)
-								
-						elif token.type == tokenize.STRING:
-							self.contents.tag_add('strings', idx_start, idx_end)
-							
-						elif token.type == tokenize.COMMENT:
-							self.contents.tag_add('comments', idx_start, idx_end)
-						
-						# token.type == tokenize.NUMBER
-						else:
-							self.contents.tag_add('numbers', idx_start, idx_end)
-					
-		
-		except IndentationError as e:
-##			for attr in ['args', 'filename', 'lineno', 'msg', 'offset', 'text']:
-##				item = getattr( e, attr)
-##				print( attr,': ', item )
-
-			# This Error needs info about whole block, one line is not enough, so quite rare.
-			#print( e.args[0], '\nIndentation errline: ', self.contents.index(tkinter.INSERT) )
-			flag_err = True
-			self.token_err = True
-
-		
-		except tokenize.TokenError as ee:
-			
-			if 'EOF in multi-line statement' in ee.args[0]:
-				self.check_pars = idx_start
-				
-			elif 'multi-line string' in ee.args[0]:
-				flag_err = True
-				self.token_err = True
-			
-			
-		# from backspace_override:
-		if self.check_pars:
-			startl = self.check_pars
-			par_err = self.checkpars(startl)
-			
-		elif self.par_err:
-			startl = False
-			par_err = self.checkpars(startl)
-
-		self.check_pars = False
-		self.par_err = par_err
-
-		if not par_err:
-			# not always checking whole file for par mismatches, so clear
-			self.contents.tag_remove('mismatch', '1.0', tkinter.END)
-			
-
-
-		if not flag_err and ( start_idx == '1.0' and end_idx == tkinter.END ):
-			#print('ok')
-			self.token_err = False
-			
-			
-	def checkpars(self, idx_start):
-		# possible par mismatch may be caused from another line,
-		# so find current block: find first empty line before and after curline
-		# then count pars in it.
-		
-		if not idx_start:
-			# line had nothing but brace in it and it were deleted
-			idx_start = self.contents.index(tkinter.INSERT)
-			
-		curline = int( idx_start.split('.')[0] )
-		startline, endline, lines = self.find_empty_lines(curline)
-		err_indexes = self.count_pars(startline, lines)
-		
-		err = False
-		
-		if err_indexes:
-			err = True
-			err_line = startline + err_indexes[0]
-			err_col = err_indexes[1]
-			err_idx = '%i.%i' % (err_line, err_col)
-			
-			self.contents.tag_remove('mismatch', '1.0', tkinter.END)
-			self.contents.tag_add('mismatch', err_idx, '%s +1c' % err_idx)
-		
-		#print(err)
-		return err
-	
-	
-	def count_pars(self, startline, lines):
-		
-		pars = list()
-		bras = list()
-		curls = list()
-		
-		opening  = [ '(', '[', '{' ]
-		closing  = [ ')', ']', '}' ]
-		
-		tags = None
-		
-		# populate lists and return at first extra closer:
-		for i in range(len(lines)):
-			
-			for j in range(len(lines[i])):
-				c = lines[i][j]
-				patt = '%i.%i' % (startline+i, j)
-				tags = self.contents.tag_names(patt)
-
-				# skip if string or comment:
-				if tags:
-					if 'strings' in tags or 'comments' in tags:
-						tags = None
-						continue
-				
-				if c in closing:
-					if c == ')':
-						if len(pars) > 0:
-							pars.pop(-1)
-						else:
-							return (i,j)
-					
-					elif c == ']':
-						if len(bras) > 0:
-							bras.pop(-1)
-						else:
-							return (i,j)
-					
-					# c == '}'
-					else:
-						if len(curls) > 0:
-							curls.pop(-1)
-						else:
-							return (i,j)
-						
-							
-				elif c in opening:
-					if c == '(':
-						pars.append((i,j))
-						
-					elif c == '[':
-						bras.append((i,j))
-					
-					# c == '{':
-					else:
-						curls.append((i,j))
-				
-		
-		# no extra closer in block.
-		# Return last extra opener:
-		idxlist = list()
-		
-		for item in [ pars, bras, curls ]:
-			if len(item) > 0:
-				idx =  item.pop(-1)
-				idxlist.append(idx)
-	
-	
-		if len(idxlist) > 0:
-			if len(idxlist) > 1:
-			
-				maxidx = max(idxlist)
-				
-				return idxlist[idxlist.index(maxidx)]
-					
-			else:
-				return idxlist[0]
-			
-		else:
-			return False
-
-		
-	def find_empty_lines(self, lnstart):
-		'''	Finds first empty lines before and after current line
-			
-			returns
-				linenumber of start and end of the block
-				and list of lines.
-
-			called from update_tokens
-		'''
-
-		lines = list()
-
-		# first empty line before curline:
-		endln = 1
-		ln = lnstart
-
-		if ln > endln:
-			ln -= 1
-			t = self.contents.get('%i.0' % ln, '%i.end' % ln)
-			
-			while t != '' and not t.isspace():
-				lines.append(t)
-				ln -= 1
-				
-				if ln < endln:
-					break
-				
-				t = self.contents.get('%i.0' % ln, '%i.end' % ln)
-			
-			ln += 1
-
-		else:
-			pass
-			# curline is firstline
-
-
-		# ln is now first empty linenum above curline or firstline
-		startline = ln
-
-
-		# add curline to list
-		ln = lnstart
-		lines.reverse()
-		t = self.contents.get('%i.0' % ln, '%i.end' % ln)
-		lines.append(t)
-
-
-		# first empty line after curline:
-		endln = int( self.contents.index(tkinter.END).split('.')[0] )
-		ln += 1
-		
-		if ln < endln:
-			
-			t = self.contents.get('%i.0' % ln, '%i.end' % ln)
-
-			while  t != '' and not t.isspace():
-				lines.append(t)
-				ln += 1
-
-				if ln > endln:
-					break
-
-				t = self.contents.get('%i.0' % ln, '%i.end' % ln)
-				
-			ln -= 1
-			
-		else:
-			# curline is lastline
-			pass
-
-		# ln is now first empty linenum after curline or lastline
-		endline = ln
-
-		return startline, endline, lines
-							
-
-########## Syntax highlight End
-########## Theme Related Begin
-
-	def change_indentation_width(self, width):
-		''' width is integer between 1-8
-		'''
-		
-		if type(width) != int: return
-		elif width == self.ind_depth: return
-		elif not 0 < width <= 8: return
-		
-		
-		self.ind_depth = width
-		self.tab_width = self.font.measure(self.ind_depth * self.tab_char)
-		self.contents.config(tabs=(self.tab_width, ))
-
-
-	def increase_scrollbar_width(self, event=None):
-		'''	Change width of scrollbar and self.contents
-			Shortcut: Ctrl-plus
-		'''
-		if self.scrollbar_width >= 100:
-			self.bell()
-			return 'break'
-			
-		self.scrollbar_width += 7
-		self.elementborderwidth += 1
-		self.scrollbar.config(width=self.scrollbar_width)
-		self.scrollbar.config(elementborderwidth=self.elementborderwidth)
-			
-		return 'break'
-		
-		
-	def decrease_scrollbar_width(self, event=None):
-		'''	Change width of scrollbar and self.contents
-			Shortcut: Ctrl-minus
-		'''
-		if self.scrollbar_width <= 0:
-			self.bell()
-			return 'break'
-			
-		self.scrollbar_width -= 7
-		self.elementborderwidth -= 1
-		self.scrollbar.config(width=self.scrollbar_width)
-		self.scrollbar.config(elementborderwidth=self.elementborderwidth)
-			
-		return 'break'
-		
-
-	def toggle_color(self, event=None):
-		
-		if self.curtheme == 'day':
-			self.curtheme = 'night'
-		else:
-			self.curtheme = 'day'
-		
-		self.update_normal_text()
-		
-		return 'break'
-
-
-	def update_normal_text(self):
-	
-		self.bgcolor, self.fgcolor = self.themes[self.curtheme]['normal_text'][:]
-			
-	
-		for tagname in self.themes[self.curtheme]:
-			bg, fg = self.themes[self.curtheme][tagname][:]
-			self.contents.tag_config(tagname, background=bg, foreground=fg)
-	
-		
-		self.contents.config(foreground=self.fgcolor, background=self.bgcolor,
-			insertbackground=self.fgcolor)
-			
-		self.ln_widget.config(foreground=self.fgcolor, background=self.bgcolor, selectbackground=self.bgcolor, selectforeground=self.fgcolor, inactiveselectbackground=self.bgcolor )
-	
-	
-	def update_fonts(self):
-		self.boldfont = self.font.copy()
-		self.boldfont.config(weight='bold')
-		
-		self.contents.tag_config('keywords', font=self.boldfont)
-		self.contents.tag_config('numbers', font=self.boldfont)
-		self.contents.tag_config('comments', font=self.boldfont)
-		self.contents.tag_config('breaks', font=self.boldfont)
-		self.contents.tag_config('calls', font=self.boldfont)
-		
-		
-		self.tab_width = self.font.measure(self.ind_depth * self.tab_char)
-		pad_x =  self.tab_width // self.ind_depth // 3
-		pad_y = pad_x
-		
-		self.contents.config(tabs=(self.tab_width, ), padx=pad_x, pady=pad_y)
-		self.ln_widget.config(padx=pad_x, pady=pad_y)
-		self.y_extra_offset = self.contents['highlightthickness'] + self.contents['bd'] + self.contents['pady']
-		#self.bbox_height = self.contents.bbox('@0,0')[3]
-		
-
-					
-	def font_choose(self, event=None):
-		if self.state != 'normal':
-			self.bell()
-			return "break"
-		
-		fonttop = tkinter.Toplevel()
-		fonttop.title('Choose Font')
-		
-		big = False
-		shortcut = "<Alt-f>"
-		
-		if self.os_type == 'mac_os':
-			big = True
-			shortcut = "<function>"
-		
-		
-		fonttop.protocol("WM_DELETE_WINDOW", lambda: ( fonttop.destroy(),
-				self.contents.bind( shortcut, self.font_choose)) )
-		
-		changefont.FontChooser( fonttop, [self.font, self.menufont], big, tracefunc=self.update_fonts, os_type=self.os_type )
-		self.contents.bind( shortcut, self.do_nothing)
-		self.to_be_closed.append(fonttop)
-	
-		return 'break'
-		
-		
-	def enter2(self, args, event=None):
-		''' When mousecursor enters hyperlink tagname in colorchooser.
-		'''
-		wid = args[0]
-		tagname = args[1]
-		
-		t = wid.textwid
-		
-##		wid.after(200, lambda kwargs={'cursor':'hand2'}: t.config(**kwargs) )
-##
-		
-		
-		t.config(cursor="hand2")
-		wid.after(50, lambda args=[tagname],
-				kwargs={'underline':1, 'font':self.boldfont}: t.tag_config(*args, **kwargs) )
-		
-		#t.tag_config(tagname, underline=1, font=self.boldfont)
-		
-		
-	def leave2(self, args, event=None):
-		''' When mousecursor leaves hyperlink tagname in colorchooser.
-		'''
-		wid = args[0]
-		tagname = args[1]
-		
-		t = wid.textwid
-		
-		t.config(cursor=self.name_of_cursor_in_text_widget)
-		wid.after(50, lambda args=[tagname],
-				kwargs={'underline':0, 'font':self.menufont}: t.tag_config(*args, **kwargs) )
-		
-		#t.tag_config(tagname, underline=0, font=self.menufont)
-		
-		
-	def lclick2(self, args, event=None):
-		'''	When clicked hyperlink in colorchooser.
-		'''
-		wid = args[0]
-		tagname = args[1]
-		
-		syntags = [
-		'normal_text',
-		'keywords',
-		'numbers',
-		'bools',
-		'strings',
-		'comments',
-		'breaks',
-		'calls',
-		'selfs',
-		'match',
-		'focus',
-		'replaced',
-		'mismatch',
-		'selected'
-		]
-		
-		modetags = [
-		'Day',
-		'Night',
-		'Text',
-		'Background'
-		]
-		
-		savetags = [
-		'Save_TMP',
-		'TMP',
-		'Start',
-		'Defaults'
-		]
-		
-		onlyfore = [
-		'keywords',
-		'numbers',
-		'bools',
-		'strings',
-		'comments',
-		'breaks',
-		'calls',
-		'selfs'
-		]
-
-		
-		if tagname in syntags:
-			
-			if tagname == 'selected':
-				tagname = 'sel'
-			
-			if wid.frontback_mode == 'foreground':
-				initcolor = self.contents.tag_cget(tagname, 'foreground')
-				patt = 'Choose fgcolor for: %s' % tagname
-				
-			else:
-				initcolor = self.contents.tag_cget(tagname, 'background')
-				patt = 'Choose bgcolor for: %s' % tagname
-			
-			res = self.tk.call('tk_chooseColor', '-initialcolor', initcolor, '-title', patt)
-				
-			tmpcolor = str(res)
-			
-			if tmpcolor in [None, '']:
-				wid.focus_set()
-				return 'break'
-			
-			
-			try:
-				if wid.frontback_mode == 'foreground':
-					self.themes[self.curtheme][tagname][1] = tmpcolor
-					self.contents.tag_config(tagname, foreground=tmpcolor)
-				else:
-					self.themes[self.curtheme][tagname][0] = tmpcolor
-					self.contents.tag_config(tagname, background=tmpcolor)
-			
-			
-				if tagname == 'normal_text':
-					self.update_normal_text()
-				
-			# if closed editor and still pressing ok in colorchooser:
-			except (tkinter.TclError, AttributeError) as e:
-				# because if closed editor, this survives
-				pass
-			
-			
-		elif tagname in modetags:
-		
-			t = wid.textwid
-		
-			if tagname == 'Day' and self.curtheme != 'day':
-				r1 = t.tag_nextrange('Day', 1.0)
-				r2 = t.tag_nextrange('Night', 1.0)
-				
-				t.delete(r1[0], r1[1])
-				t.insert(r1[0], '[X] Day-mode	', 'Day')
-				t.delete(r2[0], r2[1])
-				t.insert(r2[0], '[ ] Night-mode	', 'Night')
-				
-				self.toggle_color()
-				
-				
-			elif tagname == 'Night' and self.curtheme != 'night':
-				r1 = t.tag_nextrange('Day', 1.0)
-				r2 = t.tag_nextrange('Night', 1.0)
-				
-				t.delete(r1[0], r1[1])
-				t.insert(r1[0], '[ ] Day-mode	', 'Day')
-				t.delete(r2[0], r2[1])
-				t.insert(r2[0], '[X] Night-mode	', 'Night')
-				
-				self.toggle_color()
-				
-				
-			elif tagname == 'Text':
-				if wid.frontback_mode != 'foreground':
-					r1 = t.tag_nextrange('Text', 1.0)
-					r2 = t.tag_nextrange('Background', 1.0)
-					
-					t.delete(r1[0], r1[1])
-					t.insert(r1[0], '[X] Text color\n', 'Text')
-					
-					t.delete(r2[0], r2[1])
-					t.insert(r2[0], '[ ] Background color\n', 'Background')
-					wid.frontback_mode = 'foreground'
-					
-					t.tag_remove('disabled', 1.0, tkinter.END)
-					
-					for tag in onlyfore:
-						r3 = wid.tag_idx.get(tag)
-						t.tag_add(tag, r3[0], r3[1])
-					
-								
-			elif tagname == 'Background':
-				if wid.frontback_mode != 'background':
-					r1 = t.tag_nextrange('Text', 1.0)
-					r2 = t.tag_nextrange('Background', 1.0)
-					
-					t.delete(r1[0], r1[1])
-					t.insert(r1[0], '[ ] Text color\n', 'Text')
-					
-					t.delete(r2[0], r2[1])
-					t.insert(r2[0], '[X] Background color\n', 'Background')
-					wid.frontback_mode = 'background'
-					
-					for tag in onlyfore:
-						r3 = t.tag_nextrange(tag, 1.0)
-						wid.tag_idx.setdefault(tag, r3)
-						t.tag_remove(tag, 1.0, tkinter.END)
-						t.tag_add('disabled', r3[0], r3[1])
-						
-				
-		elif tagname in savetags:
-			
-			if tagname == 'Save_TMP':
-				wid.tmp_theme = copy.deepcopy(self.themes)
-				wid.flag_tmp = True
-				self.flash_tag(wid, tagname)
-				
-			elif tagname == 'TMP' and wid.flag_tmp:
-				self.themes = copy.deepcopy(wid.tmp_theme)
-				self.flash_tag(wid, tagname)
-				
-			elif tagname == 'Start':
-				self.themes = copy.deepcopy(wid.start_theme)
-				self.flash_tag(wid, tagname)
-				
-			elif tagname == 'Defaults':
-				self.themes = copy.deepcopy(self.default_themes)
-				self.flash_tag(wid, tagname)
-				
-				
-			if (tagname in ['Defaults', 'Start']) or (tagname == 'TMP' and wid.flag_tmp):
-			
-				for tag in self.themes[self.curtheme]:
-					bg, fg = self.themes[self.curtheme][tag][:]
-					self.contents.tag_config(tag, background=bg, foreground=fg)
-	
-				self.update_normal_text()
-				
-		
-		wid.focus_set()
-				
-				
-	def flash_tag(self, wid, tagname):
-		''' Flash save_tag when clicked in colorchooser.
-		'''
-		t = wid.textwid
-		
-		wid.after(50, lambda args=[tagname],
-				kwargs={'background':'green'}: t.tag_config(*args, **kwargs) )
-					
-		wid.after(600, lambda args=[tagname],
-				kwargs={'background':t.cget('background')}: t.tag_config(*args, **kwargs) )
-					
-	
-	def color_choose(self, event=None):
-		if self.state != 'normal':
-			self.bell()
-			return "break"
-			
-		colortop = tkinter.Toplevel()
-		c = colortop
-		c.title('Choose Color')
-		c.start_theme = copy.deepcopy(self.themes)
-		c.tmp_theme = copy.deepcopy(self.themes)
-		c.flag_tmp = False
-		
-		shortcut_color = "<Alt-s>"
-		shortcut_toggl = "<Alt-t>"
-
-		if self.os_type == 'mac_os':
-			shortcut_color = "<ssharp>"
-			shortcut_toggl = "<dagger>"
-		
-		
-		c.protocol("WM_DELETE_WINDOW", lambda: ( c.destroy(),
-				self.contents.bind( shortcut_color, self.color_choose),
-				self.contents.bind( shortcut_toggl, self.toggle_color)) )
-				
-		self.contents.bind( shortcut_color, self.do_nothing)
-		self.contents.bind( shortcut_toggl, self.do_nothing)
-		
-		#c.textfont = tkinter.font.Font(family='TkDefaulFont', size=10)
-		
-		size_title = 12
-		if self.os_type == 'mac_os': size_title = 16
-		c.titlefont = tkinter.font.Font(family='TkDefaulFont', size=size_title)
-		
-		c.textwid = tkinter.Text(c, blockcursor=True, highlightthickness=0,
-							bd=4, pady=4, padx=10, tabstyle='wordprocessor', font=self.menufont)
-		
-		c.scrollbar = tkinter.Scrollbar(c, orient=tkinter.VERTICAL, highlightthickness=0,
-							bd=0, command = c.textwid.yview)
-
-		
-		c.textwid['yscrollcommand'] = c.scrollbar.set
-		c.scrollbar.config(width=self.scrollbar_width)
-		c.scrollbar.config(elementborderwidth=self.elementborderwidth)
-
-		t = c.textwid
-		
-		t.tag_config('title', font=c.titlefont)
-		t.tag_config('disabled', foreground='#a6a6a6')
-		
-		tags = [
-		'Day',
-		'Night',
-		'Text',
-		'Background',
-		'normal_text',
-		'keywords',
-		'numbers',
-		'bools',
-		'strings',
-		'comments',
-		'breaks',
-		'calls',
-		'selfs',
-		'match',
-		'focus',
-		'replaced',
-		'mismatch',
-		'selected',
-		'Save_TMP',
-		'TMP',
-		'Start',
-		'Defaults'
-		]
-		
-		
-		
-				
-		
-		
-		for tag in tags:
-			t.tag_config(tag, font=self.menufont)
-			t.tag_bind(tag, "<Enter>",
-				lambda event, arg=[c, tag]: self.enter2(arg, event))
-			t.tag_bind(tag, "<Leave>",
-				lambda event, arg=[c, tag]: self.leave2(arg, event))
-			t.tag_bind(tag, "<ButtonRelease-1>",
-					lambda event, arg=[c, tag]: self.lclick2(arg, event))
-						
-		
-				
-		c.rowconfigure(1, weight=1)
-		c.columnconfigure(1, weight=1)
-		
-		t.grid_configure(row=0, column = 0)
-		c.scrollbar.grid_configure(row=0, column = 1, sticky='ns')
-		
-		
-		i = tkinter.INSERT
-		
-		t.insert(i, 'Before closing, load setting from: Start\n', 'title')
-		t.insert(i, 'if there were made unwanted changes.\n', 'title')
-		t.insert(i, '\nChanging color for:\n', 'title')
-		
-		
-		c.frontback_mode = None
-		c.tag_idx = dict()
-		
-		if self.curtheme == 'day':
-		
-			t.insert(i, '[X] Day-mode	', 'Day')
-			t.insert(i, '[X] Text color\n', 'Text')
-		
-			t.insert(i, '[ ] Night-mode	', 'Night')
-			t.insert(i, '[ ] Background color\n', 'Background')
-			
-			c.frontback_mode = 'foreground'
-			
-			
-		else:
-			t.insert(i, '[ ] Day-mode	', 'Day')
-			t.insert(i, '[X] Text color\n', 'Text')
-		
-			t.insert(i, '[X] Night-mode	', 'Night')
-			t.insert(i, '[ ] Background color\n', 'Background')
-			
-			c.frontback_mode = 'foreground'
-			
-		
-		
-		t.insert(i, '\nSelect tag you want to modify\n', 'title')
-		t.insert(i, 'normal text\n', 'normal_text')
-		
-		
-		t.insert(i, '\nSyntax highlight tags\n', 'title')
-		t.insert(i, 'keywords\n', 'keywords')
-		t.insert(i, 'numbers\n', 'numbers')
-		t.insert(i, 'bools\n', 'bools')
-		t.insert(i, 'strings\n', 'strings')
-		t.insert(i, 'comments\n', 'comments')
-		t.insert(i, 'breaks\n', 'breaks')
-		t.insert(i, 'calls\n', 'calls')
-		t.insert(i, 'selfs\n', 'selfs')
-	
-
-		t.insert(i, '\nSearch tags\n', 'title')
-		t.insert(i, 'match\n', 'match')
-		t.insert(i, 'focus\n', 'focus')
-		t.insert(i, 'replaced\n', 'replaced')
-	
-
-		t.insert(i, '\nParentheses\n', 'title')
-		t.insert(i, 'mismatch\n', 'mismatch')
-		
-		t.insert(i, '\nSelection\n', 'title')
-		t.insert(i, 'selected\n', 'selected')
-	
-
-		t.insert(i, '\nSave current setting to template,\n', 'title')
-		t.insert(i, 'to which you can revert later:\n', 'title')
-		t.insert(i, 'Save TMP\n', 'Save_TMP')
-		
-		t.insert(i, '\nLoad setting from:\n', 'title')
-		t.insert(i, 'TMP\n', 'TMP')
-		t.insert(i, 'Start\n', 'Start')
-		t.insert(i, 'Defaults\n', 'Defaults')
-
-
-		t.state = 'disabled'
-		t.config(insertontime=0)
-
-
-		self.to_be_closed.append(c)
-
-		return 'break'
-
-		
-########## Theme Related End
-########## Run file Related Begin
-
-	def enter(self, tagname, event=None):
-		''' Used in error-page, when mousecursor enters hyperlink tagname.
-		'''
-		self.contents.config(cursor="hand2")
-		self.contents.tag_config(tagname, underline=1)
-
-
-	def leave(self, tagname, event=None):
-		''' Used in error-page, when mousecursor leaves hyperlink tagname.
-		'''
-		self.contents.config(cursor=self.name_of_cursor_in_text_widget)
-		self.contents.tag_config(tagname, underline=0)
-
-
-	def lclick(self, tagname, event=None):
-		'''	Used in error-page, when hyperlink tagname is clicked.
-		
-			self.taglinks is dict with tagname as key
-			and function (self.taglink) as value.
-		'''
-		
-		# passing tagname-string as argument to function self.taglink()
-		# which in turn is a value of tagname-key in dictionary taglinks:
-		self.taglinks[tagname](tagname)
-		
-
-	def tag_link(self, tagname, event=None):
-		''' Used in error-page, executed when hyperlink tagname is clicked.
-		'''
-		
-		i = int(tagname.split("-")[1])
-		filepath, errline = self.errlines[i]
-		
-		filepath = pathlib.Path(filepath)
-		openfiles = [tab.filepath for tab in self.tabs]
-		
-		# clicked activetab, do nothing
-		if filepath == self.tabs[self.tabindex].filepath:
-			pass
-			
-		# clicked file that is open, switch activetab
-		elif filepath in openfiles:
-			for i,tab in enumerate(self.tabs):
-				if tab.filepath == filepath:
-					self.tabs[self.tabindex].active = False
-					self.tabindex = i
-					self.tabs[self.tabindex].active = True
-					break
-					
-		# else: open file in newtab
-		else:
-			try:
-				with open(filepath, 'r', encoding='utf-8') as f:
-					self.new_tab(error=True)
-					tmp = f.read()
-					self.tabs[self.tabindex].oldcontents = tmp
-					
-					if '.py' in filepath.suffix:
-						indentation_is_alien, indent_depth = self.check_indent_depth(tmp)
-						
-						if indentation_is_alien:
-							# Assuming user wants self.ind_depth, change it without notice:
-							tmp = self.tabs[self.tabindex].oldcontents.splitlines(True)
-							tmp[:] = [self.tabify(line, width=indent_depth) for line in tmp]
-							tmp = ''.join(tmp)
-							self.tabs[self.tabindex].contents = tmp
-							
-						else:
-							self.tabs[self.tabindex].contents = self.tabs[self.tabindex].oldcontents
-					else:
-						self.tabs[self.tabindex].contents = self.tabs[self.tabindex].oldcontents
-				
-					
-					self.tabs[self.tabindex].filepath = filepath
-					self.tabs[self.tabindex].type = 'normal'
-			except (EnvironmentError, UnicodeDecodeError) as e:
-				print(e.__str__())
-				print(f'\n Could not open file: {filepath}')
-				self.bell()
-				return
-
-		
-		self.entry.delete(0, tkinter.END)
-		self.entry.insert(0, self.tabs[self.tabindex].filepath)
-		
-		
-		self.contents.delete('1.0', tkinter.END)
-		self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
-		
-		
-		if self.syntax:
-		
-			lineend = '%s lineend' % tkinter.INSERT
-			linestart = '%s linestart' % tkinter.INSERT
-			
-			tmp = self.contents.get( linestart, lineend )
-			self.oldline = tmp
-			
-			self.token_err = True
-			self.update_tokens(start='1.0', end=tkinter.END)
-			self.token_can_update = True
-		
-		
-		# set cursor pos
-		line = errline + '.0'
-		self.contents.focus_set()
-		self.contents.mark_set('insert', line)
-		self.ensure_idx_visibility(line)
-					
-		
-		self.contents.edit_reset()
-		self.contents.edit_modified(0)
-		
-		self.contents.bind("<Button-%i>" % self.right_mousebutton_num, lambda event: self.raise_popup(event))
-		self.state = 'normal'
-		self.update_title()
-		
-
-	def run(self):
-		'''	Run file currently being edited. This can not catch errlines of
-			those exceptions that are catched. Like:
-			
-			try:
-				code we know sometimes failing with SomeError
-				(but might also fail with other error-type)
-			except SomeError:
-				some other code but no raising error
-				
-			Note: 	Above code will raise an error in case
-			 		code in try-block raises some other error than SomeError.
-					In that case those errlines will be of course catched.
-			
-			What this means: If you self.run() with intention to spot possible
-			errors in your program, you should use logging (in except-block)
-			if you are not 100% sure about your code in except-block.
-		'''
-		if (self.state != 'normal') or (self.tabs[self.tabindex].type == 'newtab'):
-			self.bell()
-			return 'break'
-			
-		self.save(forced=True)
-		
-		# https://docs.python.org/3/library/subprocess.html
-
-		res = subprocess.run(['python', self.tabs[self.tabindex].filepath], stderr=subprocess.PIPE).stderr
-		
-		err = res.decode()
-		
-		if len(err) != 0:
-			self.bind("<Escape>", self.stop_show_errors)
-			self.contents.bind("<Button-%i>" % self.right_mousebutton_num, self.do_nothing)
-			self.state = 'error'
-			
-			self.taglinks = dict()
-			self.errlines = list()
-			openfiles = [tab.filepath for tab in self.tabs]
-			
-			self.contents.delete('1.0', tkinter.END)
-			
-			for tag in self.contents.tag_names():
-				if 'hyper' in tag:
-					self.contents.tag_delete(tag)
-				
-			self.err = err.splitlines()
-			
-			for line in self.err:
-				tmp = line
-
-				tagname = "hyper-%s" % len(self.errlines)
-				self.contents.tag_config(tagname)
-				
-				# Why ButtonRelease instead of just Button-1:
-				# https://stackoverflow.com/questions/24113946/unable-to-move-text-insert-index-with-mark-set-widget-function-python-tkint
-				
-				self.contents.tag_bind(tagname, "<ButtonRelease-1>",
-					lambda event, arg=tagname: self.lclick(arg, event))
-				
-				self.contents.tag_bind(tagname, "<Enter>",
-					lambda event, arg=tagname: self.enter(arg, event))
-				
-				self.contents.tag_bind(tagname, "<Leave>",
-					lambda event, arg=tagname: self.leave(arg, event))
-				
-				self.taglinks[tagname] = self.tag_link
-				
-				# Parse filepath and linenums from errors
-				if 'File ' in line and 'line ' in line:
-					self.contents.insert(tkinter.INSERT, '\n')
-					 
-					data = line.split(',')[:2]
-					linenum = data[1][6:]
-					path = data[0][8:-1]
-					pathlen = len(path) + 2
-					filepath = pathlib.Path(path)
-					
-					self.errlines.append((filepath, linenum))
-					
-					self.contents.insert(tkinter.INSERT, tmp)
-					s0 = tmp.index(path) - 1
-					s = self.contents.index('insert linestart +%sc' % s0 )
-					e = self.contents.index('%s +%sc' % (s, pathlen) )
-					
-					self.contents.tag_add(tagname, s, e)
-						
-					if filepath in openfiles:
-						self.contents.tag_config(tagname, foreground='brown1')
-						self.contents.tag_raise(tagname)
-							
-						
-					self.contents.insert(tkinter.INSERT, '\n')
-					
-					
-				else:
-					self.contents.insert(tkinter.INSERT, tmp +"\n")
-					
-					# Make look bit nicer:
-					if self.syntax:
-						# -1 lines because we have added linebreak already.
-						start = self.contents.index('insert -1 lines linestart')
-						end = self.contents.index('insert -1 lines lineend')
-						
-						self.update_tokens(start=start, end=end, line=line)
-			
-					
-		return 'break'
-				
-
-	def show_errors(self):
-		''' Show traceback from last run with added hyperlinks.
-		'''
-		
-		if len(self.errlines) != 0:
-			self.bind("<Escape>", self.stop_show_errors)
-			self.contents.bind("<Button-%i>" % self.right_mousebutton_num, self.do_nothing)
-			self.state = 'error'
-			
-			tmp = self.contents.get('1.0', tkinter.END)
-			# [:-1]: remove unwanted extra newline
-			self.tabs[self.tabindex].contents = tmp[:-1]
-			
-			try:
-				pos = self.contents.index(tkinter.INSERT)
-			except tkinter.TclError:
-				pos = '1.0'
-				
-			self.tabs[self.tabindex].position = pos
-			self.contents.delete('1.0', tkinter.END)
-			openfiles = [tab.filepath for tab in self.tabs]
-			
-			for tag in self.contents.tag_names():
-				if 'hyper' in tag:
-					self.contents.tag_config(tag, foreground=self.fgcolor)
-			
-			i = 0
-			for line in self.err:
-				tmp = line
-				tagname = 'hyper-%d' % i
-				
-				# Parse filepath and linenums from errors
-				if 'File ' in line and 'line ' in line:
-					self.contents.insert(tkinter.INSERT, '\n')
-					data = line.split(',')[:2]
-					linenum = data[1][6:]
-					path = data[0][8:-1]
-					pathlen = len(path) + 2
-					filepath = pathlib.Path(path)
-					
-					self.contents.insert(tkinter.INSERT, tmp)
-					s0 = tmp.index(path) - 1
-					s = self.contents.index('insert linestart +%sc' % s0 )
-					e = self.contents.index('%s +%sc' % (s, pathlen) )
-					
-					self.contents.tag_add(tagname, s, e)
-					
-					if filepath in openfiles:
-						self.contents.tag_config(tagname, foreground='brown1')
-						self.contents.tag_raise(tagname)
-						
-						
-					self.contents.insert(tkinter.INSERT, '\n')
-					
-					i += 1
-					
-				else:
-					self.contents.insert(tkinter.INSERT, tmp +"\n")
-					
-					# Make look bit nicer:
-					if self.syntax:
-						# -1 lines because we have added linebreak already.
-						start = self.contents.index('insert -1 lines linestart')
-						end = self.contents.index('insert -1 lines lineend')
-						
-						self.update_tokens(start=start, end=end, line=line)
-			
-					
-									
-	def stop_show_errors(self, event=None):
-		self.state = 'normal'
-		self.bind("<Escape>", self.do_nothing)
-		self.contents.bind("<Button-%i>" % self.right_mousebutton_num, lambda event: self.raise_popup(event))
-		
-		self.entry.delete(0, tkinter.END)
-		
-		if self.tabs[self.tabindex].type == 'normal':
-			self.entry.insert(0, self.tabs[self.tabindex].filepath)
-			
-		
-		self.contents.delete('1.0', tkinter.END)
-		self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
-		
-		
-		self.do_syntax(everything=True)
-		
-		
-		# set cursor pos
-		line = self.tabs[self.tabindex].position
-		self.contents.focus_set()
-		self.contents.mark_set('insert', line)
-		self.ensure_idx_visibility(line)
-			
-			
-		self.contents.edit_reset()
-		self.contents.edit_modified(0)
-		
-		
-########## Run file Related End
-########## Overrides Begin
-
-	def move_right(self, event=None):
-		''' move cursor right with
-			ctrl-i
-		'''
-		
-		if self.state not in  [ 'normal', 'error' ]:
-			self.bell()
-			return "break"
-			
-		self.contents.event_generate('<<NextChar>>')
-		
-		return "break"
-		
-		
-	def move_left(self, event=None):
-		''' move cursor left with
-			ctrl-b
-		'''
-		
-		if self.state not in  [ 'normal', 'error' ]:
-			self.bell()
-			return "break"
-			
-		self.contents.event_generate('<<PrevChar>>')
-		
-		return "break"
-		
-		
-	def move_up(self, event=None):
-		''' move cursor up with
-			ctrl-p
-		'''
-		
-		if self.state not in  [ 'normal', 'error' ]:
-			self.bell()
-			return "break"
-			
-		self.contents.event_generate('<<PrevLine>>')
-		
-		return "break"
-		
-		
-	def move_down(self, event=None):
-		''' move cursor down with
-			ctrl-n
-		'''
-		
-		if self.state not in  [ 'normal', 'error' ]:
-			self.bell()
-			return "break"
-	
-		self.contents.event_generate('<<NextLine>>')
-		
-		return "break"
-	
-	
-##	def updown_override(self, event=None, direction=None):
-##		''' up-down override, to expand possibly incorrect indentation
-##		'''
-##
-##		if self.state != 'normal':
-##			return "continue"
-##
-##		oldpos = self.contents.index(tkinter.INSERT)
-##
-##
-##		if direction == 'down':
-##			newpos = self.contents.index( '%s + 1lines' % tkinter.INSERT)
-##
-##		# direction == 'up'
-##		else:
-##			newpos = self.contents.index( '%s - 1lines' % tkinter.INSERT)
-##
-##
-##		oldline = self.contents.get( '%s linestart' % oldpos, '%s lineend' % oldpos)
-##		newline = self.contents.get( '%s linestart' % newpos, '%s lineend' % newpos)
-##
-##
-##		if newline.isspace() or newline == '':
-##
-##			if oldline == '':
-##				return 'continue'
-##
-##			if not oldline.isspace():
-##
-##				tmp = oldline.lstrip()
-##				oldindent = oldline.index(tmp)
-##
-##				if oldindent == 0:
-##					return 'continue'
-##
-##				self.contents.delete('%s linestart' % newpos,'%s lineend' % newpos)
-##				self.contents.insert('%s linestart' % newpos, oldindent * '\t')
-##				return 'continue'
-##
-##			# coming from empty line:
-##			else:
-##				self.contents.delete('%s linestart' % newpos,'%s lineend' % newpos)
-##				self.contents.insert('%s linestart' % newpos, len(oldline) * '\t')
-##				return 'continue'
-##
-##		else:
-##			return 'continue'
-	
-	
-	def center_view(self, event=None, up=False):
-		''' Raise insertion-line
-		'''
-		if self.state != 'normal':
-			self.bell()
-			return "break"
-			
-		
-		num_lines = self.text_widget_height // self.bbox_height
-		num_scroll = num_lines // 3
-		pos = self.contents.index('insert')
-		#posint = int(float(self.contents.index('insert')))
-		# lastline of visible window
-		lastline_screen = int(float(self.contents.index("@0,65535")))
-		
-		# lastline
-		last = int(float(self.contents.index('end'))) - 1
-		curline = int(float(self.contents.index('insert'))) - 1
-		
-		
-		if up: num_scroll *= -1
-			
-		# if near fileend
-		elif curline + 2*num_scroll + 2 > last:
-			self.contents.insert(tkinter.END, num_scroll*'\n')
-			self.contents.mark_set('insert', pos)
-						
-		
-		# if near screen end
-		#elif curline + 2*num_scroll + 2 > lastline_screen:
-		self.contents.yview_scroll(num_scroll, 'units')
-		
-		
-		# No ensure_view, enable return to cursor by arrow keys
-		return "break"
-	
-	
-	def idx_lineend(self):
-	
-##		?submodifier? linestart
-##		Adjust the index to refer to the first index on the line. If the display submodifier is given, this is the first index on the display line, otherwise on the logical line.
-##
-##		?submodifier? lineend
-##		Adjust the index to refer to the last index on the line (the newline). If the display submodifier is given, this is the last index on the display line, otherwise on the logical line.
-
-		pos = self.contents.index( 'insert display lineend' )
-		return pos
-			
-			
-	def idx_linestart(self):
-		
-		# In case of wrapped lines
-		y_cursor = self.contents.bbox(tkinter.INSERT)[1]
-		p = self.contents.index( '@0,%s' % y_cursor )
-		p2 = self.contents.index( '%s linestart' % p )
-		
-		# is wrapped?
-		c1 = int(p.split('.')[1])
-		l2 = int(p2.split('.')[0])
-		
-		pos = None
-		# yes, put cursor start of line not the whole line:
-		if c1 != 0:
-			pos = p
-			
-		# no, so put cursor after indentation:
-		else:
-			tmp = self.contents.get( '%s linestart' % p2, '%s lineend' % p2 )
-			if len(tmp) > 0:
-				if not tmp.isspace():
-					tmp2 = tmp.lstrip()
-					indent = tmp.index(tmp2)
-					pos = self.contents.index( '%i.%i' % (l2, indent) )
-		
-		return pos
-		
-	
-
-	def select_by_words(self, event=None):
-		'''	Pressed ctrl or Alt + shift and arrow left or right.
-			Make <<SelectNextWord>> and <<SelectPrevWord>> to stop at lineends.
-		'''
-		if self.state not in [ 'normal', 'error' ]:
-			self.bell()
-			return "break"
-		
-		# Check if: ctrl + shift down.
-		# MacOS event is already checked.
-		if self.os_type == 'linux':
-			if event.state != 5: return
-		
-		elif self.os_type == 'windows':
-			if event.state not in [ 262157, 262149 ]: return
-		
-		
-		have_selection = len(self.contents.tag_ranges('sel')) > 0
-		selection_started_from_top = False
-		
-		if event.keysym == 'Right':
-			s = self.contents.index( 'insert')
-			e = self.idx_lineend()
-			idx_linestart = self.idx_linestart()
-			# empty line?
-			if not idx_linestart: return
-			t = self.contents.get(idx_linestart, e).strip()
-
-			
-			# tkinter.SEL_FIRST is always before tkinter.SEL_LAST
-			# no matter if selection started from top or bottom:
-			if have_selection:
-				sel_start = self.contents.index(tkinter.SEL_FIRST)
-				sel_end = self.contents.index(tkinter.SEL_LAST)
-				if s == sel_end:
-					selection_started_from_top = True
-
-				#else: selection_started_from_top = False
-
-			else:
-				selection_started_from_top = True
-				sel_start = s
-
-			
-			
-			##################### Right Real start:
-			
-			
-			self.contents.event_generate('<<NextWord>>')
-			i = self.contents.index( 'insert')
-
-			# Already at lineend, proceed to next line
-			if s == e:
-				if have_selection:
-					self.contents.tag_remove('sel', '1.0', tkinter.END)
-
-					if selection_started_from_top:
-						self.contents.tag_add('sel', sel_start, i)
-					else:
-						self.contents.tag_add('sel', i, sel_end)
-						
-				# No selection,
-				# no need to check direction of selection:
-				else:
-					self.contents.tag_add('sel', s, i)
-					
-				self.contents.mark_set('insert', i)
-
-			
-			# if i is over lineend:
-			# 	stop at lineend == e
-			elif self.contents.compare( e,'<',i ):
-				
-				if have_selection:
-					self.contents.tag_remove('sel', '1.0', tkinter.END)
-
-					if selection_started_from_top:
-						self.contents.tag_add('sel', sel_start, e)
-					else:
-						self.contents.tag_add('sel', e, sel_end)
-						
-				# No selection,
-				# no need to check direction of selection:
-				else:
-					self.contents.tag_add('sel', s, e)
-					
-				self.contents.mark_set('insert', e)
-
-
-			# i is on the current line:
-			# 	stop at i == nextword
-			else:
-				if have_selection:
-					self.contents.tag_remove('sel', '1.0', tkinter.END)
-
-					if selection_started_from_top:
-						self.contents.tag_add('sel', sel_start, i)
-					else:
-						self.contents.tag_add('sel', i, sel_end)
-						
-				# No selection,
-				# no need to check direction of selection:
-				else:
-					self.contents.tag_add('sel', s, i)
-					
-				self.contents.mark_set('insert', i)
-
-
-
-		elif event.keysym == 'Left':
-			s = self.contents.index( 'insert')
-			
-			# tkinter.SEL_FIRST is always before tkinter.SEL_LAST
-			# no matter if selection started from top or bottom:
-			if have_selection:
-				sel_start = self.contents.index(tkinter.SEL_FIRST)
-				sel_end = self.contents.index(tkinter.SEL_LAST)
-				if s != sel_start:
-					selection_started_from_top = True
-
-				#else: selection_started_from_top = False
-
-			else:
-				#selection_started_from_top = False
-				sel_end = s
-
-
-			i_orig = s
-			i_linestart = self.idx_linestart()
-			# empty line?
-			if not i_linestart: return
-			
-			
-			self.contents.event_generate('<<PrevWord>>')
-							
-			i_prevword = self.contents.index( 'insert')
-			
-
-			# Already at linestart, proceed over last word of prev line.
-			if i_orig == i_linestart:
-
-				if have_selection:
-
-					if selection_started_from_top:
-						self.contents.tag_remove('sel', '1.0', tkinter.END)
-						self.contents.tag_add('sel', sel_start, i_prevword)
-						self.contents.mark_set('insert', i_prevword)
-					else:
-						self.contents.tag_remove('sel', '1.0', tkinter.END)
-						self.contents.tag_add('sel', i_prevword, sel_end)
-						self.contents.mark_set('insert', i_prevword)
-				
-				# No selection,
-				# no need to check direction of selection:
-				else:
-					self.contents.tag_add('sel', i_prevword, s)
-					self.contents.mark_set('insert', i_prevword)
-
-				return 'break'
-
-			
-			
-			##################### Left Real start:
-			
-			
-			# if i_prevword is over(before) linestart:
-			# 	stop at linestart == i_linestart
-			if self.contents.compare( i_prevword, '<', i_linestart):
-
-				if have_selection:
-					self.contents.tag_remove('sel', '1.0', tkinter.END)
-
-					if selection_started_from_top:
-						self.contents.tag_add('sel', sel_start, i_linestart)
-					else:
-						self.contents.tag_add('sel', i_linestart, sel_end)
-				
-				
-				# No selection,
-				# no need to check direction of selection:
-				else:
-					self.contents.tag_add('sel', i_linestart, s)
-
-				self.contents.mark_set('insert', i_linestart)
-
-
-			# i_prevword is on the current line:
-			# 	stop at i_prevword
-			else:
-				if have_selection:
-					self.contents.tag_remove('sel', '1.0', tkinter.END)
-
-					if selection_started_from_top:
-						self.contents.tag_add('sel', sel_start, i_prevword)
-					else:
-						self.contents.tag_add('sel', i_prevword, sel_end)
-				
-				
-				# No selection,
-				# no need to check direction of selection:
-				else:
-					self.contents.tag_add('sel', i_prevword, s)
-
-				self.contents.mark_set('insert', i_prevword)
-
-
-		return 'break'
-	
-	
-	def move_by_words(self, event=None):
-		'''	Pressed ctrl or Alt and arrow left or right.
-			Make <<NextWord>> and <<PrevWord>> to stop at lineends.
-		'''
-		if self.state not in [ 'normal', 'error' ]:
-			self.bell()
-			return "break"
-			
-		idx_linestart = self.idx_linestart()
-		# empty line?
-		if not idx_linestart: return
-		
-		
-		# Check if: not only ctrl down, then return
-		# MacOS event is already checked.
-		if self.os_type == 'linux':
-			if event.state != 4: return
-		
-		elif self.os_type == 'windows':
-			if event.state not in [ 262156, 262148 ]: return
-			
-		
-		# Check if near lineend, so stop there
-		if event.keysym == 'Right':
-			i_orig = self.contents.index( 'insert')
-			e = self.idx_lineend()
-			# Already at lineend, proceed over first word of next line
-			if i_orig == e: return
-			
-			self.contents.event_generate('<<NextWord>>')
-			i = self.contents.index( 'insert')
-			if self.contents.compare( e, '<', i ):
-				self.contents.mark_set('insert', e)
-				
-				
-		# Check if near linestart, so stop there
-		elif event.keysym == 'Left':
-			i_orig = self.contents.index( 'insert')
-			self.contents.event_generate('<<PrevWord>>')
-			i_prevword = self.contents.index( 'insert')
-			
-			self.contents.mark_set('insert', i_orig)
-			self.goto_linestart(event=event)
-			i_linestart = self.contents.index( 'insert')
-			
-			# Already at linestart, proceed over last word of prev line
-			if i_orig == i_linestart: return
-			
-			if self.contents.compare( i_prevword, '<', i_linestart ):
-				self.contents.mark_set('insert', i_linestart)
-			else:
-				self.contents.mark_set('insert', i_prevword)
-				
-
-		return 'break'
-	
-		
-	def check_sel(self, event=None):
-		'''	Pressed arrow left or right.
-			If have selection, put cursor on the wanted side of selection.
-		'''
-		
-		if self.state in  [ 'filedialog' ]:
-			self.bell()
-			return "break"
-	
-		
-		# self.contents or self.entry
-		wid = event.widget
-			
-		# Check if have shift etc. pressed. If is, return to default bindings.
-		# macOS event is already handled in mac_cmd_overrides.
-		# macOS event here is only plain arrow left or right and has selection.
-		if self.os_type != 'mac_os':
-			if self.os_type == 'linux' and event.state != 0: return
-			if self.os_type == 'windows' and event.state not in [ 262152, 262144 ]: return
-			
-			have_selection = False
-	
-			if wid == self.entry:
-				have_selection = self.entry.selection_present()
-	
-			elif wid == self.contents:
-				have_selection = len(self.contents.tag_ranges('sel')) > 0
-	
-			else:
-				return
-
-			if not have_selection: return
-			
-		
-		s = wid.index(tkinter.SEL_FIRST)
-		e = wid.index(tkinter.SEL_LAST)
-		i = wid.index(tkinter.INSERT)
-		
-		if wid == self.contents:
-			
-			# Leave cursor where it is if have selected all
-			if s == self.contents.index('1.0') and e == self.contents.index(tkinter.END):
-				return
-			
-			self.contents.tag_remove('sel', '1.0', tkinter.END)
-			#self.wid.see('1.0')
-			
-			
-			if event.keysym == 'Right':
-				self.contents.mark_set('insert', e)
-				self.ensure_idx_visibility(e)
-				
-			elif event.keysym == 'Left':
-				self.contents.mark_set('insert', s)
-				self.ensure_idx_visibility(s)
-				
-			else:
-				return
-			
-				
-		if wid == self.entry:
-			self.entry.selection_clear()
-			
-			if event.keysym == 'Right':	self.entry.icursor(e)
-			elif event.keysym == 'Left':self.entry.icursor(s)
-			else:
-				return
-			
-		
-		return 'break'
-		
-	
-	def yank_line(self, event=None):
-		'''	copy current line to clipboard
-		'''
-		
-		if self.state not in [ 'normal', 'error' ]:
-			self.bell()
-			return "break"
-			
-			
-		curpos = self.contents.index(tkinter.INSERT)
-		t = self.contents.get('%s linestart' % curpos, '%s lineend' % curpos)
-		
-		
-		if t.strip() != '':
-			self.goto_linestart(event=event)
-			s = self.contents.index( 'insert' )
-			e = self.contents.index( '%s lineend' % curpos )
-			
-			# return cursor back to original place
-			self.contents.mark_set('insert', curpos)
-		
-			tmp = self.contents.get(s,e)
-			self.contents.clipboard_clear()
-			
-			self.contents.tag_remove('sel', '1.0', tkinter.END)
-			self.contents.tag_add('sel', s, e)
-		
-			if self.os_type != 'windows':
-				self.contents.clipboard_append(tmp)
-			else:
-				self.copy_windows(event=event)
-			
-			self.after(600, lambda args=['sel', '1.0', tkinter.END]: self.contents.tag_remove(*args) )
-		
-			
-		return 'break'
-		
-		
-	def goto_lineend(self, event=None):
-		if self.state in [ 'filedialog' ]:
-			self.bell()
-			return "break"
-		
-		idx_linestart = self.idx_linestart()
-		# empty line?
-		if not idx_linestart: return
-		
-		
-		have_selection = False
-		want_selection = False
-		
-		# ctrl-shift-a or e
-		
-		# Pressed also shift, so adjust selection
-		# Linux, macOS state:
-		# ctrl-shift == 5
-		
-		# Windows state:
-		# ctrl-shift == 13
-		
-		# Also in mac_OS:
-		# command-shift-arrowleft or right == 105
-		if event.state in [ 5 , 105, 13 ]:
-			want_selection = True
-			i = self.contents.index(tkinter.INSERT)
-				
-			if len( self.contents.tag_ranges('sel') ) > 0:
-				# need to know if selection started from top or bottom.
-				
-				
-				have_selection = True
-				s = self.contents.index(tkinter.SEL_FIRST)
-				e = self.contents.index(tkinter.SEL_LAST)
-				
-				# selection started from top
-				from_top = False
-				if self.contents.compare(s,'<',i):
-					from_top = True
-					
-				# from bottom
-				# else:	from_top = False
-		
-		
-		self.ensure_idx_visibility('insert')
-		
-		pos = self.idx_lineend()
-		
-		self.contents.see(pos)
-		self.contents.mark_set('insert', pos)
-		
-		
-		if want_selection:
-			if have_selection:
-				if from_top:
-					self.contents.tag_remove('sel', '1.0', tkinter.END)
-					self.contents.tag_add('sel', s, 'insert')
-				
-				#from bottom
-				else:
-					self.contents.tag_remove('sel', '1.0', tkinter.END)
-					self.contents.tag_add('sel', 'insert', e)
-				
-			else:
-				self.contents.tag_add('sel', i, 'insert')
-		
-		
-		# was:
-		#self.contents.event_generate('<<LineEnd>>')
-		return "break"
-		
-		
-	def goto_linestart(self, event=None):
-		if self.state in [ 'filedialog' ]:
-			self.bell()
-			return "break"
-		
-		idx_linestart = self.idx_linestart()
-		# empty line?
-		if not idx_linestart: return
-		
-		
-		have_selection = False
-		want_selection = False
-		
-		# ctrl-shift-a or e
-		
-		# Pressed also shift, so adjust selection
-		# Linux, macOS state:
-		# ctrl-shift == 5
-		
-		# Windows state:
-		# ctrl-shift == 13
-		
-		# Also in mac_OS:
-		# command-shift-arrowleft or right == 105
-		if event.state in [ 5 , 105, 13 ]:
-			want_selection = True
-			i = self.contents.index(tkinter.INSERT)
-				
-			if len( self.contents.tag_ranges('sel') ) > 0:
-				# need to know if selection started from top or bottom.
-				
-				
-				have_selection = True
-				s = self.contents.index(tkinter.SEL_FIRST)
-				e = self.contents.index(tkinter.SEL_LAST)
-				
-				# selection started from top
-				from_top = False
-				if self.contents.compare(s,'<',i):
-					from_top = True
-					
-				# from bottom
-				# else:	from_top = False
-				
-		
-		self.ensure_idx_visibility('insert')
-		
-		pos = self.idx_linestart()
-		
-		self.contents.see(pos)
-		self.contents.mark_set('insert', pos)
-	
-		if want_selection:
-			if have_selection:
-				if from_top:
-					self.contents.tag_remove('sel', '1.0', tkinter.END)
-					self.contents.tag_add('sel', s, 'insert')
-				
-				#from bottom
-				else:
-					self.contents.tag_remove('sel', '1.0', tkinter.END)
-					self.contents.tag_add('sel', 'insert', e)
-				
-			else:
-				self.contents.tag_add('sel', 'insert', i)
-					
-		
-		return "break"
-		
-		
-	def raise_popup(self, event=None):
-		if self.state != 'normal':
-			self.bell()
-			return "break"
-		
-		self.popup.post(event.x_root, event.y_root)
-		self.popup.focus_set() # Needed to remove popup when clicked outside.
-		
-		
-	def popup_focusOut(self, event=None):
-		self.popup.unpost()
-	
-	
-	def copy(self):
-		''' When copy is selected from popup-menu
-		'''
-		if self.os_type == 'windows':
-			self.copy_windows()
-		
-		else:
-			try:
-				self.clipboard_clear()
-				self.clipboard_append(self.selection_get())
-			except tkinter.TclError:
-				# is empty
-				return 'break'
-		
-
-	def move_line(self, event=None, direction=None):
-		''' Adjust cursor line indentation, with arrow left and right,
-			when pasting more than one line etc.
-		'''
-		
-		# currently this interferes with backspace_override
-		
-		# Enable continue adjusting selection area.
-		# 262152 is state when pressing arrow left-right in Win11, 262144 in Win10
-		if self.state != 'normal' or event.state not in [0, 262152, 262144 ]:
-			return 'continue'
-			
-			
-		if len(self.contents.tag_ranges('sel')) > 0:
-			insert_at_selstart = False
-			
-			s = self.contents.index(tkinter.SEL_FIRST)
-			e = self.contents.index(tkinter.SEL_LAST)
-			i = self.contents.index(tkinter.INSERT)
-			# contents of line with cursor:
-			t = self.contents.get('%s linestart' % i, '%s lineend' % i)
-			
-			if i == s:
-				insert_at_selstart = True
-			
-			# else: insert at selend
-			
-			line_s = s.split('.')[0]
-			line_e = e.split('.')[0]
-			
-			# One line only:
-			if line_s == line_e: 	return 'continue'
-
-			# cursor line is empty:
-			if len(t.strip()) == 0: return 'continue'
-
-
-			self.contents.tag_remove('sel', '1.0', tkinter.END)
-			self.contents.tag_add('sel', '%s linestart' % i, '%s lineend' % i)
-
-
-			if direction == 'left':
-
-				# Cursor at the start of the line, or there is no indentation left:
-				if i.split('.')[1] == 0 or not t[0].isspace():
-					self.contents.tag_remove('sel', '1.0', tkinter.END)
-					self.contents.tag_add('sel', s, e)
-					return 'break'
-
-				self.unindent()
-				self.contents.tag_remove('sel', '1.0', tkinter.END)
-
-				if insert_at_selstart:
-					self.contents.tag_add('sel',  '%s -1c' % s, e)
-				else:
-					self.contents.tag_add('sel', s, '%s -1c' % e)
-
-			# right
-			else:
-				self.indent()
-				self.contents.tag_remove('sel', '1.0', tkinter.END)
-
-				if insert_at_selstart:
-					self.contents.tag_add('sel',  '%s +1c' % s, e)
-				else:
-					self.contents.tag_add('sel', s, '%s +1c' % e)
-					
-
-			return 'break'
-
-		return 'continue'
-	
-
-	def paste(self, event=None):
-		'''	First line usually is in wrong place after paste
-			because of selection has not started at the beginning of the line.
-			So we put cursor at the beginning of insertion after pasting it
-			so we can start indenting it.
-		'''
-		
-		try:
-			tmp = self.clipboard_get()
-			tmp = tmp.splitlines(keepends=True)
-			
-			
-		except tkinter.TclError:
-			# is empty
-			return 'break'
-			
-		have_selection = False
-		
-		if len( self.contents.tag_ranges('sel') ) > 0:
-			selstart = self.contents.index( '%s' % tkinter.SEL_FIRST)
-			selend = self.contents.index( '%s' % tkinter.SEL_LAST)
-			
-			self.contents.tag_remove('sel', '1.0', tkinter.END)
-			have_selection = True
-			
-			
-		line = self.contents.index(tkinter.INSERT)
-		self.contents.event_generate('<<Paste>>')
-		
-		
-		# Selected many lines or
-		# one line and cursor is not at the start of next line:
-		if len(tmp) > 1:
-		
-			s = self.contents.index( '%s linestart' % line)
-			e = self.contents.index( 'insert lineend')
-			t = self.contents.get( s, e )
-			
-			if self.tabs[self.tabindex].filepath:
-				if self.can_do_syntax():
-					self.update_tokens( start=s, end=e, line=t )
-					
-			
-			if have_selection:
-				self.contents.tag_add('sel', selstart, selend)
-				
-			else:
-				self.contents.tag_add('sel', line, tkinter.INSERT)
-				
-			self.contents.mark_set('insert', line)
-			
-			
-			self.wait_for(100)
-			self.ensure_idx_visibility(line)
-			
-			
-		# Selected one line and cursor is at the start of next line:
-		elif len(tmp) == 1 and tmp[-1][-1] == '\n':
-			s = self.contents.index( '%s linestart' % line)
-			e = self.contents.index( '%s lineend' % line)
-			t = self.contents.get( s, e )
-			
-			if self.tabs[self.tabindex].filepath:
-				if self.can_do_syntax():
-					self.update_tokens( start=s, end=e, line=t )
-					
-					
-		return 'break'
-	
-
-	def undo_override(self, event=None):
-		if self.state != 'normal':
-			self.bell()
-			return "break"
-		 
-		try:
-			self.contents.edit_undo()
-			
-			
-			self.do_syntax()
-			
-			
-		except tkinter.TclError:
-			self.bell()
-			
-		return 'break'
-		
-		
-	def redo_override(self, event=None):
-		if self.state != 'normal':
-			self.bell()
-			return "break"
-			
-		try:
-			self.contents.edit_redo()
-			
-			
-			self.do_syntax()
-			
-			
-		except tkinter.TclError:
-			self.bell()
-			
-		return 'break'
-		
-		
-	def select_all(self, event=None):
-		self.contents.tag_remove('sel', '1.0', tkinter.END)
-		self.contents.tag_add('sel', 1.0, tkinter.END)
-		return "break"
-	
-	
-	def tab_override(self, event):
-		'''	Used to bind Tab-key with indent()
-		'''
-		
-		if self.state in [ 'search', 'replace', 'replace_all' ]:
-			return 'break'
-		
-		# In Windows, Tab-key-event has state 8 and shift+Tab has state 9,
-		# so because shift-tab is unbinded if in Windows, we check that here
-		# and unindent if it is the state.
-		if hasattr(event, 'state'):
-			
-			if self.os_type == 'windows':
-				
-				if event.state == 9:
-					self.unindent()
-					return 'break'
-					
-				if event.state not in [8, 0]:
-					return
-			
-			elif event.state != 0:
-				return
-				
-		# Fix for tab-key not working sometimes.
-		# This happens because os-clipboard content is (automatically)
-		# added to selection content of a Text widget, and since there is no
-		# actual selection (clipboard-text is outside from Text-widget),
-		# tab_override() gets quite broken.
-		if len(self.contents.tag_ranges('sel')) == 0:
-			return
-		
-		try:
-			tmp = self.contents.selection_get()
-			self.indent(event)
-			return 'break'
-			
-		except tkinter.TclError:
-			# No selection
-			return
-
-	
-	def backspace_override(self, event):
-		""" for syntax highlight
-		"""
-		
-		# State is 8 in windows when no other keys are pressed
-		if self.state != 'normal' or event.state not in [0, 8]:
-			return
-		
-		pars = [ '(', ')', '[', ']' , '{', '}' ]
-		
-		try:
-			
-			# Is there a selection?
-			if len(self.contents.tag_ranges('sel')) > 0:
-				tmp = self.contents.selection_get()
-				l = [ x for x in tmp if x in pars ]
-				if len(l) > 0:
-					self.par_err = True
-				
-			self.contents.delete( tkinter.SEL_FIRST, tkinter.SEL_LAST )
-			
-			self.do_syntax()
-			
-			return 'break'
-			
-				
-		except tkinter.TclError:
-			# Deleting one letter
-			
-			
-			# Rest is multiline string check
-			chars = self.contents.get( '%s - 3c' % tkinter.INSERT, '%s + 2c' % tkinter.INSERT )
-			
-			triples = ["'''", '"""']
-			doubles = ["''", '""']
-			singles = ["'", '"']
-			
-			prev_3chars = chars[:3]
-			prev_2chars = chars[1:3]
-			next_2chars = chars[-2:]
-			
-			prev_char = chars[2:3]
-			next_char = chars[-2:-1]
-		
-			quote_tests = [
-						(prev_char == '#'),
-						(prev_3chars in triples),
-						( (prev_2chars in doubles) and (next_char in singles) ),
-						( (prev_char in singles) and (next_2chars in doubles) )
-						]
-						
-			if any(quote_tests):
-				#print('#')
-				self.token_err = True
-				
-				
-			# To trigger parcheck if only one of these was in line and it was deleted:
-			if prev_char in pars:
-				self.par_err = True
-				
-				
-		#print('deleting')
-				
-		return
-
-	
-	def return_override(self, event):
-		if self.state != 'normal':
-			self.bell()
-			return "break"
-		
-		# ctrl_L-super_L-return
-		if event.state == 68:
-			self.run()
-			return "break"
-		
-		# cmd-return:
-		if self.os_type == 'mac_os' and event.state == 8:
-			self.btn_open.invoke()
-			return 'break'
-		
-		
-	
-		# Cursor indexes when pressed return:
-		line, col = map(int, self.contents.index(tkinter.INSERT).split('.'))
-		
-		
-		# First an easy case:
-		if col == 0:
-			self.contents.insert(tkinter.INSERT, '\n')
-			self.contents.see(f'{line+1}.0')
-			self.contents.edit_separator()
-			return "break"
-			
-		
-		tmp = self.contents.get('%s.0' % str(line),'%s.0 lineend' % str(line))
-		
-		# Then one special case: check if cursor is inside indentation,
-		# and line is not empty.
-		if tmp[:col].isspace() and not tmp[col:].isspace():
-			self.contents.insert(tkinter.INSERT, '\n')
-			self.contents.insert('%s.0' % str(line+1), tmp[:col])
-			self.contents.see(f'{line+1}.0')
-			self.contents.edit_separator()
-			return "break"
-			
-		else:
-			for i in range(len(tmp)):
-				if tmp[i] != '\t':
-					break
-	
-			self.contents.insert(tkinter.INSERT, '\n') # Manual newline because return is overrided.
-			self.contents.insert(tkinter.INSERT, i*'\t')
-			self.contents.see(f'{line+1}.0')
-			self.contents.edit_separator()
-			return "break"
-			
-			
-	def sbset_override(self, *args):
-		'''	Fix for: not being able to config slider min-size
-		'''
-		self.scrollbar.set(*args)
-		
-		h = self.text_widget_height
-
-		# Relative position (tuple on two floats) of
-		# slider-top (a[0]) and -bottom (a[1]) in scale 0-1, a[0] is smaller:
-		a = self.scrollbar.get()
-
-		# current slider size:
-		# (a[1]-a[0])*h
-
-		# want to set slider size to at least p (SLIDER_MINSIZE) pixels,
-		# by adding relative amount(0-1) of d to slider, that is: d/2 to both ends:
-		# ( a[1]+d/2 - (a[0]-d/2) )*h = p
-		# a[1] - a[0] + d = p/h
-		# d = p/h - a[1] + a[0]
-
-
-		d = SLIDER_MINSIZE/h - a[1] + a[0]
-
-		if h*(a[1] - a[0]) < SLIDER_MINSIZE:
-			self.scrollbar.set(a[0], a[1]+d)
-		
-		self.update_linenums()
-		
-
-########## Overrides End
-########## Utilities Begin
-
-	def insert_inspected(self):
-		''' Tries to inspect selection. On success: opens new tab and pastes lines there.
-			New tab can be safely closed with ctrl-d later, or saved with new filename.
-		'''
-		try:
-			target = self.contents.selection_get()
-		except tkinter.TclError:
-			self.bell()
-			return 'break'
-		
-		target=target.strip()
-		
-		if not len(target) > 0:
-			self.bell()
-			return 'break'
-		
-		
-		import inspect
-		is_module = False
-		
-		try:
-			mod = importlib.import_module(target)
-			is_module = True
-			filepath = inspect.getsourcefile(mod)
-			
-			if not filepath:
-				# for example: readline
-				self.bell()
-				print('Could not inspect:', target, '\nimport and use help()')
-				return 'break'
-			
-			try:
-				with open(filepath, 'r', encoding='utf-8') as f:
-					fcontents = f.read()
-					self.new_tab()
-					
-					# just in case:
-					if '.py' in filepath:
-						indentation_is_alien, indent_depth = self.check_indent_depth(fcontents)
-						
-						if indentation_is_alien:
-							# Assuming user wants self.ind_depth, change it without notice:
-							tmp = fcontents.splitlines(True)
-							tmp[:] = [self.tabify(line, width=indent_depth) for line in tmp]
-							tmp = ''.join(tmp)
-							self.tabs[self.tabindex].contents = tmp
-							
-						else:
-							self.tabs[self.tabindex].contents = fcontents
-					else:
-						self.tabs[self.tabindex].contents = fcontents
-				
-					
-					self.tabs[self.tabindex].position = '1.0'
-					self.contents.focus_set()
-					self.contents.see('1.0')
-					self.contents.mark_set('insert', '1.0')
-					self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
-					
-					if self.syntax:
-						self.token_err = True
-						self.update_tokens(start='1.0', end=tkinter.END)
-						self.token_can_update = True
-						
-					else:
-						self.token_can_update = False
-						
-						
-					self.contents.edit_reset()
-					self.contents.edit_modified(0)
-					
-					return 'break'
-					
-			except (EnvironmentError, UnicodeDecodeError) as e:
-				print(e.__str__())
-				print(f'\n Could not open file: {filepath}')
-				self.bell()
-				return 'break'
-					
-		except ModuleNotFoundError:
-			print(f'\n Is not a module: {target}')
-		except TypeError as ee:
-			print(ee.__str__())
-			self.bell()
-			return 'break'
-			
-			
-		if not is_module:
-		
-			try:
-				modulepart = target[:target.rindex('.')]
-				object_part = target[target.rindex('.')+1:]
-				mod = importlib.import_module(modulepart)
-				target_object = getattr(mod, object_part)
-				
-				l = inspect.getsourcelines(target_object)
-				t = ''.join(l[0])
-				
-				self.new_tab()
-				
-				# just in case:
-				indentation_is_alien, indent_depth = self.check_indent_depth(t)
-				
-				if indentation_is_alien:
-					# Assuming user wants self.ind_depth, change it without notice:
-					tmp = t.splitlines(True)
-					tmp[:] = [self.tabify(line, width=indent_depth) for line in tmp]
-					tmp = ''.join(tmp)
-					self.tabs[self.tabindex].contents = tmp
-					
-				else:
-					self.tabs[self.tabindex].contents = t
-				
-				
-				self.tabs[self.tabindex].position = '1.0'
-				self.contents.focus_set()
-				self.contents.see('1.0')
-				self.contents.mark_set('insert', '1.0')
-				self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
-				
-				if self.syntax:
-					self.token_err = True
-					self.update_tokens(start='1.0', end=tkinter.END)
-					self.token_can_update = True
-					
-				else:
-					self.token_can_update = False
-				
-											
-				self.contents.edit_reset()
-				self.contents.edit_modified(0)
-				
-				return 'break'
-			
-			# from .rindex()
-			except ValueError:
-				self.bell()
-				return 'break'
-				
-			except Exception as e:
-				self.bell()
-				print(e.__str__())
-				return 'break'
-		
-		return 'break'
-	
-	
-	def tabify_lines(self, event=None):
-	
-		try:
-			startline = self.contents.index(tkinter.SEL_FIRST).split(sep='.')[0]
-			endline = self.contents.index(tkinter.SEL_LAST).split(sep='.')[0]
-			
-			start = '%s.0' % startline
-			end = '%s.0 lineend' % endline
-			tmp = self.contents.get(start, end)
-			
-			indentation_is_alien, indent_depth = self.check_indent_depth(tmp)
-			
-			tmp = tmp.splitlines()
-			
-			if indentation_is_alien:
-				# Assuming user wants self.ind_depth, change it without notice:
-				tmp[:] = [self.tabify(line, width=indent_depth) for line in tmp]
-							
-			else:
-				tmp[:] = [self.tabify(line) for line in tmp]
-			
-						
-			tmp = ''.join(tmp)
-			
-			self.contents.delete(start, end)
-			self.contents.insert(start, tmp)
-			
-			
-			self.update_tokens(start=start, end=end)
-						
-															
-			self.contents.edit_separator()
-			return "break"
-		
-		except tkinter.TclError as e:
-			#print(e)
-			return "break"
-	
-	
-	def tabify(self, line, width=None):
-		
-		if width:
-			ind_width = width
-		else:
-			ind_width = self.ind_depth
-			
-		indent_stop_index = 0
-		
-		for char in line:
-			if char in [' ', '\t']: indent_stop_index += 1
-			else: break
-			
-		if indent_stop_index == 0:
-			# remove trailing space
-			if not line.isspace():
-				line = line.rstrip() + '\n'
-				
-			return line
-		
-		
-		indent_string = line[:indent_stop_index]
-		line = line[indent_stop_index:]
-		
-		# remove trailing space
-		line = line.rstrip() + '\n'
-		
-		
-		count = 0
-		for char in indent_string:
-			if char == '\t':
-				count = 0
-				continue
-			if char == ' ': count += 1
-			if count == ind_width:
-				indent_string = indent_string.replace(ind_width * ' ', '\t', True)
-				count = 0
-		
-		tabified_line = ''.join([indent_string, line])
-		
-		return tabified_line
-	
-	
-
-########## Utilities End
-########## Save and Load Begin
-
-	
-	def trace_filename(self, *args):
-		
-		# canceled
-		if self.tracevar_filename.get() == '':
-			self.entry.delete(0, tkinter.END)
-			
-			if self.tabs[self.tabindex].filepath != None:
-				self.entry.insert(0, self.tabs[self.tabindex].filepath)
-				
-		else:
-			# update self.lastdir
-			filename = pathlib.Path().cwd() / self.tracevar_filename.get()
-			self.lastdir = pathlib.Path(*filename.parts[:-1])
-		
-			self.loadfile(filename)
-		
-		
-		self.tracevar_filename.trace_remove('write', self.tracefunc_name)
-		self.tracefunc_name = None
-		self.contents.bind( "<Alt-Return>", lambda event: self.btn_open.invoke())
-		
-		self.state = 'normal'
-		
-	
-		for widget in [self.entry, self.btn_open, self.btn_save, self.contents]:
-			widget.config(state='normal')
-		
-		return 'break'
-		
-			
-	def loadfile(self, filepath):
-		''' filepath is tkinter.pathlib.Path
-		'''
-
-		filename = filepath
-		openfiles = [tab.filepath for tab in self.tabs]
-		
-		for widget in [self.entry, self.btn_open, self.btn_save, self.contents]:
-			widget.config(state='normal')
-		
-		
-		if filename in openfiles:
-			print(f'file: {filename} is already open')
-			self.bell()
-			self.entry.delete(0, tkinter.END)
-			
-			if self.tabs[self.tabindex].filepath != None:
-				self.entry.insert(0, self.tabs[self.tabindex].filepath)
-			
-			return
-		
-		if self.tabs[self.tabindex].type == 'normal':
-			self.save(activetab=True)
-		
-		# Using same tab:
-		try:
-			with open(filename, 'r', encoding='utf-8') as f:
-				tmp = f.read()
-				self.tabs[self.tabindex].oldcontents = tmp
-				
-				if '.py' in filename.suffix:
-					indentation_is_alien, indent_depth = self.check_indent_depth(tmp)
-					
-					if indentation_is_alien:
-						# Assuming user wants self.ind_depth, change it without notice:
-						tmp = self.tabs[self.tabindex].oldcontents.splitlines(True)
-						tmp[:] = [self.tabify(line, width=indent_depth) for line in tmp]
-						tmp = ''.join(tmp)
-						self.tabs[self.tabindex].contents = tmp
-						
-					else:
-						self.tabs[self.tabindex].contents = self.tabs[self.tabindex].oldcontents
-				else:
-					self.tabs[self.tabindex].contents = self.tabs[self.tabindex].oldcontents
-				
-			
-				
-				self.entry.delete(0, tkinter.END)
-				self.tabs[self.tabindex].filepath = filename
-				self.tabs[self.tabindex].type = 'normal'
-				self.tabs[self.tabindex].position = '1.0'
-				self.entry.insert(0, filename)
-				
-				
-				self.contents.delete('1.0', tkinter.END)
-				self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
-				
-				
-				self.do_syntax(everything=True)
-				
-				
-				self.contents.focus_set()
-				self.contents.see('1.0')
-				self.contents.mark_set('insert', '1.0')
-				
-				self.contents.edit_reset()
-				self.contents.edit_modified(0)
-				self.avoid_viewsync_mess()
-				
-		except (EnvironmentError, UnicodeDecodeError) as e:
-			print(e.__str__())
-			print(f'\n Could not open file: {filename}')
-			self.entry.delete(0, tkinter.END)
-			
-			if self.tabs[self.tabindex].filepath != None:
-				self.entry.insert(0, self.tabs[self.tabindex].filepath)
-				
-		return
-		
-	
-	def load(self, event=None):
-		'''	Get just the filename,
-			on success, pass it to loadfile()
-		'''
-		
-		if self.state != 'normal':
-			self.bell()
-			return 'break'
-		
-		
-		# Pressed Open-button
-		if event == None:
-		
-			self.state = 'filedialog'
-			self.contents.bind( "<Alt-Return>", self.do_nothing)
-			
-			for widget in [self.entry, self.btn_open, self.btn_save, self.contents]:
-				widget.config(state='disabled')
-				
-			self.tracevar_filename.set('empty')
-			self.tracefunc_name = self.tracevar_filename.trace_add('write', self.trace_filename)
-			
-			p = pathlib.Path().cwd()
-			
-			if self.lastdir:
-				p = p / self.lastdir
-			
-			filetop = tkinter.Toplevel()
-			filetop.title('Select File')
-			self.to_be_closed.append(filetop)
-			
-			
-			fd = fdialog.FDialog(filetop, p, self.tracevar_filename, font=self.font, menufont=self.menufont, os_type=self.os_type)
-			
-			return 'break'
-			
-
-		# Entered filename to be opened in entry:
-		else:
-			tmp = self.entry.get().strip()
-
-			if not isinstance(tmp, str) or tmp.isspace():
-				self.bell()
-				return 'break'
-	
-			filename = pathlib.Path().cwd() / tmp
-			
-			self.loadfile(filename)
-			
-			return 'break'
-
-					
-	def save(self, activetab=False, forced=False):
-		''' forced when run() or quit_me()
-			activetab=True from load() and del_tab()
-		'''
-		
-		if forced:
-			
-			# Dont want contents to be replaced with errorlines or help.
-			if self.state != 'normal':
-				self.contents.event_generate('<Escape>')
-			
-			# update active tab first
-			try:
-				pos = self.contents.index(tkinter.INSERT)
-			except tkinter.TclError:
-				pos = '1.0'
-				
-			tmp = self.contents.get('1.0', tkinter.END)
-	
-			self.tabs[self.tabindex].position = pos
-			self.tabs[self.tabindex].contents = tmp
-			
-			
-			# Then save tabs to disk
-			for tab in self.tabs:
-				if tab.type == 'normal':
-					
-					# Check indent (tabify) and rstrip:
-					tmp = tab.contents.splitlines(True)
-					tmp[:] = [self.tabify(line) for line in tmp]
-					tmp = ''.join(tmp)
-					
-					if tab.active == True:
-						tmp = tmp[:-1]
-					
-					tab.contents = tmp
-					
-					if tab.contents == tab.oldcontents:
-						continue
-					
-					try:
-						with open(tab.filepath, 'w', encoding='utf-8') as f:
-							f.write(tab.contents)
-							tab.oldcontents = tab.contents
-							
-					except EnvironmentError as e:
-						print(e.__str__())
-						print(f'\n Could not save file: {tab.filepath}')
-				else:
-					tab.position = '1.0'
-					
-			return
-
-		# if not forced (Pressed Save-button):
-
-		tmp = self.entry.get().strip()
-		
-		if not isinstance(tmp, str) or tmp.isspace():
-			print('Give a valid filename')
-			self.bell()
-			return
-		
-		fpath_in_entry = pathlib.Path().cwd() / tmp
-		
-		try:
-			pos = self.contents.index(tkinter.INSERT)
-		except tkinter.TclError:
-			pos = '1.0'
-					
-		tmp = self.contents.get('1.0', tkinter.END)
-		
-		self.tabs[self.tabindex].position = pos
-		self.tabs[self.tabindex].contents = tmp
-
-		openfiles = [tab.filepath for tab in self.tabs]
-		
-		
-		# creating new file
-		if fpath_in_entry != self.tabs[self.tabindex].filepath and not activetab:
-		
-			if fpath_in_entry in openfiles:
-				self.bell()
-				print(f'\nFile: {fpath_in_entry} already opened')
-				self.entry.delete(0, tkinter.END)
-			
-				if self.tabs[self.tabindex].filepath != None:
-					self.entry.insert(0, self.tabs[self.tabindex].filepath)
-				return
-				
-			if fpath_in_entry.exists():
-				self.bell()
-				print(f'\nCan not overwrite file: {fpath_in_entry}')
-				self.entry.delete(0, tkinter.END)
-			
-				if self.tabs[self.tabindex].filepath != None:
-					self.entry.insert(0, self.tabs[self.tabindex].filepath)
-				return
-			
-			if self.tabs[self.tabindex].type == 'newtab':
-			
-				# avoiding disk-writes, just checking filepath:
-				try:
-					with open(fpath_in_entry, 'w', encoding='utf-8') as f:
-						self.tabs[self.tabindex].filepath = fpath_in_entry
-						self.tabs[self.tabindex].type = 'normal'
-				except EnvironmentError as e:
-					print(e.__str__())
-					print(f'\n Could not save file: {fpath_in_entry}')
-					return
-				
-				if self.tabs[self.tabindex].filepath != None:
-					self.entry.delete(0, tkinter.END)
-					self.entry.insert(0, self.tabs[self.tabindex].filepath)
-					
-					
-					self.do_syntax()
-			
-				
-				# set cursor pos
-				try:
-					line = self.tabs[self.tabindex].position
-					self.contents.focus_set()
-					self.contents.mark_set('insert', line)
-					self.ensure_idx_visibility(line)
-					
-				except tkinter.TclError:
-					self.tabs[self.tabindex].position = '1.0'
-				
-				self.contents.edit_reset()
-				self.contents.edit_modified(0)
-				
-					
-				
-			# want to create new file with same contents:
-			else:
-				try:
-					with open(fpath_in_entry, 'w', encoding='utf-8') as f:
-						pass
-				except EnvironmentError as e:
-					print(e.__str__())
-					print(f'\n Could not save file: {fpath_in_entry}')
-					self.entry.delete(0, tkinter.END)
-			
-					if self.tabs[self.tabindex].filepath != None:
-						self.entry.insert(0, self.tabs[self.tabindex].filepath)
-					return
-					
-				self.new_tab()
-				self.tabs[self.tabindex].filepath = fpath_in_entry
-				self.tabs[self.tabindex].contents = tmp
-				self.tabs[self.tabindex].position = pos
-				self.tabs[self.tabindex].type = 'normal'
-				
-				self.entry.delete(0, tkinter.END)
-				self.entry.insert(0, self.tabs[self.tabindex].filepath)
-				
-			
-				self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
-		
-				
-				self.do_syntax(everything=True)
-				
-				
-				# set cursor pos
-				try:
-					line = self.tabs[self.tabindex].position
-					self.contents.focus_set()
-					self.contents.mark_set('insert', line)
-					self.ensure_idx_visibility(line)
-					
-				except tkinter.TclError:
-					self.tabs[self.tabindex].position = '1.0'
-				
-				
-				self.contents.edit_reset()
-				self.contents.edit_modified(0)
-				
-				
-		else:
-			# skip unnecessary disk-writing silently
-			if not activetab:
-				return
-
-			# if closing tab or loading file:
-		
-			# Check indent (tabify) and rstrip:
-			tmp = self.tabs[self.tabindex].contents.splitlines(True)
-			tmp[:] = [self.tabify(line) for line in tmp]
-			tmp = ''.join(tmp)[:-1]
-			
-			if self.tabs[self.tabindex].contents == self.tabs[self.tabindex].oldcontents:
-				return
-				
-			try:
-				with open(self.tabs[self.tabindex].filepath, 'w', encoding='utf-8') as f:
-					f.write(tmp)
-					
-			except EnvironmentError as e:
-				print(e.__str__())
-				print(f'\n Could not save file: {self.tabs[self.tabindex].filepath}')
-				return
-				
-		############# Save End #######################################
-	
-########## Save and Load End
-########## Gotoline and Help Begin
-	
-	def do_gotoline(self, event=None):
-		try:
-			tmp = self.entry.get().strip()
-			
-			if tmp in ['-1', '']:
-				line = tkinter.END
-			else:
-				line = tmp + '.0'
-				
-			self.contents.focus_set()
-			self.contents.mark_set('insert', line)
-			self.ensure_idx_visibility(line)
-			
-			
-			try:
-				pos = self.contents.index(tkinter.INSERT)
-			except tkinter.TclError:
-				pos = '1.0'
-				
-			self.tabs[self.tabindex].position = pos
-			self.stop_gotoline()
-			
-		except tkinter.TclError as e:
-			print(e)
-			self.stop_gotoline()
-			
-		return "break"
-		
-	
-	def stop_gotoline(self, event=None):
-		self.state = 'normal'
-		self.bind("<Escape>", self.do_nothing)
-		self.entry.bind("<Return>", self.load)
-		self.entry.delete(0, tkinter.END)
-		if self.tabs[self.tabindex].filepath:
-			self.entry.insert(0, self.tabs[self.tabindex].filepath)
-		self.update_title()
-		
-		# set cursor pos
-		try:
-			line = self.tabs[self.tabindex].position
-			self.contents.focus_set()
-			self.contents.mark_set('insert', line)
-			self.ensure_idx_visibility(line)
-		
-		except tkinter.TclError:
-			self.tabs[self.tabindex].position = '1.0'
-		
-		return "break"
-		
-	
-	def gotoline(self, event=None):
-		if self.state != 'normal':
-			self.bell()
-			return "break"
-		
-		self.state = 'gotoline'
-		
-		try:
-			pos = self.contents.index(tkinter.INSERT)
-		except tkinter.TclError:
-			pos = '1.0'
-		
-		self.tabs[self.tabindex].position = pos
-		
-		# Remove extra line
-		endline = int(self.contents.index(tkinter.END).split('.')[0]) - 1
-		
-		self.entry.bind("<Return>", self.do_gotoline)
-		self.bind("<Escape>", self.stop_gotoline)
-		self.title('Go to line, 1-%s:' % endline)
-		self.entry.delete(0, tkinter.END)
-		self.entry.focus_set()
-		return "break"
-	
-	
-	def stop_help(self, event=None):
-		self.state = 'normal'
-		
-		self.entry.config(state='normal')
-		self.contents.config(state='normal')
-		self.btn_open.config(state='normal')
-		self.btn_save.config(state='normal')
-		
-		if self.tabs[self.tabindex].filepath:
-			self.entry.insert(0, self.tabs[self.tabindex].filepath)
-		
-		self.token_can_update = True
-		self.contents.delete('1.0', tkinter.END)
-		self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
-		
-		
-		self.do_syntax(everything=True)
-		
-		
-		# set cursor pos
-		try:
-			line = self.tabs[self.tabindex].position
-			self.contents.focus_set()
-			self.contents.mark_set('insert', line)
-			self.ensure_idx_visibility(line)
-			
-		except tkinter.TclError:
-			self.tabs[self.tabindex].position = '1.0'
-		
-			
-		self.contents.edit_reset()
-		self.contents.edit_modified(0)
-		self.avoid_viewsync_mess()
-		
-		self.bind("<Escape>", self.do_nothing)
-		self.contents.bind("<Button-%i>" % self.right_mousebutton_num, lambda event: self.raise_popup(event))
-		
-		
-	def help(self, event=None):
-		if self.state != 'normal':
-			self.bell()
-			return "break"
-			
-		self.state = 'help'
-		
-		try:
-			pos = self.contents.index(tkinter.INSERT)
-		except tkinter.TclError:
-			pos = '1.0'
-		
-		self.tabs[self.tabindex].position = pos
-		tmp = self.contents.get('1.0', tkinter.END)
-		# [:-1]: remove unwanted extra newline
-		self.tabs[self.tabindex].contents = tmp[:-1]
-		
-		self.token_can_update = False
-		
-		self.entry.delete(0, tkinter.END)
-		self.contents.delete('1.0', tkinter.END)
-		self.contents.insert(tkinter.INSERT, self.helptxt)
-		
-		self.entry.config(state='disabled')
-		self.contents.config(state='disabled')
-		self.btn_open.config(state='disabled')
-		self.btn_save.config(state='disabled')
-		
-		self.contents.bind("<Button-%i>" % self.right_mousebutton_num, self.do_nothing)
-		self.bind("<Escape>", self.stop_help)
-			
-########## Gotoline and Help End
-########## Indent and Comment Begin
-	
-	def check_indent_depth(self, contents):
-		'''Contents is contents of py-file as string.'''
-		
-		words = [
-				'def ',
-				'if ',
-				'for ',
-				'while ',
-				'class '
-				]
-				
-		tmp = contents.splitlines()
-		
-		for word in words:
-			
-			for i in range(len(tmp)):
-				line = tmp[i]
-				if word in line:
-					
-					# Trying to check if at the beginning of new block:
-					if line.strip()[-1] == ':':
-						# Offset is num of empty lines between this line and next
-						# non empty line
-						nextline = None
-						
-						for offset in range(1, len(tmp)-i):
-							nextline = tmp[i+offset]
-							if nextline.strip() == '': continue
-							else: break
-							
-							
-						if not nextline:
-							continue
-						
-						
-						# Now should have next non empty line,
-						# so start parsing it:
-						flag_space = False
-						indent_0 = 0
-						indent_1 = 0
-		
-						for char in line:
-							if char in [' ', '\t']: indent_0 += 1
-							else: break
-		
-						for char in nextline:
-							# Check if indent done with spaces:
-							if char == ' ':
-								flag_space = True
-		
-							if char in [' ', '\t']: indent_1 += 1
-							else: break
-						
-						
-						indent = indent_1 - indent_0
-						#print(indent)
-						tests = [
-								( indent <= 0 ),
-								( not flag_space and indent > 1 )
-								]
-						
-						if any(tests):
-							#print('indent err')
-							#skipping
-							continue
-						
-						
-						# All is good, do nothing:
-						if not flag_space:
-							return False, 0
-							
-						# Found one block with spaced indentation,
-						# assuming it is used in whole file.
-						else:
-							if indent != self.ind_depth:
-								return True, indent
-							
-							else:
-								return False, 0
-					
-		return False, 0
-	
-	
-	def indent(self, event=None):
-		if self.state != 'normal':
-			self.bell()
-			
-		try:
-			startline = int(self.contents.index(tkinter.SEL_FIRST).split(sep='.')[0])
-			endline = int(self.contents.index(tkinter.SEL_LAST).split(sep='.')[0])
-			i = self.contents.index(tkinter.INSERT)
-			
-			start_idx = self.contents.index(tkinter.SEL_FIRST)
-			end_idx = self.contents.index(tkinter.SEL_LAST)
-					
-			self.contents.tag_remove('sel', '1.0', tkinter.END)
-			self.contents.tag_add('sel', start_idx, end_idx)
-			
-		
-			if len(self.contents.tag_ranges('sel')) != 0:
-					
-				# is start of selection viewable?
-				if not self.contents.bbox(tkinter.SEL_FIRST):
-					
-					self.wait_for(150)
-					self.ensure_idx_visibility(tkinter.SEL_FIRST, back=4)
-					self.wait_for(100)
-						
-			
-			for linenum in range(startline, endline+1):
-				self.contents.mark_set(tkinter.INSERT, '%s.0' % linenum)
-				self.contents.insert(tkinter.INSERT, '\t')
-			
-			
-			if startline == endline:
-				self.contents.mark_set(tkinter.INSERT, '%s +1c' %i)
-			
-			elif self.contents.compare(tkinter.SEL_FIRST, '<', tkinter.INSERT):
-				self.contents.mark_set(tkinter.INSERT, tkinter.SEL_FIRST)
-				
-			self.ensure_idx_visibility('insert', back=4)
-			self.contents.edit_separator()
-			
-		except tkinter.TclError:
-			pass
-			
-
-	def unindent(self, event=None):
-		if self.state != 'normal':
-			self.bell()
-			return "break"
-			
-		try:
-			# unindenting curline only:
-			if len(self.contents.tag_ranges('sel')) == 0:
-				startline = int( self.contents.index(tkinter.INSERT).split(sep='.')[0] )
-				endline = startline
-	
-			else:
-				startline = int(self.contents.index(tkinter.SEL_FIRST).split(sep='.')[0])
-				endline = int(self.contents.index(tkinter.SEL_LAST).split(sep='.')[0])
-			
-			i = self.contents.index(tkinter.INSERT)
-			
-			# Check there is enough space in every line:
-			flag_continue = True
-			
-			for linenum in range(startline, endline+1):
-				tmp = self.contents.get('%s.0' % linenum, '%s.0 lineend' % linenum)
-				
-				if len(tmp) != 0 and tmp[0] != '\t':
-					flag_continue = False
-					break
-				
-			if flag_continue:
-				
-				if len(self.contents.tag_ranges('sel')) != 0:
-					
-					# is start of selection viewable?
-					if not self.contents.bbox(tkinter.SEL_FIRST):
-						
-						self.wait_for(150)
-						self.ensure_idx_visibility('insert', back=4)
-						self.wait_for(100)
-						
-						
-				for linenum in range(startline, endline+1):
-					tmp = self.contents.get('%s.0' % linenum, '%s.0 lineend' % linenum)
-				
-					if len(tmp) != 0:
-						if len(self.contents.tag_ranges('sel')) != 0:
-							self.contents.mark_set(tkinter.INSERT, '%s.0' % linenum)
-							self.contents.delete(tkinter.INSERT, '%s+%dc' % (tkinter.INSERT, 1))
-						
-						else:
-							self.contents.delete( '%s.0' % linenum, '%s.0 +1c' % linenum)
-				
-		
-				# is selection made from down to top or from right to left?
-				if len(self.contents.tag_ranges('sel')) != 0:
-				
-					if startline == endline:
-						self.contents.mark_set(tkinter.INSERT, '%s -1c' %i)
-					
-					elif self.contents.compare(tkinter.SEL_FIRST, '<', tkinter.INSERT):
-						self.contents.mark_set(tkinter.INSERT, tkinter.SEL_FIRST)
-						
-					# is start of selection viewable?
-					if not self.contents.bbox(tkinter.SEL_FIRST):
-						self.ensure_idx_visibility('insert', back=4)
-					
-				self.contents.edit_separator()
-		
-		except tkinter.TclError as e:
-			pass
-			
-		return "break"
-	
-	
-	def comment(self, event=None):
-		if self.state != 'normal':
-			self.bell()
-			return "break"
-			
-		try:
-			s = self.contents.index(tkinter.SEL_FIRST)
-			e = self.contents.index(tkinter.SEL_LAST)
-		
-			startline = int( s.split('.')[0] )
-			startpos = self.contents.index( '%s linestart' % s )
-			
-			endline = int( e.split('.')[0] )
-			endpos = self.contents.index( '%s lineend' % e )
-			
-			
-			for linenum in range(startline, endline+1):
-				self.contents.mark_set(tkinter.INSERT, '%s.0' % linenum)
-				self.contents.insert(tkinter.INSERT, '##')
-				
-						
-			self.update_tokens(start=startpos, end=endpos)
-			
-				
-			self.contents.edit_separator()
-			return "break"
-		
-		except tkinter.TclError as e:
-			print(e)
-			return "break"
-	
-
-	def uncomment(self, event=None):
-		''' Should work even if there are uncommented lines between commented lines. '''
-		if self.state != 'normal':
-			self.bell()
-			return "break"
-			
-		try:
-			s = self.contents.index(tkinter.SEL_FIRST)
-			e = self.contents.index(tkinter.SEL_LAST)
-		
-			startline = int(s.split('.')[0])
-			endline = int(e.split('.')[0])
-			startpos = self.contents.index('%s linestart' % s)
-			endpos = self.contents.index('%s lineend' % e)
-				
-			changed = False
-			
-			for linenum in range(startline, endline+1):
-				self.contents.mark_set(tkinter.INSERT, '%s.0' % linenum)
-				tmp = self.contents.get('%s.0' % linenum,'%s.0 lineend' % linenum)
-				
-				if tmp.lstrip()[:2] == '##':
-					tmp = tmp.replace('##', '', 1)
-					self.contents.delete('%s.0' % linenum,'%s.0 lineend' % linenum)
-					self.contents.insert(tkinter.INSERT, tmp)
-					changed = True
-					
-					
-			if changed:
-			
-				self.update_tokens(start=startpos, end=endpos)
-				
-				self.contents.edit_separator()
-			
-		except tkinter.TclError as e:
-			print(e)
-		return "break"
-		
-########## Indent and Comment End
-################ Search Begin
-	
-	def check_next_event(self, event=None):
-		
-		if event.keysym == 'Left':
-			line = self.lastcursorpos
-			self.contents.tag_remove('sel', '1.0', tkinter.END)
-			self.contents.mark_set('insert', line)
-			self.ensure_idx_visibility(line)
-			
-			
-			self.contents.unbind("<Any-Key>", funcid=self.anykeyid)
-			self.contents.unbind("<Any-Button>", funcid=self.anybutid)
-			
-			f = self.check_sel
-			if self.os_type == 'mac_os': f = self.mac_cmd_overrides
-			
-			self.bid_left = self.contents.bind("<Left>", f )
-		
-			return 'break'
-			
-		else:
-			self.contents.unbind("<Any-Key>", funcid=self.anykeyid)
-			self.contents.unbind("<Any-Button>", funcid=self.anybutid)
-			
-			f = self.check_sel
-			if self.os_type == 'mac_os': f = self.mac_cmd_overrides
-			self.bid_left = self.contents.bind("<Left>", f )
-			
-			return
-			
-		
-		
-	def search_next(self, event=None):
-		'''	Do last search from cursor position, show and select next match.
-			
-			This is for cases when you can not do replace ALL.
-			You need to choose when to insert AND insertion is not always
-			the same. But replace is too limited (can not insert, like in search).
-			So you do normal search and quit quickly. Then copy your insertion
-			'pattern' in clipboard, what you add to certain matches and then
-			maybe change something else, or you need sometimes delete match and
-			insert your clipboard 'pattern' etc...
-			
-			In short:
-			1: Do normal search
-			2: copy what you need to have in clipboard
-			3: ctrl-backspace until in right place
-			4: now easy to delete or add clipboard contents etc..
-			5: repeat 3-4
-			
-			shortcut: ctrl-backspace
-		'''
-		
-		if self.state != 'normal' or self.old_word == '':
-			self.bell()
-			return "break"
-			
-			
-		wordlen = len(self.old_word)
-		self.lastcursorpos = self.contents.index(tkinter.INSERT)
-		pos = self.contents.search(self.old_word, 'insert +1c', tkinter.END)
-		
-		# Try again from the beginning this time:
-		if not pos:
-			pos = self.contents.search(self.old_word, '1.0', tkinter.END)
-			
-			# no oldword in file:
-			if not pos:
-				self.bell()
-				#print('no')
-				return "break"
-		
-		# Go back to last place with arrow left
-		self.anykeyid = self.contents.bind( "<Any-Key>", self.check_next_event)
-		self.anybutid = self.contents.bind( "<Any-Button>", self.check_next_event)
-		
-		# Without this one can not search by holding ctrl down and
-		# pressing and releasing repeatedly backspace only:
-		if self.bid_left: self.contents.unbind("<Left>", self.bid_left)
-		self.bid_left = None
-		
-		
-		lastpos = "%s + %dc" % (pos, wordlen)
-		self.contents.tag_remove('sel', '1.0', tkinter.END)
-		self.contents.tag_add('sel', pos, lastpos)
-		self.contents.mark_set('insert', lastpos)
-		line = pos
-		self.ensure_idx_visibility(line)
-					
-		return "break"
-
-
-	def show_next(self, event=None):
-		if self.state not in [ 'search', 'replace', 'replace_all' ]:
-			return
-			
-		match_ranges = self.contents.tag_ranges('match')
-		
-		# check if at last match or beyond:
-		i = len(match_ranges) - 2
-		last = match_ranges[i]
-	
-		if self.contents.compare(self.search_idx[0], '>=', last):
-			self.search_idx = ('1.0', '1.0')
-				
-		if self.search_idx != ('1.0', '1.0'):
-			self.contents.tag_remove('focus', self.search_idx[0], self.search_idx[1])
-		else:
-			self.contents.tag_remove('focus', '1.0', tkinter.END)
-		
-		
-		self.search_idx = self.contents.tag_nextrange('match', self.search_idx[1])
-		line = self.search_idx[0]
-		
-		# is it viewable?
-		if not self.contents.bbox(line):
-			self.wait_for(100)
-		
-		self.ensure_idx_visibility(line)
-		
-		
-		# change color
-		self.contents.tag_add('focus', self.search_idx[0], self.search_idx[1])
-		
-		# compare found to match
-		ref = self.contents.tag_ranges('focus')[0]
-		
-		for idx in range(self.search_matches):
-			tmp = match_ranges[idx*2]
-			if self.contents.compare(ref, '==', tmp): break
-		
-		
-		if self.state == 'replace':
-			self.title( f'Replace: {idx+1}/{self.search_matches}' )
-		else:
-			self.title( f'Search: {idx+1}/{self.search_matches}' )
-		
-		
-		if self.search_matches == 1:
-			self.bind("<Control-n>", self.do_nothing)
-			self.bind("<Control-p>", self.do_nothing)
-		
-		return 'break'
-		
-
-	def show_prev(self, event=None):
-		
-		if self.state not in [ 'search', 'replace', 'replace_all' ]:
-			return
-		
-		match_ranges = self.contents.tag_ranges('match')
-		
-		first = match_ranges[0]
-	
-		if self.contents.compare(self.search_idx[0], '<=', first):
-			self.search_idx = (tkinter.END, tkinter.END)
-		
-		if self.search_idx != (tkinter.END, tkinter.END):
-			self.contents.tag_remove('focus', self.search_idx[0], self.search_idx[1])
-		else:
-			self.contents.tag_remove('focus', '1.0', tkinter.END)
-		
-		self.search_idx = self.contents.tag_prevrange('match', self.search_idx[0])
-		
-		line = self.search_idx[0]
-		# is it viewable?
-		if not self.contents.bbox(line):
-			self.wait_for(100)
-		
-		self.ensure_idx_visibility(line)
-		
-		# change color
-		self.contents.tag_add('focus', self.search_idx[0], self.search_idx[1])
-		
-		# compare found to match
-		ref = self.contents.tag_ranges('focus')[0]
-		
-		for idx in range(self.search_matches):
-			tmp = match_ranges[idx*2]
-			if self.contents.compare(ref, '==', tmp): break
-			
-		
-		if self.state == 'replace':
-			self.title( f'Replace: {idx+1}/{self.search_matches}' )
-		else:
-			self.title( f'Search: {idx+1}/{self.search_matches}' )
-		
-		
-		if self.search_matches == 1:
-			self.bind("<Control-n>", self.do_nothing)
-			self.bind("<Control-p>", self.do_nothing)
-			
-		return 'break'
-		
-		
-	def start_search(self, event=None):
-		self.old_word = self.entry.get()
-		self.contents.tag_remove('match', '1.0', tkinter.END)
-		self.contents.tag_remove('focus', '1.0', tkinter.END)
-		self.search_idx = ('1.0', '1.0')
-		self.search_matches = 0
-		
-		if len(self.old_word) != 0:
-			pos = '1.0'
-			wordlen = len(self.old_word)
-			flag_start = True
-			
-			while True:
-				pos = self.contents.search(self.old_word, pos, tkinter.END)
-				if not pos: break
-				self.search_matches += 1
-				lastpos = "%s + %dc" % (pos, wordlen)
-				self.contents.tag_add('match', pos, lastpos)
-				if flag_start:
-					flag_start = False
-					self.contents.focus_set()
-					self.wait_for(100)
-					self.show_next()
-				pos = "%s + %dc" % (pos, wordlen+1)
-				
-		if self.search_matches > 0:
-			self.contents.bind("<Button-%i>" % self.right_mousebutton_num, self.do_nothing)
-			
-			if self.state == 'search':
-				self.title( f'Search: 1/{self.search_matches}' )
-				
-				self.bind("<Control-n>", self.show_next)
-				self.bind("<Control-p>", self.show_prev)
-			
-			else:
-				self.title('Replace %s matches with:' % str(self.search_matches))
-				self.entry.bind("<Return>", self.start_replace)
-				self.entry.focus_set()
-		else:
-			self.bell()
-				
-		return 'break'
-		
-		
-	def update_curpos(self, event=None):
-		self.save_pos = self.contents.index(tkinter.INSERT)
-		
-		# This is needed to enable replacing with Return.
-		# Because of binding to self in start_replace().
-		# And when pressing contents with mouse, self.contents gets focus,
-		# so put it back to self.
-		self.focus_set()
-		
-		return "break"
-			
-			
-	def clear_search_tags(self, event=None):
-		if self.state != 'normal':
-			return "break"
-			
-		self.contents.tag_remove('replaced', '1.0', tkinter.END)
-		self.bind("<Escape>", self.do_nothing)
-		
-	
-	def stop_search(self, event=None):
-		self.contents.config(state='normal')
-		self.entry.config(state='normal')
-		self.btn_open.config(state='normal')
-		self.btn_save.config(state='normal')
-		self.replace_overlap_index = None
-		self.contents.bind("<Button-%i>" % self.right_mousebutton_num, lambda event: self.raise_popup(event))
-		
-		#self.wait_for(200)
-		self.contents.tag_remove('focus', '1.0', tkinter.END)
-		self.contents.tag_remove('match', '1.0', tkinter.END)
-			
-		# Leave marks on replaced areas, Esc clears.
-		if len(self.contents.tag_ranges('replaced')) > 0:
-			self.bind("<Escape>", self.clear_search_tags)
-		else:
-			self.bind("<Escape>", self.do_nothing)
-			
-		
-		self.entry.bind("<Return>", self.load)
-		self.entry.delete(0, tkinter.END)
-	
-		if self.tabs[self.tabindex].filepath:
-			self.entry.insert(0, self.tabs[self.tabindex].filepath)
-	
-		self.new_word = ''
-		self.search_matches = 0
-		self.update_title()
-		flag_all = False
-		if self.state == 'replace_all': flag_all = True
-		
-		if self.state in [ 'replace_all', 'replace' ]:
-			
-				self.state = 'normal'
-				
-				self.do_syntax()
-				
-				
-		self.state = 'normal'
-		self.contents.unbind( "<Control-n>", funcid=self.bid1 )
-		self.contents.unbind( "<Control-p>", funcid=self.bid2 )
-		self.contents.unbind( "<ButtonRelease-1>", funcid=self.bid3 )
-		self.contents.bind( "<Control-n>", self.move_down)
-		self.contents.bind( "<Control-p>", self.move_up)
-		self.bind( "<Return>", self.do_nothing)
-		
-		
-		#self.wait_for(200)
-		
-		# set cursor pos
-		try:
-			if self.save_pos:
-				line = self.save_pos
-				self.tabs[self.tabindex].position = line
-				self.save_pos = None
-			else:
-				line = self.tabs[self.tabindex].position
-			
-			self.contents.focus_set()
-			self.contents.mark_set('insert', line)
-	
-			if not flag_all:
-				self.ensure_idx_visibility(line)
-			
-		except tkinter.TclError:
-			self.tabs[self.tabindex].position = self.contents.index(tkinter.INSERT)
-			
-	
-	def search(self, event=None):
-		if self.state != 'normal':
-			self.bell()
-			return "break"
-		
-		# save cursor pos
-		try:
-			self.tabs[self.tabindex].position = self.contents.index(tkinter.INSERT)
-		
-		except tkinter.TclError:
-			pass
-			
-		self.state = 'search'
-		self.btn_open.config(state='disabled')
-		self.btn_save.config(state='disabled')
-		self.entry.bind("<Return>", self.start_search)
-		self.bind("<Escape>", self.stop_search)
-		
-		self.bid1 = self.contents.bind("<Control-n>", func=self.skip_bindlevel )
-		self.bid2 = self.contents.bind("<Control-p>", func=self.skip_bindlevel )
-		self.bid3 = self.contents.bind("<ButtonRelease-1>", func=self.update_curpos, add=True )
-		
-		self.title('Search:')
-		self.entry.delete(0, tkinter.END)
-		
-		# autofill from clipboard
-		try:
-			tmp = self.clipboard_get()
-			if 80 > len(tmp) > 0:
-				self.entry.insert(tkinter.END, tmp)
-				self.entry.select_to(tkinter.END)
-				self.entry.icursor(tkinter.END)
-				
-		# empty clipboard
-		except tkinter.TclError:
-			pass
-			
-		self.contents.config(state='disabled')
-		self.entry.focus_set()
-		return "break"
-			
-
-################ Search End
-################ Replace Begin
-
-	def replace(self, event=None, state='replace'):
-		if self.state != 'normal':
-			self.bell()
-			return "break"
-		
-		# save cursor pos
-		try:
-			self.tabs[self.tabindex].position = self.contents.index(tkinter.INSERT)
-		
-		except tkinter.TclError:
-			pass
-		
-		self.state = state
-		self.btn_open.config(state='disabled')
-		self.btn_save.config(state='disabled')
-		self.entry.bind("<Return>", self.start_search)
-		self.bind("<Escape>", self.stop_search)
-		self.bid1 = self.contents.bind("<Control-n>", func=self.skip_bindlevel )
-		self.bid2 = self.contents.bind("<Control-p>", func=self.skip_bindlevel )
-		self.bid3 = self.contents.bind("<ButtonRelease-1>", func=self.update_curpos, add=True )
-		
-		self.title('Replace this:')
-		self.entry.delete(0, tkinter.END)
-		
-		# autofill from clipboard
-		try:
-			tmp = self.clipboard_get()
-			if 80 > len(tmp) > 0:
-				self.entry.insert(tkinter.END, tmp)
-				self.entry.select_to(tkinter.END)
-				self.entry.icursor(tkinter.END)
-	
-		except tkinter.TclError:
-			pass
-			
-		
-		self.contents.config(state='disabled')
-		self.entry.focus_set()
-		return "break"
-
-
-	def replace_all(self, event=None):
-		if self.state != 'normal':
-			self.bell()
-			return "break"
-			
-		self.replace(event, state='replace_all')
-		
-		
-	def do_single_replace(self, event=None):
-	
-		
-		# Apply normal 'Replace and proceed to next by pressing Return' -behaviour
-		c = self.contents.tag_nextrange('focus', 1.0)
-		
-		if not len(c) > 0:
-			self.show_next()
-			return 'break'
-			
-		
-		# Start of actual replacing
-		self.contents.config(state='normal')
-		self.search_matches = 0
-		
-		if self.replace_overlap_index != None:
-			
-			if self.replace_overlap_index == 0:
-				range_func = self.contents.tag_nextrange
-			
-			else:
-				range_func = self.contents.tag_prevrange
-		else:
-			range_func = self.contents.tag_prevrange
-			
-		wordlen = len(self.old_word)
-		wordlen2 = len(self.new_word)
-		pos = '1.0'
-		self.contents.tag_remove('match', '1.0', tkinter.END)
-		
-		while True:
-			pos = self.contents.search(self.old_word, pos, tkinter.END)
-			if not pos: break
-			
-			if 'replaced' in self.contents.tag_names(pos):
-				x = range_func('replaced', pos)
-				if len(x) == 0:
-					x = range_func('replaced', pos)
-				# replaced already, skip
-				pos = "%s + %dc" % ( x[1], wordlen2+1 )
-				
-			else:
-				lastpos = "%s + %dc" % (pos, wordlen)
-				self.contents.tag_add('match', pos, lastpos)
-				pos = "%s + %dc" % (pos, wordlen+1)
-				self.search_matches += 1
-			
-			
-		self.contents.tag_remove('focus', self.search_idx[0], self.search_idx[1])
-		self.contents.tag_remove('match', self.search_idx[0], self.search_idx[1])
-		self.contents.delete(self.search_idx[0], self.search_idx[1])
-		self.contents.insert(self.search_idx[0], self.new_word)
-		
-		# tag replacement to avoid rematching same place
-		p = "%s + %dc" % (self.search_idx[0], wordlen2)
-		self.contents.tag_add('replaced', self.search_idx[0], p)
-		
-		
-		self.contents.config(state='disabled')
-		
-		self.search_matches -= 1
-		
-		if self.search_matches == 0:
-			self.wait_for(100)
-			self.stop_search()
-
-	
-	def do_replace_all(self, event=None):
-		
-		self.contents.config(state='normal')
-		wordlen = len(self.old_word)
-		wordlen2 = len(self.new_word)
-		pos = '1.0'
-		
-		while True:
-			pos = self.contents.search(self.old_word, pos, tkinter.END)
-			if not pos: break
-			
-			lastpos = "%s + %dc" % ( pos, wordlen )
-			lastpos2 = "%s + %dc" % ( pos, wordlen2 )
-			
-			self.contents.delete( pos, lastpos )
-			self.contents.insert( pos, self.new_word )
-			self.contents.tag_add( 'replaced', pos, lastpos2 )
-				
-			pos = "%s + %dc" % (pos, wordlen+1)
-			
-		# show lastpos but dont put cursor on it
-		line = lastpos
-		self.wait_for(100)
-		self.ensure_idx_visibility(line)
-
-
-		self.stop_search()
-		
-		
-	def start_replace(self, event=None):
-		self.new_word = self.entry.get()
-		
-		if self.old_word == self.new_word:
-			return 'break'
-				
-		self.bind("<Control-n>", self.show_next)
-		self.bind("<Control-p>", self.show_prev)
-		
-		# prevent focus messing
-		self.entry.bind("<Return>", self.do_nothing)
-		self.entry.config(state='disabled')
-		self.focus_set()
-		
-		self.contents.tag_remove('replaced', '1.0', tkinter.END)
-		
-		
-		if self.state == 'replace':
-		
-			self.replace_overlap_index = None
-			
-			if self.old_word in self.new_word:
-				self.replace_overlap_index = self.new_word.index(self.old_word)
-				
-			self.title( f'Replace: 1/{self.search_matches}' )
-			self.bind( "<Return>", self.do_single_replace)
-			
-		elif self.state == 'replace_all':
-			self.bind( "<Return>", self.do_replace_all)
-			self.title('Replacing ALL %s matches of %s with: %s' % (str(self.search_matches), self.old_word, self.new_word) )
-			
-		return 'break'
-		
-		
-################ Replace End
-########### Class Editor End
-
+############ Stucture briefing Begin
+
+# Stucture briefing
+# TODO
+# Imports
+# Class Tab
+
+####################
+# Class Editor Begin
+#
+# Constants
+# init etc.
+# Linenumbers
+# Tab Related
+# Configuration Related
+# Syntax highlight
+# Theme Related
+# Run file Related
+# Select and move
+# Overrides
+# Utilities
+# Save and Load
+# Gotoline and Help
+# Indent and Comment
+# Search
+# Replace
+#
+# Class Editor End
+
+############ Stucture briefing End
+############ TODO Begin
+
+#
+
+############ TODO End
+############ Imports Begin
+
+# From standard library
+import tkinter.font
+import tkinter
+import pathlib
+import json
+import copy
+
+# Used in init
+import importlib.resources
+import importlib.metadata
+import sys
+
+# Used in syntax highlight
+import tokenize
+import keyword
+import io
+
+# From current directory
+from . import wordexpand
+from . import changefont
+from . import fdialog
+
+# For executing edited file in the same env than this editor, which is nice:
+# It means you have your installed dependencies available. By self.run()
+import subprocess
+
+# For making paste to work in Windows
+import threading
+		
+############ Imports End
+############ Class Tab Begin
+					
+class Tab:
+	'''	Represents a tab-page of an Editor-instance
+	'''
+	
+	def __init__(self, **entries):
+		self.active = True
+		self.filepath = None
+		self.contents = ''
+		self.oldcontents = ''
+		self.position = '1.0'
+		self.type = 'newtab'
+		
+		self.__dict__.update(entries)
+		
+		
+	def __str__(self):
+		
+		return	'\nfilepath: %s\nactive: %s\ntype: %s\nposition: %s' % (
+				str(self.filepath),
+				str(self.active),
+				self.type,
+				self.position
+				)
+				
+				
+############ Class Tab End
+############ Class Editor Begin
+
+###############################################################################
+# config(**options) Modifies one or more widget options. If no options are
+# given, method returns a dictionary containing all current option values.
+#
+# https://tcl.tk/man/tcl9.0/TkCmd/index.html
+#
+# Look in: 'text', 'event' and 'bind'
+#
+# https://docs.python.org/3/library/tkinter.html
+#
+###############################################################################
+
+############ Constants Begin
+CONFPATH = 'editor.cnf'
+ICONPATH = 'editor.png'
+HELPPATH = 'help.txt'
+HELP_MAC = 'help_mac.txt'
+
+VERSION = importlib.metadata.version(__name__)
+
+
+TAB_WIDTH = 4
+TAB_WIDTH_CHAR = 'A'
+
+SLIDER_MINSIZE = 66
+
+
+GOODFONTS = [
+			'Andale Mono',
+			'Noto Mono',
+			'Bitstream Vera Sans Mono',
+			'Liberation Mono',
+			'DejaVu Sans Mono',
+			'Inconsolata',
+			'Courier 10 Pitch',
+			'Consolas',
+			'Courier New',
+			'Noto Sans Mono',
+			'Courier'
+			]
+			
+############ Constants End
+			
+class Editor(tkinter.Toplevel):
+
+	alive = False
+	
+	pkg_contents = None
+	no_icon = True
+	pic = None
+	helptxt = None
+	
+	root = None
+	
+	mac_term = None
+	win_id = None
+	os_type = None
+	
+	if sys.platform == 'darwin': os_type = 'mac_os'
+	elif sys.platform[:3] == 'win': os_type = 'windows'
+	elif sys.platform.count('linux'): os_type = 'linux'
+	else: os_type = 'linux'
+		
+	
+	if os_type == 'mac_os':
+		# macOS: Get name of terminal App.
+		# Used to give focus back to it when closing editor, in quit_me()
+		
+		# This have to be before tkinter.tk()
+		# or we get 'Python' as appname.
+		try:
+			
+##			# With this method we get appname with single run but is still slower
+##			# than the two run method used earlier and now below:
+##			tmp = ['lsappinfo', 'metainfo']
+##			tmp = subprocess.run(tmp, check=True, capture_output=True).stdout.decode()
+##			# Returns many lines.
+##			# Line of interest is like:
+##			#bringForwardOrder = "Terminal" ASN:0x0-0x1438437:  "Safari" ASN:0x0-0x1447446:  "Python" ASN:0x0-0x1452451:  "Finder" ASN:0x0-0x1436435:
+##
+##			# Get that line
+##			tmp = tmp.partition('bringForwardOrder')[2]
+##			# Get appname from line
+##			mac_term = tmp.split(sep='"', maxsplit=2)[1]
+			
+			
+			tmp = ['lsappinfo', 'front']
+			tmp = subprocess.run(tmp, check=True, capture_output=True).stdout.decode()
+			tmp = tmp[:-1]
+			
+			tmp = ('lsappinfo info -only name %s' % tmp).split()
+			tmp = subprocess.run(tmp, check=True, capture_output=True).stdout.decode()
+			tmp = tmp[:-1]
+			mac_term = tmp.split('=')[1].strip('"')
+			
+			# Get window id in case many windows of app is open
+			tmp = ['osascript', '-e', 'id of window 1 of app "%s"' % mac_term]
+			tmp = subprocess.run(tmp, check=True, capture_output=True).stdout.decode()
+			
+			win_id = tmp[:-1]
+			del tmp
+			
+			#print(win_id)
+			#print('AAAAAAAAA', mac_term)
+		
+		except (FileNotFoundError, subprocess.SubprocessError):
+			pass
+
+	
+	def __new__(cls):
+	
+		if not cls.root:
+			#print('BBBB')
+			# Was earlier v.0.2.2 in init:
+
+			# self.root = tkinter.Tk().withdraw()
+
+			# wich worked in Debian 11, but not in Debian 12,
+			# resulted error msg like: class str has no some attribute etc.
+			# After changing this line in init to:
+
+			# self.root = tkinter.Tk()
+			# self.root.withdraw()
+
+			# Editor would launch, but after closing and reopening in the same python-console-instance,
+			# there would be same kind of messages but about icon, and also fonts would change.
+			# This is why that stuff is now here to keep those references.
+
+			cls.root = tkinter.Tk()
+			cls.root.withdraw()
+
+		
+		if not cls.pkg_contents:
+			cls.pkg_contents = importlib.resources.files(__name__)
+			
+
+		if cls.pkg_contents:
+
+			if cls.no_icon:
+				for item in cls.pkg_contents.iterdir():
+
+					if item.name == ICONPATH:
+						try:
+							cls.pic = tkinter.Image("photo", file=item)
+							cls.no_icon = False
+							break
+
+						except tkinter.TclError as e:
+							print(e)
+
+			if not cls.helptxt:
+				for item in cls.pkg_contents.iterdir():
+					
+					helpfile = HELPPATH
+					if cls.os_type == 'mac_os': helpfile = HELP_MAC
+
+					if item.name == helpfile:
+						try:
+							cls.helptxt = item.read_text()
+							break
+
+						except Exception as e:
+							print(e.__str__())
+
+
+		if cls.no_icon: print('Could not load icon-file.')
+
+
+		if not cls.alive:
+			return super(Editor, cls).__new__(cls)
+			
+		else:
+			print('Instance of ', cls, ' already running!\n')
+			
+			# By raising error the object creation is totally aborted.
+			raise ValueError()
+			
+			
+
+	def __init__(self):
+		
+		self.root = self.__class__.root
+		super().__init__(self.root, class_='Henxel', bd=4)
+		self.protocol("WM_DELETE_WINDOW", self.quit_me)
+		
+		
+		# other widgets
+		self.to_be_closed = list()
+		
+		self.ln_string = ''
+		self.want_ln = True
+		self.syntax = True
+		self.oldconf = None
+		self.tab_char = TAB_WIDTH_CHAR
+			
+		if sys.prefix != sys.base_prefix:
+			self.env = sys.prefix
+		else:
+			self.env = None
+		
+		self.tabs = list()
+		self.tabindex = None
+		self.branch = None
+		self.version = VERSION
+		self.os_type = self.__class__.os_type
+		
+		
+		self.font = tkinter.font.Font(family='TkDefaulFont', size=12, name='textfont')
+		self.menufont = tkinter.font.Font(family='TkDefaulFont', size=10, name='menufont')
+		
+		# get current git-branch
+		try:
+			self.branch = subprocess.run('git branch --show-current'.split(),
+					check=True, capture_output=True).stdout.decode().strip()
+		except Exception as e:
+			pass
+		
+		
+		# This marks range of focus-tag:
+		self.search_idx = ('1.0', '1.0')
+		
+		self.search_matches = 0
+		self.old_word = ''
+		self.new_word = ''
+		
+		self.errlines = list()
+		
+		# When clicked with mouse button 1 while searching
+		# to set cursor position to that position clicked.
+		self.save_pos = None
+		
+		# used in load()
+		self.tracevar_filename = tkinter.StringVar()
+		self.tracefunc_name = None
+		self.lastdir = None
+
+		self.check_pars = False
+		self.par_err = False
+		
+		self.waitvar = tkinter.IntVar()
+		self.fullscreen = False
+		self.state = 'normal'
+		
+		
+		self.helptxt = 'Could not load help-file. Press ESC to return.'
+		
+		if self.__class__.helptxt:
+			self.helptxt = self.__class__.helptxt
+					
+		try:
+			self.tk.call('wm','iconphoto', self._w, self.__class__.pic)
+		except tkinter.TclError as e:
+			print(e)
+		
+		
+		# Initiate widgets
+		####################################
+		self.btn_git = tkinter.Button(self, takefocus=0)
+		
+		if self.branch:
+			branch = self.branch[:5]
+			self.btn_git.config(font=self.menufont, relief='flat', highlightthickness=0,
+						padx=0, text=branch, state='disabled')
+
+			if 'main' in self.branch or 'master' in self.branch:
+				self.btn_git.config(disabledforeground='brown1')
+
+		else:
+			self.btn_git.config(font=self.menufont, relief='flat', highlightthickness=0,
+						padx=0, bitmap='info', state='disabled')
+
+		
+		self.entry = tkinter.Entry(self, bd=4, highlightthickness=0)
+		if self.os_type != 'mac_os': self.entry.config(bg='#d9d9d9')
+		self.entry.bind("<Return>", self.load)
+		
+		self.btn_open=tkinter.Button(self, takefocus=0, text='Open', bd=4, highlightthickness=0, command=self.load)
+		self.btn_save=tkinter.Button(self, takefocus=0, text='Save', bd=4, highlightthickness=0, command=self.save)
+		
+		# Get conf:
+		string_representation = None
+		data = None
+		
+		# Try to apply saved configurations:
+		if self.env:
+			p = pathlib.Path(self.env) / CONFPATH
+		
+		if self.env and p.exists():
+			try:
+				with open(p, 'r', encoding='utf-8') as f:
+					string_representation = f.read()
+					data = json.loads(string_representation)
+						
+			except EnvironmentError as e:
+				print(e.__str__())	# __str__() is for user (print to screen)
+				#print(e.__repr__())	# __repr__() is for developer (log to file)
+				print(f'\n Could not load existing configuration file: {p}')
+			
+		if data:
+			self.oldconf = string_representation
+			self.load_config(data)
+			
+		
+		self.ln_widget = tkinter.Text(self, width=4, padx=10, highlightthickness=0, bd=4, pady=4)
+		self.ln_widget.tag_config('justright', justify=tkinter.RIGHT)
+		
+		# disable copying linenumbers:
+		shortcut = '<Mod1-Key-c>'
+		if self.os_type != 'mac_os': shortcut = '<Control-c>'
+		self.ln_widget.bind(shortcut, self.no_copy_ln)
+		
+		self.contents = tkinter.Text(self, undo=True, maxundo=-1, autoseparators=True, tabstyle='wordprocessor', highlightthickness=0, bd=4, pady=4, padx=10)
+		
+		self.scrollbar = tkinter.Scrollbar(self, orient=tkinter.VERTICAL, highlightthickness=0, bd=0, command = self.contents.yview)
+
+		# tab-completion, used in tab_override()
+		self.expander = wordexpand.ExpandWord(self.contents)
+		
+		
+		# Needed in leave() taglink in: Run file Related
+		self.name_of_cursor_in_text_widget = self.contents['cursor']
+		
+		self.popup = tkinter.Menu(self.contents, tearoff=0, bd=0, activeborderwidth=0)
+		self.popup.bind("<FocusOut>", self.popup_focusOut) # to remove popup when clicked outside
+		self.popup.add_command(label="         run", command=self.run)
+		self.popup.add_command(label="        copy", command=self.copy)
+		self.popup.add_command(label="       paste", command=self.paste)
+		self.popup.add_command(label="##   comment", command=self.comment)
+		self.popup.add_command(label="   uncomment", command=self.uncomment)
+		self.popup.add_command(label="  select all", command=self.select_all)
+		self.popup.add_command(label="     inspect", command=self.insert_inspected)
+		self.popup.add_command(label="      errors", command=self.show_errors)
+		self.popup.add_command(label="        help", command=self.help)
+
+		
+		# Get anchor-name of selection-start.
+		# Used in for example select_by_words():
+		self.contents.insert(1.0, 'asd')
+		# This is needed to get some tcl-objects created,
+		# ::tcl::WordBreakRE and self.anchorname
+		self.contents.event_generate('<<SelectNextWord>>')
+		# This is needed to clear selection
+		# otherwise left at the end of file:
+		self.contents.event_generate('<<PrevLine>>')
+		
+		# Now also this array is created which is needed
+		# in RE-fixing ctrl-leftright behaviour in Windows below.
+		# self.tk.eval('parray ::tcl::WordBreakRE')
+		
+		self.anchorname = None
+		for item in self.contents.mark_names():
+			if 'tk::' in item:
+				self.anchorname = item
+				break
+		
+		self.contents.delete('1.0', '1.3')
+		
+		# In Win11 event: <<NextWord>> does not work (as supposed) but does so in Linux and macOS
+		# https://www.tcl.tk/man/tcl9.0/TclCmd/tclvars.html
+		# https://www.tcl.tk/man/tcl9.0/TclCmd/library.html
+
+		if self.os_type == 'windows':
+			
+			# To fix: replace array ::tcl::WordBreakRE contents with newer version, and
+			# replace proc tk::TextNextWord with newer version which was looked in Debian 12
+			# Need for some reason generate event: <<NextWord>> before this,
+			# because array ::tcl::WordBreakRE does not exist yet,
+			# but after this event it does. This was done above.
+
+			self.tk.eval('set l3 [list previous {\W*(\w+)\W*$} after {\w\W|\W\w} next {\w*\W+\w} end {\W*\w+\W} before {^.*(\w\W|\W\w)}] ')
+			self.tk.eval('array set ::tcl::WordBreakRE $l3 ')
+			self.tk.eval('proc tk::TextNextWord {w start} {TextNextPos $w $start tcl_endOfWord} ')
+
+		
+		if data:
+			self.apply_config()
+			
+			# Hide selection in linenumbers
+			self.ln_widget.config( selectbackground=self.bgcolor, selectforeground=self.fgcolor, inactiveselectbackground=self.bgcolor )
+			
+		
+		# Colors Begin #######################
+			
+		red = r'#c01c28'
+		cyan = r'#2aa1b3'
+		magenta = r'#a347ba'
+		green = r'#26a269'
+		orange = r'#e95b38'
+		gray = r'#508490'
+		black = r'#000000'
+		white = r'#d3d7cf'
+		
+		
+		self.default_themes = dict()
+		self.default_themes['day'] = d = dict()
+		self.default_themes['night'] = n = dict()
+		
+		# self.default_themes[self.curtheme][tagname] = [backgroundcolor, foregroundcolor]
+		d['normal_text'] = [white, black]
+		n['normal_text'] = [black, white]
+		
+		# if background is same as sel background, change
+		
+		d['keywords'] = ['', orange]
+		n['keywords'] = ['', 'deep sky blue']
+		d['numbers'] = ['', red]
+		n['numbers'] = ['', red]
+		d['bools'] = ['', magenta]
+		n['bools'] = ['', magenta]
+		d['strings'] = ['', green]
+		n['strings'] = ['', green]
+		d['comments'] = ['', gray]
+		n['comments'] = ['', gray]
+		d['calls'] = ['', cyan]
+		n['calls'] = ['', cyan]
+		d['breaks'] = ['', orange]
+		n['breaks'] = ['', orange]
+		d['selfs'] = ['', gray]
+		n['selfs'] = ['', gray]
+		
+		d['match'] = ['lightyellow', 'black']
+		n['match'] = ['lightyellow', 'black']
+		d['focus'] = ['lightgreen', 'black']
+		n['focus'] = ['lightgreen', 'black']
+		d['replaced'] = ['yellow', 'black']
+		n['replaced'] = ['yellow', 'black']
+		
+		d['mismatch'] = ['brown1', 'white']
+		n['mismatch'] = ['brown1', 'white']
+		
+		d['sel'] = ['#c3c3c3', black]
+		n['sel'] = ['#c3c3c3', black]
+		
+		
+		# if no conf:
+		if self.tabindex == None:
+		
+			self.tabindex = -1
+			self.new_tab()
+			
+			self.curtheme = 'night'
+			self.themes = copy.deepcopy(self.default_themes)
+			
+			for tagname in self.themes[self.curtheme]:
+				bg, fg = self.themes[self.curtheme][tagname][:]
+				self.contents.tag_config(tagname, background=bg, foreground=fg)
+			
+			
+			self.bgcolor, self.fgcolor = self.themes[self.curtheme]['normal_text'][:]
+			
+			
+			# Set Font Begin ##################################################
+			fontname = None
+						
+			fontfamilies = [f for f in tkinter.font.families()]
+			
+			for font in GOODFONTS:
+				if font in fontfamilies:
+					fontname = font
+					break
+					
+			if not fontname:
+				fontname = 'TkDefaulFont'
+				
+			
+			size0, size1 = 12, 10
+			# There is no font-scaling in macOS?
+			if self.os_type == 'mac_os': size0, size1 = 22, 16
+				
+				
+			# Initialize rest of configurables
+			self.font.config(family=fontname, size=size0)
+			self.menufont.config(family=fontname, size=size1)
+			
+			self.scrollbar_width, self.elementborderwidth = 16, 2
+			if self.os_type == 'linux': self.scrollbar_width, self.elementborderwidth = 30, 4
+			
+			self.scrollbar.config(width=self.scrollbar_width)
+			self.scrollbar.config(elementborderwidth=self.elementborderwidth)
+			
+			self.ind_depth = TAB_WIDTH
+			self.tab_width = self.font.measure(self.ind_depth * self.tab_char)
+			
+
+
+			# One char lenght is: self.tab_width // self.ind_depth
+			# Use this in measuring padding
+			pad_x =  self.tab_width // self.ind_depth // 3
+			pad_y = pad_x
+
+
+			self.contents.config(font=self.font, foreground=self.fgcolor,
+				background=self.bgcolor, insertbackground=self.fgcolor,
+				tabs=(self.tab_width, ), padx=pad_x, pady=pad_y)
+				
+			self.entry.config(font=self.menufont)
+			self.btn_open.config(font=self.menufont)
+			self.btn_save.config(font=self.menufont)
+			self.popup.config(font=self.menufont)
+			
+			self.btn_git.config(font=self.menufont)
+			
+			self.ln_widget.config(font=self.font, foreground=self.fgcolor, background=self.bgcolor, selectbackground=self.bgcolor, selectforeground=self.fgcolor, inactiveselectbackground=self.bgcolor, state='disabled', padx=pad_x, pady=pad_y)
+
+		
+		# Widgets are initiated, now more configuration
+		################################################
+		# Needed in update_linenums(), there is more info.
+		self.update_idletasks()
+		# if self.y_extra_offset > 0, it needs attention
+		self.y_extra_offset = self.contents['highlightthickness'] + self.contents['bd'] + self.contents['pady']
+		# Needed in update_linenums() and sbset_override()
+		self.bbox_height = self.contents.bbox('@0,0')[3]
+		self.text_widget_height = self.scrollbar.winfo_height()
+				
+		self.contents['yscrollcommand'] = lambda *args: self.sbset_override(*args)
+		
+		
+		
+		
+		# Bindigs Begin
+		####################################################
+		self.right_mousebutton_num = 3
+		
+		if self.os_type == 'mac_os':
+			self.right_mousebutton_num = 2
+			
+			# Default cmd-q does not trigger quit_me
+			# Override Cmd-Q:
+			# https://www.tcl.tk/man/tcl8.6/TkCmd/tk_mac.html
+			self.root.createcommand("tk::mac::Quit", self.quit_me)
+			#self.root.createcommand("tk::mac::OnHide", self.test_hide)
+				
+		self.contents.bind( "<Button-%i>" % self.right_mousebutton_num, self.raise_popup)
+		
+		
+		if self.os_type == 'windows':
+			# fix copying to clipboard in Windows.
+			self.bind( "<Control-c>", self.copy_windows)
+		
+		
+		if self.os_type == 'linux':
+			self.contents.bind( "<ISO_Left_Tab>", self.unindent)
+		
+		
+		############################################################
+		# In macOS all Alt-shortcuts makes some special symbol.
+		# Have to bind to this symbol-name to get Alt-shorcuts work.
+		# For example binding to Alt-f:
+		# self.contents.bind( "<function>", self.font_choose)
+		
+		# Except that tkinter does not give all symbol names, like
+		# Alt-x or l
+		# which makes these key-combinations quite unbindable.
+		# It would be much easier if one could do bindings normally:
+		# Alt-SomeKey
+		# like in Linux and Windows.
+		
+		# Also binding to combinations which has Command-key (apple-key)
+		# (or Meta-key as reported by events.py)
+		# must use Mod1-Key as modifier name:
+		# Mod1-Key-n == Command-Key-n
+		
+		# fn-key -bindings have to be done by checking the state of the event
+		# in proxy-callback: mac_cmd_overrides
+		
+		# In short, In macOS one can not just bind like:
+		# Command-n
+		# fn-f
+		# Alt-f
+		
+		# This is the reason why below is some extra
+		# and strange looking binding-lines when using macOS.
+		##############################################################
+		if self.os_type != 'mac_os':
+			
+			self.bind( "<Alt-n>", self.new_tab)
+			self.bind( "<Control-q>", self.quit_me)
+			self.contents.bind( "<Alt-s>", self.color_choose)
+			self.contents.bind( "<Alt-t>", self.toggle_color)
+			
+			self.bind( "<Alt-w>", self.walk_tabs)
+			self.bind( "<Alt-q>", lambda event: self.walk_tabs(event, **{'back':True}) )
+			
+			self.contents.bind( "<Alt-Return>", lambda event: self.btn_open.invoke())
+			self.contents.bind( "<Alt-l>", self.toggle_ln)
+			self.contents.bind( "<Alt-x>", self.toggle_syntax)
+			self.contents.bind( "<Alt-f>", self.font_choose)
+		
+			self.contents.bind( "<Control-v>", self.paste)
+			self.contents.bind( "<Control-y>", self.yank_line)
+			
+			self.contents.bind( "<Control-Left>", self.move_by_words)
+			self.contents.bind( "<Control-Right>", self.move_by_words)
+			self.contents.bind( "<Control-Shift-Left>", self.select_by_words)
+			self.contents.bind( "<Control-Shift-Right>", self.select_by_words)
+			
+			self.contents.bind( "<Control-Up>", self.move_many_lines)
+			self.contents.bind( "<Control-Down>", self.move_many_lines)
+			self.contents.bind( "<Control-Shift-Up>", self.move_many_lines)
+			self.contents.bind( "<Control-Shift-Down>", self.move_many_lines)
+			
+			# Used in check_next_event
+			self.bid_left = self.contents.bind("<Left>", self.check_sel)
+			
+			self.contents.bind("<Right>", self.check_sel)
+			self.entry.bind("<Left>", self.check_sel)
+			self.entry.bind("<Right>", self.check_sel)
+		
+		
+		#self.os_type == 'mac_os':
+		else:
+			# Used in check_next_event
+			self.bid_left = self.contents.bind( "<Left>", self.mac_cmd_overrides)
+			
+			self.contents.bind( "<Right>", self.mac_cmd_overrides)
+			
+			
+			self.contents.bind( "<Up>", self.mac_cmd_overrides)
+			self.contents.bind( "<Down>", self.mac_cmd_overrides)
+			
+			self.entry.bind( "<Right>", self.mac_cmd_overrides)
+			self.entry.bind( "<Left>", self.mac_cmd_overrides)
+			
+			self.contents.bind( "<f>", self.mac_cmd_overrides)		# + fn full screen
+			
+			# Have to bind using Mod1 as modifier name if want bind to Command-key,
+			# Last line is the only one working:
+			#self.contents.bind( "<Meta-Key-k>", lambda event, arg=('AAA'): print(arg) )
+			#self.contents.bind( "<Command-Key-k>", lambda event, arg=('AAA'): print(arg) )
+			#self.contents.bind( "<Mod1-Key-k>", lambda event, arg=('AAA'): print(arg) )
+			
+			
+			self.contents.bind( "<Mod1-Key-y>", self.yank_line)
+			self.contents.bind( "<Mod1-Key-n>", self.new_tab)
+			self.contents.bind( "<Mod1-Key-f>", self.search)
+			self.contents.bind( "<Mod1-Key-v>", self.paste)
+			self.contents.bind( "<Mod1-Key-R>", self.replace_all)
+			self.contents.bind( "<Mod1-Key-g>", self.gotoline)
+			self.contents.bind( "<Mod1-Key-a>", self.goto_linestart)
+			self.contents.bind( "<Mod1-Key-e>", self.goto_lineend)
+			self.entry.bind( "<Mod1-Key-a>", self.goto_linestart)
+			self.entry.bind( "<Mod1-Key-e>", self.goto_lineend)
+			self.contents.bind( "<Mod1-Key-r>", self.replace)
+			self.contents.bind( "<Mod1-Key-z>", self.undo_override)
+			self.contents.bind( "<Mod1-Key-Z>", self.redo_override)
+			
+			# Could not get keysym for Alt-l and x, so use ctrl
+			self.contents.bind( "<Control-l>", self.toggle_ln)
+			self.contents.bind( "<Control-x>", self.toggle_syntax)
+			
+			self.contents.bind( "<Shift-Tab>", self.unindent)
+			
+			# have to bind to symbol name to get Alt-shorcuts work in macOS
+			# This is: Alt-f
+			self.contents.bind( "<function>", self.font_choose)		# Alt-f
+			self.contents.bind( "<dagger>", self.toggle_color)		# Alt-t
+			self.contents.bind( "<ssharp>", self.color_choose)		# Alt-s
+			
+			
+		#######################################################
+		
+		
+		self.bind( "<Control-R>", self.replace_all)
+		self.bind( "<Control-g>", self.gotoline)
+		self.bind( "<Control-r>", self.replace)
+
+		self.bind( "<Escape>", self.do_nothing )
+		self.bind( "<Return>", self.do_nothing)
+		self.bind( "<Control-minus>", self.decrease_scrollbar_width)
+		self.bind( "<Control-plus>", self.increase_scrollbar_width)
+		
+		# If accidentally pressed too early when searching:
+		self.entry.bind("<Control-n>", self.do_nothing_without_bell)
+		self.entry.bind("<Control-p>", self.do_nothing_without_bell)
+		self.ln_widget.bind("<Control-n>", self.do_nothing_without_bell)
+		self.ln_widget.bind("<Control-p>", self.do_nothing_without_bell)
+		
+		self.contents.bind( "<Control-a>", self.goto_linestart)
+		self.contents.bind( "<Control-e>", self.goto_lineend)
+		self.contents.bind( "<Control-A>", self.goto_linestart)
+		self.contents.bind( "<Control-E>", self.goto_lineend)
+		
+		if self.os_type == 'windows':
+			self.entry.bind( "<Control-E>", lambda event, arg=('<<SelectLineEnd>>'): self.entry.event_generate)
+			self.entry.bind( "<Control-A>", lambda event, arg=('<<SelectLineStart>>'): self.entry.event_generate)
+		
+		self.contents.bind( "<Control-i>", self.move_right)
+		self.contents.bind( "<Control-b>", self.move_left)
+		self.contents.bind( "<Control-n>", self.move_down)
+		self.contents.bind( "<Control-p>", self.move_up)
+		
+		self.contents.bind( "<Control-j>", self.center_view)
+		self.contents.bind( "<Control-u>", lambda event: self.center_view(event, **{'up':True}) )
+		
+		self.contents.bind( "<Return>", self.return_override)
+		
+		self.contents.bind( "<Control-d>", self.del_tab)
+		self.contents.bind( "<Control-Q>", lambda event: self.del_tab(event, **{'save':False}) )
+		
+		self.contents.bind( "<Shift-Return>", self.comment)
+		self.contents.bind( "<Shift-BackSpace>", self.uncomment)
+		self.contents.bind( "<Tab>", self.tab_override)
+		
+		self.contents.bind( "<Control-t>", self.tabify_lines)
+		self.contents.bind( "<Control-z>", self.undo_override)
+		self.contents.bind( "<Control-Z>", self.redo_override)
+		self.contents.bind( "<Control-f>", self.search)
+		
+		self.contents.bind( "<BackSpace>", self.backspace_override)
+		self.contents.bind( "<Control-BackSpace>", self.search_next)
+		
+		
+##		# this move_line interferes with search_next,check_nextevent, so not in use
+##		self.contents.bind("<Left>", lambda event: self.move_line(event, **{'direction':'left'} ))
+##		self.contents.bind("<Right>", lambda event: self.move_line(event, **{'direction':'right'} ))
+##
+##		# updown_override not in use
+##		self.contents.bind("<Up>", lambda event: self.updown_override(event, **{'direction':'up'} ))
+##		self.contents.bind("<Down>", lambda event: self.updown_override(event, **{'direction':'down'} ))
+		
+		
+		# Unbind some default bindings
+		# Paragraph-bindings: too easy to press by accident
+		self.contents.unbind_class('Text', '<<NextPara>>')
+		self.contents.unbind_class('Text', '<<PrevPara>>')
+		self.contents.unbind_class('Text', '<<SelectNextPara>>')
+		self.contents.unbind_class('Text', '<<SelectPrevPara>>')
+		
+		# LineStart and -End:
+		# fix goto_linestart-end and
+		# enable tab-walking in mac_os with cmd-left-right
+		self.contents.unbind_class('Text', '<<LineStart>>')
+		self.contents.unbind_class('Text', '<<LineEnd>>')
+		self.contents.unbind_class('Text', '<<SelectLineEnd>>')
+		self.contents.unbind_class('Text', '<<SelectLineStart>>')
+		
+		
+		# Register validation-functions, note the tuple-syntax:
+		self.validate_gotoline = (self.register(self.do_validate_gotoline), '%i', '%S', '%P')
+		self.validate_search = (self.register(self.do_validate_search), '%i', '%s', '%S')
+		
+		
+		self.helptxt = f'{self.helptxt}\n\nHenxel v. {self.version}'
+		
+		# Widgets are configured
+		###############################
+		#
+		# Syntax-highlight Begin #################
+		self.keywords = keyword.kwlist
+		self.keywords.insert(0, 'self')
+		
+		self.bools = [ 'False', 'True', 'None' ]
+		self.breaks = [
+						'break',
+						'return',
+						'continue',
+						'pass',
+						'raise',
+						'assert',
+						'yield'
+						]
+						
+		self.tests = [
+					'not',
+					'or',
+					'and',
+					'in',
+					'as'
+					]
+		
+		self.tagnames = [
+				'keywords',
+				'numbers',
+				'bools',
+				'strings',
+				'comments',
+				'breaks',
+				'calls',
+				'selfs'
+				]
+		
+		
+		self.boldfont = self.font.copy()
+		self.boldfont.config(weight='bold')
+		
+		self.contents.tag_config('keywords', font=self.boldfont)
+		self.contents.tag_config('numbers', font=self.boldfont)
+		self.contents.tag_config('comments', font=self.boldfont)
+		self.contents.tag_config('breaks', font=self.boldfont)
+		self.contents.tag_config('calls', font=self.boldfont)
+
+		# search tags have highest priority
+		self.contents.tag_raise('match')
+		self.contents.tag_raise('replaced')
+		self.contents.tag_raise('sel')
+		self.contents.tag_raise('focus')
+		
+		
+		self.oldline = ''
+		self.token_err = False
+		self.token_can_update = False
+		self.oldlinenum = self.contents.index(tkinter.INSERT).split('.')[0]
+		
+		self.do_syntax(everything=True)
+			
+		self.contents.bind( "<<WidgetViewSync>>", self.viewsync)
+		# Viewsync-event does not trigger at window size changes,
+		# to get linenumbers right, we bind to this:
+		self.contents.bind("<Configure>", self.handle_configure)
+		
+		
+		####  Syntax-highlight End  ######################################
+		
+		# Layout Begin
+		################################
+		self.rowconfigure(1, weight=1)
+		self.columnconfigure(1, weight=1)
+		
+		# It seems that widget is shown on screen when doing grid_configure
+		self.btn_git.grid_configure(row=0, column = 0, sticky='nsew')
+		self.entry.grid_configure(row=0, column = 1, sticky='nsew')
+		self.btn_open.grid_configure(row=0, column = 2, sticky='nsew')
+		self.btn_save.grid_configure(row=0, column = 3, columnspan=2, sticky='nsew')
+		
+		
+		self.ln_widget.grid_configure(row=1, column = 0, sticky='nswe')
+			
+		# If want linenumbers:
+		if self.want_ln:
+			self.contents.grid_configure(row=1, column=1, columnspan=3, sticky='nswe')
+		
+		else:
+			self.contents.grid_configure(row=1, column=0, columnspan=4, sticky='nswe')
+			self.ln_widget.grid_remove()
+			
+		self.scrollbar.grid_configure(row=1,column=4, sticky='nse')
+
+		
+		# set cursor pos:
+		line = self.tabs[self.tabindex].position
+		
+		if self.os_type == 'windows':
+			self.contents.focus_force()
+		else:
+			self.contents.focus_set()
+		
+		
+		try:
+			self.contents.mark_set('insert', line)
+			self.ensure_idx_visibility(line)
+			
+		except tkinter.TclError:
+			self.contents.mark_set('insert', '1.0')
+			self.tabs[self.tabindex].position = '1.0'
+			self.contents.see('1.0')
+				
+		
+		self.avoid_viewsync_mess()
+		self.update_idletasks()
+		self.viewsync()
+		self.__class__.alive = True
+		self.update_title()
+		
+		############################# init End ##########################
+		
+	
+	def update_title(self, event=None):
+		tail = len(self.tabs) - self.tabindex - 1
+		self.title( f'Henxel {"0"*self.tabindex}@{"0"*(tail)}' )
+		
+	
+	def handle_configure(self, event=None):
+		'''	In case of size change, like maximize etc. viewsync-event is not
+			generated in such situation so need to bind to <Configure>-event.
+		'''
+		# Handle fullscreen toggles
+		self.update_idletasks()
+		
+		if self.wm_attributes('-fullscreen') == 1:
+			if self.fullscreen == False:
+				#print('normal --> full  config')
+				self.fullscreen = True
+		else:
+			if self.fullscreen == True:
+				#print('full --> normal  config')
+				self.fullscreen = False
+				
+		
+		self.text_widget_height = self.scrollbar.winfo_height()
+		self.update_linenums()
+		
+	
+	def copy_windows(self, event=None):
+		
+		
+		try:
+			#self.clipboard_clear()
+			tmp = self.selection_get()
+			
+			
+			# https://stackoverflow.com/questions/51921386
+			# pyperclip approach works in windows fine
+			# import clipboard as cb
+			# cb.copy(tmp)
+			
+			# os.system approach also works but freezes editor for a little time
+			
+			
+			d = dict()
+			d['input'] = tmp.encode('ascii')
+			
+			t = threading.Thread( target=subprocess.run, args=('clip',), kwargs=d, daemon=True )
+			#t.setDeamon(True)
+			t.start()
+			
+				
+			#self.clipboard_append(tmp)
+		except tkinter.TclError:
+			# is empty
+			return 'break'
+			
+			
+		#print(#self.clipboard_get())
+		return 'break'
+		
+	
+	def wait_for(self, ms):
+		# This is important, 'cancel' all bindings which checks the state.
+		state = self.state
+		self.state = 'waiting'
+		
+		self.waitvar.set(False)
+		self.after(ms, self.waiter)
+		self.wait_variable(self.waitvar)
+		
+		# 'Release' bindings
+		self.state = state
+		
+	
+	def waiter(self):
+		self.waitvar.set(True)
+		
+	
+	def do_nothing(self, event=None):
+		self.bell()
+		return 'break'
+		
+	
+	def do_nothing_without_bell(self, event=None):
+		return 'break'
+	
+	
+	def test_bind(self, event=None):
+		print('jou')
+	
+	
+	def skip_bindlevel(self, event=None):
+		return 'continue'
+		
+	
+	def ensure_idx_visibility(self, index, back=None):
+		b=2
+		if back:
+			b=back
+			
+		self.contents.mark_set('insert', index)
+		s = self.contents.bbox('%s - %ilines' % (index,b))
+		e = self.contents.bbox('%s + 4lines' % index)
+		
+		tests = [
+				not s,
+				not e,
+				( s and s[1] < 0 )
+				]
+				
+		if any(tests):
+			self.contents.see('%s - %ilines' % (index,b))
+			self.update_idletasks()
+			self.contents.see('%s + 4lines' % index)
+		
+		
+	def quit_me(self, event=None):
+	
+		self.save(forced=True)
+		self.save_config()
+		
+		# affects color, fontchoose, load:
+		for widget in self.to_be_closed:
+			widget.destroy()
+		
+		self.quit()
+		self.destroy()
+		
+		
+		# Activate terminal
+		if self.os_type == 'mac_os':
+		
+			# This osascript-language is funny
+			# https://ss64.com/osx/osascript.html
+			
+			mac_term = 'Terminal'
+			
+			
+			
+			try:
+				# Giving focus back to python terminal-window is not very simple task in macOS
+				# https://apple.stackexchange.com/questions/421137
+				tmp = None
+				if self.__class__.mac_term and self.__class__.win_id:
+					mac_term = self.__class__.mac_term
+					win_id  = self.__class__.win_id
+
+					
+					if mac_term == 'iTerm2':
+						tmp = [ 'osascript', '-e', 'tell app "%s" to select windows whose id = %s' % (mac_term, win_id), '-e', 'tell app "%s" to activate' % mac_term ]
+						
+					else:
+						tmp = [ 'osascript', '-e', 'tell app "%s" to set frontmost of windows whose id = %s to true' % (mac_term, win_id), '-e', 'tell app "%s" to activate' % mac_term ]
+
+
+
+
+				elif self.__class__.mac_term:
+					mac_term = self.__class__.mac_term
+					tmp = ['osascript', '-e', 'tell app "%s" to activate' % mac_term ]
+
+				else:
+					tmp = ['osascript', '-e', 'tell app "%s" to activate' % mac_term ]
+
+				subprocess.run(tmp)
+
+
+			except (FileNotFoundError, subprocess.SubprocessError):
+				pass
+			
+			# No need to put in thread
+			#t = threading.Thread( target=subprocess.run, args=(tmp,), daemon=True )
+			#t.start()
+			
+		
+		if self.tracefunc_name:
+			self.tracevar_filename.trace_remove('write', self.tracefunc_name)
+		
+		del self.font
+		del self.menufont
+		del self.boldfont
+		
+		# this is maybe not necessary
+		del self.entry
+		del self.btn_open
+		del self.btn_save
+		del self.btn_git
+		del self.contents
+		del self.ln_widget
+		del self.scrollbar
+		del self.popup
+				
+		self.__class__.alive = False
+		
+	
+	def avoid_viewsync_mess(self, event=None):
+		# Avoid viewsync messing when cursor
+		# position is in line with multiline string marker:
+		
+		if self.tabs[self.tabindex].filepath:
+			if self.can_do_syntax():
+				pos = self.tabs[self.tabindex].position
+				lineend = '%s lineend' % pos
+				linestart = '%s linestart' % pos
+				tmp = self.contents.get( linestart, lineend )
+				self.oldline = tmp
+				self.oldlinenum = pos.split('.')[0]
+				self.token_can_update = True
+
+
+	def viewsync(self, event=None):
+		'''	Triggered when event is <<WidgetViewSync>>
+			Used to update linenumbers and syntax highlight.
+		
+			This event itself is generated *after* when inserting, deleting or on screen geometry change, but
+			not when just scrolling (like yview). Almost all font-changes also generates this event.
+		'''
+		# More info in update_linenums()
+		self.bbox_height = self.contents.bbox('@0,0')[3]
+		self.text_widget_height = self.scrollbar.winfo_height()
+		self.update_linenums()
+		
+		if self.tabs[self.tabindex].filepath:
+			if self.can_do_syntax():
+				if self.token_can_update:
+				
+					#  tag alter triggers this event if font changes, like from normal to bold.
+					# --> need to check if line is changed to prevent self-trigger
+					line_idx = self.contents.index( tkinter.INSERT )
+					linenum = line_idx.split('.')[0]
+					#prev_char = self.contents.get( '%s - 1c' % tkinter.INSERT )
+					
+					
+					lineend = '%s lineend' % line_idx
+					linestart = '%s linestart' % line_idx
+					
+					tmp = self.contents.get( linestart, lineend )
+					
+					if self.oldline != tmp or self.oldlinenum != linenum:
+					
+						#print('sync')
+						self.oldline = tmp
+						self.oldlinenum = linenum
+						self.update_tokens(start=linestart, end=lineend, line=tmp)
+				
+
+############## Linenumbers Begin
+
+	def no_copy_ln(self, event=None):
+		return 'break'
+		
+	
+	def toggle_ln(self, event=None):
+		
+		# if dont want linenumbers:
+		if self.want_ln:
+			# remove remembers grid-options
+			self.ln_widget.grid_remove()
+			self.contents.grid_configure(column=0, columnspan=4)
+			self.want_ln = False
+		else:
+			self.contents.grid_configure(column=1, columnspan=3)
+			self.ln_widget.grid()
+			
+			self.want_ln = True
+		
+		return 'break'
+		
+	
+	def get_linenums(self):
+
+		x = 0
+		line = '0'
+		col= ''
+		ln = ''
+
+		# line-height is used as step, it depends on font:
+		step = self.bbox_height
+
+		nl = '\n'
+		lineMask = '%s\n'
+		
+		# @x,y is tkinter text-index -notation:
+		# The character that covers the (x,y) -coordinate within the text's window.
+		indexMask = '@0,%d'
+		
+		# stepping lineheight at time, checking index of each lines first cell, and splitting it.
+		
+		for i in range(0, self.text_widget_height, step):
+
+			ll, cc = self.contents.index( indexMask % i).split('.')
+
+			if line == ll:
+				# is the line wrapping:
+				if col != cc:
+					col = cc
+					ln += nl
+			else:
+				line, col = ll, cc
+				# -5: show up to four smallest number (0-9999)
+				# then starts again from 0 (when actually 10000)
+				ln += (lineMask % line)[-5:]
+				
+		return ln
+
+	
+	def update_linenums(self):
+
+		# self.ln_widget is linenumber-widget,
+		# self.ln_string is string which holds the linenumbers in self.ln_widget
+		tt = self.ln_widget
+		ln = self.get_linenums()
+		
+		if self.ln_string != ln:
+			self.ln_string = ln
+			
+			# 1 - 3 : adjust linenumber-lines with text-lines
+			
+			# 1:
+			# @0,0 is currently visible first character at
+			# x=0 y=0 in text-widget.
+			
+			# 2: bbox returns this kind of tuple: (3, -9, 19, 38)
+			# (bbox is cell that holds a character)
+			# (x-offset, y-offset, width, height) in pixels
+			# Want y-offset of first visible line, and reverse it:
+			
+			y_offset = self.contents.bbox('@0,0')[1]
+			
+			y_offset *= -1
+			
+			#if self.y_extra_offset > 0, we need this:
+			if y_offset != 0:
+				y_offset += self.y_extra_offset
+				
+			tt.config(state='normal')
+			tt.delete('1.0', tkinter.END)
+			tt.insert('1.0', self.ln_string)
+			tt.tag_add('justright', '1.0', tkinter.END)
+			
+			# 3: Then scroll lineswidget same amount to fix offset
+			# compared to text-widget:
+			tt.yview_scroll(y_offset, 'pixels')
+
+			tt.config(state='disabled')
+
+		
+############## Linenumbers End
+############## Tab Related Begin
+
+	
+	def mac_cmd_overrides(self, event=None):
+		'''	Used to catch key-combinations like Alt-shift-Right
+			in macOS, which are difficult to bind.
+		'''
+		
+		
+		# Pressed Cmd + Shift + arrow left or right.
+		# Want: select line from cursor.
+		
+		# Pressed Cmd + Shift + arrow up or down.
+		# Want: select 10 lines from cursor.
+		if event.state == 105:
+		
+			# self.contents or self.entry
+			wid = event.widget
+			
+			# Enable select from in entry
+			if wid == self.entry:
+				return
+			
+			# Enable select from in contents
+			elif wid == self.contents:
+				
+				if event.keysym == 'Right':
+					self.goto_lineend(event=event)
+					
+				elif event.keysym == 'Left':
+					self.goto_linestart(event=event)
+					
+				elif event.keysym == 'Up':
+					for i in range(10):
+						self.contents.event_generate('<<SelectPrevLine>>')
+				
+				elif event.keysym == 'Down':
+					for i in range(10):
+						self.contents.event_generate('<<SelectNextLine>>')
+					
+				else:
+					return
+			
+			return 'break'
+		
+		
+		# Pressed Cmd + arrow left or right.
+		# Want: walk tabs.
+		
+		# Pressed Cmd + arrow up or down.
+		# Want: move cursor 10 lines from cursor.
+		elif event.state == 104:
+	
+			if event.keysym == 'Right':
+				self.walk_tabs(event=event)
+				
+			elif event.keysym == 'Left':
+				self.walk_tabs(event=event, **{'back':True})
+	
+			elif event.keysym == 'Up':
+					for i in range(10):
+						self.contents.event_generate('<<PrevLine>>')
+				
+			elif event.keysym == 'Down':
+				for i in range(10):
+					self.contents.event_generate('<<NextLine>>')
+				
+			else:
+				return
+			
+			return 'break'
+			
+			
+		# Pressed Alt + arrow left or right.
+		elif event.state == 112:
+			
+			if event.keysym in ['Up', 'Down']: return
+			
+			# self.contents or self.entry
+			wid = event.widget
+			
+			if wid == self.entry:
+				
+				if event.keysym == 'Right':
+					self.entry.event_generate('<<NextWord>>')
+					
+				elif event.keysym == 'Left':
+					self.entry.event_generate('<<PrevWord>>')
+					
+				else:
+					return
+		
+			else:
+				res = self.move_by_words(event=event)
+				return res
+			
+			return 'break'
+		
+		
+		# Pressed Alt + Shift + arrow left or right.
+		elif event.state == 113:
+		
+			if event.keysym in ['Up', 'Down']: return
+			
+			# self.contents or self.entry
+			wid = event.widget
+			
+			if wid == self.entry:
+				
+				if event.keysym == 'Right':
+					self.entry.event_generate('<<SelectNextWord>>')
+					
+				elif event.keysym == 'Left':
+					self.entry.event_generate('<<SelectPrevWord>>')
+					
+				else:
+					return
+		
+			else:
+				res = self.select_by_words(event=event)
+				return res
+				
+			return 'break'
+			
+			
+		# Pressed arrow left or right.
+		# If have selection, put cursor on the wanted side of selection.
+		# +shift: 97
+		
+		# Pressed arrow up or down: return event.
+		elif event.state == 97: return
+		
+		elif event.state == 96:
+			
+			if event.keysym in ['Up', 'Down']: return
+				
+			# self.contents or self.entry
+			wid = event.widget
+			have_selection = False
+
+			if wid == self.entry:
+				have_selection = self.entry.selection_present()
+
+			elif wid == self.contents:
+				have_selection = len(self.contents.tag_ranges('sel')) > 0
+
+			else:
+				return
+
+			if have_selection:
+				if event.keysym == 'Right':
+					self.check_sel(event=event)
+						
+				elif event.keysym == 'Left':
+					self.check_sel(event=event)
+					
+				else:
+					return
+				
+			else:
+				return
+				
+			return 'break'
+			
+		
+		# Pressed Fn
+		elif event.state == 64:
+
+			# fullscreen
+			if event.keysym == 'f':
+				# prevent inserting 'f' when doing fn-f:
+				return 'break'
+
+			# Some shortcuts does not insert.
+			# Like fn-h does not insert h.
+			else:
+				return
+				
+		return
+	
+	
+	def new_tab(self, event=None, error=False):
+	
+		# event == None when clicked hyper-link in tag_link()
+		if self.state != 'normal' and event != None:
+			self.bell()
+			return 'break'
+		
+		
+		
+		if len(self.tabs) > 0  and not error:
+			try:
+				pos = self.contents.index(tkinter.INSERT)
+				
+			except tkinter.TclError:
+				pos = '1.0'
+				
+			self.tabs[self.tabindex].position = pos
+			
+			tmp = self.contents.get('1.0', tkinter.END)
+			# [:-1]: remove unwanted extra newline
+			self.tabs[self.tabindex].contents = tmp[:-1]
+			
+			
+		self.contents.delete('1.0', tkinter.END)
+		self.entry.delete(0, tkinter.END)
+		
+		if len(self.tabs) > 0:
+			self.tabs[self.tabindex].active = False
+			
+		newtab = Tab()
+		
+		self.tabindex += 1
+		self.tabs.insert(self.tabindex, newtab)
+		
+		self.contents.focus_set()
+		self.contents.see('1.0')
+		self.contents.mark_set('insert', '1.0')
+		
+		self.contents.edit_reset()
+		self.contents.edit_modified(0)
+		
+		self.update_title()
+		return 'break'
+		
+		
+	def del_tab(self, event=None, save=True):
+
+		if self.state != 'normal':
+			self.bell()
+			return 'break'
+			
+		if ((len(self.tabs) == 1) and self.tabs[self.tabindex].type == 'newtab'):
+			self.contents.delete('1.0', tkinter.END)
+			self.bell()
+			return 'break'
+
+		if self.tabs[self.tabindex].type == 'normal' and save:
+			self.save(activetab=True)
+			
+		self.tabs.pop(self.tabindex)
+			
+		if (len(self.tabs) == 0):
+			newtab = Tab()
+			self.tabs.append(newtab)
+	
+		if self.tabindex > 0:
+			self.tabindex -= 1
+	
+		self.tabs[self.tabindex].active = True
+		self.entry.delete(0, tkinter.END)
+		
+		if self.tabs[self.tabindex].filepath:
+			self.entry.insert(0, self.tabs[self.tabindex].filepath)
+			self.entry.xview_moveto(1.0)
+			
+		
+		self.contents.delete('1.0', tkinter.END)
+		self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
+		
+		
+		self.do_syntax(everything=True)
+		
+		# set cursor pos
+		line = self.tabs[self.tabindex].position
+		self.contents.focus_set()
+		
+		try:
+			self.contents.mark_set('insert', line)
+			self.ensure_idx_visibility(line)
+			
+		except tkinter.TclError:
+			self.contents.mark_set('insert', '1.0')
+			self.tabs[self.tabindex].position = '1.0'
+			self.contents.see('1.0')
+		
+			
+		self.contents.edit_reset()
+		self.contents.edit_modified(0)
+		
+		self.avoid_viewsync_mess()
+		self.update_title()
+		
+		return 'break'
+
+		
+	def walk_tabs(self, event=None, back=False):
+	
+		if self.state != 'normal' or len(self.tabs) < 2:
+			self.bell()
+			return "break"
+		
+		
+		self.tabs[self.tabindex].active = False
+		
+		try:
+			pos = self.contents.index(tkinter.INSERT)
+		except tkinter.TclError:
+			pos = '1.0'
+		
+		self.tabs[self.tabindex].position = pos
+			
+		tmp = self.contents.get('1.0', tkinter.END)
+		# [:-1]: remove unwanted extra newline
+		self.tabs[self.tabindex].contents = tmp[:-1]
+			
+		idx = self.tabindex
+		
+		if back:
+			if idx == 0:
+				idx = len(self.tabs)
+			idx -= 1
+			
+		else:
+			if idx == len(self.tabs) - 1:
+				idx = -1
+			idx += 1
+		
+		self.tabindex = idx
+		self.tabs[self.tabindex].active = True
+		self.entry.delete(0, tkinter.END)
+
+
+		if self.tabs[self.tabindex].filepath:
+			self.entry.insert(0, self.tabs[self.tabindex].filepath)
+			self.entry.xview_moveto(1.0)
+		
+		self.token_can_update = False
+		self.contents.delete('1.0', tkinter.END)
+		self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
+	
+		if self.tabs[self.tabindex].filepath:
+			if self.can_do_syntax():
+				self.update_tokens(start='1.0', end=tkinter.END, everything=True)
+
+		# set cursor pos
+		line = self.tabs[self.tabindex].position
+		self.contents.focus_set()
+		
+		try:
+			self.contents.mark_set('insert', line)
+			self.ensure_idx_visibility(line)
+			
+		except tkinter.TclError:
+			self.contents.mark_set('insert', '1.0')
+			self.tabs[self.tabindex].position = '1.0'
+			self.contents.see('1.0')
+
+		
+		self.contents.edit_reset()
+		self.contents.edit_modified(0)
+		
+		self.avoid_viewsync_mess()
+		self.update_title()
+		
+		return 'break'
+
+########## Tab Related End
+########## Configuration Related Begin
+
+	def save_config(self, event=None):
+		data = self.get_config()
+		
+		string_representation = json.dumps(data)
+		
+		if string_representation == self.oldconf:
+			return
+			
+		if self.env:
+			p = pathlib.Path(self.env) / CONFPATH
+			try:
+				with open(p, 'w', encoding='utf-8') as f:
+					f.write(string_representation)
+			except EnvironmentError as e:
+				print(e.__str__())
+				print('\nCould not save configuration')
+		else:
+			print('\nNot saving configuration when not in venv.')
+		
+	
+	def load_config(self, data):
+		
+		font, menufont = self.fonts_exists(data)
+		self.set_config(data, font, menufont)
+		
+	
+	def fonts_exists(self, dictionary):
+		
+		res = True
+		fontfamilies = [f for f in tkinter.font.families()]
+		
+		font = dictionary['font']['family']
+		
+		if font not in fontfamilies:
+			print(f'Font {font.upper()} does not exist.')
+			font = False
+		
+		menufont = dictionary['menufont']['family']
+		
+		if dictionary['menufont']['family'] not in fontfamilies:
+			print(f'Font {menufont.upper()} does not exist.')
+			menufont = False
+			
+		return font, menufont
+		
+		
+	def get_config(self):
+		dictionary = dict()
+		dictionary['curtheme'] = self.curtheme
+		dictionary['lastdir'] = self.lastdir.__str__()
+		
+		# Replace possible Tkdefaulfont as family with real name,
+		# if not mac_os, because tkinter.font.Font does not recognise
+		# this: .APPLESYSTEMUIFONT
+
+		if self.os_type == 'mac_os':
+		
+			if self.font.cget('family') == 'TkDefaulFont':
+				dictionary['font'] = self.font.config()
+				
+			else:
+				dictionary['font'] = self.font.actual()
+				
+			if self.menufont.cget('family') == 'TkDefaulFont':
+				dictionary['menufont'] = self.menufont.config()
+				
+			else:
+				dictionary['menufont'] = self.menufont.actual()
+				
+		else:
+			dictionary['font'] = self.font.actual()
+			dictionary['menufont'] = self.menufont.actual()
+
+		
+		dictionary['scrollbar_width'] = self.scrollbar_width
+		dictionary['elementborderwidth'] = self.elementborderwidth
+		dictionary['want_ln'] = self.want_ln
+		dictionary['syntax'] = self.syntax
+		dictionary['ind_depth'] = self.ind_depth
+		dictionary['themes'] = self.themes
+		
+		for tab in self.tabs:
+			tab.contents = ''
+			tab.oldcontents = ''
+			
+			# Convert tab.filepath to string for serialization
+			if tab.filepath:
+				tab.filepath = tab.filepath.__str__()
+		
+		tmplist = [ tab.__dict__ for tab in self.tabs ]
+		dictionary['tabs'] = tmplist
+		
+		return dictionary
+		
+		
+	def set_config(self, dictionary, font, menufont):
+		
+		# Set Font Begin ##############################
+		
+		# Both missing:
+		if not font and not menufont:
+			fontname = None
+			
+			fontfamilies = [f for f in tkinter.font.families()]
+			
+			for font in GOODFONTS:
+				if font in fontfamilies:
+					fontname = font
+					break
+			
+			if not fontname:
+				fontname = 'TkDefaulFont'
+				
+			dictionary['font']['family'] = fontname
+			dictionary['menufont']['family'] = fontname
+		
+		# One missing, copy existing:
+		elif bool(font) ^ bool(menufont):
+			if font:
+				dictionary['menufont']['family'] = font
+			else:
+				dictionary['font']['family'] = menufont
+			
+			
+		self.font.config(**dictionary['font'])
+		self.menufont.config(**dictionary['menufont'])
+		self.scrollbar_width 	= dictionary['scrollbar_width']
+		self.elementborderwidth	= dictionary['elementborderwidth']
+		self.want_ln = dictionary['want_ln']
+		self.syntax = dictionary['syntax']
+		self.ind_depth = dictionary['ind_depth']
+		self.themes = dictionary['themes']
+		self.curtheme = dictionary['curtheme']
+		
+		self.bgcolor, self.fgcolor = self.themes[self.curtheme]['normal_text'][:]
+			
+		self.lastdir = dictionary['lastdir']
+		
+		if self.lastdir != None:
+			self.lastdir = pathlib.Path(dictionary['lastdir'])
+			if not self.lastdir.exists():
+				self.lastdir = None
+		
+		self.tabs = [ Tab(**item) for item in dictionary['tabs'] ]
+		
+		# Have to step backwards here to avoid for-loop breaking
+		# while removing items from the container.
+		
+		for i in range(len(self.tabs)-1, -1, -1):
+			tab = self.tabs[i]
+			
+			if tab.type == 'normal':
+				try:
+					with open(tab.filepath, 'r', encoding='utf-8') as f:
+						tmp = f.read()
+						tab.contents = tmp
+						tab.oldcontents = tab.contents
+						
+					tab.filepath = pathlib.Path(tab.filepath)
+					
+					
+				except (EnvironmentError, UnicodeDecodeError) as e:
+					print(e.__str__())
+					self.tabs.pop(i)
+			else:
+				tab.filepath = None
+				tab.position = '1.0'
+				
+		for i,tab in enumerate(self.tabs):
+			if tab.active == True:
+				self.tabindex = i
+				break
+		
+
+	def apply_config(self):
+		
+		if self.tabindex == None:
+			if len(self.tabs) == 0:
+				self.tabindex = -1
+				self.new_tab()
+			# recently active normal tab is gone:
+			else:
+				self.tabindex = 0
+				self.tabs[self.tabindex].active = True
+		
+
+		self.tab_width = self.font.measure(self.ind_depth * TAB_WIDTH_CHAR)
+		
+		pad_x =  self.tab_width // self.ind_depth // 3
+		pad_y = pad_x
+
+		for tagname in self.themes[self.curtheme]:
+			bg, fg = self.themes[self.curtheme][tagname][:]
+			self.contents.tag_config(tagname, background=bg, foreground=fg)
+		
+		
+		self.contents.config(font=self.font, foreground=self.fgcolor,
+			background=self.bgcolor, insertbackground=self.fgcolor,
+			tabs=(self.tab_width, ), padx=pad_x, pady=pad_y)
+			
+		self.scrollbar.config(width=self.scrollbar_width)
+		self.scrollbar.config(elementborderwidth=self.elementborderwidth)
+		
+		self.ln_widget.config(font=self.font, foreground=self.fgcolor, background=self.bgcolor,
+			padx=pad_x, pady=pad_y)
+			
+		self.entry.config(font=self.menufont)
+		self.btn_open.config(font=self.menufont)
+		self.btn_save.config(font=self.menufont)
+		self.btn_git.config(font=self.menufont)
+		self.popup.config(font=self.menufont)
+		
+		if self.tabs[self.tabindex].type == 'normal':
+			self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
+			self.entry.insert(0, self.tabs[self.tabindex].filepath)
+			self.entry.xview_moveto(1.0)
+			
+			
+		self.contents.edit_reset()
+		self.contents.edit_modified(0)
+		
+########## Configuration Related End
+########## Syntax highlight Begin
+	
+	def toggle_syntax(self, event=None):
+		
+		if self.syntax:
+			self.syntax = False
+			self.token_can_update = False
+			
+			for tag in self.tagnames:
+				self.contents.tag_remove( tag, '1.0', tkinter.END )
+				
+			return 'break'
+	
+		else:
+			self.syntax = True
+			self.do_syntax(everything=True)
+			
+			return 'break'
+			
+	
+	def can_do_syntax(self):
+	
+		return '.py' in self.tabs[self.tabindex].filepath.suffix and self.syntax
+		
+		
+	def do_syntax(self, everything=False):
+	
+		if self.tabs[self.tabindex].filepath:
+			if self.can_do_syntax():
+			
+				self.token_err = True
+				content_is_uptodate = everything
+				self.update_tokens(start='1.0', end=tkinter.END, everything=content_is_uptodate)
+				self.token_can_update = True
+				
+			else:
+				self.token_err = False
+				self.token_can_update = False
+			
+		else:
+			self.token_err = False
+			self.token_can_update = False
+			
+	
+	def update_tokens(self, start=None, end=None, line=None, everything=False):
+	
+		start_idx = start
+		end_idx = end
+		linecontents = None
+		
+		if not everything:
+			if line:
+				linecontents = line
+				test1 = [
+					self.token_err,
+					( '"""' in linecontents and '#' in linecontents ),
+					( "'''" in linecontents and '#' in linecontents )
+					]
+			else:
+				test1 = [self.token_err]
+				
+				
+			if any(test1):
+				start_idx = '1.0'
+				end_idx = tkinter.END
+				linecontents = None
+				#print('err')
+		
+			# check if inside multiline string
+			elif 'strings' in self.contents.tag_names(tkinter.INSERT) and \
+					not ( start_idx == '1.0' and end_idx == tkinter.END ):
+				
+				try:
+					s, e = self.contents.tag_prevrange('strings', tkinter.INSERT)
+					l0, l1 = map( lambda x: int( x.split('.')[0] ), [s, e] )
+				
+					if l0 != l1:
+						start_idx, end_idx = (s, e)
+						linecontents = None
+		
+				except ValueError:
+					pass
+			
+			
+			if not linecontents:
+				tmp = self.contents.get( start_idx, end_idx )
+				
+			else:
+				tmp = linecontents
+				
+		else:
+			tmp = self.tabs[self.tabindex].contents
+			
+		
+		
+		prev_char = self.contents.get( '%s - 1c' % tkinter.INSERT, tkinter.INSERT )
+		if prev_char in [ '(', ')', '[', ']' , '{', '}' ]:
+			self.par_err = True
+		
+		linenum = int(start_idx.split('.')[0])
+		flag_err = False
+		#print(self.token_err)
+		
+		
+		try:
+			par_err = None
+			
+			with io.BytesIO( tmp.encode('utf-8') ) as fo:
+			
+				tokens = tokenize.tokenize( fo.readline )
+			
+				# Remove old tags:
+				for tag in self.tagnames:
+					self.contents.tag_remove( tag, start_idx, end_idx )
+					
+				# Retag:
+				idx_start = None
+				for token in tokens:
+					#print(token)
+					
+					# token.line contains line as string which contains token.
+					
+					if token.type == tokenize.NAME or \
+						( token.type in [ tokenize.NUMBER, tokenize.STRING, tokenize.COMMENT] ) or \
+						( token.exact_type == tokenize.LPAR ):
+						
+						# initiate indexes with correct linenum
+						s0, s1 = map(str, [ token.start[0] + linenum - 1, token.start[1] ] )
+						e0, e1 = map(str, [ token.end[0] + linenum - 1, token.end[1] ] )
+						idx_start = s0 + '.' + s1
+						idx_end = e0 + '.' + e1
+						
+						
+						if token.type == tokenize.NAME:
+							
+							#lastoken = token
+							last_idx_start = idx_start
+							last_idx_end = idx_end
+							
+							if token.string in self.keywords:
+							
+								if token.string == 'self':
+									self.contents.tag_add('selfs', idx_start, idx_end)
+								
+								elif token.string in self.bools:
+									self.contents.tag_add('bools', idx_start, idx_end)
+									
+##								elif token.string in self.tests:
+##									self.contents.tag_add('tests', idx_start, idx_end)
+								
+								elif token.string in self.breaks:
+									self.contents.tag_add('breaks', idx_start, idx_end)
+								
+								else:
+									self.contents.tag_add('keywords', idx_start, idx_end)
+								
+						
+						# calls
+						elif token.exact_type == tokenize.LPAR:
+							# Need to know if last char before ( was not empty.
+							# Previously used test was:
+							#if self.contents.get( '%s - 1c' % idx_start, idx_start ).strip():
+							
+							# token.line contains line as string which contains token.
+							prev_char_idx = token.start[1]-1
+							if prev_char_idx > -1 and token.line[prev_char_idx].isalnum():
+								self.contents.tag_add('calls', last_idx_start, last_idx_end)
+								
+						elif token.type == tokenize.STRING:
+							self.contents.tag_add('strings', idx_start, idx_end)
+							
+						elif token.type == tokenize.COMMENT:
+							self.contents.tag_add('comments', idx_start, idx_end)
+						
+						# token.type == tokenize.NUMBER
+						else:
+							self.contents.tag_add('numbers', idx_start, idx_end)
+					
+		
+		except IndentationError as e:
+##			for attr in ['args', 'filename', 'lineno', 'msg', 'offset', 'text']:
+##				item = getattr( e, attr)
+##				print( attr,': ', item )
+
+			# This Error needs info about whole block, one line is not enough, so quite rare.
+			#print( e.args[0], '\nIndentation errline: ', self.contents.index(tkinter.INSERT) )
+			flag_err = True
+			self.token_err = True
+
+		
+		except tokenize.TokenError as ee:
+			
+			if 'EOF in multi-line statement' in ee.args[0]:
+				self.check_pars = idx_start
+				
+			elif 'multi-line string' in ee.args[0]:
+				flag_err = True
+				self.token_err = True
+			
+			
+		# from backspace_override:
+		if self.check_pars:
+			startl = self.check_pars
+			par_err = self.checkpars(startl)
+			
+		elif self.par_err:
+			startl = False
+			par_err = self.checkpars(startl)
+
+		self.check_pars = False
+		self.par_err = par_err
+
+		if not par_err:
+			# not always checking whole file for par mismatches, so clear
+			self.contents.tag_remove('mismatch', '1.0', tkinter.END)
+			
+
+
+		if not flag_err and ( start_idx == '1.0' and end_idx == tkinter.END ):
+			#print('ok')
+			self.token_err = False
+			
+			
+	def checkpars(self, idx_start):
+		# possible par mismatch may be caused from another line,
+		# so find current block: find first empty line before and after curline
+		# then count pars in it.
+		
+		if not idx_start:
+			# line had nothing but brace in it and it were deleted
+			idx_start = self.contents.index(tkinter.INSERT)
+			
+		curline = int( idx_start.split('.')[0] )
+		startline, endline, lines = self.find_empty_lines(curline)
+		err_indexes = self.count_pars(startline, lines)
+		
+		err = False
+		
+		if err_indexes:
+			err = True
+			err_line = startline + err_indexes[0]
+			err_col = err_indexes[1]
+			err_idx = '%i.%i' % (err_line, err_col)
+			
+			self.contents.tag_remove('mismatch', '1.0', tkinter.END)
+			self.contents.tag_add('mismatch', err_idx, '%s +1c' % err_idx)
+		
+		#print(err)
+		return err
+	
+	
+	def count_pars(self, startline, lines):
+		
+		pars = list()
+		bras = list()
+		curls = list()
+		
+		opening  = [ '(', '[', '{' ]
+		closing  = [ ')', ']', '}' ]
+		
+		tags = None
+		
+		# populate lists and return at first extra closer:
+		for i in range(len(lines)):
+			
+			for j in range(len(lines[i])):
+				c = lines[i][j]
+				patt = '%i.%i' % (startline+i, j)
+				tags = self.contents.tag_names(patt)
+
+				# skip if string or comment:
+				if tags:
+					if 'strings' in tags or 'comments' in tags:
+						tags = None
+						continue
+				
+				if c in closing:
+					if c == ')':
+						if len(pars) > 0:
+							pars.pop(-1)
+						else:
+							return (i,j)
+					
+					elif c == ']':
+						if len(bras) > 0:
+							bras.pop(-1)
+						else:
+							return (i,j)
+					
+					# c == '}'
+					else:
+						if len(curls) > 0:
+							curls.pop(-1)
+						else:
+							return (i,j)
+						
+							
+				elif c in opening:
+					if c == '(':
+						pars.append((i,j))
+						
+					elif c == '[':
+						bras.append((i,j))
+					
+					# c == '{':
+					else:
+						curls.append((i,j))
+				
+		
+		# no extra closer in block.
+		# Return last extra opener:
+		idxlist = list()
+		
+		for item in [ pars, bras, curls ]:
+			if len(item) > 0:
+				idx =  item.pop(-1)
+				idxlist.append(idx)
+	
+	
+		if len(idxlist) > 0:
+			if len(idxlist) > 1:
+			
+				maxidx = max(idxlist)
+				
+				return idxlist[idxlist.index(maxidx)]
+					
+			else:
+				return idxlist[0]
+			
+		else:
+			return False
+
+		
+	def find_empty_lines(self, lnstart):
+		'''	Finds first empty lines before and after current line
+			
+			returns
+				linenumber of start and end of the block
+				and list of lines.
+
+			called from update_tokens
+		'''
+
+		lines = list()
+
+		# first empty line before curline:
+		endln = 1
+		ln = lnstart
+
+		if ln > endln:
+			ln -= 1
+			t = self.contents.get('%i.0' % ln, '%i.end' % ln)
+			
+			while t != '' and not t.isspace():
+				lines.append(t)
+				ln -= 1
+				
+				if ln < endln:
+					break
+				
+				t = self.contents.get('%i.0' % ln, '%i.end' % ln)
+			
+			ln += 1
+
+		else:
+			pass
+			# curline is firstline
+
+
+		# ln is now first empty linenum above curline or firstline
+		startline = ln
+
+
+		# add curline to list
+		ln = lnstart
+		lines.reverse()
+		t = self.contents.get('%i.0' % ln, '%i.end' % ln)
+		lines.append(t)
+
+
+		# first empty line after curline:
+		endln = int( self.contents.index(tkinter.END).split('.')[0] )
+		ln += 1
+		
+		if ln < endln:
+			
+			t = self.contents.get('%i.0' % ln, '%i.end' % ln)
+
+			while  t != '' and not t.isspace():
+				lines.append(t)
+				ln += 1
+
+				if ln > endln:
+					break
+
+				t = self.contents.get('%i.0' % ln, '%i.end' % ln)
+				
+			ln -= 1
+			
+		else:
+			# curline is lastline
+			pass
+
+		# ln is now first empty linenum after curline or lastline
+		endline = ln
+
+		return startline, endline, lines
+							
+
+########## Syntax highlight End
+########## Theme Related Begin
+
+	def change_indentation_width(self, width):
+		''' width is integer between 1-8
+		'''
+		
+		if type(width) != int: return
+		elif width == self.ind_depth: return
+		elif not 0 < width <= 8: return
+		
+		
+		self.ind_depth = width
+		self.tab_width = self.font.measure(self.ind_depth * self.tab_char)
+		self.contents.config(tabs=(self.tab_width, ))
+
+
+	def increase_scrollbar_width(self, event=None):
+		'''	Change width of scrollbar and self.contents
+			Shortcut: Ctrl-plus
+		'''
+		if self.scrollbar_width >= 100:
+			self.bell()
+			return 'break'
+			
+		self.scrollbar_width += 7
+		self.elementborderwidth += 1
+		self.scrollbar.config(width=self.scrollbar_width)
+		self.scrollbar.config(elementborderwidth=self.elementborderwidth)
+			
+		return 'break'
+		
+		
+	def decrease_scrollbar_width(self, event=None):
+		'''	Change width of scrollbar and self.contents
+			Shortcut: Ctrl-minus
+		'''
+		if self.scrollbar_width <= 0:
+			self.bell()
+			return 'break'
+			
+		self.scrollbar_width -= 7
+		self.elementborderwidth -= 1
+		self.scrollbar.config(width=self.scrollbar_width)
+		self.scrollbar.config(elementborderwidth=self.elementborderwidth)
+			
+		return 'break'
+		
+
+	def toggle_color(self, event=None):
+		
+		if self.curtheme == 'day':
+			self.curtheme = 'night'
+		else:
+			self.curtheme = 'day'
+		
+		self.update_normal_text()
+		
+		return 'break'
+
+
+	def update_normal_text(self):
+	
+		self.bgcolor, self.fgcolor = self.themes[self.curtheme]['normal_text'][:]
+			
+	
+		for tagname in self.themes[self.curtheme]:
+			bg, fg = self.themes[self.curtheme][tagname][:]
+			self.contents.tag_config(tagname, background=bg, foreground=fg)
+	
+		
+		self.contents.config(foreground=self.fgcolor, background=self.bgcolor,
+			insertbackground=self.fgcolor)
+			
+		self.ln_widget.config(foreground=self.fgcolor, background=self.bgcolor, selectbackground=self.bgcolor, selectforeground=self.fgcolor, inactiveselectbackground=self.bgcolor )
+	
+	
+	def update_fonts(self):
+		self.boldfont = self.font.copy()
+		self.boldfont.config(weight='bold')
+		
+		self.contents.tag_config('keywords', font=self.boldfont)
+		self.contents.tag_config('numbers', font=self.boldfont)
+		self.contents.tag_config('comments', font=self.boldfont)
+		self.contents.tag_config('breaks', font=self.boldfont)
+		self.contents.tag_config('calls', font=self.boldfont)
+		
+		
+		self.tab_width = self.font.measure(self.ind_depth * self.tab_char)
+		pad_x =  self.tab_width // self.ind_depth // 3
+		pad_y = pad_x
+		
+		self.contents.config(tabs=(self.tab_width, ), padx=pad_x, pady=pad_y)
+		self.ln_widget.config(padx=pad_x, pady=pad_y)
+		self.y_extra_offset = self.contents['highlightthickness'] + self.contents['bd'] + self.contents['pady']
+		#self.bbox_height = self.contents.bbox('@0,0')[3]
+		
+
+					
+	def font_choose(self, event=None):
+		if self.state != 'normal':
+			self.bell()
+			return "break"
+		
+		fonttop = tkinter.Toplevel()
+		fonttop.title('Choose Font')
+		
+		big = False
+		shortcut = "<Alt-f>"
+		
+		if self.os_type == 'mac_os':
+			big = True
+			shortcut = "<function>"
+		
+		
+		fonttop.protocol("WM_DELETE_WINDOW", lambda: ( fonttop.destroy(),
+				self.contents.bind( shortcut, self.font_choose)) )
+		
+		changefont.FontChooser( fonttop, [self.font, self.menufont], big, tracefunc=self.update_fonts, os_type=self.os_type )
+		self.contents.bind( shortcut, self.do_nothing)
+		self.to_be_closed.append(fonttop)
+	
+		return 'break'
+		
+		
+	def enter2(self, args, event=None):
+		''' When mousecursor enters hyperlink tagname in colorchooser.
+		'''
+		wid = args[0]
+		tagname = args[1]
+		
+		t = wid.textwid
+		
+##		wid.after(200, lambda kwargs={'cursor':'hand2'}: t.config(**kwargs) )
+##
+		
+		
+		t.config(cursor="hand2")
+		wid.after(50, lambda args=[tagname],
+				kwargs={'underline':1, 'font':self.boldfont}: t.tag_config(*args, **kwargs) )
+		
+		#t.tag_config(tagname, underline=1, font=self.boldfont)
+		
+		
+	def leave2(self, args, event=None):
+		''' When mousecursor leaves hyperlink tagname in colorchooser.
+		'''
+		wid = args[0]
+		tagname = args[1]
+		
+		t = wid.textwid
+		
+		t.config(cursor=self.name_of_cursor_in_text_widget)
+		wid.after(50, lambda args=[tagname],
+				kwargs={'underline':0, 'font':self.menufont}: t.tag_config(*args, **kwargs) )
+		
+		#t.tag_config(tagname, underline=0, font=self.menufont)
+		
+		
+	def lclick2(self, args, event=None):
+		'''	When clicked hyperlink in colorchooser.
+		'''
+		wid = args[0]
+		tagname = args[1]
+		
+		syntags = [
+		'normal_text',
+		'keywords',
+		'numbers',
+		'bools',
+		'strings',
+		'comments',
+		'breaks',
+		'calls',
+		'selfs',
+		'match',
+		'focus',
+		'replaced',
+		'mismatch',
+		'selected'
+		]
+		
+		modetags = [
+		'Day',
+		'Night',
+		'Text',
+		'Background'
+		]
+		
+		savetags = [
+		'Save_TMP',
+		'TMP',
+		'Start',
+		'Defaults'
+		]
+		
+		onlyfore = [
+		'keywords',
+		'numbers',
+		'bools',
+		'strings',
+		'comments',
+		'breaks',
+		'calls',
+		'selfs'
+		]
+
+		
+		if tagname in syntags:
+			
+			if tagname == 'selected':
+				tagname = 'sel'
+			
+			if wid.frontback_mode == 'foreground':
+				initcolor = self.contents.tag_cget(tagname, 'foreground')
+				patt = 'Choose fgcolor for: %s' % tagname
+				
+			else:
+				initcolor = self.contents.tag_cget(tagname, 'background')
+				patt = 'Choose bgcolor for: %s' % tagname
+			
+			res = self.tk.call('tk_chooseColor', '-initialcolor', initcolor, '-title', patt)
+				
+			tmpcolor = str(res)
+			
+			if tmpcolor in [None, '']:
+				wid.focus_set()
+				return 'break'
+			
+			
+			try:
+				if wid.frontback_mode == 'foreground':
+					self.themes[self.curtheme][tagname][1] = tmpcolor
+					self.contents.tag_config(tagname, foreground=tmpcolor)
+				else:
+					self.themes[self.curtheme][tagname][0] = tmpcolor
+					self.contents.tag_config(tagname, background=tmpcolor)
+			
+			
+				if tagname == 'normal_text':
+					self.update_normal_text()
+				
+			# if closed editor and still pressing ok in colorchooser:
+			except (tkinter.TclError, AttributeError) as e:
+				# because if closed editor, this survives
+				pass
+			
+			
+		elif tagname in modetags:
+		
+			t = wid.textwid
+		
+			if tagname == 'Day' and self.curtheme != 'day':
+				r1 = t.tag_nextrange('Day', 1.0)
+				r2 = t.tag_nextrange('Night', 1.0)
+				
+				t.delete(r1[0], r1[1])
+				t.insert(r1[0], '[X] Day-mode	', 'Day')
+				t.delete(r2[0], r2[1])
+				t.insert(r2[0], '[ ] Night-mode	', 'Night')
+				
+				self.toggle_color()
+				
+				
+			elif tagname == 'Night' and self.curtheme != 'night':
+				r1 = t.tag_nextrange('Day', 1.0)
+				r2 = t.tag_nextrange('Night', 1.0)
+				
+				t.delete(r1[0], r1[1])
+				t.insert(r1[0], '[ ] Day-mode	', 'Day')
+				t.delete(r2[0], r2[1])
+				t.insert(r2[0], '[X] Night-mode	', 'Night')
+				
+				self.toggle_color()
+				
+				
+			elif tagname == 'Text':
+				if wid.frontback_mode != 'foreground':
+					r1 = t.tag_nextrange('Text', 1.0)
+					r2 = t.tag_nextrange('Background', 1.0)
+					
+					t.delete(r1[0], r1[1])
+					t.insert(r1[0], '[X] Text color\n', 'Text')
+					
+					t.delete(r2[0], r2[1])
+					t.insert(r2[0], '[ ] Background color\n', 'Background')
+					wid.frontback_mode = 'foreground'
+					
+					t.tag_remove('disabled', 1.0, tkinter.END)
+					
+					for tag in onlyfore:
+						r3 = wid.tag_idx.get(tag)
+						t.tag_add(tag, r3[0], r3[1])
+					
+								
+			elif tagname == 'Background':
+				if wid.frontback_mode != 'background':
+					r1 = t.tag_nextrange('Text', 1.0)
+					r2 = t.tag_nextrange('Background', 1.0)
+					
+					t.delete(r1[0], r1[1])
+					t.insert(r1[0], '[ ] Text color\n', 'Text')
+					
+					t.delete(r2[0], r2[1])
+					t.insert(r2[0], '[X] Background color\n', 'Background')
+					wid.frontback_mode = 'background'
+					
+					for tag in onlyfore:
+						r3 = t.tag_nextrange(tag, 1.0)
+						wid.tag_idx.setdefault(tag, r3)
+						t.tag_remove(tag, 1.0, tkinter.END)
+						t.tag_add('disabled', r3[0], r3[1])
+						
+				
+		elif tagname in savetags:
+			
+			if tagname == 'Save_TMP':
+				wid.tmp_theme = copy.deepcopy(self.themes)
+				wid.flag_tmp = True
+				self.flash_tag(wid, tagname)
+				
+			elif tagname == 'TMP' and wid.flag_tmp:
+				self.themes = copy.deepcopy(wid.tmp_theme)
+				self.flash_tag(wid, tagname)
+				
+			elif tagname == 'Start':
+				self.themes = copy.deepcopy(wid.start_theme)
+				self.flash_tag(wid, tagname)
+				
+			elif tagname == 'Defaults':
+				self.themes = copy.deepcopy(self.default_themes)
+				self.flash_tag(wid, tagname)
+				
+				
+			if (tagname in ['Defaults', 'Start']) or (tagname == 'TMP' and wid.flag_tmp):
+			
+				for tag in self.themes[self.curtheme]:
+					bg, fg = self.themes[self.curtheme][tag][:]
+					self.contents.tag_config(tag, background=bg, foreground=fg)
+	
+				self.update_normal_text()
+				
+		
+		wid.focus_set()
+				
+				
+	def flash_tag(self, wid, tagname):
+		''' Flash save_tag when clicked in colorchooser.
+		'''
+		t = wid.textwid
+		
+		wid.after(50, lambda args=[tagname],
+				kwargs={'background':'green'}: t.tag_config(*args, **kwargs) )
+					
+		wid.after(600, lambda args=[tagname],
+				kwargs={'background':t.cget('background')}: t.tag_config(*args, **kwargs) )
+					
+	
+	def color_choose(self, event=None):
+		if self.state != 'normal':
+			self.bell()
+			return "break"
+			
+		colortop = tkinter.Toplevel()
+		c = colortop
+		c.title('Choose Color')
+		c.start_theme = copy.deepcopy(self.themes)
+		c.tmp_theme = copy.deepcopy(self.themes)
+		c.flag_tmp = False
+		
+		shortcut_color = "<Alt-s>"
+		shortcut_toggl = "<Alt-t>"
+
+		if self.os_type == 'mac_os':
+			shortcut_color = "<ssharp>"
+			shortcut_toggl = "<dagger>"
+		
+		
+		c.protocol("WM_DELETE_WINDOW", lambda: ( c.destroy(),
+				self.contents.bind( shortcut_color, self.color_choose),
+				self.contents.bind( shortcut_toggl, self.toggle_color)) )
+				
+		self.contents.bind( shortcut_color, self.do_nothing)
+		self.contents.bind( shortcut_toggl, self.do_nothing)
+		
+		#c.textfont = tkinter.font.Font(family='TkDefaulFont', size=10)
+		
+		size_title = 12
+		if self.os_type == 'mac_os': size_title = 16
+		c.titlefont = tkinter.font.Font(family='TkDefaulFont', size=size_title)
+		
+		c.textwid = tkinter.Text(c, blockcursor=True, highlightthickness=0,
+							bd=4, pady=4, padx=10, tabstyle='wordprocessor', font=self.menufont)
+		
+		c.scrollbar = tkinter.Scrollbar(c, orient=tkinter.VERTICAL, highlightthickness=0,
+							bd=0, command = c.textwid.yview)
+
+		
+		c.textwid['yscrollcommand'] = c.scrollbar.set
+		c.scrollbar.config(width=self.scrollbar_width)
+		c.scrollbar.config(elementborderwidth=self.elementborderwidth)
+
+		t = c.textwid
+		
+		t.tag_config('title', font=c.titlefont)
+		t.tag_config('disabled', foreground='#a6a6a6')
+		
+		tags = [
+		'Day',
+		'Night',
+		'Text',
+		'Background',
+		'normal_text',
+		'keywords',
+		'numbers',
+		'bools',
+		'strings',
+		'comments',
+		'breaks',
+		'calls',
+		'selfs',
+		'match',
+		'focus',
+		'replaced',
+		'mismatch',
+		'selected',
+		'Save_TMP',
+		'TMP',
+		'Start',
+		'Defaults'
+		]
+		
+		
+		
+				
+		
+		
+		for tag in tags:
+			t.tag_config(tag, font=self.menufont)
+			t.tag_bind(tag, "<Enter>",
+				lambda event, arg=[c, tag]: self.enter2(arg, event))
+			t.tag_bind(tag, "<Leave>",
+				lambda event, arg=[c, tag]: self.leave2(arg, event))
+			t.tag_bind(tag, "<ButtonRelease-1>",
+					lambda event, arg=[c, tag]: self.lclick2(arg, event))
+						
+		
+				
+		c.rowconfigure(1, weight=1)
+		c.columnconfigure(1, weight=1)
+		
+		t.grid_configure(row=0, column = 0)
+		c.scrollbar.grid_configure(row=0, column = 1, sticky='ns')
+		
+		
+		i = tkinter.INSERT
+		
+		t.insert(i, 'Before closing, load setting from: Start\n', 'title')
+		t.insert(i, 'if there were made unwanted changes.\n', 'title')
+		t.insert(i, '\nChanging color for:\n', 'title')
+		
+		
+		c.frontback_mode = None
+		c.tag_idx = dict()
+		
+		if self.curtheme == 'day':
+		
+			t.insert(i, '[X] Day-mode	', 'Day')
+			t.insert(i, '[X] Text color\n', 'Text')
+		
+			t.insert(i, '[ ] Night-mode	', 'Night')
+			t.insert(i, '[ ] Background color\n', 'Background')
+			
+			c.frontback_mode = 'foreground'
+			
+			
+		else:
+			t.insert(i, '[ ] Day-mode	', 'Day')
+			t.insert(i, '[X] Text color\n', 'Text')
+		
+			t.insert(i, '[X] Night-mode	', 'Night')
+			t.insert(i, '[ ] Background color\n', 'Background')
+			
+			c.frontback_mode = 'foreground'
+			
+		
+		
+		t.insert(i, '\nSelect tag you want to modify\n', 'title')
+		t.insert(i, 'normal text\n', 'normal_text')
+		
+		
+		t.insert(i, '\nSyntax highlight tags\n', 'title')
+		t.insert(i, 'keywords\n', 'keywords')
+		t.insert(i, 'numbers\n', 'numbers')
+		t.insert(i, 'bools\n', 'bools')
+		t.insert(i, 'strings\n', 'strings')
+		t.insert(i, 'comments\n', 'comments')
+		t.insert(i, 'breaks\n', 'breaks')
+		t.insert(i, 'calls\n', 'calls')
+		t.insert(i, 'selfs\n', 'selfs')
+	
+
+		t.insert(i, '\nSearch tags\n', 'title')
+		t.insert(i, 'match\n', 'match')
+		t.insert(i, 'focus\n', 'focus')
+		t.insert(i, 'replaced\n', 'replaced')
+	
+
+		t.insert(i, '\nParentheses\n', 'title')
+		t.insert(i, 'mismatch\n', 'mismatch')
+		
+		t.insert(i, '\nSelection\n', 'title')
+		t.insert(i, 'selected\n', 'selected')
+	
+
+		t.insert(i, '\nSave current setting to template,\n', 'title')
+		t.insert(i, 'to which you can revert later:\n', 'title')
+		t.insert(i, 'Save TMP\n', 'Save_TMP')
+		
+		t.insert(i, '\nLoad setting from:\n', 'title')
+		t.insert(i, 'TMP\n', 'TMP')
+		t.insert(i, 'Start\n', 'Start')
+		t.insert(i, 'Defaults\n', 'Defaults')
+
+
+		t.state = 'disabled'
+		t.config(insertontime=0)
+
+
+		self.to_be_closed.append(c)
+
+		return 'break'
+
+		
+########## Theme Related End
+########## Run file Related Begin
+
+	def enter(self, tagname, event=None):
+		''' Used in error-page, when mousecursor enters hyperlink tagname.
+		'''
+		self.contents.config(cursor="hand2")
+		self.contents.tag_config(tagname, underline=1)
+
+
+	def leave(self, tagname, event=None):
+		''' Used in error-page, when mousecursor leaves hyperlink tagname.
+		'''
+		self.contents.config(cursor=self.name_of_cursor_in_text_widget)
+		self.contents.tag_config(tagname, underline=0)
+
+
+	def lclick(self, tagname, event=None):
+		'''	Used in error-page, when hyperlink tagname is clicked.
+		
+			self.taglinks is dict with tagname as key
+			and function (self.taglink) as value.
+		'''
+		
+		# passing tagname-string as argument to function self.taglink()
+		# which in turn is a value of tagname-key in dictionary taglinks:
+		self.taglinks[tagname](tagname)
+		
+
+	def tag_link(self, tagname, event=None):
+		''' Used in error-page, executed when hyperlink tagname is clicked.
+		'''
+		
+		i = int(tagname.split("-")[1])
+		filepath, errline = self.errlines[i]
+		
+		filepath = pathlib.Path(filepath)
+		openfiles = [tab.filepath for tab in self.tabs]
+		
+		# clicked activetab, do nothing
+		if filepath == self.tabs[self.tabindex].filepath:
+			pass
+			
+		# clicked file that is open, switch activetab
+		elif filepath in openfiles:
+			for i,tab in enumerate(self.tabs):
+				if tab.filepath == filepath:
+					self.tabs[self.tabindex].active = False
+					self.tabindex = i
+					self.tabs[self.tabindex].active = True
+					break
+					
+		# else: open file in newtab
+		else:
+			try:
+				with open(filepath, 'r', encoding='utf-8') as f:
+					self.new_tab(error=True)
+					tmp = f.read()
+					self.tabs[self.tabindex].oldcontents = tmp
+					
+					if '.py' in filepath.suffix:
+						indentation_is_alien, indent_depth = self.check_indent_depth(tmp)
+						
+						if indentation_is_alien:
+							# Assuming user wants self.ind_depth, change it without notice:
+							tmp = self.tabs[self.tabindex].oldcontents.splitlines(True)
+							tmp[:] = [self.tabify(line, width=indent_depth) for line in tmp]
+							tmp = ''.join(tmp)
+							self.tabs[self.tabindex].contents = tmp
+							
+						else:
+							self.tabs[self.tabindex].contents = self.tabs[self.tabindex].oldcontents
+					else:
+						self.tabs[self.tabindex].contents = self.tabs[self.tabindex].oldcontents
+				
+					
+					self.tabs[self.tabindex].filepath = filepath
+					self.tabs[self.tabindex].type = 'normal'
+			except (EnvironmentError, UnicodeDecodeError) as e:
+				print(e.__str__())
+				print(f'\n Could not open file: {filepath}')
+				self.bell()
+				return
+
+		
+		self.entry.delete(0, tkinter.END)
+		self.entry.insert(0, self.tabs[self.tabindex].filepath)
+		self.entry.xview_moveto(1.0)
+		
+		
+		self.contents.delete('1.0', tkinter.END)
+		self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
+		
+		
+		if self.syntax:
+		
+			lineend = '%s lineend' % tkinter.INSERT
+			linestart = '%s linestart' % tkinter.INSERT
+			
+			tmp = self.contents.get( linestart, lineend )
+			self.oldline = tmp
+			
+			self.token_err = True
+			self.update_tokens(start='1.0', end=tkinter.END)
+			self.token_can_update = True
+		
+		
+		# set cursor pos
+		line = errline + '.0'
+		self.contents.focus_set()
+		self.contents.mark_set('insert', line)
+		self.ensure_idx_visibility(line)
+					
+		
+		self.contents.edit_reset()
+		self.contents.edit_modified(0)
+		
+		self.contents.bind("<Button-%i>" % self.right_mousebutton_num, lambda event: self.raise_popup(event))
+		self.state = 'normal'
+		self.update_title()
+		
+
+	def run(self):
+		'''	Run file currently being edited. This can not catch errlines of
+			those exceptions that are catched. Like:
+			
+			try:
+				code we know sometimes failing with SomeError
+				(but might also fail with other error-type)
+			except SomeError:
+				some other code but no raising error
+				
+			Note: 	Above code will raise an error in case
+			 		code in try-block raises some other error than SomeError.
+					In that case those errlines will be of course catched.
+			
+			What this means: If you self.run() with intention to spot possible
+			errors in your program, you should use logging (in except-block)
+			if you are not 100% sure about your code in except-block.
+		'''
+		if (self.state != 'normal') or (self.tabs[self.tabindex].type == 'newtab'):
+			self.bell()
+			return 'break'
+			
+		self.save(forced=True)
+		
+		# https://docs.python.org/3/library/subprocess.html
+
+		res = subprocess.run(['python', self.tabs[self.tabindex].filepath], stderr=subprocess.PIPE).stderr
+		
+		err = res.decode()
+		
+		if len(err) != 0:
+			self.bind("<Escape>", self.stop_show_errors)
+			self.contents.bind("<Button-%i>" % self.right_mousebutton_num, self.do_nothing)
+			self.state = 'error'
+			
+			self.taglinks = dict()
+			self.errlines = list()
+			openfiles = [tab.filepath for tab in self.tabs]
+			
+			self.contents.delete('1.0', tkinter.END)
+			
+			for tag in self.contents.tag_names():
+				if 'hyper' in tag:
+					self.contents.tag_delete(tag)
+				
+			self.err = err.splitlines()
+			
+			for line in self.err:
+				tmp = line
+
+				tagname = "hyper-%s" % len(self.errlines)
+				self.contents.tag_config(tagname)
+				
+				# Why ButtonRelease instead of just Button-1:
+				# https://stackoverflow.com/questions/24113946/unable-to-move-text-insert-index-with-mark-set-widget-function-python-tkint
+				
+				self.contents.tag_bind(tagname, "<ButtonRelease-1>",
+					lambda event, arg=tagname: self.lclick(arg, event))
+				
+				self.contents.tag_bind(tagname, "<Enter>",
+					lambda event, arg=tagname: self.enter(arg, event))
+				
+				self.contents.tag_bind(tagname, "<Leave>",
+					lambda event, arg=tagname: self.leave(arg, event))
+				
+				self.taglinks[tagname] = self.tag_link
+				
+				# Parse filepath and linenums from errors
+				if 'File ' in line and 'line ' in line:
+					self.contents.insert(tkinter.INSERT, '\n')
+					 
+					data = line.split(',')[:2]
+					linenum = data[1][6:]
+					path = data[0][8:-1]
+					pathlen = len(path) + 2
+					filepath = pathlib.Path(path)
+					
+					self.errlines.append((filepath, linenum))
+					
+					self.contents.insert(tkinter.INSERT, tmp)
+					s0 = tmp.index(path) - 1
+					s = self.contents.index('insert linestart +%sc' % s0 )
+					e = self.contents.index('%s +%sc' % (s, pathlen) )
+					
+					self.contents.tag_add(tagname, s, e)
+						
+					if filepath in openfiles:
+						self.contents.tag_config(tagname, foreground='brown1')
+						self.contents.tag_raise(tagname)
+							
+						
+					self.contents.insert(tkinter.INSERT, '\n')
+					
+					
+				else:
+					self.contents.insert(tkinter.INSERT, tmp +"\n")
+					
+					# Make look bit nicer:
+					if self.syntax:
+						# -1 lines because we have added linebreak already.
+						start = self.contents.index('insert -1 lines linestart')
+						end = self.contents.index('insert -1 lines lineend')
+						
+						self.update_tokens(start=start, end=end, line=line)
+			
+					
+		return 'break'
+				
+
+	def show_errors(self):
+		''' Show traceback from last run with added hyperlinks.
+		'''
+		
+		if len(self.errlines) != 0:
+			self.bind("<Escape>", self.stop_show_errors)
+			self.contents.bind("<Button-%i>" % self.right_mousebutton_num, self.do_nothing)
+			self.state = 'error'
+			
+			tmp = self.contents.get('1.0', tkinter.END)
+			# [:-1]: remove unwanted extra newline
+			self.tabs[self.tabindex].contents = tmp[:-1]
+			
+			try:
+				pos = self.contents.index(tkinter.INSERT)
+			except tkinter.TclError:
+				pos = '1.0'
+				
+			self.tabs[self.tabindex].position = pos
+			self.contents.delete('1.0', tkinter.END)
+			openfiles = [tab.filepath for tab in self.tabs]
+			
+			for tag in self.contents.tag_names():
+				if 'hyper' in tag:
+					self.contents.tag_config(tag, foreground=self.fgcolor)
+			
+			i = 0
+			for line in self.err:
+				tmp = line
+				tagname = 'hyper-%d' % i
+				
+				# Parse filepath and linenums from errors
+				if 'File ' in line and 'line ' in line:
+					self.contents.insert(tkinter.INSERT, '\n')
+					data = line.split(',')[:2]
+					linenum = data[1][6:]
+					path = data[0][8:-1]
+					pathlen = len(path) + 2
+					filepath = pathlib.Path(path)
+					
+					self.contents.insert(tkinter.INSERT, tmp)
+					s0 = tmp.index(path) - 1
+					s = self.contents.index('insert linestart +%sc' % s0 )
+					e = self.contents.index('%s +%sc' % (s, pathlen) )
+					
+					self.contents.tag_add(tagname, s, e)
+					
+					if filepath in openfiles:
+						self.contents.tag_config(tagname, foreground='brown1')
+						self.contents.tag_raise(tagname)
+						
+						
+					self.contents.insert(tkinter.INSERT, '\n')
+					
+					i += 1
+					
+				else:
+					self.contents.insert(tkinter.INSERT, tmp +"\n")
+					
+					# Make look bit nicer:
+					if self.syntax:
+						# -1 lines because we have added linebreak already.
+						start = self.contents.index('insert -1 lines linestart')
+						end = self.contents.index('insert -1 lines lineend')
+						
+						self.update_tokens(start=start, end=end, line=line)
+			
+					
+									
+	def stop_show_errors(self, event=None):
+		self.state = 'normal'
+		self.bind("<Escape>", self.do_nothing)
+		self.contents.bind("<Button-%i>" % self.right_mousebutton_num, lambda event: self.raise_popup(event))
+		
+		self.entry.delete(0, tkinter.END)
+		
+		if self.tabs[self.tabindex].type == 'normal':
+			self.entry.insert(0, self.tabs[self.tabindex].filepath)
+			self.entry.xview_moveto(1.0)
+			
+		
+		self.contents.delete('1.0', tkinter.END)
+		self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
+		
+		
+		self.do_syntax(everything=True)
+		
+		
+		# set cursor pos
+		line = self.tabs[self.tabindex].position
+		self.contents.focus_set()
+		self.contents.mark_set('insert', line)
+		self.ensure_idx_visibility(line)
+			
+			
+		self.contents.edit_reset()
+		self.contents.edit_modified(0)
+		
+		
+########## Run file Related End
+########## Select and move Begin
+
+	def move_right(self, event=None):
+		''' move cursor right with
+			ctrl-i
+		'''
+		
+		if self.state not in  [ 'normal', 'error' ]:
+			self.bell()
+			return "break"
+			
+		self.contents.event_generate('<<NextChar>>')
+		
+		return "break"
+		
+		
+	def move_left(self, event=None):
+		''' move cursor left with
+			ctrl-b
+		'''
+		
+		if self.state not in  [ 'normal', 'error' ]:
+			self.bell()
+			return "break"
+			
+		self.contents.event_generate('<<PrevChar>>')
+		
+		return "break"
+		
+		
+	def move_up(self, event=None):
+		''' move cursor up with
+			ctrl-p
+		'''
+		
+		if self.state not in  [ 'normal', 'error' ]:
+			self.bell()
+			return "break"
+			
+		self.contents.event_generate('<<PrevLine>>')
+		
+		return "break"
+		
+		
+	def move_down(self, event=None):
+		''' move cursor down with
+			ctrl-n
+		'''
+		
+		if self.state not in  [ 'normal', 'error' ]:
+			self.bell()
+			return "break"
+	
+		self.contents.event_generate('<<NextLine>>')
+		
+		return "break"
+	
+	
+##	def updown_override(self, event=None, direction=None):
+##		''' up-down override, to expand possibly incorrect indentation
+##		'''
+##
+##		if self.state != 'normal':
+##			return "continue"
+##
+##		oldpos = self.contents.index(tkinter.INSERT)
+##
+##
+##		if direction == 'down':
+##			newpos = self.contents.index( '%s + 1lines' % tkinter.INSERT)
+##
+##		# direction == 'up'
+##		else:
+##			newpos = self.contents.index( '%s - 1lines' % tkinter.INSERT)
+##
+##
+##		oldline = self.contents.get( '%s linestart' % oldpos, '%s lineend' % oldpos)
+##		newline = self.contents.get( '%s linestart' % newpos, '%s lineend' % newpos)
+##
+##
+##		if newline.isspace() or newline == '':
+##
+##			if oldline == '':
+##				return 'continue'
+##
+##			if not oldline.isspace():
+##
+##				tmp = oldline.lstrip()
+##				oldindent = oldline.index(tmp)
+##
+##				if oldindent == 0:
+##					return 'continue'
+##
+##				self.contents.delete('%s linestart' % newpos,'%s lineend' % newpos)
+##				self.contents.insert('%s linestart' % newpos, oldindent * '\t')
+##				return 'continue'
+##
+##			# coming from empty line:
+##			else:
+##				self.contents.delete('%s linestart' % newpos,'%s lineend' % newpos)
+##				self.contents.insert('%s linestart' % newpos, len(oldline) * '\t')
+##				return 'continue'
+##
+##		else:
+##			return 'continue'
+	
+	
+	def move_many_lines(self, event=None):
+		''' Move or select 10 lines from cursor.
+		'''
+		
+		if self.state != 'normal':
+			self.bell()
+			return "break"
+		
+		if event.widget != self.contents:
+			return
+		
+		
+		# Check if: not only ctrl (+shift) down, then return
+		if self.os_type == 'linux':
+			if event.state not in  [4, 5]: return
+		
+		elif self.os_type == 'windows':
+			if event.state not in [ 262156, 262148, 262157, 262149 ]: return
+				
+		
+		# Pressed Control + Shift + arrow up or down.
+		# Want: select 10 lines from cursor.
+		
+		# Pressed Control + arrow up or down.
+		# Want: move 10 lines from cursor.
+						
+		if event.keysym == 'Up':
+			e = '<<SelectPrevLine>>'
+			
+			if event.state not in [ 5, 262157, 262149 ]:
+				e = '<<PrevLine>>'
+			
+			for i in range(10):
+				self.contents.event_generate(e)
+				
+			return 'break'
+		
+		elif event.keysym == 'Down':
+			e = '<<SelectNextLine>>'
+			
+			if event.state not in [ 5, 262157, 262149 ]:
+				e = '<<NextLine>>'
+			
+			for i in range(10):
+				self.contents.event_generate(e)
+			
+			return 'break'
+		
+		else:
+			return
+			
+			
+	
+	def center_view(self, event=None, up=False):
+		''' Raise insertion-line
+		'''
+		if self.state != 'normal':
+			self.bell()
+			return "break"
+			
+		
+		num_lines = self.text_widget_height // self.bbox_height
+		num_scroll = num_lines // 3
+		pos = self.contents.index('insert')
+		#posint = int(float(self.contents.index('insert')))
+		# lastline of visible window
+		lastline_screen = int(float(self.contents.index("@0,65535")))
+		
+		# lastline
+		last = int(float(self.contents.index('end'))) - 1
+		curline = int(float(self.contents.index('insert'))) - 1
+		
+		
+		if up: num_scroll *= -1
+			
+		# if near fileend
+		elif curline + 2*num_scroll + 2 > last:
+			self.contents.insert(tkinter.END, num_scroll*'\n')
+			self.contents.mark_set('insert', pos)
+						
+		
+		# if near screen end
+		#elif curline + 2*num_scroll + 2 > lastline_screen:
+		self.contents.yview_scroll(num_scroll, 'units')
+		
+		
+		# No ensure_view, enable return to cursor by arrow keys
+		return "break"
+	
+	
+	def idx_lineend(self):
+	
+##		?submodifier? linestart
+##		Adjust the index to refer to the first index on the line. If the display submodifier is given, this is the first index on the display line, otherwise on the logical line.
+##
+##		?submodifier? lineend
+##		Adjust the index to refer to the last index on the line (the newline). If the display submodifier is given, this is the last index on the display line, otherwise on the logical line.
+
+		pos = self.contents.index( 'insert display lineend' )
+		return pos
+		
+			
+	def idx_linestart(self):
+		
+		# In case of wrapped lines
+		y_cursor = self.contents.bbox(tkinter.INSERT)[1]
+		p = self.contents.index( '@0,%s' % y_cursor )
+		p2 = self.contents.index( '%s linestart' % p )
+		
+		# is wrapped?
+		c1 = int(p.split('.')[1])
+		l2 = int(p2.split('.')[0])
+		
+		pos = None
+		# yes, put cursor start of line not the whole line:
+		if c1 != 0:
+			pos = p
+			
+		# no, so put cursor after indentation:
+		else:
+			tmp = self.contents.get( '%s linestart' % p2, '%s lineend' % p2 )
+			if len(tmp) > 0:
+				if not tmp.isspace():
+					tmp2 = tmp.lstrip()
+					indent = tmp.index(tmp2)
+					pos = self.contents.index( '%i.%i' % (l2, indent) )
+		
+		return pos
+		
+	
+
+	def select_by_words(self, event=None):
+		'''	Pressed ctrl or Alt + shift and arrow left or right.
+			Make <<SelectNextWord>> and <<SelectPrevWord>> to stop at lineends.
+		'''
+		if self.state not in [ 'normal', 'error', 'search', 'replace', 'replace_all' ]:
+			self.bell()
+			return "break"
+		
+		###########################################
+		# Get marknames: self.contents.mark_names()
+		# It gives something like this if there has been or is a selection:
+		# 'insert', 'current', 'tk::anchor1'.
+		# This: 'tk::anchor1' is name of the selection-start-mark
+		# used here as in self.anchorname below.
+		# This is done because adjusting only 'sel' -tags
+		# is not sufficient in selection handling, when not using
+		# builtin-events, <<SelectNextWord>> and <<SelectPrevWord>>.
+		###########################################
+
+
+		# Check if: ctrl + shift down.
+		# MacOS event is already checked.
+		if self.os_type == 'linux':
+			if event.state != 5: return
+		
+		elif self.os_type == 'windows':
+			if event.state not in [ 262157, 262149 ]: return
+		
+		
+		have_selection = len(self.contents.tag_ranges('sel')) > 0
+		selection_started_from_top = False
+		
+		if event.keysym == 'Right':
+			s = self.contents.index( 'insert')
+			e = self.idx_lineend()
+			idx_linestart = self.idx_linestart()
+			# empty line?
+			if not idx_linestart: return
+			t = self.contents.get(idx_linestart, e).strip()
+
+			
+			# tkinter.SEL_FIRST is always before tkinter.SEL_LAST
+			# no matter if selection started from top or bottom:
+			if have_selection:
+				sel_start = self.contents.index(tkinter.SEL_FIRST)
+				sel_end = self.contents.index(tkinter.SEL_LAST)
+				if s == sel_end:
+					selection_started_from_top = True
+
+				#else: selection_started_from_top = False
+
+			else:
+				selection_started_from_top = True
+				sel_start = s
+
+			
+			
+			##################### Right Real start:
+			
+			
+			self.contents.event_generate('<<NextWord>>')
+			i = self.contents.index( 'insert')
+
+			# Already at lineend, proceed to next line
+			if s == e:
+				if have_selection:
+					self.contents.tag_remove('sel', '1.0', tkinter.END)
+
+					if selection_started_from_top:
+						self.contents.mark_set(self.anchorname, sel_start)
+						self.contents.tag_add('sel', sel_start, i)
+					else:
+						self.contents.mark_set(self.anchorname, sel_end)
+						self.contents.tag_add('sel', i, sel_end)
+						
+				# No selection,
+				# no need to check direction of selection:
+				else:
+					self.contents.mark_set(self.anchorname, s)
+					self.contents.tag_add('sel', s, i)
+					
+				self.contents.mark_set('insert', i)
+
+			
+			# if i is over lineend:
+			# 	stop at lineend == e
+			elif self.contents.compare( e,'<',i ):
+				
+				if have_selection:
+					self.contents.tag_remove('sel', '1.0', tkinter.END)
+
+					if selection_started_from_top:
+						self.contents.mark_set(self.anchorname, sel_start)
+						self.contents.tag_add('sel', sel_start, e)
+					else:
+						self.contents.mark_set(self.anchorname, sel_end)
+						self.contents.tag_add('sel', e, sel_end)
+						
+				# No selection,
+				# no need to check direction of selection:
+				else:
+					self.contents.mark_set(self.anchorname, s)
+					self.contents.tag_add('sel', s, e)
+					
+				self.contents.mark_set('insert', e)
+
+
+			# i is on the current line:
+			# 	stop at i == nextword
+			else:
+				
+				if have_selection:
+					self.contents.tag_remove('sel', '1.0', tkinter.END)
+
+					if selection_started_from_top:
+						self.contents.mark_set(self.anchorname, sel_start)
+						self.contents.tag_add('sel', sel_start, i)
+						
+					else:
+						self.contents.mark_set(self.anchorname, sel_end)
+						self.contents.tag_add('sel', i, sel_end)
+						
+						
+				# No selection,
+				# no need to check direction of selection:
+				else:
+					self.contents.mark_set(self.anchorname, s)
+					self.contents.tag_add('sel', s, i)
+					
+					
+				self.contents.mark_set('insert', i)
+				
+				
+
+		elif event.keysym == 'Left':
+			s = self.contents.index( 'insert')
+			
+			# tkinter.SEL_FIRST is always before tkinter.SEL_LAST
+			# no matter if selection started from top or bottom:
+			if have_selection:
+				sel_start = self.contents.index(tkinter.SEL_FIRST)
+				sel_end = self.contents.index(tkinter.SEL_LAST)
+				if s != sel_start:
+					selection_started_from_top = True
+
+				#else: selection_started_from_top = False
+
+			else:
+				#selection_started_from_top = False
+				sel_end = s
+
+
+			i_orig = s
+			i_linestart = self.idx_linestart()
+			# empty line?
+			if not i_linestart: return
+			
+			
+			
+			##################### Left Real start:
+			
+			
+			self.contents.event_generate('<<PrevWord>>')
+			i_prevword = self.contents.index( 'insert')
+			
+
+			# Already at linestart, proceed over last word of prev line.
+			if i_orig == i_linestart:
+
+				if have_selection:
+					
+					self.contents.tag_remove('sel', '1.0', tkinter.END)
+
+					if selection_started_from_top:
+						self.contents.mark_set(self.anchorname, sel_start)
+						self.contents.tag_add('sel', sel_start, i_prevword)
+					else:
+						self.contents.mark_set(self.anchorname, sel_end)
+						self.contents.tag_add('sel', i_prevword, sel_end)
+						
+				# No selection,
+				# no need to check direction of selection:
+				else:
+					self.contents.mark_set(self.anchorname, s)
+					self.contents.tag_add('sel', i_prevword, s)
+					
+				self.contents.mark_set('insert', i_prevword)
+
+			
+			# if i_prevword is over(before) linestart:
+			# 	stop at linestart == i_linestart
+			elif self.contents.compare( i_prevword, '<', i_linestart):
+
+				if have_selection:
+					self.contents.tag_remove('sel', '1.0', tkinter.END)
+
+					if selection_started_from_top:
+						self.contents.mark_set(self.anchorname, sel_start)
+						self.contents.tag_add('sel', sel_start, i_linestart)
+					else:
+						self.contents.mark_set(self.anchorname, sel_end)
+						self.contents.tag_add('sel', i_linestart, sel_end)
+								
+				# No selection,
+				# no need to check direction of selection:
+				else:
+					self.contents.mark_set(self.anchorname, s)
+					self.contents.tag_add('sel', i_linestart, s)
+
+				self.contents.mark_set('insert', i_linestart)
+
+
+			# i_prevword is on the current line:
+			# 	stop at i_prevword
+			else:
+				if have_selection:
+					self.contents.tag_remove('sel', '1.0', tkinter.END)
+
+					if selection_started_from_top:
+						self.contents.mark_set(self.anchorname, sel_start)
+						self.contents.tag_add('sel', sel_start, i_prevword)
+					else:
+						self.contents.mark_set(self.anchorname, sel_end)
+						self.contents.tag_add('sel', i_prevword, sel_end)
+								
+				# No selection,
+				# no need to check direction of selection:
+				else:
+					self.contents.mark_set(self.anchorname, s)
+					self.contents.tag_add('sel', i_prevword, s)
+
+				self.contents.mark_set('insert', i_prevword)
+
+
+		return 'break'
+	
+	
+	def move_by_words(self, event=None):
+		'''	Pressed ctrl or Alt and arrow left or right.
+			Make <<NextWord>> and <<PrevWord>> to stop at lineends.
+		'''
+		if self.state not in [ 'normal', 'error', 'search', 'replace', 'replace_all' ]:
+			self.bell()
+			return "break"
+			
+		idx_linestart = self.idx_linestart()
+		# empty line?
+		if not idx_linestart: return
+		
+		
+		# Check if: not only ctrl down, then return
+		# MacOS event is already checked.
+		if self.os_type == 'linux':
+			if event.state != 4: return
+		
+		elif self.os_type == 'windows':
+			if event.state not in [ 262156, 262148 ]: return
+			
+		
+		# Check if near lineend, so stop there
+		if event.keysym == 'Right':
+			i_orig = self.contents.index( 'insert')
+			e = self.idx_lineend()
+			# Already at lineend, proceed over first word of next line
+			if i_orig == e: return
+			
+			self.contents.event_generate('<<NextWord>>')
+			i = self.contents.index( 'insert')
+			if self.contents.compare( e, '<', i ):
+				self.contents.mark_set('insert', e)
+				
+				
+		# Check if near linestart, so stop there
+		elif event.keysym == 'Left':
+			i_orig = self.contents.index( 'insert')
+			self.contents.event_generate('<<PrevWord>>')
+			i_prevword = self.contents.index( 'insert')
+			
+			self.contents.mark_set('insert', i_orig)
+			self.goto_linestart(event=event)
+			i_linestart = self.contents.index( 'insert')
+			
+			# Already at linestart, proceed over last word of prev line
+			if i_orig == i_linestart: return
+			
+			if self.contents.compare( i_prevword, '<', i_linestart ):
+				self.contents.mark_set('insert', i_linestart)
+			else:
+				self.contents.mark_set('insert', i_prevword)
+				
+
+		return 'break'
+	
+		
+	def check_sel(self, event=None):
+		'''	Pressed arrow left or right.
+			If have selection, put cursor on the wanted side of selection.
+		'''
+		
+		if self.state in  [ 'filedialog' ]:
+			self.bell()
+			return "break"
+	
+		
+		# self.contents or self.entry
+		wid = event.widget
+			
+		# Check if have shift etc. pressed. If is, return to default bindings.
+		# macOS event is already handled in mac_cmd_overrides.
+		# macOS event here is only plain arrow left or right and has selection.
+		if self.os_type != 'mac_os':
+			if self.os_type == 'linux' and event.state != 0: return
+			if self.os_type == 'windows' and event.state not in [ 262152, 262144 ]: return
+			
+			have_selection = False
+	
+			if wid == self.entry:
+				have_selection = self.entry.selection_present()
+	
+			elif wid == self.contents:
+				have_selection = len(self.contents.tag_ranges('sel')) > 0
+	
+			else:
+				return
+	
+			if not have_selection: return
+			
+		
+		s = wid.index(tkinter.SEL_FIRST)
+		e = wid.index(tkinter.SEL_LAST)
+		i = wid.index(tkinter.INSERT)
+		
+		if wid == self.contents:
+			
+			# Leave cursor where it is if have selected all
+			if s == self.contents.index('1.0') and e == self.contents.index(tkinter.END):
+				return
+			
+			self.contents.tag_remove('sel', '1.0', tkinter.END)
+			#self.wid.see('1.0')
+			
+			
+			if event.keysym == 'Right':
+				self.contents.mark_set('insert', e)
+				self.ensure_idx_visibility(e)
+				
+			elif event.keysym == 'Left':
+				self.contents.mark_set('insert', s)
+				self.ensure_idx_visibility(s)
+				
+			else:
+				return
+			
+				
+		if wid == self.entry:
+			self.entry.selection_clear()
+			
+			if event.keysym == 'Right':
+				self.entry.icursor(e)
+				self.entry.xview_moveto(1.0)
+				
+			elif event.keysym == 'Left':
+				
+				if self.state in ['search', 'replace', 'replace_all']:
+					tmp = self.entry.get()
+					s = tmp.index(':') + 2
+				
+				self.entry.icursor(s)
+				self.entry.xview_moveto(0)
+			
+			else:
+				return
+			
+		
+		return 'break'
+		
+	
+	def yank_line(self, event=None):
+		'''	copy current line to clipboard
+		'''
+		
+		if self.state not in [ 'normal', 'error', 'search', 'replace', 'replace_all' ]:
+			self.bell()
+			return "break"
+			
+			
+		curpos = self.contents.index(tkinter.INSERT)
+		t = self.contents.get('%s linestart' % curpos, '%s lineend' % curpos)
+		
+		
+		if t.strip() != '':
+			self.goto_linestart(event=event)
+			s = self.contents.index( 'insert' )
+			e = self.contents.index( '%s lineend' % curpos )
+			
+			# return cursor back to original place
+			self.contents.mark_set('insert', curpos)
+		
+			tmp = self.contents.get(s,e)
+			self.contents.clipboard_clear()
+			
+			self.contents.tag_remove('sel', '1.0', tkinter.END)
+			self.contents.tag_add('sel', s, e)
+		
+			if self.os_type != 'windows':
+				self.contents.clipboard_append(tmp)
+			else:
+				self.copy_windows(event=event)
+			
+			self.after(600, lambda args=['sel', '1.0', tkinter.END]: self.contents.tag_remove(*args) )
+		
+			
+		return 'break'
+		
+		
+	def goto_lineend(self, event=None):
+		if self.state in [ 'filedialog' ]:
+			self.bell()
+			return "break"
+		
+		
+		wid = event.widget
+		if wid == self.entry:
+			wid.selection_clear()
+			idx = tkinter.END
+			wid.icursor(idx)
+			wid.xview_moveto(1.0)
+			return 'break'
+		
+		
+		idx_linestart = self.idx_linestart()
+		# Empty line?
+		if not idx_linestart: return "break"
+		
+		
+		have_selection = False
+		want_selection = False
+		
+		# ctrl-(shift)?-a or e
+		# and cmd-a or e in macOS
+		
+		# If want selection:
+		
+		# Pressed also shift, so adjust selection
+		# Linux, macOS state:
+		# ctrl-shift == 5
+		
+		# Windows state:
+		# ctrl-shift == 13
+		
+		# Also in mac_OS:
+		# command-shift-arrowleft or right == 105
+		# Note: command-shift-a or e not binded.
+		
+		# If want selection:
+		if event.state in [ 5, 105, 13 ]:
+			want_selection = True
+			i = self.contents.index(tkinter.INSERT)
+				
+			if len( self.contents.tag_ranges('sel') ) > 0:
+				# Need to know if selection started from top or bottom.
+				
+				
+				have_selection = True
+				s = self.contents.index(tkinter.SEL_FIRST)
+				e = self.contents.index(tkinter.SEL_LAST)
+				
+				# Selection started from top
+				from_top = False
+				if self.contents.compare(s,'<',i):
+					from_top = True
+					
+				# From bottom
+				# else:	from_top = False
+		
+		
+		# Dont want selection, ctrl/cmd-a/e:
+		else:
+			self.contents.tag_remove('sel', '1.0', tkinter.END)
+		
+		
+		self.ensure_idx_visibility('insert')
+		
+		pos = self.idx_lineend()
+		
+		self.contents.see(pos)
+		self.contents.mark_set('insert', pos)
+		
+		
+		if want_selection:
+			if have_selection:
+				self.contents.tag_remove('sel', '1.0', tkinter.END)
+					
+				if from_top:
+					self.contents.mark_set(self.anchorname, s)
+					self.contents.tag_add('sel', s, 'insert')
+				
+				# From bottom:
+				else:
+					self.contents.mark_set(self.anchorname, e)
+					self.contents.tag_add('sel', 'insert', e)
+				
+			else:
+				self.contents.mark_set(self.anchorname, i)
+				self.contents.tag_add('sel', i, 'insert')
+		
+		
+		return "break"
+		
+		
+	def goto_linestart(self, event=None):
+		if self.state in [ 'filedialog' ]:
+			self.bell()
+			return "break"
+		
+		wid = event.widget
+		if wid == self.entry:
+			wid.selection_clear()
+			idx = 0
+			if self.state in ['search', 'replace', 'replace_all']:
+				tmp = wid.get()
+				idx = tmp.index(':') + 2
+			
+			wid.icursor(idx)
+			wid.xview_moveto(0)
+			return 'break'
+			
+		
+		idx_linestart = self.idx_linestart()
+		# Empty line?
+		if not idx_linestart: return "break"
+		
+		
+		have_selection = False
+		want_selection = False
+		
+		# ctrl-(shift)?-a or e
+		# and cmd-a or e in macOS
+		
+		# If want selection:
+		
+		# Pressed also shift, so adjust selection
+		# Linux, macOS state:
+		# ctrl-shift == 5
+		
+		# Windows state:
+		# ctrl-shift == 13
+		
+		# Also in mac_OS:
+		# command-shift-arrowleft or right == 105
+		# Note: command-shift-a or e not binded.
+		
+		# If want selection:
+		if event.state in [ 5 , 105, 13 ]:
+			want_selection = True
+			i = self.contents.index(tkinter.INSERT)
+				
+			if len( self.contents.tag_ranges('sel') ) > 0:
+				# Need to know if selection started from top or bottom.
+				
+				
+				have_selection = True
+				s = self.contents.index(tkinter.SEL_FIRST)
+				e = self.contents.index(tkinter.SEL_LAST)
+				
+				# Selection started from top
+				from_top = False
+				if self.contents.compare(s,'<',i):
+					from_top = True
+					
+				# From bottom
+				# else:	from_top = False
+		
+		
+		# Dont want selection, ctrl/cmd-a/e:
+		else:
+			self.contents.tag_remove('sel', '1.0', tkinter.END)
+			
+		
+		self.ensure_idx_visibility('insert')
+		
+		pos = self.idx_linestart()
+		
+		self.contents.see(pos)
+		self.contents.mark_set('insert', pos)
+	
+		if want_selection:
+			
+			if have_selection:
+				self.contents.tag_remove('sel', '1.0', tkinter.END)
+				
+				if from_top:
+					self.contents.mark_set(self.anchorname, s)
+					self.contents.tag_add('sel', s, 'insert')
+				
+				# From bottom
+				else:
+					self.contents.mark_set(self.anchorname, e)
+					self.contents.tag_add('sel', 'insert', e)
+				
+			else:
+				self.contents.mark_set(self.anchorname, i)
+				self.contents.tag_add('sel', 'insert', i)
+					
+		
+		return "break"
+
+########## Select and move End
+########## Overrides Begin
+
+	def raise_popup(self, event=None):
+		if self.state != 'normal':
+			self.bell()
+			return "break"
+		
+		self.popup.post(event.x_root, event.y_root)
+		self.popup.focus_set() # Needed to remove popup when clicked outside.
+		
+		
+	def popup_focusOut(self, event=None):
+		self.popup.unpost()
+	
+	
+	def copy(self):
+		''' When copy is selected from popup-menu
+		'''
+		if self.os_type == 'windows':
+			self.copy_windows()
+		
+		else:
+			try:
+				self.clipboard_clear()
+				self.clipboard_append(self.selection_get())
+			except tkinter.TclError:
+				# is empty
+				return 'break'
+		
+
+	def move_line(self, event=None, direction=None):
+		''' Adjust cursor line indentation, with arrow left and right,
+			when pasting more than one line etc.
+		'''
+		
+		# currently this interferes with backspace_override
+		
+		# Enable continue adjusting selection area.
+		# 262152 is state when pressing arrow left-right in Win11, 262144 in Win10
+		if self.state != 'normal' or event.state not in [0, 262152, 262144 ]:
+			return 'continue'
+			
+			
+		if len(self.contents.tag_ranges('sel')) > 0:
+			insert_at_selstart = False
+			
+			s = self.contents.index(tkinter.SEL_FIRST)
+			e = self.contents.index(tkinter.SEL_LAST)
+			i = self.contents.index(tkinter.INSERT)
+			# contents of line with cursor:
+			t = self.contents.get('%s linestart' % i, '%s lineend' % i)
+			
+			if i == s:
+				insert_at_selstart = True
+			
+			# else: insert at selend
+			
+			line_s = s.split('.')[0]
+			line_e = e.split('.')[0]
+			
+			# One line only:
+			if line_s == line_e: 	return 'continue'
+
+			# cursor line is empty:
+			if len(t.strip()) == 0: return 'continue'
+
+
+			self.contents.tag_remove('sel', '1.0', tkinter.END)
+			self.contents.tag_add('sel', '%s linestart' % i, '%s lineend' % i)
+
+
+			if direction == 'left':
+
+				# Cursor at the start of the line, or there is no indentation left:
+				if i.split('.')[1] == 0 or not t[0].isspace():
+					self.contents.tag_remove('sel', '1.0', tkinter.END)
+					self.contents.tag_add('sel', s, e)
+					return 'break'
+
+				self.unindent()
+				self.contents.tag_remove('sel', '1.0', tkinter.END)
+
+				if insert_at_selstart:
+					self.contents.tag_add('sel',  '%s -1c' % s, e)
+				else:
+					self.contents.tag_add('sel', s, '%s -1c' % e)
+
+			# right
+			else:
+				self.indent()
+				self.contents.tag_remove('sel', '1.0', tkinter.END)
+
+				if insert_at_selstart:
+					self.contents.tag_add('sel',  '%s +1c' % s, e)
+				else:
+					self.contents.tag_add('sel', s, '%s +1c' % e)
+					
+
+			return 'break'
+
+		return 'continue'
+	
+
+	def paste(self, event=None):
+		'''	First line usually is in wrong place after paste
+			because of selection has not started at the beginning of the line.
+			So we put cursor at the beginning of insertion after pasting it
+			so we can start indenting it.
+		'''
+		
+		try:
+			tmp = self.clipboard_get()
+			tmp = tmp.splitlines(keepends=True)
+			
+			
+		except tkinter.TclError:
+			# is empty
+			return 'break'
+			
+		have_selection = False
+		
+		if len( self.contents.tag_ranges('sel') ) > 0:
+			selstart = self.contents.index( '%s' % tkinter.SEL_FIRST)
+			selend = self.contents.index( '%s' % tkinter.SEL_LAST)
+			
+			self.contents.tag_remove('sel', '1.0', tkinter.END)
+			have_selection = True
+			
+			
+		line = self.contents.index(tkinter.INSERT)
+		self.contents.event_generate('<<Paste>>')
+		
+		
+		# Selected many lines or
+		# one line and cursor is not at the start of next line:
+		if len(tmp) > 1:
+		
+			s = self.contents.index( '%s linestart' % line)
+			e = self.contents.index( 'insert lineend')
+			t = self.contents.get( s, e )
+			
+			if self.tabs[self.tabindex].filepath:
+				if self.can_do_syntax():
+					self.update_tokens( start=s, end=e, line=t )
+					
+			
+			if have_selection:
+				self.contents.tag_add('sel', selstart, selend)
+				
+			else:
+				self.contents.tag_add('sel', line, tkinter.INSERT)
+				
+			self.contents.mark_set('insert', line)
+			
+			
+			self.wait_for(100)
+			self.ensure_idx_visibility(line)
+			
+			
+		# Selected one line and cursor is at the start of next line:
+		elif len(tmp) == 1 and tmp[-1][-1] == '\n':
+			s = self.contents.index( '%s linestart' % line)
+			e = self.contents.index( '%s lineend' % line)
+			t = self.contents.get( s, e )
+			
+			if self.tabs[self.tabindex].filepath:
+				if self.can_do_syntax():
+					self.update_tokens( start=s, end=e, line=t )
+					
+					
+		return 'break'
+	
+
+	def undo_override(self, event=None):
+		if self.state != 'normal':
+			self.bell()
+			return "break"
+		 
+		try:
+			self.contents.edit_undo()
+			
+			
+			self.do_syntax()
+			
+			
+		except tkinter.TclError:
+			self.bell()
+			
+		return 'break'
+		
+		
+	def redo_override(self, event=None):
+		if self.state != 'normal':
+			self.bell()
+			return "break"
+			
+		try:
+			self.contents.edit_redo()
+			
+			
+			self.do_syntax()
+			
+			
+		except tkinter.TclError:
+			self.bell()
+			
+		return 'break'
+		
+		
+	def select_all(self, event=None):
+		self.contents.tag_remove('sel', '1.0', tkinter.END)
+		self.contents.tag_add('sel', 1.0, tkinter.END)
+		return "break"
+	
+	
+	def space_override(self, event):
+		'''	Used to bind Space-key when searching or replacing.
+		'''
+		
+		if self.state not in [ 'search', 'replace', 'replace_all' ]:
+			return
+		
+		# self.search_idx marks range of focus-tag:
+		self.save_pos = self.search_idx[1]
+		self.stop_search()
+		
+		return 'break'
+	
+	
+	def tab_override(self, event):
+		'''	Used to bind Tab-key with indent() and expander.expand_word()
+		'''
+		
+		if self.state in [ 'search', 'replace', 'replace_all' ]:
+			return 'break'
+		
+		# In Windows, Tab-key-event has state 8 and shift+Tab has state 9,
+		# so because shift-tab is unbinded if in Windows, we check that here
+		# and unindent if it is the state.
+		if hasattr(event, 'state'):
+			
+			if self.os_type == 'windows':
+				
+				if event.state == 9:
+					self.unindent()
+					return 'break'
+					
+				if event.state not in [8, 0]:
+					return
+			
+			elif event.state != 0:
+				return
+				
+		# Fix for tab-key not working sometimes.
+		# This happens because os-clipboard content is (automatically)
+		# added to selection content of a Text widget, and since there is no
+		# actual selection (clipboard-text is outside from Text-widget),
+		# tab_override() gets quite broken.
+		
+		if len(self.contents.tag_ranges('sel')) == 0:
+			
+			# Expand word Begin
+			pos = self.contents.index(tkinter.INSERT)
+			lineend = '%s lineend' % pos
+			linestart = '%s linestart' % pos
+			tmp = self.contents.get( linestart, lineend )
+			startline, startcol = map(int, pos.split(sep='.') )
+			
+			prev_char = None
+			next_char = None
+			
+			
+			# Check not at the indent 0:
+			if startcol > 0:
+				prev_char = tmp[startcol-1:startcol]
+				
+			else:
+				return
+			
+			
+			if prev_char and ( prev_char in self.expander.wordchars ):
+				self.expander.expand_word()
+				return 'break'
+				
+			else:
+				return
+				
+			# Expand word End
+			
+		try:
+			tmp = self.contents.selection_get()
+			self.indent(event)
+			return 'break'
+			
+		except tkinter.TclError:
+			# No selection
+			return
+
+	
+	def backspace_override(self, event):
+		""" for syntax highlight
+		"""
+		
+		# State is 8 in windows when no other keys are pressed
+		if self.state != 'normal' or event.state not in [0, 8]:
+			return
+		
+		pars = [ '(', ')', '[', ']' , '{', '}' ]
+		
+		try:
+			
+			# Is there a selection?
+			if len(self.contents.tag_ranges('sel')) > 0:
+				tmp = self.contents.selection_get()
+				l = [ x for x in tmp if x in pars ]
+				if len(l) > 0:
+					self.par_err = True
+				
+			self.contents.delete( tkinter.SEL_FIRST, tkinter.SEL_LAST )
+			
+			self.do_syntax()
+			
+			return 'break'
+			
+				
+		except tkinter.TclError:
+			# Deleting one letter
+			
+			
+			# Rest is multiline string check
+			chars = self.contents.get( '%s - 3c' % tkinter.INSERT, '%s + 2c' % tkinter.INSERT )
+			
+			triples = ["'''", '"""']
+			doubles = ["''", '""']
+			singles = ["'", '"']
+			
+			prev_3chars = chars[:3]
+			prev_2chars = chars[1:3]
+			next_2chars = chars[-2:]
+			
+			prev_char = chars[2:3]
+			next_char = chars[-2:-1]
+		
+			quote_tests = [
+						(prev_char == '#'),
+						(prev_3chars in triples),
+						( (prev_2chars in doubles) and (next_char in singles) ),
+						( (prev_char in singles) and (next_2chars in doubles) )
+						]
+						
+			if any(quote_tests):
+				#print('#')
+				self.token_err = True
+				
+				
+			# To trigger parcheck if only one of these was in line and it was deleted:
+			if prev_char in pars:
+				self.par_err = True
+				
+				
+		#print('deleting')
+				
+		return
+
+	
+	def return_override(self, event):
+		if self.state != 'normal':
+			self.bell()
+			return "break"
+		
+		
+		# macOS, open file with cmd-return:
+		if self.os_type == 'mac_os' and event.state == 8:
+			self.btn_open.invoke()
+			return 'break'
+		
+		
+		# Cursor indexes when pressed return:
+		line, col = map(int, self.contents.index(tkinter.INSERT).split('.'))
+		
+		
+		# First an easy case:
+		if col == 0:
+			self.contents.insert(tkinter.INSERT, '\n')
+			self.contents.see(f'{line+1}.0')
+			self.contents.edit_separator()
+			return "break"
+			
+		
+		tmp = self.contents.get('%s.0' % str(line),'%s.0 lineend' % str(line))
+		
+		# Then one special case: check if cursor is inside indentation,
+		# and line is not empty.
+		if tmp[:col].isspace() and not tmp[col:].isspace():
+			self.contents.insert(tkinter.INSERT, '\n')
+			self.contents.insert('%s.0' % str(line+1), tmp[:col])
+			self.contents.see(f'{line+1}.0')
+			self.contents.edit_separator()
+			return "break"
+			
+		else:
+			# rstrip space to prevent indentation sailing.
+			if tmp[col:].isspace():
+				self.contents.delete(tkinter.INSERT, 'insert lineend')
+				
+			for i in range(len(tmp[:col]) + 1):
+				if tmp[i] != '\t':
+					break
+	
+			self.contents.insert(tkinter.INSERT, '\n') # Manual newline because return is overrided.
+			self.contents.insert(tkinter.INSERT, i*'\t')
+			self.contents.see(f'{line+1}.0')
+			self.contents.edit_separator()
+			return "break"
+			
+			
+	def sbset_override(self, *args):
+		'''	Fix for: not being able to config slider min-size
+		'''
+		self.scrollbar.set(*args)
+		
+		h = self.text_widget_height
+
+		# Relative position (tuple on two floats) of
+		# slider-top (a[0]) and -bottom (a[1]) in scale 0-1, a[0] is smaller:
+		a = self.scrollbar.get()
+
+		# current slider size:
+		# (a[1]-a[0])*h
+
+		# want to set slider size to at least p (SLIDER_MINSIZE) pixels,
+		# by adding relative amount(0-1) of d to slider, that is: d/2 to both ends:
+		# ( a[1]+d/2 - (a[0]-d/2) )*h = p
+		# a[1] - a[0] + d = p/h
+		# d = p/h - a[1] + a[0]
+
+
+		d = SLIDER_MINSIZE/h - a[1] + a[0]
+
+		if h*(a[1] - a[0]) < SLIDER_MINSIZE:
+			self.scrollbar.set(a[0], a[1]+d)
+		
+		self.update_linenums()
+		
+########## Overrides End
+########## Utilities Begin
+
+	def insert_inspected(self):
+		''' Tries to inspect selection. On success: opens new tab and pastes lines there.
+			New tab can be safely closed with ctrl-d later, or saved with new filename.
+		'''
+		try:
+			target = self.contents.selection_get()
+		except tkinter.TclError:
+			self.bell()
+			return 'break'
+		
+		target=target.strip()
+		
+		if not len(target) > 0:
+			self.bell()
+			return 'break'
+		
+		
+		import inspect
+		is_module = False
+		
+		try:
+			mod = importlib.import_module(target)
+			is_module = True
+			filepath = inspect.getsourcefile(mod)
+			
+			if not filepath:
+				# for example: readline
+				self.bell()
+				print('Could not inspect:', target, '\nimport and use help()')
+				return 'break'
+			
+			try:
+				with open(filepath, 'r', encoding='utf-8') as f:
+					fcontents = f.read()
+					self.new_tab()
+					
+					# just in case:
+					if '.py' in filepath:
+						indentation_is_alien, indent_depth = self.check_indent_depth(fcontents)
+						
+						if indentation_is_alien:
+							# Assuming user wants self.ind_depth, change it without notice:
+							tmp = fcontents.splitlines(True)
+							tmp[:] = [self.tabify(line, width=indent_depth) for line in tmp]
+							tmp = ''.join(tmp)
+							self.tabs[self.tabindex].contents = tmp
+				
+						else:
+							self.tabs[self.tabindex].contents = fcontents
+					else:
+						self.tabs[self.tabindex].contents = fcontents
+				
+					
+					self.tabs[self.tabindex].position = '1.0'
+					self.contents.focus_set()
+					self.contents.see('1.0')
+					self.contents.mark_set('insert', '1.0')
+					self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
+					
+					if self.syntax:
+						self.token_err = True
+						self.update_tokens(start='1.0', end=tkinter.END)
+						self.token_can_update = True
+						
+					else:
+						self.token_can_update = False
+						
+						
+					self.contents.edit_reset()
+					self.contents.edit_modified(0)
+					
+					return 'break'
+					
+			except (EnvironmentError, UnicodeDecodeError) as e:
+				print(e.__str__())
+				print(f'\n Could not open file: {filepath}')
+				self.bell()
+				return 'break'
+					
+		except ModuleNotFoundError:
+			print(f'\n Is not a module: {target}')
+		except TypeError as ee:
+			print(ee.__str__())
+			self.bell()
+			return 'break'
+			
+			
+		if not is_module:
+		
+			try:
+				modulepart = target[:target.rindex('.')]
+				object_part = target[target.rindex('.')+1:]
+				mod = importlib.import_module(modulepart)
+				target_object = getattr(mod, object_part)
+				
+				l = inspect.getsourcelines(target_object)
+				t = ''.join(l[0])
+				
+				self.new_tab()
+				
+				# just in case:
+				indentation_is_alien, indent_depth = self.check_indent_depth(t)
+				
+				if indentation_is_alien:
+					# Assuming user wants self.ind_depth, change it without notice:
+					tmp = t.splitlines(True)
+					tmp[:] = [self.tabify(line, width=indent_depth) for line in tmp]
+					tmp = ''.join(tmp)
+					self.tabs[self.tabindex].contents = tmp
+					
+				else:
+					self.tabs[self.tabindex].contents = t
+				
+				
+				self.tabs[self.tabindex].position = '1.0'
+				self.contents.focus_set()
+				self.contents.see('1.0')
+				self.contents.mark_set('insert', '1.0')
+				self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
+				
+				if self.syntax:
+					self.token_err = True
+					self.update_tokens(start='1.0', end=tkinter.END)
+					self.token_can_update = True
+					
+				else:
+					self.token_can_update = False
+				
+											
+				self.contents.edit_reset()
+				self.contents.edit_modified(0)
+				
+				return 'break'
+			
+			# from .rindex()
+			except ValueError:
+				self.bell()
+				return 'break'
+				
+			except Exception as e:
+				self.bell()
+				print(e.__str__())
+				return 'break'
+		
+		return 'break'
+	
+	
+	def tabify_lines(self, event=None):
+	
+		try:
+			startline = self.contents.index(tkinter.SEL_FIRST).split(sep='.')[0]
+			endline = self.contents.index(tkinter.SEL_LAST).split(sep='.')[0]
+			
+			start = '%s.0' % startline
+			end = '%s.0 lineend' % endline
+			tmp = self.contents.get(start, end)
+			
+			indentation_is_alien, indent_depth = self.check_indent_depth(tmp)
+			
+			tmp = tmp.splitlines()
+			
+			if indentation_is_alien:
+				# Assuming user wants self.ind_depth, change it without notice:
+				tmp[:] = [self.tabify(line, width=indent_depth) for line in tmp]
+							
+			else:
+				tmp[:] = [self.tabify(line) for line in tmp]
+			
+						
+			tmp = ''.join(tmp)
+			
+			self.contents.delete(start, end)
+			self.contents.insert(start, tmp)
+			
+			
+			self.update_tokens(start=start, end=end)
+						
+															
+			self.contents.edit_separator()
+			return "break"
+		
+		except tkinter.TclError as e:
+			#print(e)
+			return "break"
+	
+	
+	def tabify(self, line, width=None):
+		
+		if width:
+			ind_width = width
+		else:
+			ind_width = self.ind_depth
+			
+		indent_stop_index = 0
+		
+		for char in line:
+			if char in [' ', '\t']: indent_stop_index += 1
+			else: break
+			
+		if indent_stop_index == 0:
+			# remove trailing space
+			if not line.isspace():
+				line = line.rstrip() + '\n'
+				
+			return line
+		
+		
+		indent_string = line[:indent_stop_index]
+		line = line[indent_stop_index:]
+		
+		# remove trailing space
+		line = line.rstrip() + '\n'
+		
+		
+		count = 0
+		for char in indent_string:
+			if char == '\t':
+				count = 0
+				continue
+			if char == ' ': count += 1
+			if count == ind_width:
+				indent_string = indent_string.replace(ind_width * ' ', '\t', True)
+				count = 0
+		
+		tabified_line = ''.join([indent_string, line])
+		
+		return tabified_line
+	
+	
+
+########## Utilities End
+########## Save and Load Begin
+
+	
+	def trace_filename(self, *args):
+		
+		# canceled
+		if self.tracevar_filename.get() == '':
+			self.entry.delete(0, tkinter.END)
+			
+			if self.tabs[self.tabindex].filepath != None:
+				self.entry.insert(0, self.tabs[self.tabindex].filepath)
+				self.entry.xview_moveto(1.0)
+				
+		else:
+			# update self.lastdir
+			filename = pathlib.Path().cwd() / self.tracevar_filename.get()
+			self.lastdir = pathlib.Path(*filename.parts[:-1])
+		
+			self.loadfile(filename)
+		
+		
+		self.tracevar_filename.trace_remove('write', self.tracefunc_name)
+		self.tracefunc_name = None
+		self.contents.bind( "<Alt-Return>", lambda event: self.btn_open.invoke())
+		
+		self.state = 'normal'
+		
+	
+		for widget in [self.entry, self.btn_open, self.btn_save, self.contents]:
+			widget.config(state='normal')
+		
+		return 'break'
+		
+			
+	def loadfile(self, filepath):
+		''' filepath is tkinter.pathlib.Path
+		'''
+
+		filename = filepath
+		openfiles = [tab.filepath for tab in self.tabs]
+		
+		for widget in [self.entry, self.btn_open, self.btn_save, self.contents]:
+			widget.config(state='normal')
+		
+		
+		if filename in openfiles:
+			print(f'file: {filename} is already open')
+			self.bell()
+			self.entry.delete(0, tkinter.END)
+			
+			if self.tabs[self.tabindex].filepath != None:
+				self.entry.insert(0, self.tabs[self.tabindex].filepath)
+				self.entry.xview_moveto(1.0)
+				
+			return
+		
+		if self.tabs[self.tabindex].type == 'normal':
+			self.save(activetab=True)
+		
+		# Using same tab:
+		try:
+			with open(filename, 'r', encoding='utf-8') as f:
+				tmp = f.read()
+				self.tabs[self.tabindex].oldcontents = tmp
+				
+				if '.py' in filename.suffix:
+					indentation_is_alien, indent_depth = self.check_indent_depth(tmp)
+					
+					if indentation_is_alien:
+						# Assuming user wants self.ind_depth, change it without notice:
+						tmp = self.tabs[self.tabindex].oldcontents.splitlines(True)
+						tmp[:] = [self.tabify(line, width=indent_depth) for line in tmp]
+						tmp = ''.join(tmp)
+						self.tabs[self.tabindex].contents = tmp
+						
+					else:
+						self.tabs[self.tabindex].contents = self.tabs[self.tabindex].oldcontents
+				else:
+					self.tabs[self.tabindex].contents = self.tabs[self.tabindex].oldcontents
+				
+			
+				
+				self.entry.delete(0, tkinter.END)
+				self.tabs[self.tabindex].filepath = filename
+				self.tabs[self.tabindex].type = 'normal'
+				self.tabs[self.tabindex].position = '1.0'
+				self.entry.insert(0, filename)
+				self.entry.xview_moveto(1.0)
+				
+				
+				self.contents.delete('1.0', tkinter.END)
+				self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
+				
+				
+				self.do_syntax(everything=True)
+				
+				
+				self.contents.focus_set()
+				self.contents.see('1.0')
+				self.contents.mark_set('insert', '1.0')
+				
+				self.contents.edit_reset()
+				self.contents.edit_modified(0)
+				self.avoid_viewsync_mess()
+				
+		except (EnvironmentError, UnicodeDecodeError) as e:
+			print(e.__str__())
+			print(f'\n Could not open file: {filename}')
+			self.entry.delete(0, tkinter.END)
+			
+			if self.tabs[self.tabindex].filepath != None:
+				self.entry.insert(0, self.tabs[self.tabindex].filepath)
+				self.entry.xview_moveto(1.0)
+				
+		return
+		
+	
+	def load(self, event=None):
+		'''	Get just the filename,
+			on success, pass it to loadfile()
+		'''
+		
+		if self.state != 'normal':
+			self.bell()
+			return 'break'
+		
+		
+		# Pressed Open-button
+		if event == None:
+		
+			self.state = 'filedialog'
+			self.contents.bind( "<Alt-Return>", self.do_nothing)
+			
+			for widget in [self.entry, self.btn_open, self.btn_save, self.contents]:
+				widget.config(state='disabled')
+				
+			self.tracevar_filename.set('empty')
+			self.tracefunc_name = self.tracevar_filename.trace_add('write', self.trace_filename)
+			
+			p = pathlib.Path().cwd()
+			
+			if self.lastdir:
+				p = p / self.lastdir
+			
+			filetop = tkinter.Toplevel()
+			filetop.title('Select File')
+			self.to_be_closed.append(filetop)
+			
+			
+			fd = fdialog.FDialog(filetop, p, self.tracevar_filename, font=self.font, menufont=self.menufont, os_type=self.os_type)
+			
+			return 'break'
+			
+
+		# Entered filename to be opened in entry:
+		else:
+			tmp = self.entry.get().strip()
+
+			if not isinstance(tmp, str) or tmp.isspace():
+				self.bell()
+				return 'break'
+	
+			filename = pathlib.Path().cwd() / tmp
+			
+			self.loadfile(filename)
+			
+			return 'break'
+
+					
+	def save(self, activetab=False, forced=False):
+		''' forced when run() or quit_me()
+			activetab=True from load() and del_tab()
+		'''
+		
+		if forced:
+			
+			# Dont want contents to be replaced with errorlines or help.
+			if self.state != 'normal':
+				self.contents.event_generate('<Escape>')
+			
+			# update active tab first
+			try:
+				pos = self.contents.index(tkinter.INSERT)
+			except tkinter.TclError:
+				pos = '1.0'
+				
+			tmp = self.contents.get('1.0', tkinter.END)
+	
+			self.tabs[self.tabindex].position = pos
+			self.tabs[self.tabindex].contents = tmp
+			
+			
+			# Then save tabs to disk
+			for tab in self.tabs:
+				if tab.type == 'normal':
+					
+					# Check indent (tabify) and rstrip:
+					tmp = tab.contents.splitlines(True)
+					tmp[:] = [self.tabify(line) for line in tmp]
+					tmp = ''.join(tmp)
+					
+					if tab.active == True:
+						tmp = tmp[:-1]
+					
+					tab.contents = tmp
+					
+					if tab.contents == tab.oldcontents:
+						continue
+					
+					try:
+						with open(tab.filepath, 'w', encoding='utf-8') as f:
+							f.write(tab.contents)
+							tab.oldcontents = tab.contents
+							
+					except EnvironmentError as e:
+						print(e.__str__())
+						print(f'\n Could not save file: {tab.filepath}')
+				else:
+					tab.position = '1.0'
+					
+			return
+
+		# if not forced (Pressed Save-button):
+
+		tmp = self.entry.get().strip()
+		
+		if not isinstance(tmp, str) or tmp.isspace():
+			print('Give a valid filename')
+			self.bell()
+			return
+		
+		fpath_in_entry = pathlib.Path().cwd() / tmp
+		
+		try:
+			pos = self.contents.index(tkinter.INSERT)
+		except tkinter.TclError:
+			pos = '1.0'
+					
+		tmp = self.contents.get('1.0', tkinter.END)
+		
+		self.tabs[self.tabindex].position = pos
+		self.tabs[self.tabindex].contents = tmp
+
+		openfiles = [tab.filepath for tab in self.tabs]
+		
+		
+		# creating new file
+		if fpath_in_entry != self.tabs[self.tabindex].filepath and not activetab:
+		
+			if fpath_in_entry in openfiles:
+				self.bell()
+				print(f'\nFile: {fpath_in_entry} already opened')
+				self.entry.delete(0, tkinter.END)
+			
+				if self.tabs[self.tabindex].filepath != None:
+					self.entry.insert(0, self.tabs[self.tabindex].filepath)
+					self.entry.xview_moveto(1.0)
+					
+				return
+				
+			if fpath_in_entry.exists():
+				self.bell()
+				print(f'\nCan not overwrite file: {fpath_in_entry}')
+				self.entry.delete(0, tkinter.END)
+			
+				if self.tabs[self.tabindex].filepath != None:
+					self.entry.insert(0, self.tabs[self.tabindex].filepath)
+					self.entry.xview_moveto(1.0)
+					
+				return
+			
+			if self.tabs[self.tabindex].type == 'newtab':
+			
+				# avoiding disk-writes, just checking filepath:
+				try:
+					with open(fpath_in_entry, 'w', encoding='utf-8') as f:
+						self.tabs[self.tabindex].filepath = fpath_in_entry
+						self.tabs[self.tabindex].type = 'normal'
+				except EnvironmentError as e:
+					print(e.__str__())
+					print(f'\n Could not save file: {fpath_in_entry}')
+					return
+				
+				if self.tabs[self.tabindex].filepath != None:
+					self.entry.delete(0, tkinter.END)
+					self.entry.insert(0, self.tabs[self.tabindex].filepath)
+					self.entry.xview_moveto(1.0)
+					
+					self.do_syntax()
+			
+				
+				# set cursor pos
+				try:
+					line = self.tabs[self.tabindex].position
+					self.contents.focus_set()
+					self.contents.mark_set('insert', line)
+					self.ensure_idx_visibility(line)
+					
+				except tkinter.TclError:
+					self.tabs[self.tabindex].position = '1.0'
+				
+				self.contents.edit_reset()
+				self.contents.edit_modified(0)
+				
+					
+				
+			# want to create new file with same contents:
+			else:
+				try:
+					with open(fpath_in_entry, 'w', encoding='utf-8') as f:
+						pass
+				except EnvironmentError as e:
+					print(e.__str__())
+					print(f'\n Could not save file: {fpath_in_entry}')
+					self.entry.delete(0, tkinter.END)
+			
+					if self.tabs[self.tabindex].filepath != None:
+						self.entry.insert(0, self.tabs[self.tabindex].filepath)
+						self.entry.xview_moveto(1.0)
+						
+					return
+					
+				self.new_tab()
+				self.tabs[self.tabindex].filepath = fpath_in_entry
+				self.tabs[self.tabindex].contents = tmp
+				self.tabs[self.tabindex].position = pos
+				self.tabs[self.tabindex].type = 'normal'
+				
+				self.entry.delete(0, tkinter.END)
+				self.entry.insert(0, self.tabs[self.tabindex].filepath)
+				self.entry.xview_moveto(1.0)
+				
+			
+				self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
+		
+				
+				self.do_syntax(everything=True)
+				
+				
+				# set cursor pos
+				try:
+					line = self.tabs[self.tabindex].position
+					self.contents.focus_set()
+					self.contents.mark_set('insert', line)
+					self.ensure_idx_visibility(line)
+					
+				except tkinter.TclError:
+					self.tabs[self.tabindex].position = '1.0'
+				
+				
+				self.contents.edit_reset()
+				self.contents.edit_modified(0)
+				
+				
+		else:
+			# skip unnecessary disk-writing silently
+			if not activetab:
+				return
+
+			# if closing tab or loading file:
+		
+			# Check indent (tabify) and rstrip:
+			tmp = self.tabs[self.tabindex].contents.splitlines(True)
+			tmp[:] = [self.tabify(line) for line in tmp]
+			tmp = ''.join(tmp)[:-1]
+			
+			if self.tabs[self.tabindex].contents == self.tabs[self.tabindex].oldcontents:
+				return
+				
+			try:
+				with open(self.tabs[self.tabindex].filepath, 'w', encoding='utf-8') as f:
+					f.write(tmp)
+					
+			except EnvironmentError as e:
+				print(e.__str__())
+				print(f'\n Could not save file: {self.tabs[self.tabindex].filepath}')
+				return
+				
+		############# Save End #######################################
+	
+########## Save and Load End
+########## Gotoline and Help Begin
+	
+	def do_gotoline(self, event=None):
+		''' If tkinter.END is linenumber of last line:
+			When linenumber given is positive and between 0 - tkinter.END,
+			go to start of that line, if greater, go to tkinter.END.
+			
+			When given negative number between -1 - -tkinter.END or so,
+			start counting from tkinter.END towards beginning and
+			go to that line.
+		
+		'''
+		
+		try:
+			# Get stuff after prompt
+			tmp = self.entry.get()
+			idx = self.entry.len_prompt
+			tmp = tmp[idx:].strip()
+			
+			
+			if tmp in ['-1', '']:
+				line = tkinter.END
+			
+			elif '-' not in tmp:
+				line = tmp + '.0'
+				
+			elif tmp[0] == '-' and '-' not in tmp[1:]:
+				if int(tmp[1:]) < int(self.entry.endline):
+					line = self.entry.endline + '.0 -%s lines' % tmp[1:]
+				else:
+					line = tkinter.END
+			
+			else:
+				line = tkinter.INSERT
+				
+			self.contents.focus_set()
+			self.contents.mark_set('insert', line)
+			self.ensure_idx_visibility(line)
+			
+			
+			try:
+				pos = self.contents.index(tkinter.INSERT)
+			except tkinter.TclError:
+				pos = '1.0'
+				
+			self.tabs[self.tabindex].position = pos
+			self.stop_gotoline()
+			
+		except tkinter.TclError as e:
+			print(e)
+			self.stop_gotoline()
+			
+		return "break"
+		
+	
+	def stop_gotoline(self, event=None):
+		self.state = 'normal'
+		self.bind("<Escape>", self.do_nothing)
+		
+		self.entry.config(validate='none')
+		
+		self.entry.bind("<Return>", self.load)
+		self.entry.delete(0, tkinter.END)
+		if self.tabs[self.tabindex].filepath:
+			self.entry.insert(0, self.tabs[self.tabindex].filepath)
+			self.entry.xview_moveto(1.0)
+			
+		
+		# Set cursor pos
+		try:
+			line = self.tabs[self.tabindex].position
+			self.contents.focus_set()
+			self.contents.mark_set('insert', line)
+			self.ensure_idx_visibility(line)
+		
+		except tkinter.TclError:
+			self.tabs[self.tabindex].position = '1.0'
+		
+		return "break"
+		
+	
+	def gotoline(self, event=None):
+		if self.state != 'normal':
+			self.bell()
+			return "break"
+		
+		self.state = 'gotoline'
+		
+		try:
+			pos = self.contents.index(tkinter.INSERT)
+		except tkinter.TclError:
+			pos = '1.0'
+		
+		self.tabs[self.tabindex].position = pos
+		
+		# Remove extra line, this is number of lines in contents
+		self.entry.endline = str(int(self.contents.index(tkinter.END).split('.')[0]) - 1)
+		
+		self.entry.bind("<Return>", self.do_gotoline)
+		self.bind("<Escape>", self.stop_gotoline)
+		
+		self.entry.delete(0, tkinter.END)
+		self.entry.focus_set()
+		
+		patt = 'Go to line, 1-%s: ' % self.entry.endline
+		self.entry.len_prompt = len(patt)
+		self.entry.insert(0, patt)
+		self.entry.config(validate='key', validatecommand=self.validate_gotoline)
+		
+		return "break"
+	
+	
+	def do_validate_gotoline(self, i, S, P):
+		'''	i is index of action,
+			S is new string to be validated,
+			P is all content of entry.
+		'''
+		
+		#print(i,S,P)
+		max_idx = self.entry.len_prompt + len(self.entry.endline) + 1
+		
+		if int(i) < self.entry.len_prompt:
+			self.entry.selection_clear()
+			self.entry.icursor(self.entry.len_prompt)
+			
+			return S == ''
+			
+		elif len(P) > max_idx:
+			return S == ''
+		
+		elif S.isdigit() or S == '-':
+			return True
+			
+		else:
+			return S == ''
+		
+	
+	def stop_help(self, event=None):
+		self.state = 'normal'
+		
+		self.entry.config(state='normal')
+		self.contents.config(state='normal')
+		self.btn_open.config(state='normal')
+		self.btn_save.config(state='normal')
+		
+		if self.tabs[self.tabindex].filepath:
+			self.entry.insert(0, self.tabs[self.tabindex].filepath)
+			self.entry.xview_moveto(1.0)
+			
+		self.token_can_update = True
+		self.contents.delete('1.0', tkinter.END)
+		self.contents.insert(tkinter.INSERT, self.tabs[self.tabindex].contents)
+		
+		
+		self.do_syntax(everything=True)
+		
+		
+		# set cursor pos
+		try:
+			line = self.tabs[self.tabindex].position
+			self.contents.focus_set()
+			self.contents.mark_set('insert', line)
+			self.ensure_idx_visibility(line)
+			
+		except tkinter.TclError:
+			self.tabs[self.tabindex].position = '1.0'
+		
+			
+		self.contents.edit_reset()
+		self.contents.edit_modified(0)
+		self.avoid_viewsync_mess()
+		
+		self.bind("<Escape>", self.do_nothing)
+		self.contents.bind("<Button-%i>" % self.right_mousebutton_num, lambda event: self.raise_popup(event))
+		
+		
+	def help(self, event=None):
+		if self.state != 'normal':
+			self.bell()
+			return "break"
+			
+		self.state = 'help'
+		
+		try:
+			pos = self.contents.index(tkinter.INSERT)
+		except tkinter.TclError:
+			pos = '1.0'
+		
+		self.tabs[self.tabindex].position = pos
+		tmp = self.contents.get('1.0', tkinter.END)
+		# [:-1]: remove unwanted extra newline
+		self.tabs[self.tabindex].contents = tmp[:-1]
+		
+		self.token_can_update = False
+		
+		self.entry.delete(0, tkinter.END)
+		self.contents.delete('1.0', tkinter.END)
+		self.contents.insert(tkinter.INSERT, self.helptxt)
+		
+		self.entry.config(state='disabled')
+		self.contents.config(state='disabled')
+		self.btn_open.config(state='disabled')
+		self.btn_save.config(state='disabled')
+		
+		self.contents.bind("<Button-%i>" % self.right_mousebutton_num, self.do_nothing)
+		self.bind("<Escape>", self.stop_help)
+			
+########## Gotoline and Help End
+########## Indent and Comment Begin
+	
+	def check_indent_depth(self, contents):
+		'''Contents is contents of py-file as string.'''
+		
+		words = [
+				'def ',
+				'if ',
+				'for ',
+				'while ',
+				'class '
+				]
+				
+		tmp = contents.splitlines()
+		
+		for word in words:
+			
+			for i in range(len(tmp)):
+				line = tmp[i]
+				if word in line:
+					
+					# Trying to check if at the beginning of new block:
+					if line.strip()[-1] == ':':
+						# Offset is num of empty lines between this line and next
+						# non empty line
+						nextline = None
+						
+						for offset in range(1, len(tmp)-i):
+							nextline = tmp[i+offset]
+							if nextline.strip() == '': continue
+							else: break
+							
+							
+						if not nextline:
+							continue
+						
+						
+						# Now should have next non empty line,
+						# so start parsing it:
+						flag_space = False
+						indent_0 = 0
+						indent_1 = 0
+		
+						for char in line:
+							if char in [' ', '\t']: indent_0 += 1
+							else: break
+		
+						for char in nextline:
+							# Check if indent done with spaces:
+							if char == ' ':
+								flag_space = True
+		
+							if char in [' ', '\t']: indent_1 += 1
+							else: break
+						
+						
+						indent = indent_1 - indent_0
+						#print(indent)
+						tests = [
+								( indent <= 0 ),
+								( not flag_space and indent > 1 )
+								]
+						
+						if any(tests):
+							#print('indent err')
+							#skipping
+							continue
+						
+						
+						# All is good, do nothing:
+						if not flag_space:
+							return False, 0
+							
+						# Found one block with spaced indentation,
+						# assuming it is used in whole file.
+						else:
+							if indent != self.ind_depth:
+								return True, indent
+							
+							else:
+								return False, 0
+					
+		return False, 0
+	
+	
+	def indent(self, event=None):
+		if self.state != 'normal':
+			self.bell()
+			
+		try:
+			startline = int(self.contents.index(tkinter.SEL_FIRST).split(sep='.')[0])
+			endline = int(self.contents.index(tkinter.SEL_LAST).split(sep='.')[0])
+			i = self.contents.index(tkinter.INSERT)
+			
+			start_idx = self.contents.index(tkinter.SEL_FIRST)
+			end_idx = self.contents.index(tkinter.SEL_LAST)
+					
+			self.contents.tag_remove('sel', '1.0', tkinter.END)
+			self.contents.tag_add('sel', start_idx, end_idx)
+			
+		
+			if len(self.contents.tag_ranges('sel')) != 0:
+					
+				# is start of selection viewable?
+				if not self.contents.bbox(tkinter.SEL_FIRST):
+					
+					self.wait_for(150)
+					self.ensure_idx_visibility(tkinter.SEL_FIRST, back=4)
+					self.wait_for(100)
+						
+			
+			for linenum in range(startline, endline+1):
+				self.contents.mark_set(tkinter.INSERT, '%s.0' % linenum)
+				self.contents.insert(tkinter.INSERT, '\t')
+			
+			
+			if startline == endline:
+				self.contents.mark_set(tkinter.INSERT, '%s +1c' %i)
+			
+			elif self.contents.compare(tkinter.SEL_FIRST, '<', tkinter.INSERT):
+				self.contents.mark_set(tkinter.INSERT, tkinter.SEL_FIRST)
+				
+			self.ensure_idx_visibility('insert', back=4)
+			self.contents.edit_separator()
+			
+		except tkinter.TclError:
+			pass
+			
+
+	def unindent(self, event=None):
+		if self.state != 'normal':
+			self.bell()
+			return "break"
+			
+		try:
+			# unindenting curline only:
+			if len(self.contents.tag_ranges('sel')) == 0:
+			
+				startline = int(self.contents.index(tkinter.INSERT).split(sep='.')[0])
+				endline = startline
+				
+			else:
+				startline = int(self.contents.index(tkinter.SEL_FIRST).split(sep='.')[0])
+				endline = int(self.contents.index(tkinter.SEL_LAST).split(sep='.')[0])
+			
+			i = self.contents.index(tkinter.INSERT)
+			
+			# Check there is enough space in every line:
+			flag_continue = True
+			
+			for linenum in range(startline, endline+1):
+				tmp = self.contents.get('%s.0' % linenum, '%s.0 lineend' % linenum)
+				
+				if len(tmp) != 0 and tmp[0] != '\t':
+					flag_continue = False
+					break
+				
+			if flag_continue:
+				
+				if len(self.contents.tag_ranges('sel')) != 0:
+					
+					# is start of selection viewable?
+					if not self.contents.bbox(tkinter.SEL_FIRST):
+						
+						self.wait_for(150)
+						self.ensure_idx_visibility('insert', back=4)
+						self.wait_for(100)
+						
+						
+				for linenum in range(startline, endline+1):
+					tmp = self.contents.get('%s.0' % linenum, '%s.0 lineend' % linenum)
+				
+					if len(tmp) != 0:
+						if len(self.contents.tag_ranges('sel')) != 0:
+							self.contents.mark_set(tkinter.INSERT, '%s.0' % linenum)
+							self.contents.delete(tkinter.INSERT, '%s+%dc' % (tkinter.INSERT, 1))
+						
+						else:
+							self.contents.delete( '%s.0' % linenum, '%s.0 +1c' % linenum)
+				
+		
+				# is selection made from down to top or from right to left?
+				if len(self.contents.tag_ranges('sel')) != 0:
+				
+					if startline == endline:
+						self.contents.mark_set(tkinter.INSERT, '%s -1c' %i)
+					
+					elif self.contents.compare(tkinter.SEL_FIRST, '<', tkinter.INSERT):
+						self.contents.mark_set(tkinter.INSERT, tkinter.SEL_FIRST)
+						
+					# is start of selection viewable?
+					if not self.contents.bbox(tkinter.SEL_FIRST):
+						self.ensure_idx_visibility('insert', back=4)
+					
+				self.contents.edit_separator()
+		
+		except tkinter.TclError as e:
+			pass
+			
+		return "break"
+	
+	
+	def comment(self, event=None):
+		if self.state != 'normal':
+			self.bell()
+			return "break"
+			
+		try:
+			s = self.contents.index(tkinter.SEL_FIRST)
+			e = self.contents.index(tkinter.SEL_LAST)
+		
+			startline = int( s.split('.')[0] )
+			startpos = self.contents.index( '%s linestart' % s )
+			
+			endline = int( e.split('.')[0] )
+			endpos = self.contents.index( '%s lineend' % e )
+			
+			
+			for linenum in range(startline, endline+1):
+				self.contents.mark_set(tkinter.INSERT, '%s.0' % linenum)
+				self.contents.insert(tkinter.INSERT, '##')
+				
+						
+			self.update_tokens(start=startpos, end=endpos)
+			
+				
+			self.contents.edit_separator()
+			return "break"
+		
+		except tkinter.TclError as e:
+			print(e)
+			return "break"
+	
+
+	def uncomment(self, event=None):
+		''' Should work even if there are uncommented lines between commented lines. '''
+		if self.state != 'normal':
+			self.bell()
+			return "break"
+			
+		try:
+			s = self.contents.index(tkinter.SEL_FIRST)
+			e = self.contents.index(tkinter.SEL_LAST)
+		
+			startline = int(s.split('.')[0])
+			endline = int(e.split('.')[0])
+			startpos = self.contents.index('%s linestart' % s)
+			endpos = self.contents.index('%s lineend' % e)
+				
+			changed = False
+			
+			for linenum in range(startline, endline+1):
+				self.contents.mark_set(tkinter.INSERT, '%s.0' % linenum)
+				tmp = self.contents.get('%s.0' % linenum,'%s.0 lineend' % linenum)
+				
+				if tmp.lstrip()[:2] == '##':
+					tmp = tmp.replace('##', '', 1)
+					self.contents.delete('%s.0' % linenum,'%s.0 lineend' % linenum)
+					self.contents.insert(tkinter.INSERT, tmp)
+					changed = True
+					
+					
+			if changed:
+			
+				self.update_tokens(start=startpos, end=endpos)
+				
+				self.contents.edit_separator()
+			
+		except tkinter.TclError as e:
+			print(e)
+		return "break"
+		
+########## Indent and Comment End
+################ Search Begin
+	
+	def check_next_event(self, event=None):
+		
+		if event.keysym == 'Left':
+			line = self.lastcursorpos
+			self.contents.tag_remove('sel', '1.0', tkinter.END)
+			self.contents.mark_set('insert', line)
+			self.ensure_idx_visibility(line)
+			
+			
+			self.contents.unbind("<Any-Key>", funcid=self.anykeyid)
+			self.contents.unbind("<Any-Button>", funcid=self.anybutid)
+			
+			f = self.check_sel
+			if self.os_type == 'mac_os': f = self.mac_cmd_overrides
+			
+			self.bid_left = self.contents.bind("<Left>", f )
+		
+			return 'break'
+			
+		else:
+			self.contents.unbind("<Any-Key>", funcid=self.anykeyid)
+			self.contents.unbind("<Any-Button>", funcid=self.anybutid)
+			
+			f = self.check_sel
+			if self.os_type == 'mac_os': f = self.mac_cmd_overrides
+			self.bid_left = self.contents.bind("<Left>", f )
+			
+			return
+			
+		
+		
+	def search_next(self, event=None):
+		'''	Do last search from cursor position, show and select next match.
+			
+			This is for cases when you can not do replace ALL.
+			You need to choose when to insert AND insertion is not always
+			the same. But replace is too limited (can not insert, like in search).
+			So you do normal search and quit quickly. Then copy your insertion
+			'pattern' in clipboard, what you add to certain matches and then
+			maybe change something else, or you need sometimes delete match and
+			insert your clipboard 'pattern' etc...
+			
+			In short:
+			1: Do normal search
+			2: copy what you need to have in clipboard
+			3: ctrl-backspace until in right place
+			4: now easy to delete or add clipboard contents etc..
+			5: repeat 3-4
+			
+			shortcut: ctrl-backspace
+		'''
+		
+		if self.state != 'normal' or self.old_word == '':
+			self.bell()
+			return "break"
+			
+			
+		wordlen = len(self.old_word)
+		self.lastcursorpos = self.contents.index(tkinter.INSERT)
+		pos = self.contents.search(self.old_word, 'insert +1c', tkinter.END)
+		
+		# Try again from the beginning this time:
+		if not pos:
+			pos = self.contents.search(self.old_word, '1.0', tkinter.END)
+			
+			# no oldword in file:
+			if not pos:
+				self.bell()
+				#print('no')
+				return "break"
+		
+		# Go back to last place with arrow left
+		self.anykeyid = self.contents.bind( "<Any-Key>", self.check_next_event)
+		self.anybutid = self.contents.bind( "<Any-Button>", self.check_next_event)
+		
+		# Without this one can not search by holding ctrl down and
+		# pressing and releasing repeatedly backspace only:
+		if self.bid_left: self.contents.unbind("<Left>", self.bid_left)
+		self.bid_left = None
+		
+		
+		lastpos = "%s + %dc" % (pos, wordlen)
+		self.contents.tag_remove('sel', '1.0', tkinter.END)
+		self.contents.mark_set(self.anchorname, pos)
+		self.contents.tag_add('sel', pos, lastpos)
+		self.contents.mark_set('insert', lastpos)
+		line = pos
+		self.ensure_idx_visibility(line)
+					
+		return "break"
+
+
+	def show_next(self, event=None):
+		if self.state not in [ 'search', 'replace', 'replace_all' ]:
+			return
+			
+		match_ranges = self.contents.tag_ranges('match')
+		
+		# Check if at last match or beyond:
+		i = len(match_ranges) - 2
+		last = match_ranges[i]
+		
+		# self.search_idx marks range of focus-tag:
+		if self.contents.compare(self.search_idx[0], '>=', last):
+			self.search_idx = ('1.0', '1.0')
+				
+		if self.search_idx != ('1.0', '1.0'):
+			self.contents.tag_remove('focus', self.search_idx[0], self.search_idx[1])
+		else:
+			self.contents.tag_remove('focus', '1.0', tkinter.END)
+		
+		
+		# self.search_idx marks range of focus-tag.
+		# Here focus is moved to next match after current focus:
+		self.search_idx = self.contents.tag_nextrange('match', self.search_idx[1])
+		line = self.search_idx[0]
+		
+		# Is it viewable?
+		if not self.contents.bbox(line):
+			self.wait_for(100)
+		
+		self.ensure_idx_visibility(line)
+		
+		
+		if self.entry.flag_start:
+			if self.state == 'search':
+				self.wait_for(100)
+				bg, fg = self.themes[self.curtheme]['match'][:]
+				self.contents.tag_config('match', background=bg, foreground=fg)
+			self.wait_for(200)
+			
+		
+		# Change color
+		# self.search_idx marks range of focus-tag. Here focus-tag is changed.
+		self.contents.tag_add('focus', self.search_idx[0], self.search_idx[1])
+		
+		# Compare above range of focus-tag to match_ranges to get current
+		# index position among all current matches. Like if we now have 10 matches left,
+		# and last position was 1/11, but then one match got replaced,
+		# so we now are at 1/10 and after this show next-call we should be at 2/10.
+		ref = self.contents.tag_ranges('focus')[0]
+		
+		for idx in range(self.search_matches):
+			tmp = match_ranges[idx*2]
+			if self.contents.compare(ref, '==', tmp): break
+		
+		
+		if self.state != 'search':
+			
+			if self.entry.flag_start:
+				self.entry.flag_start = False
+				self.entry.config(validate='key')
+				
+			else:
+				lenght_of_search_position_index = len(str(idx+1))
+				lenght_of_search_matches = len(str(self.search_matches))
+				diff = lenght_of_search_matches - lenght_of_search_position_index
+				patt = f'{diff*" "}{idx+1}/{self.search_matches}'
+				
+				self.entry.config(validate='none')
+				tmp = self.entry.get()
+				idx_0 = tmp.index('/')
+				idx = tmp.index(' ', idx_0)
+				self.entry.delete(0, idx)
+				self.entry.insert(0, patt)
+				self.entry.config(validate='key')
+				
+			
+		else:
+			if self.entry.flag_start:
+				self.entry.flag_start = False
+				self.entry.config(validate='key')
+				
+			else:
+				
+				lenght_of_search_position_index = len(str(idx+1))
+				lenght_of_search_matches = len(str(self.search_matches))
+				diff = lenght_of_search_matches - lenght_of_search_position_index
+				patt = f'{diff*" "}{idx+1}'
+				
+				self.entry.config(validate='none')
+				self.entry.delete(0, lenght_of_search_matches)
+				self.entry.insert(0, patt)
+				self.entry.config(validate='key')
+				
+			
+		
+		if self.search_matches == 1:
+			self.bind("<Control-n>", self.do_nothing)
+			self.bind("<Control-p>", self.do_nothing)
+			
+		
+		self.entry.xview_moveto(0)
+		
+		return 'break'
+		
+
+	def show_prev(self, event=None):
+		
+		if self.state not in [ 'search', 'replace', 'replace_all' ]:
+			return
+		
+		match_ranges = self.contents.tag_ranges('match')
+		
+		first = match_ranges[0]
+		
+		# self.search_idx marks range of focus-tag:
+		if self.contents.compare(self.search_idx[0], '<=', first):
+			self.search_idx = (tkinter.END, tkinter.END)
+		
+		if self.search_idx != (tkinter.END, tkinter.END):
+			self.contents.tag_remove('focus', self.search_idx[0], self.search_idx[1])
+		else:
+			self.contents.tag_remove('focus', '1.0', tkinter.END)
+		
+		
+		# self.search_idx marks range of focus-tag.
+		# Here focus is moved to previous match before current focus:
+		self.search_idx = self.contents.tag_prevrange('match', self.search_idx[0])
+		line = self.search_idx[0]
+		
+		# Is it viewable?
+		if not self.contents.bbox(line):
+			self.wait_for(100)
+		
+		self.ensure_idx_visibility(line)
+		
+		
+		# Change color
+		# self.search_idx marks range of focus-tag. Here focus-tag is changed.
+		self.contents.tag_add('focus', self.search_idx[0], self.search_idx[1])
+		
+		# Compare above range of focus-tag to match_ranges to get current
+		# index position among all current matches. Like if we now have 11 matches left,
+		# and last position was 2/12, but then one match got replaced,
+		# so we now are at say 2/11 and after this show prev-call we should be at 1/11.
+		ref = self.contents.tag_ranges('focus')[0]
+		
+		for idx in range(self.search_matches):
+			tmp = match_ranges[idx*2]
+			if self.contents.compare(ref, '==', tmp): break
+			
+		
+		if self.state != 'search':
+			
+			lenght_of_search_position_index = len(str(idx+1))
+			lenght_of_search_matches = len(str(self.search_matches))
+			diff = lenght_of_search_matches - lenght_of_search_position_index
+			patt = f'{diff*" "}{idx+1}/{self.search_matches}'
+			
+			self.entry.config(validate='none')
+			tmp = self.entry.get()
+			idx_0 = tmp.index('/')
+			idx = tmp.index(' ', idx_0)
+			self.entry.delete(0, idx)
+			self.entry.insert(0, patt)
+			self.entry.config(validate='key')
+			
+			
+		else:
+			
+			lenght_of_search_position_index = len(str(idx+1))
+			lenght_of_search_matches = len(str(self.search_matches))
+			diff = lenght_of_search_matches - lenght_of_search_position_index
+			patt = f'{diff*" "}{idx+1}'
+			
+			self.entry.config(validate='none')
+			self.entry.delete(0, lenght_of_search_matches)
+			self.entry.insert(0, patt)
+			self.entry.config(validate='key')
+			
+			
+		if self.search_matches == 1:
+			self.bind("<Control-n>", self.do_nothing)
+			self.bind("<Control-p>", self.do_nothing)
+		
+		
+		self.entry.xview_moveto(0)
+		
+		return 'break'
+		
+		
+	def start_search(self, event=None):
+		
+		# Get stuff after prompt
+		tmp_orig = self.entry.get()
+		
+		idx = tmp_orig.index(':') + 2
+		tmp = tmp_orig[idx:].strip()
+		
+		if len(tmp) == 0 or tmp == self.old_word:
+			self.bell()
+			return 'break'
+		
+		self.old_word = tmp
+		
+		self.contents.tag_remove('match', '1.0', tkinter.END)
+		self.contents.tag_remove('focus', '1.0', tkinter.END)
+		self.search_idx = ('1.0', '1.0')
+		self.search_matches = 0
+		
+		if len(self.old_word) != 0:
+			pos = '1.0'
+			wordlen = len(self.old_word)
+			self.contents.tag_config('match', background='', foreground='')
+			
+			while True:
+				pos = self.contents.search(self.old_word, pos, tkinter.END)
+				if not pos: break
+				self.search_matches += 1
+				lastpos = "%s + %dc" % (pos, wordlen)
+				self.contents.tag_add('match', pos, lastpos)
+				pos = "%s + %dc" % (pos, wordlen+1)
+				
+				
+		if self.search_matches > 0:
+			self.contents.bind("<Button-%i>" % self.right_mousebutton_num, self.do_nothing)
+			self.entry.config(validate='none')
+				
+			if self.state == 'search':
+				self.bind("<Control-n>", self.show_next)
+				self.bind("<Control-p>", self.show_prev)
+				
+				
+				lenght_of_search_matches = len(str(self.search_matches))
+				diff = lenght_of_search_matches - 1
+				patt = f'{diff*" "}1/{self.search_matches} '
+				idx = tmp_orig.index('Sea')
+				self.entry.delete(0, idx)
+				self.entry.insert(0, patt)
+				self.entry.flag_start = True
+				
+				
+				self.contents.focus_set()
+				self.wait_for(100)
+				self.show_next()
+				
+				
+			else:
+				patt = 'Replace %s matches with: ' % str(self.search_matches)
+				idx = tmp_orig.index(':') + 2
+				self.entry.delete(0, idx)
+				self.entry.insert(0, patt)
+				
+				self.entry.select_from(len(patt))
+				self.entry.select_to(tkinter.END)
+				self.entry.icursor(len(patt))
+				self.entry.xview_moveto(0)
+				
+
+				bg, fg = self.themes[self.curtheme]['match'][:]
+				self.contents.tag_config('match', background=bg, foreground=fg)
+				
+				
+				self.entry.bind("<Return>", self.start_replace)
+				self.entry.focus_set()
+				self.entry.config(validate='key')
+				
+		else:
+			self.bell()
+			bg, fg = self.themes[self.curtheme]['match'][:]
+			self.contents.tag_config('match', background=bg, foreground=fg)
+			self.bind("<Control-n>", self.do_nothing)
+			self.bind("<Control-p>", self.do_nothing)
+			
+			
+				
+		return 'break'
+		
+	
+	def update_curpos(self, event=None, doubleclick=False):
+		self.save_pos = self.contents.index(tkinter.INSERT)
+		
+		if doubleclick:
+			self.stop_search()
+		
+		else:
+			# This is needed to enable replacing with Return.
+			# Because of binding to self in start_replace().
+			# And when pressing contents with mouse, self.contents gets focus,
+			# so put it back to self.
+			self.focus_set()
+		
+		return "break"
+			
+			
+	def clear_search_tags(self, event=None):
+		if self.state != 'normal':
+			return "break"
+			
+		self.contents.tag_remove('replaced', '1.0', tkinter.END)
+		self.bind("<Escape>", self.do_nothing)
+		
+	
+	def stop_search(self, event=None):
+		self.contents.config(state='normal')
+		self.entry.config(state='normal')
+		self.btn_open.config(state='normal')
+		self.btn_save.config(state='normal')
+		self.contents.bind("<Button-%i>" % self.right_mousebutton_num, lambda event: self.raise_popup(event))
+		
+		#self.wait_for(200)
+		self.contents.tag_remove('focus', '1.0', tkinter.END)
+		self.contents.tag_remove('match', '1.0', tkinter.END)
+		self.contents.tag_remove('sel', '1.0', tkinter.END)
+		
+		# Leave marks on replaced areas, Esc clears.
+		if len(self.contents.tag_ranges('replaced')) > 0:
+			self.bind("<Escape>", self.clear_search_tags)
+		else:
+			self.bind("<Escape>", self.do_nothing)
+			
+		
+		self.entry.config(validate='none')
+		self.entry.flag = None
+		
+		
+		self.entry.bind("<Return>", self.load)
+		self.entry.delete(0, tkinter.END)
+	
+		if self.tabs[self.tabindex].filepath:
+			self.entry.insert(0, self.tabs[self.tabindex].filepath)
+			self.entry.xview_moveto(1.0)
+			
+		self.new_word = ''
+		self.search_matches = 0
+		flag_all = False
+		if self.state == 'replace_all': flag_all = True
+		
+		if self.state in [ 'replace_all', 'replace' ]:
+			
+				self.state = 'normal'
+				
+				self.do_syntax()
+				
+				
+		self.state = 'normal'
+		self.contents.unbind( "<Control-n>", funcid=self.bid1 )
+		self.contents.unbind( "<Control-p>", funcid=self.bid2 )
+		self.contents.unbind( "<Double-Button-1>", funcid=self.bid3 )
+		self.contents.unbind( "<space>", funcid=self.bid4 )
+		self.contents.bind( "<Control-n>", self.move_down)
+		self.contents.bind( "<Control-p>", self.move_up)
+		self.contents.bind("<Return>", self.return_override)
+		self.entry.bind("<Control-n>", self.do_nothing_without_bell)
+		self.entry.bind("<Control-p>", self.do_nothing_without_bell)
+		self.bind( "<Return>", self.do_nothing_without_bell)
+		
+		
+		#self.wait_for(200)
+		
+		# set cursor pos
+		try:
+			if self.save_pos:
+				line = self.save_pos
+				self.tabs[self.tabindex].position = line
+				self.save_pos = None
+			else:
+				line = self.tabs[self.tabindex].position
+			
+			self.contents.focus_set()
+			self.contents.mark_set('insert', line)
+	
+			if not flag_all:
+				self.ensure_idx_visibility(line)
+			
+		except tkinter.TclError:
+			self.tabs[self.tabindex].position = self.contents.index(tkinter.INSERT)
+		
+		return "break"
+	
+	
+	def search(self, event=None):
+		'''	Ctrl-f --> search --> start_search --> show_next / show_prev --> stop_search
+		'''
+		
+		if self.state != 'normal':
+			self.bell()
+			return "break"
+		
+		# Save cursor pos
+		try:
+			self.tabs[self.tabindex].position = self.contents.index(tkinter.INSERT)
+		
+		except tkinter.TclError:
+			pass
+			
+		self.state = 'search'
+		self.old_word = ''
+		self.btn_open.config(state='disabled')
+		self.btn_save.config(state='disabled')
+		self.entry.bind("<Return>", self.start_search)
+		self.bind("<Escape>", self.stop_search)
+		
+		self.bid1 = self.contents.bind("<Control-n>", func=self.skip_bindlevel )
+		self.bid2 = self.contents.bind("<Control-p>", func=self.skip_bindlevel )
+		self.entry.bind("<Control-n>", self.skip_bindlevel)
+		self.entry.bind("<Control-p>", self.skip_bindlevel)
+		
+		
+		self.bid3 = self.contents.bind("<Double-Button-1>",
+			func=lambda event: self.update_curpos(event, **{'doubleclick':True}), add=True )
+		
+		self.bid4 = self.contents.bind("<space>", func=self.space_override )
+		
+		
+		self.entry.delete(0, tkinter.END)
+		
+		
+		# Autofill from clipboard
+		try:
+			tmp = self.clipboard_get()
+			if 80 > len(tmp) > 0:
+				self.entry.insert(tkinter.END, tmp)
+				self.entry.xview_moveto(1.0)
+				self.entry.select_to(tkinter.END)
+				self.entry.icursor(tkinter.END)
+				
+		# Empty clipboard
+		except tkinter.TclError:
+			pass
+			
+		
+		self.entry.flag = None
+		patt = 'Search: '
+		self.entry.len_prompt = len(patt)
+		self.entry.insert(0, patt)
+		self.entry.config(validate='key', validatecommand=self.validate_search)
+		
+		self.contents.config(state='disabled')
+		self.entry.focus_set()
+		
+		return "break"
+		
+		
+	def do_validate_search(self, i, s, S):
+		'''	i is index of action,
+			s is string before action,
+			S is new string to be validated
+		'''
+		
+		#print(i,s,S)
+		# 'focusin'
+		# 'focusout'
+		
+		idx = s.index(':') + 2
+			
+		if int(i) < idx or self.entry.flag == 'replace_all':
+			self.entry.selection_clear()
+			self.entry.icursor(idx)
+			
+			return S == ''
+			
+		else:
+			return True
+
+################ Search End
+################ Replace Begin
+
+	def replace(self, event=None, state='replace'):
+		'''	Ctrl-r --> replace --> start_search --> start_replace
+			--> show_next / show_prev / do_single_replace --> stop_search
+		'''
+		
+		if self.state != 'normal':
+			self.bell()
+			return "break"
+		
+		# Save cursor pos
+		try:
+			self.tabs[self.tabindex].position = self.contents.index(tkinter.INSERT)
+		
+		except tkinter.TclError:
+			pass
+		
+		self.state = state
+		self.old_word = ''
+		self.btn_open.config(state='disabled')
+		self.btn_save.config(state='disabled')
+		self.entry.bind("<Return>", self.start_search)
+		self.bind("<Escape>", self.stop_search)
+		self.bid1 = self.contents.bind("<Control-n>", func=self.skip_bindlevel )
+		self.bid2 = self.contents.bind("<Control-p>", func=self.skip_bindlevel )
+		self.entry.bind("<Control-n>", self.skip_bindlevel)
+		self.entry.bind("<Control-p>", self.skip_bindlevel)
+		
+		
+		self.bid3 = self.contents.bind("<Double-Button-1>",
+			func=lambda event: self.update_curpos(event, **{'doubleclick':True}), add=True )
+		
+		self.bid4 = self.contents.bind("<space>", func=self.space_override )
+		
+		
+		self.entry.delete(0, tkinter.END)
+		
+		
+		# Autofill from clipboard
+		try:
+			tmp = self.clipboard_get()
+			if 80 > len(tmp) > 0:
+				self.entry.insert(tkinter.END, tmp)
+				self.entry.xview_moveto(1.0)
+				self.entry.select_to(tkinter.END)
+				self.entry.icursor(tkinter.END)
+	
+		except tkinter.TclError:
+			pass
+			
+		
+		self.entry.flag = None
+		
+		patt = 'Replace this: '
+		self.entry.len_prompt = len(patt)
+		self.entry.insert(0, patt)
+		self.entry.config(validate='key', validatecommand=self.validate_search)
+		
+		self.wait_for(400)
+		self.contents.tag_remove('replaced', '1.0', tkinter.END)
+		
+		self.contents.config(state='disabled')
+		self.entry.focus_set()
+		return "break"
+
+
+	def replace_all(self, event=None):
+		if self.state != 'normal':
+			self.bell()
+			return "break"
+			
+		self.replace(event, state='replace_all')
+		
+		
+	def do_single_replace(self, event=None):
+		
+		# Enable changing newword between replaces Begin
+		#################
+		# Get stuff after prompt
+		tmp_orig = self.entry.get()
+		idx = tmp_orig.index(':') + 2
+		tmp = tmp_orig[idx:].strip()
+		
+		# Replacement-string has changed
+		if tmp != self.new_word:
+			
+			# Not allowed to do this:
+			if tmp == self.old_word:
+
+				self.entry.config(validate='none')
+				self.entry.delete(idx, tkinter.END)
+				self.entry.insert(tkinter.END, self.new_word)
+				self.entry.config(validate='key')
+				self.bell()
+
+				return 'break'
+
+			else:
+				self.new_word = tmp
+		# Enable changing newword between replaces End
+		#################
+		
+
+		
+		# Apply normal 'Replace and proceed to next by pressing Return' -behaviour.
+		# If last replace was done by pressing Return, there is currently no focus-tag.
+		# Check this and get focus-tag with show_next() if this is the case, and break.
+		# This means that the actual replacing happens only when have focus-tag.
+		c = self.contents.tag_nextrange('focus', 1.0)
+		
+		if not len(c) > 0:
+			self.show_next()
+			return 'break'
+			
+		
+		# Start of actual replacing
+		self.contents.config(state='normal')
+		
+		wordlen = len(self.old_word)
+		wordlen2 = len(self.new_word)
+		
+		
+		# self.search_idx marks range of focus-tag:
+		self.contents.tag_remove('focus', self.search_idx[0], self.search_idx[1])
+		self.contents.tag_remove('match', self.search_idx[0], self.search_idx[1])
+		self.contents.delete(self.search_idx[0], self.search_idx[1])
+		self.contents.insert(self.search_idx[0], self.new_word)
+		
+		# tag replacement to avoid rematching same place
+		p = "%s + %dc" % (self.search_idx[0], wordlen2)
+		self.contents.tag_add('replaced', self.search_idx[0], p)
+		
+		
+		self.contents.config(state='disabled')
+		
+		self.search_matches -= 1
+		
+		if self.search_matches == 0:
+			self.wait_for(100)
+			self.stop_search()
+
+	
+	def do_replace_all(self, event=None):
+		
+		self.contents.config(state='normal')
+		wordlen = len(self.old_word)
+		wordlen2 = len(self.new_word)
+		pos = '1.0'
+		
+		while True:
+			pos = self.contents.search(self.old_word, pos, tkinter.END)
+			if not pos: break
+			
+			lastpos = "%s + %dc" % ( pos, wordlen )
+			lastpos2 = "%s + %dc" % ( pos, wordlen2 )
+			
+			self.contents.delete( pos, lastpos )
+			self.contents.insert( pos, self.new_word )
+			self.contents.tag_add( 'replaced', pos, lastpos2 )
+				
+			pos = "%s + %dc" % (pos, wordlen+1)
+			
+		# Show lastpos but dont put cursor on it
+		line = lastpos
+		self.wait_for(100)
+		self.ensure_idx_visibility(line)
+
+		self.stop_search()
+		
+		
+	def start_replace(self, event=None):
+		
+		# Get stuff after prompt
+		tmp_orig = self.entry.get()
+		idx = tmp_orig.index(':') + 2
+		tmp = tmp_orig[idx:].strip()
+		self.new_word = tmp
+		
+		# No check for empty newword to enable deletion.
+		
+		if self.old_word == self.new_word:
+			self.bell()
+			return 'break'
+		
+		
+		self.entry.config(validate='none')
+		
+		lenght_of_search_matches = len(str(self.search_matches))
+		diff = lenght_of_search_matches - 1
+		idx = tmp_orig.index(':')
+		self.entry.delete(0, idx)
+			
+		patt = f'{diff*" "}1/{self.search_matches} Replace with'
+			
+		if self.state == 'replace_all':
+			patt = f'{diff*" "}1/{self.search_matches} Replace ALL with'
+			self.entry.flag = 'replace_all'
+			
+		self.entry.insert(0, patt)
+		
+		
+		self.entry.flag_start = True
+		self.wait_for(100)
+		self.show_next()
+		
+		
+		self.bind("<Control-n>", self.show_next)
+		self.bind("<Control-p>", self.show_prev)
+		self.entry.bind("<Return>", self.skip_bindlevel)
+		self.contents.bind("<Return>", self.skip_bindlevel)
+		self.focus_set()
+		
+		
+		if self.state == 'replace':
+			self.bind( "<Return>", self.do_single_replace)
+			
+		elif self.state == 'replace_all':
+			self.bind( "<Return>", self.do_replace_all)
+			
+		return 'break'
+		
+		
+################ Replace End
+########### Class Editor End
```

### Comparing `henxel-0.3.0/src/henxel/changefont.py` & `henxel-0.3.1/src/henxel/changefont.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,387 +1,387 @@
-import tkinter.font
-import tkinter
-
-
-class FontChooser:
-		
-	def __init__(self, master, fontlist, big=False, tracefunc=None, os_type='linux'):
-		'''	master		tkinter.Toplevel
-			fontlist	list of tkinter.font.Font instances
-			big			If true start with bigger font.
-			tracefunc	callable, used in change_font. It arranges variable
-						observer for change on any item in fontlist.
-						This is practically same as if there would be virtual
-						event <<FontChanged>> and tracefunc binded to it.
-		'''
-		
-		self.top = master
-		self.fonts = fontlist
-		
-		if tracefunc:
-			self.tracefunc = tracefunc
-		else:
-			self.tracefunc = None
-		
-		self.badfonts = [
-					'Standard Symbols PS',
-					'OpenSymbol',
-					'Noto Color Emoji',
-					'FontAwesome',
-					'Dingbats',
-					'Droid Sans Fallback',
-					'D050000L'
-					]
-		
-		
-		self.max = 42
-		self.min = 8
-		
-		self.topframe = tkinter.Frame(self.top)
-		self.bottomframe = tkinter.Frame(self.top)
-		self.topframe.pack()
-		self.bottomframe.pack()
-		
-
-		self.option_menu_list = list()
-
-		for font in self.fonts:
-			self.option_menu_list.append(font.name)
-		
-		self.var = tkinter.StringVar()
-		self.var.set(self.option_menu_list[0])
-		self.font = tkinter.font.nametofont(self.var.get())
-		
-		self.optionmenu = tkinter.OptionMenu(self.topframe, self.var, *self.option_menu_list, command=self.optionmenu_command)
-		
-		# Set font of dropdown button:
-		self.optionmenu.config(font=('TkDefaultFont',10))
-		
-		# Set font of dropdown items:
-		self.menu = self.topframe.nametowidget(self.optionmenu.menuname)
-		self.menu.config(font=('TkDefaultFont',10))
-		
-		# Optionmenu contains font-instances to be configured:
-		self.optionmenu.pack(side=tkinter.LEFT)
-		
-		
-		self.button = tkinter.Button(self.topframe, text='BIG', command=self.button_command)
-		self.button.pack()
-		self.scrollbar = tkinter.Scrollbar(self.topframe)
-		
-		# Listbox contains font-choises to select from:
-		self.lb = tkinter.Listbox(self.topframe, font=('TkDefaultFont', 10), selectmode=tkinter.SINGLE, width=40, yscrollcommand=self.scrollbar.set)
-		self.lb.pack(pady=10, side='left')
-		self.scrollbar.pack(side='left', fill='y')
-		self.scrollbar.config(width=30, elementborderwidth=4, command=self.lb.yview)
-		
-		if os_type != 'linux':
-			self.scrollbar.configure(width=16, elementborderwidth=2)
-			
-				
-		# With spinbox we set font size:
-		self.sb = tkinter.Spinbox(self.topframe, font=('TkDefaultFont', 10), from_=self.min, to=self.max, increment=2, width=3, command=self.change_font)
-		self.sb.pack(pady=10, anchor='w')
-		
-		# Make checkboxes for other font configurations
-		self.bold = tkinter.StringVar()
-		self.cb1 = tkinter.Checkbutton(self.topframe, font=('TkDefaultFont', 10), offvalue='normal', onvalue='bold', text='Bold', variable=self.bold)
-		self.cb1.pack(pady=10, anchor='w')
-		self.cb1.config(command=lambda args=[self.bold, 'weight']: self.checkbutton_command(args))
-		
-		
-##		self.italic = tkinter.StringVar()
-##		self.cb2 = tkinter.Checkbutton(self.topframe, font=('TkDefaultFont', 10), offvalue='roman', onvalue='italic', text='Italic', variable=self.italic)
-##		self.cb2.pack(pady=10, anchor='w')
-##		self.cb2.config(command=lambda args=[self.italic, 'slant']: self.checkbutton_command(args))
-##
-##		self.underline = tkinter.StringVar()
-##		self.cb3 = tkinter.Checkbutton(self.topframe, font=('TkDefaultFont', 10), offvalue=0, onvalue=1, text='Underline', variable=self.underline)
-##		self.cb3.pack(pady=10, anchor='w')
-##		self.cb3.config(command=lambda args=[self.underline, 'underline']: self.checkbutton_command(args))
-##
-##		self.overstrike = tkinter.StringVar()
-##		self.cb4 = tkinter.Checkbutton(self.topframe, font=('TkDefaultFont', 10), offvalue=0, onvalue=1, text='Overstrike', variable=self.overstrike)
-##		self.cb4.pack(pady=10, anchor='w')
-##		self.cb4.config(command=lambda args=[self.overstrike, 'overstrike']: self.checkbutton_command(args))
-		
-		
-		
-		self.filter_mono = tkinter.IntVar()
-		self.cb5 = tkinter.Checkbutton(self.topframe, font=('TkDefaultFont', 10), offvalue=0, onvalue=1, text='Mono', variable=self.filter_mono)
-		self.cb5.pack(pady=10, anchor='w')
-		self.cb5.config(command=self.filter_fonts)
-		
-		self.filter_const_height = tkinter.IntVar()
-		self.cb6 = tkinter.Checkbutton(self.topframe, font=('TkDefaultFont', 10), offvalue=0, onvalue=1, text='Const height', variable=self.filter_const_height)
-		self.cb6.pack(pady=10, anchor='w')
-		self.cb6.config(command=self.filter_fonts)
-		
-			
-		info_text = '''Being monospaced does not guarantee same lineheight between lines not containing bold text
-and lines that do contain bold text, like keywords.
-Courier for example is monospaced but does not have this kind of constant lineheight.
-If choosing other than constant lineheight font, linenumbers
-can have little offset. If this does not bother, then select any monospaced for programming.'''
-
-
-		self.l = tkinter.Label(self.bottomframe, text=info_text, font=('TkDefaultFont', 10), anchor="e", justify=tkinter.LEFT)
-		self.l.pack(padx=4, pady=4)
-		
-		
-		# Get current fontsize and show it in spinbox
-		self.sb.delete(0, 'end')
-		fontsize = self.font['size']
-		self.sb.insert(0, fontsize)
-
-
-		# Check rest font configurations:
-		self.cb1.deselect()
-##		self.cb2.deselect()
-##		self.cb3.deselect()
-##		self.cb4.deselect()
-		self.cb5.deselect()
-		self.cb6.deselect()
-		
-		if self.font['weight'] == 'bold': self.cb1.select()
-##		if self.font['slant'] == 'italic': self.cb2.select()
-##		if self.font['underline'] == 1: self.cb3.select()
-##		if self.font['overstrike'] == 1: self.cb4.select()
-
-		self.lb.bind('<ButtonRelease-1>', self.change_font)
-			
-		
-		# Increase font-size
-		if big: self.button_command()
-		
-		
-		self.fontnames = list()
-		self.fontnames_mono = list()
-		self.fontnames_const_line = list()
-		self.fontnames_const_line_mono = list()
-		
-		self.top.after(200, self.get_fonts)
-		
-		
-	def button_command(self, event=None):
-		'''	In case there is not font-scaling in use by OS and
-			using hdpi-screen.
-		'''
-		widgetlist = [
-					self.optionmenu,
-					self.menu,
-					self.lb,
-					self.sb,
-					self.cb1,
-##					self.cb2,
-##					self.cb3,
-##					self.cb4,
-					self.cb5,
-					self.cb6,
-					self.l
-					]
-					
-		if self.button['text'] == 'BIG':
-			for widget in widgetlist:
-				widget.config(font=('TkDefaultFont', 20))
-			
-		if self.button['text'] == 'SMALL':
-			for widget in widgetlist:
-				widget.config(font=('TkDefaultFont', 10))
-				
-		if self.button['text'] == 'BIG':
-			self.button['text'] = 'SMALL'
-		else:
-			self.button['text'] = 'BIG'
-			
-	
-	
-	def filter_fonts(self, event=None):
-		'''	Show all fonts, mono-spaced, constant line height, or
-			mono-spaced and constant line height depending on cb5 and cb6
-			settings.
-		'''
-	
-		filter_mono = self.filter_mono.get()
-		filter_const_height = self.filter_const_height.get()
-
-		fonts = None
-		
-		if filter_mono and filter_const_height:
-			fonts = self.fontnames_const_line_mono
-					
-		elif filter_mono:
-			fonts = self.fontnames_mono
-			
-		elif filter_const_height:
-			fonts = self.fontnames_const_line
-		
-		else:
-			fonts = self.fontnames
-		
-		
-		
-		self.top.selection_clear()
-		self.lb.delete(0, 'end')
-		
-		
-		for name in fonts:
-			self.lb.insert('end', name)
-		
-		
-		# Show current fontname in listbox if found
-		try:
-			fontname = self.font.actual("family")
-			fontindex = fonts.index(fontname)
-			self.top.after(100, lambda args=[fontindex]: self.lb.select_set(args))
-			self.top.after(300, lambda args=[fontindex]: self.lb.see(args))
-			
-		except ValueError:
-			# not in list
-			pass
-	
-	
-	def checkbutton_command(self, args, event=None):
-		'''	args[0] is tkinter.StringVar instance
-			args[1] is string
-		'''
-		var = args[0]
-		key = args[1]
-		
-		
-		self.font[key] = var.get()
-		
-		if self.tracefunc:
-			self.tracefunc()
-		
-		
-	def optionmenu_command(self, event=None):
-		'''	When font(instance) is selected from optionmenu.
-		'''
-		self.font = tkinter.font.nametofont(self.var.get())
-		self.top.selection_clear()
-		
-		try:
-			fontname = self.font.actual("family")
-			fontindex = self.fontnames.index(fontname)
-			self.lb.select_set(fontindex)
-			self.lb.see(fontindex)
-		
-		except ValueError:
-			# not in list
-			pass
-
-		
-		self.sb.delete(0, 'end')
-		fontsize = self.font['size']
-		self.sb.insert(0, fontsize)
-		
-		self.cb1.deselect()
-##		self.cb2.deselect()
-##		self.cb3.deselect()
-##		self.cb4.deselect()
-		
-		if self.font['weight'] == 'bold': self.cb1.select()
-##		if self.font['slant'] == 'italic': self.cb2.select()
-##		if self.font['underline'] == 1: self.cb3.select()
-##		if self.font['overstrike'] == 1: self.cb4.select()
-
-		
-	def change_font(self, event=None):
-		'''	Change values of current font-instance.
-		'''
-		
-		l = None
-		l = self.lb.curselection()
-		
-		#print(type(l), l)
-
-		if l in [(), None, ""]:
-			self.font.config(
-				size=self.sb.get()
-				)
-		
-		else:
-			f = self.lb.get(l)
-		
-			self.font.config(
-				family=f,
-				size=self.sb.get()
-				)
-
-
-		if self.tracefunc:
-			self.tracefunc()
-
-	
-	def get_fonts(self):
-		'''	Return list of fonts, that have: same lineheight between normal
-			lines and lines with bold font.
-		'''
-		
-		font1 = tkinter.font.Font(family='TkDefaultFont', size=12)
-		boldfont = font1.copy()
-		boldfont.config(weight='bold')
-		
-		# Second test: filter out vertical fonts.
-		def test_font(f):
-			return f in self.badfonts or f[0] == '@'
-			
-		
-		fontnames = [f for f in tkinter.font.families() if not test_font(f)]
-		
-		# Remove duplicates then sort
-		s = set(fontnames)
-		fontnames = [f for f in s]
-		fontnames.sort()
-		
-		
-		for name in fontnames:
-			font1.config(family=name)
-			boldfont.config(family=name)
-			
-			l1=font1.metrics()['linespace']
-			l2=boldfont.metrics()['linespace']
-			
-			a1=font1.metrics()['ascent']
-			a2=boldfont.metrics()['ascent']
-			
-			d1=font1.metrics()['descent']
-			d2=boldfont.metrics()['descent']
-			
-			f1=font1.metrics()['fixed']
-			f2=boldfont.metrics()['fixed']
-			
-			
-			# Give info that something is happening.
-			self.fontnames.append(name)
-			self.lb.insert('end', name)
-			self.lb.see('end')
-			self.top.update_idletasks()
-			
-			
-			# This guarantees same lineheight between
-			# normal and bold lines. Consolas for example.
-			if l1 == l2 and a1 == a2 and d1 == d2:
-				self.fontnames_const_line.append(name)
-			
-				if f1 == True and f1 == f2:
-					self.fontnames_const_line_mono.append(name)
-			
-			
-			# Being monospaced does not guarantee same lineheight between
-			# normal and bold lines. Courier for example.
-			if f1 == True and f1 == f2:
-				self.fontnames_mono.append(name)
-					
-			
-
-		# Show current fontname in listbox
-		try:
-			fontname = self.font.actual("family")
-			fontindex = self.fontnames.index(fontname)
-			self.top.after(100, lambda args=[fontindex]: self.lb.select_set(args))
-			self.top.after(300, lambda args=[fontindex]: self.lb.see(args))
-			
-		except ValueError:
-			# not in list
-			pass
+import tkinter.font
+import tkinter
+
+
+class FontChooser:
+		
+	def __init__(self, master, fontlist, big=False, tracefunc=None, os_type='linux'):
+		'''	master		tkinter.Toplevel
+			fontlist	list of tkinter.font.Font instances
+			big			If true start with bigger font.
+			tracefunc	callable, used in change_font. It arranges variable
+						observer for change on any item in fontlist.
+						This is practically same as if there would be virtual
+						event <<FontChanged>> and tracefunc binded to it.
+		'''
+		
+		self.top = master
+		self.fonts = fontlist
+		
+		if tracefunc:
+			self.tracefunc = tracefunc
+		else:
+			self.tracefunc = None
+		
+		self.badfonts = [
+					'Standard Symbols PS',
+					'OpenSymbol',
+					'Noto Color Emoji',
+					'FontAwesome',
+					'Dingbats',
+					'Droid Sans Fallback',
+					'D050000L'
+					]
+		
+		
+		self.max = 42
+		self.min = 8
+		
+		self.topframe = tkinter.Frame(self.top)
+		self.bottomframe = tkinter.Frame(self.top)
+		self.topframe.pack()
+		self.bottomframe.pack()
+		
+
+		self.option_menu_list = list()
+
+		for font in self.fonts:
+			self.option_menu_list.append(font.name)
+		
+		self.var = tkinter.StringVar()
+		self.var.set(self.option_menu_list[0])
+		self.font = tkinter.font.nametofont(self.var.get())
+		
+		self.optionmenu = tkinter.OptionMenu(self.topframe, self.var, *self.option_menu_list, command=self.optionmenu_command)
+		
+		# Set font of dropdown button:
+		self.optionmenu.config(font=('TkDefaultFont',10))
+		
+		# Set font of dropdown items:
+		self.menu = self.topframe.nametowidget(self.optionmenu.menuname)
+		self.menu.config(font=('TkDefaultFont',10))
+		
+		# Optionmenu contains font-instances to be configured:
+		self.optionmenu.pack(side=tkinter.LEFT)
+		
+		
+		self.button = tkinter.Button(self.topframe, text='BIG', command=self.button_command)
+		self.button.pack()
+		self.scrollbar = tkinter.Scrollbar(self.topframe)
+		
+		# Listbox contains font-choises to select from:
+		self.lb = tkinter.Listbox(self.topframe, font=('TkDefaultFont', 10), selectmode=tkinter.SINGLE, width=40, yscrollcommand=self.scrollbar.set)
+		self.lb.pack(pady=10, side='left')
+		self.scrollbar.pack(side='left', fill='y')
+		self.scrollbar.config(width=30, elementborderwidth=4, command=self.lb.yview)
+		
+		if os_type != 'linux':
+			self.scrollbar.configure(width=16, elementborderwidth=2)
+			
+				
+		# With spinbox we set font size:
+		self.sb = tkinter.Spinbox(self.topframe, font=('TkDefaultFont', 10), from_=self.min, to=self.max, increment=2, width=3, command=self.change_font)
+		self.sb.pack(pady=10, anchor='w')
+		
+		# Make checkboxes for other font configurations
+		self.bold = tkinter.StringVar()
+		self.cb1 = tkinter.Checkbutton(self.topframe, font=('TkDefaultFont', 10), offvalue='normal', onvalue='bold', text='Bold', variable=self.bold)
+		self.cb1.pack(pady=10, anchor='w')
+		self.cb1.config(command=lambda args=[self.bold, 'weight']: self.checkbutton_command(args))
+		
+		
+##		self.italic = tkinter.StringVar()
+##		self.cb2 = tkinter.Checkbutton(self.topframe, font=('TkDefaultFont', 10), offvalue='roman', onvalue='italic', text='Italic', variable=self.italic)
+##		self.cb2.pack(pady=10, anchor='w')
+##		self.cb2.config(command=lambda args=[self.italic, 'slant']: self.checkbutton_command(args))
+##
+##		self.underline = tkinter.StringVar()
+##		self.cb3 = tkinter.Checkbutton(self.topframe, font=('TkDefaultFont', 10), offvalue=0, onvalue=1, text='Underline', variable=self.underline)
+##		self.cb3.pack(pady=10, anchor='w')
+##		self.cb3.config(command=lambda args=[self.underline, 'underline']: self.checkbutton_command(args))
+##
+##		self.overstrike = tkinter.StringVar()
+##		self.cb4 = tkinter.Checkbutton(self.topframe, font=('TkDefaultFont', 10), offvalue=0, onvalue=1, text='Overstrike', variable=self.overstrike)
+##		self.cb4.pack(pady=10, anchor='w')
+##		self.cb4.config(command=lambda args=[self.overstrike, 'overstrike']: self.checkbutton_command(args))
+		
+		
+		
+		self.filter_mono = tkinter.IntVar()
+		self.cb5 = tkinter.Checkbutton(self.topframe, font=('TkDefaultFont', 10), offvalue=0, onvalue=1, text='Mono', variable=self.filter_mono)
+		self.cb5.pack(pady=10, anchor='w')
+		self.cb5.config(command=self.filter_fonts)
+		
+		self.filter_const_height = tkinter.IntVar()
+		self.cb6 = tkinter.Checkbutton(self.topframe, font=('TkDefaultFont', 10), offvalue=0, onvalue=1, text='Const height', variable=self.filter_const_height)
+		self.cb6.pack(pady=10, anchor='w')
+		self.cb6.config(command=self.filter_fonts)
+		
+			
+		info_text = '''Being monospaced does not guarantee same lineheight between lines not containing bold text
+and lines that do contain bold text, like keywords.
+Courier for example is monospaced but does not have this kind of constant lineheight.
+If choosing other than constant lineheight font, linenumbers
+can have little offset. If this does not bother, then select any monospaced for programming.'''
+
+
+		self.l = tkinter.Label(self.bottomframe, text=info_text, font=('TkDefaultFont', 10), anchor="e", justify=tkinter.LEFT)
+		self.l.pack(padx=4, pady=4)
+		
+		
+		# Get current fontsize and show it in spinbox
+		self.sb.delete(0, 'end')
+		fontsize = self.font['size']
+		self.sb.insert(0, fontsize)
+
+
+		# Check rest font configurations:
+		self.cb1.deselect()
+##		self.cb2.deselect()
+##		self.cb3.deselect()
+##		self.cb4.deselect()
+		self.cb5.deselect()
+		self.cb6.deselect()
+		
+		if self.font['weight'] == 'bold': self.cb1.select()
+##		if self.font['slant'] == 'italic': self.cb2.select()
+##		if self.font['underline'] == 1: self.cb3.select()
+##		if self.font['overstrike'] == 1: self.cb4.select()
+
+		self.lb.bind('<ButtonRelease-1>', self.change_font)
+			
+		
+		# Increase font-size
+		if big: self.button_command()
+		
+		
+		self.fontnames = list()
+		self.fontnames_mono = list()
+		self.fontnames_const_line = list()
+		self.fontnames_const_line_mono = list()
+		
+		self.top.after(200, self.get_fonts)
+		
+		
+	def button_command(self, event=None):
+		'''	In case there is not font-scaling in use by OS and
+			using hdpi-screen.
+		'''
+		widgetlist = [
+					self.optionmenu,
+					self.menu,
+					self.lb,
+					self.sb,
+					self.cb1,
+##					self.cb2,
+##					self.cb3,
+##					self.cb4,
+					self.cb5,
+					self.cb6,
+					self.l
+					]
+					
+		if self.button['text'] == 'BIG':
+			for widget in widgetlist:
+				widget.config(font=('TkDefaultFont', 20))
+			
+		if self.button['text'] == 'SMALL':
+			for widget in widgetlist:
+				widget.config(font=('TkDefaultFont', 10))
+				
+		if self.button['text'] == 'BIG':
+			self.button['text'] = 'SMALL'
+		else:
+			self.button['text'] = 'BIG'
+			
+	
+	
+	def filter_fonts(self, event=None):
+		'''	Show all fonts, mono-spaced, constant line height, or
+			mono-spaced and constant line height depending on cb5 and cb6
+			settings.
+		'''
+	
+		filter_mono = self.filter_mono.get()
+		filter_const_height = self.filter_const_height.get()
+
+		fonts = None
+		
+		if filter_mono and filter_const_height:
+			fonts = self.fontnames_const_line_mono
+					
+		elif filter_mono:
+			fonts = self.fontnames_mono
+			
+		elif filter_const_height:
+			fonts = self.fontnames_const_line
+		
+		else:
+			fonts = self.fontnames
+		
+		
+		
+		self.top.selection_clear()
+		self.lb.delete(0, 'end')
+		
+		
+		for name in fonts:
+			self.lb.insert('end', name)
+		
+		
+		# Show current fontname in listbox if found
+		try:
+			fontname = self.font.actual("family")
+			fontindex = fonts.index(fontname)
+			self.top.after(100, lambda args=[fontindex]: self.lb.select_set(args))
+			self.top.after(300, lambda args=[fontindex]: self.lb.see(args))
+			
+		except ValueError:
+			# not in list
+			pass
+	
+	
+	def checkbutton_command(self, args, event=None):
+		'''	args[0] is tkinter.StringVar instance
+			args[1] is string
+		'''
+		var = args[0]
+		key = args[1]
+		
+		
+		self.font[key] = var.get()
+		
+		if self.tracefunc:
+			self.tracefunc()
+		
+		
+	def optionmenu_command(self, event=None):
+		'''	When font(instance) is selected from optionmenu.
+		'''
+		self.font = tkinter.font.nametofont(self.var.get())
+		self.top.selection_clear()
+		
+		try:
+			fontname = self.font.actual("family")
+			fontindex = self.fontnames.index(fontname)
+			self.lb.select_set(fontindex)
+			self.lb.see(fontindex)
+		
+		except ValueError:
+			# not in list
+			pass
+
+		
+		self.sb.delete(0, 'end')
+		fontsize = self.font['size']
+		self.sb.insert(0, fontsize)
+		
+		self.cb1.deselect()
+##		self.cb2.deselect()
+##		self.cb3.deselect()
+##		self.cb4.deselect()
+		
+		if self.font['weight'] == 'bold': self.cb1.select()
+##		if self.font['slant'] == 'italic': self.cb2.select()
+##		if self.font['underline'] == 1: self.cb3.select()
+##		if self.font['overstrike'] == 1: self.cb4.select()
+
+		
+	def change_font(self, event=None):
+		'''	Change values of current font-instance.
+		'''
+		
+		l = None
+		l = self.lb.curselection()
+		
+		#print(type(l), l)
+
+		if l in [(), None, ""]:
+			self.font.config(
+				size=self.sb.get()
+				)
+		
+		else:
+			f = self.lb.get(l)
+		
+			self.font.config(
+				family=f,
+				size=self.sb.get()
+				)
+
+
+		if self.tracefunc:
+			self.tracefunc()
+
+	
+	def get_fonts(self):
+		'''	Return list of fonts, that have: same lineheight between normal
+			lines and lines with bold font.
+		'''
+		
+		font1 = tkinter.font.Font(family='TkDefaultFont', size=12)
+		boldfont = font1.copy()
+		boldfont.config(weight='bold')
+		
+		# Second test: filter out vertical fonts.
+		def test_font(f):
+			return f in self.badfonts or f[0] == '@'
+			
+		
+		fontnames = [f for f in tkinter.font.families() if not test_font(f)]
+		
+		# Remove duplicates then sort
+		s = set(fontnames)
+		fontnames = [f for f in s]
+		fontnames.sort()
+		
+		
+		for name in fontnames:
+			font1.config(family=name)
+			boldfont.config(family=name)
+			
+			l1=font1.metrics()['linespace']
+			l2=boldfont.metrics()['linespace']
+			
+			a1=font1.metrics()['ascent']
+			a2=boldfont.metrics()['ascent']
+			
+			d1=font1.metrics()['descent']
+			d2=boldfont.metrics()['descent']
+			
+			f1=font1.metrics()['fixed']
+			f2=boldfont.metrics()['fixed']
+			
+			
+			# Give info that something is happening.
+			self.fontnames.append(name)
+			self.lb.insert('end', name)
+			self.lb.see('end')
+			self.top.update_idletasks()
+			
+			
+			# This guarantees same lineheight between
+			# normal and bold lines. Consolas for example.
+			if l1 == l2 and a1 == a2 and d1 == d2:
+				self.fontnames_const_line.append(name)
+			
+				if f1 == True and f1 == f2:
+					self.fontnames_const_line_mono.append(name)
+			
+			
+			# Being monospaced does not guarantee same lineheight between
+			# normal and bold lines. Courier for example.
+			if f1 == True and f1 == f2:
+				self.fontnames_mono.append(name)
+					
+			
+
+		# Show current fontname in listbox
+		try:
+			fontname = self.font.actual("family")
+			fontindex = self.fontnames.index(fontname)
+			self.top.after(100, lambda args=[fontindex]: self.lb.select_set(args))
+			self.top.after(300, lambda args=[fontindex]: self.lb.see(args))
+			
+		except ValueError:
+			# not in list
+			pass
```

### Comparing `henxel-0.3.0/src/henxel/wordexpand.py` & `henxel-0.3.1/src/henxel/wordexpand.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,127 +1,135 @@
-'''Complete the current word before the cursor with words in the editor.
-
-This file is taken from Python:idlelib -github-page:
-https://github.com/python/cpython/tree/3.11/Lib/idlelib/
-
-Each event that is binded to expander replaces the word with a
-different word with the same prefix. The search for matches begins
-before the target and moves toward the top of the editor. It then starts
-after the cursor and moves down. It then returns to the original word and
-the cycle starts again.
-
-Changing the current text line or leaving the cursor in a different
-place before requesting the next selection causes ExpandWord to reset
-its state.
-'''
-
-
-import re
-
-
-class ExpandWord:
-	wordchars = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789_'
-	# string.ascii_letters + string.digits + "_"
-
-
-	def __init__(self, textwid):
-		"textwid is tkinter.Text -widget"
-		
-		self.textwid = textwid
-		self.bell = self.textwid.bell
-		self.state = None
-
-
-	def expand_word_event(self, event):
-		"Replace the current word with the next expansion."
-		
-		curinsert = self.textwid.index("insert")
-		curline = self.textwid.get("insert linestart", "insert lineend")
-		
-		if not self.state:
-			words = self.getwords()
-			index = 0
-		else:
-			words, index, insert, line = self.state
-			
-			if insert != curinsert or line != curline:
-				words = self.getwords()
-				index = 0
-				
-		if not words:
-			self.bell()
-			
-			return "break"
-			
-			
-		word = self.getprevword()
-		self.textwid.delete("insert - %d chars" % len(word), "insert")
-		newword = words[index]
-		index = (index + 1) % len(words)
-		
-		if index == 0:
-			self.bell()            # Warn we cycled around
-			
-		self.textwid.insert("insert", newword)
-		curinsert = self.textwid.index("insert")
-		curline = self.textwid.get("insert linestart", "insert lineend")
-		self.state = words, index, curinsert, curline
-		
-		return "break"
-
-
-	def getwords(self):
-		"Return a list of words that match the prefix before the cursor."
-		
-		word = self.getprevword()
-
-		if not word:
-			return []
-
-		before = self.textwid.get("1.0", "insert wordstart")
-		wbefore = re.findall(r"\b" + word + r"\w+\b", before)
-		del before
-
-		after = self.textwid.get("insert wordend", "end")
-		wafter = re.findall(r"\b" + word + r"\w+\b", after)
-		del after
-
-		if not wbefore and not wafter:
-			return []
-
-
-		words = []
-		dict = {}
-		
-		# search backwards through words before
-		wbefore.reverse()
-
-		for w in wbefore:
-			if dict.get(w):
-				continue
-				
-			words.append(w)
-			dict[w] = w
-
-		# search onwards through words after
-		for w in wafter:
-			if dict.get(w):
-				continue
-			
-			words.append(w)
-			dict[w] = w
-
-		words.append(word)
-		return words
-
-
-	def getprevword(self):
-		"Return the word prefix before the cursor."
-
-		line = self.textwid.get("insert linestart", "insert")
-		i = len(line)
-
-		while i > 0 and line[i-1] in self.wordchars:
-			i = i-1
-
-		return line[i:]
-
+'''Complete the current word before the cursor with words in the editor.
+
+This file is taken from Python:idlelib -github-page:
+https://github.com/python/cpython/tree/3.11/Lib/idlelib/
+
+Each call to expand_word() replaces the word with a
+different word with the same prefix. The search for matches begins
+before the target and moves toward the top of the editor. It then starts
+after the cursor and moves down. It then returns to the original word and
+the cycle starts again.
+
+Changing the current text line or leaving the cursor in a different
+place before requesting the next selection causes ExpandWord to reset
+its state.
+'''
+
+
+import re
+
+
+class ExpandWord:
+	wordchars = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789_.'
+	# string.ascii_letters + string.digits + "_" + "."
+
+
+	def __init__(self, textwid):
+		"textwid is tkinter.Text -widget"
+		
+		self.textwid = textwid
+		self.bell = self.textwid.bell
+		self.state = None
+		
+
+	def expand_word(self):
+		"Replace the current word with the next expansion."
+		
+		curinsert = self.textwid.index("insert")
+		curline = self.textwid.get("insert linestart", "insert lineend")
+		
+		# if used first time:
+		if not self.state:
+			words = self.getwords()
+			index = 0
+			
+			
+		# if used second time:
+		else:
+			words, index, insert, line = self.state
+			
+			if insert != curinsert or line != curline:
+				words = self.getwords()
+				index = 0
+				
+				
+		if not words:
+			self.bell()
+			return "break"
+			
+			
+			
+		word = self.getprevword()
+		self.textwid.delete("insert - %d chars" % len(word), "insert")
+		
+		newword = words[index]
+		index = (index + 1) % len(words)
+		
+		if index == 0:
+			self.bell()            # Warn we cycled around
+			
+		self.textwid.insert("insert", newword)
+		
+
+		curinsert = self.textwid.index("insert")
+		curline = self.textwid.get("insert linestart", "insert lineend")
+		self.state = words, index, curinsert, curline
+		
+		return "break"
+
+			
+	def getwords(self):
+		"Return a list of words that match the prefix before the cursor."
+		
+		word = self.getprevword()
+
+		if not word:
+			return []
+
+		before = self.textwid.get("1.0", "insert wordstart")
+		wbefore = re.findall(r"\b" + word + r"\w+\b", before)
+		del before
+
+		after = self.textwid.get("insert wordend", "end")
+		wafter = re.findall(r"\b" + word + r"\w+\b", after)
+		del after
+
+		if not wbefore and not wafter:
+			return []
+		
+		
+		words = []
+		dict = {}
+		
+		# search backwards through words before
+		wbefore.reverse()
+
+		for w in wbefore:
+			if dict.get(w):
+				continue
+				
+			words.append(w)
+			dict[w] = w
+
+		# search onwards through words after
+		for w in wafter:
+			if dict.get(w):
+				continue
+			
+			words.append(w)
+			dict[w] = w
+
+		words.append(word)
+		return words
+
+
+	def getprevword(self):
+		"Return the word prefix before the cursor."
+
+		line = self.textwid.get("insert linestart", "insert")
+		i = len(line)
+
+		while i > 0 and line[i-1] in self.wordchars:
+			i = i-1
+
+		return line[i:]
+
```

