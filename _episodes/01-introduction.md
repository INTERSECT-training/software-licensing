---
title: "Introduction"
teaching: 0
exercises: 0
questions:
- "Key question (FIXME)"
objectives:
- "First learning objective. (FIXME)"
keypoints:
- "First key point. Brief Answer to questions. (FIXME)"
---
# An Introduction to Software Licensing

David E\. Bernholdt

\(he/him\)

Oak Ridge National Laboratory

Software Productivity and Sustainability track @ Argonne Training Program on Extreme\-Scale Computing summer school

Contributors: David E\. Bernholdt \(ORNL\)\, Michael A\. Heroux \(SNL\)\, James Willenbring \(SNL\)

# License, Citation and Acknowledgements

__License and Citation__

This work is licensed under a [Creative](http://creativecommons.org/licenses/by/4.0/)[ Commons Attribution 4\.0 International License](http://creativecommons.org/licenses/by-sa/4.0/) \(CC BY 4\.0\)\.

__The requested citation the overall tutorial is: David E\. Bernholdt\, Anshu Dubey\, Todd Gamblin\, Jared O’Neal\, and __  __Boyana__  __ R\. Norris\, Software Productivity and Sustainability track\, in Argonne Training Program on Extreme\-Scale Computing__  __\, St__  __\. Charles\, Illinois\, 2022\. DOI: __  __[10\.6084/m9\.figshare\.20416215](https://doi.org/10.6084/m9.figshare.20416215)__  __\.__

Individual modules may be cited as  _Speaker\, Module Title_ \, in Better Scientific Software tutorial\, ISC\, 2022 …

__Acknowledgements__

This work was supported by the U\.S\. Department of Energy Office of Science\, Office of Advanced Scientific Computing Research \(ASCR\)\, and by the Exascale Computing Project \(17\-SC\-20\-SC\)\, a collaborative effort of the U\.S\. Department of Energy Office of Science and the National Nuclear Security Administration _\._

This work was performed in part at the Argonne National Laboratory\, which is managed by UChicago Argonne\, LLC for the U\.S\. Department of Energy under Contract No\. DE\-AC02\-06CH11357\.

This work was performed in part at the Lawrence Livermore National Laboratory\, which is managed by Lawrence Livermore National Security\, LLC for the U\.S\. Department of Energy under Contract No\. DE\-AC52\-07NA27344\.

This work was performed in part at the Los Alamos National Laboratory\, which is managed by Triad National Security\, LLC for the U\.S\. Department of Energy under Contract No\.89233218CNA000001

This work was performed in part at the Oak Ridge National Laboratory\, which is managed by UT\-Battelle\, LLC for the U\.S\. Department of Energy under Contract No\. DE\-AC05\-00OR22725\.

This work was performed in part at Sandia National Laboratories\. Sandia National Laboratories is a multi\-mission laboratory managed and operated by National Technology and Engineering Solutions of Sandia\, LLC\.\, a wholly owned subsidiary of Honeywell International\, Inc\.\, for the U\.S\. Department of Energy’s National Nuclear Security Administration under contract DE\-NA0003525\.

This work was performed in part at University of Oregon through a subcontract with Argonne National Laboratory\.

![]({{ page.root }}/fig/licensing0.png)

# Bottom Line Up Front

__How you choose to license your software should be viewed as a __  _tool_  __ to help accomplish your goals for that software\.  __

_There is no universal “right answer”\!_

_The answer may not be your decision\._

This tutorial will present common terminology\, and examples of some of the considerations that might go into choosing a license\.

The intent is to get you thinking\, not to give you answers\.

_This is not legal advice_ \. Consult with true experts before making any consequential decisions\!

# Some Terminology and Background

# Copyright, Patents, Trademarks, and Licenses

* __Copyright__  grants the creator of an  __original work __ exclusive rights to its use and distribution\, including limits on derivative works
* A  __patent__  grants the inventor of  __something new\, useful\, and non\-obvious __ the rights to its production\, use\, and distribution
* A  __trademark__  is a  __sign\, design\, or expression __ which identifies products or services __ __ from a particular source\, as distinguished from other sources
* __Licenses__  are used to transfer \(selected\) rights in a work\, invention\, or mark from one party to another
  * Software licenses are mostly about copyright\, but can contain clauses on patents and trademarks too

# Your Software Starts Out Copyrighted

* Under the law\, the software you write is subject to  __copyright on creation__
  * You don’t have to do anything special to claim copyright
  * Unless you specify some license\, all rights are reserved to the owner of the copyright
* The copyright owner may be  __you\, or your employer__
  * “Work for hire” \(i\.e\.\, as part of your job\) is probably owned by your employer\.  Employment contracts often make IP rights explicit\.
  * Question 1: Who owns the rights in the work you create?
  * Homework: Find out\!
  * If your employer owns the copyright\, you probably have to get formal permission to license and distribute your software
* Exception: Works created by the US government cannot be copyrighted
  * They are considered to be in the public domain
    * Comment: Originally to ensure public access to the US legal code

# The Licensing Spectrum

Proprietary or Closed Licenses

Free or Open Licenses

__Free vs Open Source?__

“Free” in licensing discussions should refer strictly to “freedom” \(to do certain things with the software\)

Often gets conflated with “free as in beer”\, muddling the discussion\.  Hence some prefer term “open source”

__Major names in Free/Open Source Software:__

Free Software Foundation \(FSF\) [http://fsf\.org/licensing](http://fsf.org/licensing)

Open Source Initiative \(OSI\) [http://opensource\.org](http://opensource.org/)

All Rights Reserved

_Common misconception: _  _Nothing in the definition of free or open source software prevents you from making money from it\! \(more later\)_

# Defining Free Software: The Four Freedoms

* _From the Free Software Foundation_
* The freedom to  __run the program __ for any purpose
* The freedom to  __study how the program works__ \, and  __change it__  so it does your computing as you wish
  * __Access to the source code __ is a precondition for this
* The freedom to  __redistribute copies __ so you can help your neighbor
* The freedom to  __distribute copies of your modified versions __ to others\.  By doing this you can give the whole community a chance to benefit from your changes
  * __Access to the source code __ is a precondition for this
* _The OSI has a definition which amounts to the same thing\, for most purposes_

# Permissive vs Copyleft OS Licenses

Permissive

Copyleft

* Licensee can distribute derivative works as they see fit
  * Relicensing of derivatives is allowed
  * Including proprietary licenses
* Examples
  * Apache License
  * MIT License
  * BSD License

* Licensee must distribute derivative works as open source
  * Also referred to as “restrictive” or “viral”
* Examples
  * GPL \(v2 and v3\)
  * LGPL

_Note: _ Derived works may be held private and never released

# What is a Derivative Work?

* _A derivative work is an expressive creation that includes major copyright\-protected elements of a previously created first work _ \(Wikipedia\)
* Basically: modifications to someone else’s software
* But what about linking to a library? \(Statically vs dynamically?\) Interacting via pipes?  Use as a component in a coupled multiphysics application?
  * Opinions differ
  * FSF \(GPL\) considers everything in a single executable to be a derived work \(source of “viral” label\)
  * LGPL created for libraries – says linking not considered derived work
  * Matters less for permissive licenses
  * Leads to concerns over “compatibility” in combining software under different licenses \(more later\)

# Test: Is this an Open Source License?(A real-world example)

In order to acquire access to the code sources\, the recipient agrees:

to compile/use the XYZZY source code AS IS without modification; users however are welcome to request changes\, or to contribute modifications subject to approval of the authors;

if the copy of the XYZZY downloaded by the authorized user is made available to third parties\, to ensure that the user agreement is followed by the third parties;

to send a one\-time email to xyzzy@example\.com describing planned research using that module

prior to publication\, to email a draft of the article/letter/note to xyzzy@example\.com

to include in published results or presentations the proper code name\(s\) and appropriate references\.

# Answer: Is this an Open Source License? No(A real-world example)

In order to acquire access to the code sources\, the recipient agrees:

to compile/use the XYZZY source code AS IS without modification; users however are welcome to request changes\, or to contribute modifications subject to approval of the authors;

if the copy of the XYZZY downloaded by the authorized user is made available to third parties\, to ensure that the user agreement is followed by the third parties;

_This violates the freedom of being able to distribute copies of your modified version of the code to others_

_Perhaps they want to impose some measure of “quality control” over modifications?  Maybe they’ve had problems in the past with users distributing modified code with errors that are believed to reflect poorly on the original code?_

_Possible alternative: Some open source licenses include a requirement that derivatives must be clearly distinguished from the original \(e\.g\.\, different name\)_

# Choosing a License

# Considerations in Choosing a License

* What rights do you want to retain or grant?
  * Who can use the program? \(proprietary vs open\)
  * Can users see the source code? \(proprietary vs open\)
  * Can users modify the source code? \(proprietary vs open\)
  * Can the users redistribute original or modified code? \(proprietary vs open\)
  * Can modified code be relicensed? \(permissive vs copyleft\)
* Compatibility with software under other licenses
  * Permissive licenses have fewer issues
  * [http://www\.fsf\.org/licensing/](error:ppt-link-parsing-issue)
* Labeling of derived works
  * Derived works must be identifieddifferently than original work
* Patent grant/retaliation
* Expectations of the community you want to engage?

* _Use an existing free/open source license rather than inventing a new one\!_
  * _FSF and OSI certify many existing licenses \(~80\) as meeting their criteria_

# Popular OSI-Approved Licenses

| License | Type | GPL-Compatible | Patent Grant |
| :-: | :-: | :-: | :-: |
| Apache License 2.0  | Permissive | v3,not v2 | yes |
| BSD 2-Clause and 3-Clause licenses | Permissive | yes | silent |
| GNU General Public License (GPL) v3 | Copyleft | yes | yes |
| GNU Library or "Lesser" General Public License (LGPL) v3 | Weak Copyleft | yes | yes |
| MIT license (MIT) | Permissive | yes | silent |
| Mozilla Public License 2.0 | Permissive | yes | yes |
| Common Development and Distribution License | Permissive | no | yes |
| Eclipse Public License 2.0 | Weak Copyleft | yes | yes |
| Affero General Public License v3 (network use == distribution) | Copyleft | yes | yes |

![]({{ page.root }}/fig/licensing1.png)

# ChooseALicense.com (by GitHub)

* Primarily a decision\-tree approach to helping you choose a license
* But backed by a repository with analysis of 30\+ widely used licenses
* __The easiest way to access the whole list is to go to the “Appendix”__
  * __[https://choosealicense\.com/appendix/](https://choosealicense.com/appendix/)__
  * A portion of the Appendix is shown at left
* This is implemented in a GitHub repository with Jekyll\, and open to pull requests\!

# Consideration: Software Business Models

| Approach | Proprietary | Copyleft  | Permissive  |
| :-: | :-: | :-: | :-: |
| Sell the software | yes | yes | yes |
| “Fremium” or “dual licensing” allows free use by some, paid by others | yes | yes | yes |
| Relicense to proprietary | n/a | no | yes |
| Sell convenience, e.g., packaging, installation media, pre-compiled executables | yes | yes | yes |
| Sell professional services around the software, e.g., training, technical support, consulting | yes | yes | yes |
| Sell custom development services, e.g., proprietary extensions, accelerated development | yes | yes | yes |
| Sell software-as-a-service (SaaS) | yes | yes | yes |
| Sell the research | yes | yes | yes |

# Consideration: Don’t Want Others to Profit from my Open Source Software

* A permissive license allows someone else to take derivatives proprietary
* A copyleft license will prevent that
* __But there may be other considerations…__
* What if you  _do_  want a commercial entity to use your software?
  * Exposure\, broader distribution
* Copyleft is scary to many commercial entities
  * How far does the viral license reach into other parts of the product?
  * Legal opinions differ\, no case law yet
    * Lawyers will tend toward a conservative answer: avoid copyleft software
    * _Experience: some companies will not consider working with copyleft software_
    * _Experience: some companies consider staff working on copyleft software to be “contaminated” and will not allow them work on other software_
* Even in non\-commercial environments\, copyleft may raise compatibility concerns

# The Software-as-a-Service Conundrum

* Many software\-as\-a\-service \(SaaS\) products make extensive use of open source software
* Some software developers don’t like the possibility that another company can trivially monetize \(other people’s\) software by turning it into a SaaS product
  * It may compete with their own SaaS offerings
  * The SaaS provider can keep enhancements proprietary and while making the benefits available in the SaaS product
* Attempts to curb this via licensing result in licenses that are not open source
  * In some cases\, key modules are changed to proprietary licenses\, while others remain open
* See: [https://arstechnica\.com/information\-technology/2019/10/is\-the\-software\-world\-taking\-too\-much\-from\-the\-open\-source\-community/](https://arstechnica.com/information-technology/2019/10/is-the-software-world-taking-too-much-from-the-open-source-community/)

# Consideration: Protecting my Intellectual Property

* If I make my source code freely available\, then others can use the novel ideas embodied in it to “scoop” me
* Proprietary licenses \(obviously\) allow you to keep source private
* Open source licenses don’t require that you make derived works public\, only that  _if_  you do\, you make the source available
* Delay public release until you’ve had a reasonable chance to exploit the results of your work
  * Until initial papers are published
  * Fixed time period \(e\.g\.\, one year\)
    * A similar compromise is sometimes used in academic publishing: sponsor may want open access but allow publisher a proprietary exploitation period \(often 1 year\) before making it openly available

# Patent Clauses in Software Licenses

* Software patents can be a serious consideration today
  * Regardless of philosophical arguments for or against\, software patents are a reality
  * If you’re using a piece of software \(even open source\) that is covered by a patent and you don’t have a license for the patent\, you’re infringing
  * Not being aware of a patent does not excuse the infringement
  * You can be sued for monetary damages
* Many common software licenses are silent on patents
  * Especially older ones \(e\.g\.\, BSD\, GPLv2\)
* Some newer licenses do include patent clauses
  * Usually a royalty\-free license to use patented content \(e\.g\. Apache 2\.0\, GPLv3\)
  * Some explicitly say that they do not grant any patent rights \(e\.g\.\, BSD 3\-Clause Clear\)
  * Or retaliation clauses: “if you sue me for patent infringement\, you can’t use this software”

# License Compatibility

* In practice\, most software is a  __combined work __ of some kind
  * Multiple packages with \(potentially\) different licenses \(e\.g\. main package and dependencies\)
  * Do the license terms allow the packages to be distributed \(or even used\) together?
  * Is the combined work considered a derived work?
* Different licenses have different concepts of what constitutes a derived work and how derivatives may or must be licensed
  * Example: strong copyleft considers linking to produce a derived work\, and requires derivatives be distributed under the same license as the original
* There are different interpretations of what licenses are compatible
  * Little litigation so far
* Most significant concerns tend to be about distribution of software
  * Larger projects starting to pay more attention to his

# License Compatibility in Pictures

![]({{ page.root }}/fig/licensing2.png)

One view of license compatibility between common FOSS software licenses\. The arrows denote a one directional compatibility\, therefore better compatibility on the left side than on the right side\.  _By David A\. Wheeler \- _  _[http://www\.dwheeler\.com/essays/floss\-license\-slide\.html](http://www.dwheeler.com/essays/floss-license-slide.html)_  _\, CC BY\-SA 3\.0\, _  _[https://commons\.wikimedia\.org/w/index\.php?curid=41060008](https://commons.wikimedia.org/w/index.php?curid=41060008)_  _ _  _via _  _[https://en\.wikipedia\.org/wiki/License\_compatibility](https://en.wikipedia.org/wiki/License_compatibility)_

# Strategies for Reducing License Compatibility Concerns

* Don’t distribute other software packages as part of yours
  * Especially if you’re distributing binaries
  * If you need to modify other software\, try to upstream changes or ship only patches instead
* Consider the licenses of your immediate software ecosystem
  * Your dependencies
  * Other software yours is likely to be used with
  * Think about how your software interacts with other packages in the ecosystem
    * Recall earlier discussion of the different definitions of “derived work” for different licenses
* Consider the licensing practices of the community or target audience
* Permissive licenses tend to have fewer compatibility problems
* Consider relicensing your software
  * More on this coming up

# Considerations Favoring Open Source

Challenges of managing and archiving the paperwork associated with proprietary licenses

Explicit license agreements can inhibit \(legal\) use of software

I want to support peer review and reproducibility in science

My sponsor requires that I release my software as open source

I believe that the results of publicly\-funded research should be publicly available

I want to build a self\-sustaining community around my software

# A Few More Points About our Real-World Example

In order to acquire access to the code sources\, the recipient agrees:

to compile/use the XYZZY source code AS IS without modification; users however are welcome to request changes\, or to contribute modifications subject to approval of the authors;

if the copy of the XYZZY downloaded by the authorized user is made available to third parties\, to ensure that the user agreement is followed by the third parties;

to send a one\-time email to xyzzy@example\.com describing planned research using that module

prior to publication\, to email a draft of the article/letter/note to xyzzy@example\.com

to include in published results or presentations the proper code name\(s\) and appropriate references\.

# Why are these Clauses Included?

prior to publication\, to email a draft of the article/letter/note to xyzzy@example\.com

_An attempt to address prior experience with users misusing the code and producing publications with erroneous results\, thus reflecting poorly on the code used to obtain them\.  _

_Creates a burden on the code owners\._

_Not sure how strongly they attempt to enforce this\._

to include in published results or presentations the proper code name\(s\) and appropriate references\.

_A natural desire for the software to be credited in papers where it is used\.  _

_Does not violate free/open source software principles\.  _

_Some licenses require attribution\, but usually only in source code\._

_Creative Commons licenses can include an attribution clause \(see later slide\)_

_Possible alternative: CITATION file?_

# Some Related Matters

# Software Licenses Can be Changed

* You may start out using one license for your code and later discover unanticipated problems
* Or maybe your goals change
* __But changing licenses is not necessarily easy__
* \(Generally\) each and every contributor to a code holds a copyright interest in it
* Each and every contributor must be contacted and agree to the relicensing
  * In practice\, different institutions may have different ideas of “due diligence”
  * Keep good records of contributors; try to keep them current
* Contributor license agreements \(CLAs\) and contribution transfer agreements \(CTAs\) can simplify this
  * But present different challenges \(see upcoming slide\)

# Changing License Example #1

* Organization owns copyright for several software packages
  * Licensed LGPL
* Authorship agreements were signed at time copyright was asserted
* Several packages contained third\-party source files
  * A variety of licenses
* Many packages received contributions from other authors since initial copyright assertion
* Many prospective \(particularly industry\) customers were wary of LGPL
  * Decision was made to relicense to BSD

# Changing License Example #1 (continued)

* Contributions were deemed to be substantive or “bug fix”
  * This was a distinction suggested by a lawyer\, every situation will be different
* All third\-party software was judged to have a compatible or incompatible license
* Most packages were eventually relicensed\, a few were not
* A contributor agreement was adopted after this
  * Proved challenging in practice and is largely not used\.
* Considered building an agreement into pull\-request template
  * Not clear if that is enforceable
  * Often people do not have the ability to agree on behalf of their employer

# Changing License Example #2

* Another case of moving to a less restrictive license
* Effort was made to obtain agreement from all 400\+ contributors
* This was successful\, except one contributor had passed away
  * His contribution was removed from the code base
* This was a more careful and exhaustive effort than the first example
  * Not implying it is better or worse

# Accepting Code Contributions

* Code contributions are implicitly offered under the current license
* Some projects require a contributor agreement
  * Contributor license agreement \(CLA\) defines the terms between the contributor and the maintainers of the software
  * Contributor transfer agreement \(CTA\) transfers copyright ownership from contributor to maintainers
  * Developer Certificate of Origin \(DCO\) has been proposed as an alternative to CLAs
    * Developer asserts that they have permission to submit the code\. Not a signed legal contract
* Why?
  * Clarify or make explicit terms of contribution \(awareness by contributor\)
  * Obtain additional rights\, e\.g\.\, relicensing\, patents\, etc\.
  * Ensure “clear title” to make the contribution
* Why not?
  * Creates “barriers to entry” – may discourage potential contributors
  * Legal agreements that may require official review and signature
    * _Experience: Lost funding for a project because lawyers wouldn’t agree to terms of a CLA_
* _See Resources slide for several viewpoints _

# Managing Copyright Notices in Software

* All this does no good if you don’t make the license you’ve chosen clear to all
* Need to  __assert copyright __ and make  __license terms__  explicit
* Do these centrally or in every file?
  * Single COPYING or LICENSE file per package \(or directory\)
  * In comments at the top of the file
  * Advantages and disadvantages to each
* _Best practice: do both_
  * Intelligently\, to make it as easy to maintain as possible – script updates\!
* Authorship \(separate\, but related\)
  * Version control is best way to maintain accurate records of authorship
* See [Managing Copyright Information within a Free Software Project](http://softwarefreedom.org/resources/2012/ManagingCopyrightInformation.html) for details
* Also [Software Package Data Exchange](https://spdx.org/) \(SPDX\, emerging standard\)

![]({{ page.root }}/fig/licensing3.png)

# Open Licensing of Non-Software Artifacts

* Creative Commons is a family of licenses analogous to open source\, but for things other than software
* License variants
  * CC BY \(Attribution\)
  * CC BY\-SA \(Attribution\-ShareAlike\)
  * CC BY\-ND \(Attribution\-NoDerivs\)
  * CC BY\-NC \(Attribution\-NonCommercial\)
  * CC BY\-NC\-SA \(Attribution\-NonCommercial\-ShareAlike\)
  * CC BY\-NC\-ND \(Attribution\-NonCommercial\-NoDerivs\)
* CC0 Public Domain Dedication
  * Indicates intent to place artifact in the public domain
  * Doesn’t satisfy legal requirements in all jurisdictions
* _See _  _[https://creativecommons\.org](https://creativecommons.org/)_

![]({{ page.root }}/fig/licensing4.png)

# Additional Resources

[Software Freedom Law Center](http://softwarefreedom.org/) \(SFLC\)

[https://en\.wikipedia\.org/wiki/License\_compatibility](https://en.wikipedia.org/wiki/License_compatibility)

[http://contributoragreements\.org/](http://contributoragreements.org/)\, [https://developercertificate\.org/](https://developercertificate.org/) and [http://ebb\.org/bkuhn/blog/2014/06/09/do\-not\-need\-cla\.html](http://ebb.org/bkuhn/blog/2014/06/09/do-not-need-cla.html)

[US DOE ASCR \(open source\) software policy](https://science.energy.gov/~/media/ascr/pdf/research/docs/Doe_lab_developed_software_policy.pdf)

_Your institution’s Technology Transfer Office \(or equivalent\)_

_An Intellectual Property Lawyer \(knowledgeable in software\)_

Talk to colleagues and learn from their experiences

# Additional resources recommended by others (1/3)

* _I have not yet studied these carefully myself\, but I trust the people who recommend them\._
* [Neil ](https://www.software.ac.uk/about/staff/person/neil-chue-hong)[Chue](https://www.software.ac.uk/about/staff/person/neil-chue-hong)[ Hong](https://www.software.ac.uk/about/staff/person/neil-chue-hong) \(Software Sustainability Institute\) from his tutorial [An Introduction to Software Licensing](https://softwaresaved.github.io/software-licensing-workshop/#/15) \(yes\, the same title as this presentation\, but developed completely independently\)
  * [The Whys and ](http://www.astrobetter.com/blog/2014/03/10/the-whys-and-hows-of-licensing-scientific-code/)[Hows](http://www.astrobetter.com/blog/2014/03/10/the-whys-and-hows-of-licensing-scientific-code/)[ of Licensing Scientific Code](http://www.astrobetter.com/blog/2014/03/10/the-whys-and-hows-of-licensing-scientific-code/)
  * [A Quick Guide to Software Licensing for the Scientist\-Programmer](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1002598)
  * [The Legal Side to Open Source](https://opensource.guide/legal/)
  * [The International Free and Open Source Lawbook](http://ifosslawbook.org/)
  * [qLegal: advice for tech start\-ups \+ entrepreneurs](http://www.qlegal.qmul.ac.uk/)
  * [tl;dr legal: Software Licenses in Plain English](https://tldrlegal.com/)
  * Open Source Software Watch

* _I have not yet studied these carefully myself\, but I trust the people who recommend them\._
* [Todd ](https://people.llnl.gov/gamblin2)[Gamblin](https://people.llnl.gov/gamblin2) \(LLNL\)
  * License compatibility resources
    * [Open Source Licenses and their Compatibility](https://janelia-flyem.github.io/licenses.html)
    * [Which Licenses May Not be Included within Apache Products?](https://www.apache.org/legal/resolved.html#category-x)
  * \(Re\-\) Licensing considerations of various organizations
    * [LLVM Contemplates Relicensing](https://lwn.net/Articles/701155/)\, [LLVM Relicensing Effort](https://foundation.llvm.org/docs/relicensing/)
    * HEP Software Foundation [licensing working group](https://hepsoftwarefoundation.org/activities/licensing.html)\, particularly:
      * [https://hepsoftwarefoundation\.org/organization/2017/02/21/licensing\.html](https://hepsoftwarefoundation.org/organization/2017/02/21/licensing.html)
      * [https://hepsoftwarefoundation\.org/organization/2018/05/09/licensing\.html](https://hepsoftwarefoundation.org/organization/2018/05/09/licensing.html) included this [Update on Software Licensing](https://indico.cern.ch/event/727095/contributions/2992610/attachments/1647248/2633145/HSF_Licensing_Intro_2018-05-09.pdf)
    * EasyBuild: [GPLv2 licensing is a big issue\, consider relicensing to BSD](https://github.com/easybuilders/easybuild-framework/issues/335)
    * [GEANT Intellectual Property Rights Policy](https://geant3plus.archive.geant.net/Documents/GN3_10_325GEANTIPRPolicyv1.2_30SEP11.pdf)

* _I have not yet studied these carefully myself\, but I trust the people who recommend them_
* More from [Todd ](https://people.llnl.gov/gamblin2)[Gamblin](https://people.llnl.gov/gamblin2) \(LLNL\)
  * Patents in software licenses
    * [Why so little love for the patent grant in the MIT License?](https://opensource.com/article/18/3/patent-grant-mit-license)
    * [React’s New MIT License: The Circus Enters Its Third Ring](https://medium.com/@dwalsh.sdlr/reacts-new-mit-license-the-circus-enters-it-s-third-ring-2f1bf989a67f)
    * [GitLab freezes ](https://www.theregister.co.uk/2017/09/20/gitlab_suspends_graphql_project_over_facebook_license_terms/)[GraphQL](https://www.theregister.co.uk/2017/09/20/gitlab_suspends_graphql_project_over_facebook_license_terms/)[ project amid looming Facebook patent fears](https://www.theregister.co.uk/2017/09/20/gitlab_suspends_graphql_project_over_facebook_license_terms/)
    * Rust: [Rust license changing \(very slightly\)](https://mail.mozilla.org/pipermail/rust-dev/2012-November/002664.html)\, [Why dual MIT/ASL2 license?](https://doc.rust-lang.org/1.4.0/complement-project-faq.html#why-dual-mit/asl2-license?)

{% include links.md %}