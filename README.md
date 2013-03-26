# Seatbelt Profiles


## Description ##

This is a fork of a collection of profiles for the OSX Application 
Sandbox called Seatbelt. For some background information on how
this whole thing works, check out [Dion Blazakis's Blackhat Talk](https://media.blackhat.com/bh-dc-11/Blazakis/BlackHat_DC_2011_Blazakis_Apple_Sandbox-wp.pdf).
~~My~~ **The original author's** hopes ~~are~~ **were** that people will start to make their own by maybe forking ~~this~~ **the original** repository and adding new rules and profiles to it. 

## Basic Usage ##

To get things rolling immediately you should just be able to run the corresponding shell scripts. ~~I have~~ **The original author has** taken care to make them portable. Dropping to a terminal (for example) and running: `./safari.sh` should fire up a "fresh" Safari. 
To learn more about the sandbox profile syntax you can't easily [google for them](http://www.google.com/search?q=version+1+filetype:sb). You can however learn a bit by looking at the ones that ship with OS X by default by dropping to a terminal and
looking in `/usr/share/sandbox`, `/System/Library/Sandbox/Profiles`, or `/Library/Sandbox/Profiles`, or `System/Library/Sandbox/Profiles`:

     stephens-computer:sandbox_profiles s7$ cd /usr/share/sandbox/
     stephens-computer:sandbox s7$ ls
     awacsd.sb                    mds.sb                       sshd.sb
     bsd.sb                       mdworker.sb                  syslogd.sb
     cvmsCompAgent.sb             named.sb                     xgridagentd.sb
     cvmsServer.sb                ntpd.sb                      xgridagentd_task_nobody.sb
     fontmover.sb                 portmap.sb                   xgridagentd_task_somebody.sb
     kadmind.sb                   preview.sb                   xgridcontrollerd.sb
     krb5kdc.sb                   quicklookd-job-creation.sb
     mDNSResponder.sb             quicklookd.sb

You can also glean a bit more by checking the manpages for `sandbox-exec(1)`, `sandbox_init(3)`, `sandbox(7)`, and `sandboxd(8)`.


