# 2017-11 Raleigh Puppet User Group Meeting notes
+ [This RPUG November meeting on meetup.com](https://www.meetup.com/Raleigh-Puppet-User-Group/events/243275400/)

## RPUG News
+ [Next meeting is Monday December 4 at Red Hat Annex](https://www.meetup.com/Raleigh-Puppet-User-Group/events/244868225/)
+ January meeting is tentatively scheduled for Monday January 8 in Cary.

## Puppet ecosystem software announcements and news bits
+ [Puppet Platform 5.3.2 is now available](https://groups.google.com/forum/#!topic/puppet-announce/jfodzecqLdQ)
+ [Puppet Enterprise 2016.4.8 and 2017.2.4 are now available](https://groups.google.com/forum/#!topic/puppet-announce/m492BkL9GFs)
+ [Puppet Enterprise 2017.3.1 is now available](https://groups.google.com/forum/#!topic/puppet-announce/NS_w5wSUjoI)
+ [Updated the commercial product lifecycle](https://puppet.com/misc/puppet-enterprise-lifecycle)
+ [Forge Support for Modules with Puppet Tasks ](https://forge.puppet.com/modules?with_tasks=true)
+ [Puppet Bolt 0.6.0 released](https://groups.google.com/forum/#!topic/puppet-announce/hMO43gCuTCw)
  - prompting for a password securely rather than requiring it on the command line
  - a security-related bug was fixed where previously Bolt would did not securely verify keys for hosts it had not connected to before.
+ [PDK 1.2 is now available](https://groups.google.com/forum/#!topic/puppet-announce/0B9zzxlhXfE)
  - `pdk new task` generates a new Puppet task
  - `pdk validate` lints task metadata
+ [Foreman 1.16.0-RC2 available for testing](https://groups.google.com/forum/#!topic/foreman-announce/cI0SUU5Ypec)
  - Drop Puppet 3 support in v1.16 as it is deprecated in v1.15
  - Add Puppet 5 support
  - Add the ability to search for a puppet class in the configuration groups
+ [Foreman 1.15.6 bug-fix release](https://groups.google.com/forum/#!topic/foreman-announce/YyiBA_swqys)
  - number of puppet v4 related big fixes during the v1.15.x lifecycle.
+ Puppet tips from Example42 blog:
  - [Week 45 - Save the dates](https://www.example42.com/2017/11/06/example42_events/)
  - [Week 44 - Puppet Code Development IDE](https://www.example42.com/2017/10/30/puppet_development_ide/)
  - [Week 43 - Bolt and tasks with PSICK](https://www.example42.com/2017/10/23/bolt_and_tasks_with_psick/)
  - [Week 42 - Puppet plans and tasks](https://www.example42.com/2017/10/16/plans_and_tasks/)
  - [Week 41 - Introducing PSICK - The Infrastructure Puppet module](https://www.example42.com/2017/10/08/introducing-psick-infrastructure-module/)
  - [Week 40 - Tenant modules](https://www.example42.com/2017/10/02/tenant-modules/)
  - [Week 39 - Secure data management with multiple eyaml keys](https://www.example42.com/2017/09/25/multiple_eyaml_keys/)
  - [Week 38 - When to place data in hiera](https://www.example42.com/2017/09/18/when-to-place-data-in-hiera/)
  - [Week 37 - Automated, reusable hiera eyaml setup](https://www.example42.com/2017/09/11/automate-reusable-eyaml-setup/)

## Selected news items from Puppet.com Blog:
+ [Talking Tech, Puppet’s new webinar series. Register here.](http://info.puppet.com/Talking-Tech-webinar-series-registration.html)
  - Delivering Infrastructure and Security Policy as Code with Puppet and CyberArk Conjur on 8 November
  - Manage F5 BIG-IP Infrastructure with Puppet on 14 November
  - Shift Left: Puppet + CloudPassage = New Approach to Securing DevOps on 15 November

# Meeting's topic: PuppetConf 2017
+ [PuppetConf 2017 Schedule](https://puppetconf17.sched.com/)
+ Big takeways:
  - [Puppet Discovery](https://puppet.com/blog/announcing-puppet-discovery)
    + My summary of it: A technical preview release to let you peer into IT infrastructure where ever they are local, remote, cloud, etc.
  - [Puppet Tasks](https://puppet.com/blog/easily-automate-ad-hoc-work-new-puppet-tasks) is available in two flavors:
    + Puppet Bolt: a agentless open source task runner CLI and executes adhock commands via SSH on Linux and WinRM on Windows.
    + Puppet Enterprise Task Management: Bolt plus WebGUI, RBAC, audit trails, and team-oriented workflows.
  - PDK
  - Resource API
+ Lots of focus on being operating system agnostic for both local development (PDK, editors) and for resources that get managed.
+ [Puppetconf 2017 - Youtube playlist](https://www.youtube.com/watch?v=0u4yo7_-dwg&list=PLV86BgbREluVYuJaYGQ0-ep45NCAFe3OQ&index=1), [Slides ](https://www.slideshare.net/PuppetLabs/presentations),  [Photos.](https://www.flickr.com/photos/puppetlabs/albums/72157689760583916)
+ [2017 Contributor Summit Kickoff & State of the Community](https://youtu.be/T6N4Cm-FJuI?list=PLV86BgbREluVYuJaYGQ0-ep45NCAFe3OQ)
  - Get a feel for the community, though this session contains some of the details and info from the keynote.
  - Some [recommendations from Eric](https://youtu.be/T6N4Cm-FJuI?list=PLV86BgbREluVYuJaYGQ0-ep45NCAFe3OQ&t=1748) on upgrading from puppet v3 to v4.
+ "Beyond RSpec: Innovative Strategies for Confident CI – Kevin Paulisse, GitHub
  - [Video](https://www.youtube.com/watch?v=TkzrUT-ZPQ8), [Slides](https://speakerdeck.com/kpaulisse/puppetconf-2017-beyond-rspec-innovative-strategies-for-confident-ci)
  - Just a fantastic compilation of testing tools and techniques
+ Tried to get into ["Complexity requires simplicity – Martin Alfke, example42 GmbH"](https://www.youtube.com/watch?v=Rp_po_f3MDY) but it was full so went to ["A Not-So-Bumpy Road to Puppet4 at CERN – Nacho Barrientos, CERN"](https://www.youtube.com/watch?v=rqiLQpR3oxo), and in both cases they were excellent.
+ [Puppet Platform: A Path Forward – Eric Sorenson, Puppet](https://www.youtube.com/watch?v=vXwOHMhSmgE)
  - I thought this would be road-map of sorts, but most of the presenation time (approx 30 minutes) was spent looking backward to previous releases 0.2x, 2.x, 3.x. Very little of future was revealed.
+ [How People Actually Write Puppet – Gareth Rushgrove, Puppet](https://www.youtube.com/watch?v=uS0C0dM1StQ)
  - Gareth used Googl's BigQuery to examine public GitHub repos of puppet code and got interesting insights into how puppet code is made.
+ [What's in a Name? Scaling ENC with DNS- Cameron Nicholson, Apple Inc.](https://www.youtube.com/watch?v=AH51NRAWfXs&list=PLV86BgbREluVYuJaYGQ0-ep45NCAFe3OQ&index=4)
  - Great talk that tackles scaling your ENC beyond thousands of nodes
+ [Automated System Compliance from the Inside Out – Trevor Vaughan, Onyx Point](https://www.youtube.com/watch?v=Vp2jTq4dC9c)
  - If you are using puppet or want to use puppet in a USA-centric regulated environment, then this talk is for you.
+ [Hiera 5: The Full Data Enchilada – Henrik Lindberg, Puppet](https://www.youtube.com/watch?v=laA1HGvXB_0)
  - Best summary of this talk is "Everything you wanted to know about Hiera 5 but were afraid to ask."
