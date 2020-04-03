# GitLab
My works related to GitLab, a web-based DevOps lifecycle tool that provides a Git-repository manager developed by GitLab Inc.

## Table of Contents
1. [Introduction.](#introduction)
2. [Official references websites.](#references)
3. [Initializing GitLab.](#initializing) 
4. [GitLab developers.](#developers)
5. [GitHub notes.](#github)
6. [GitHub repository calculation.](#calculation)

<a name="introduction"></a>
## 1. Introduction.
<img src="gitlab.png" height="110">
GitLab is a web-based DevOps lifecycle tool that provides a Git-repository manager providing wiki, issue-tracking and CI/CD pipeline features, using an open-source license, developed by GitLab Inc. The software was created by Ukrainians Dmitriy Zaporozhets and Valery Sizov, and is used by several large tech companies including Cisco, IBM, Sony, Jülich Research Center, NASA, Alibaba, Oracle, Invincea, O'Reilly Media, Leibniz-Rechenzentrum (LRZ), CERN, European XFEL, GNOME Foundation, Boeing, Autodata, NVIDIA, and SpaceX.
<br /><br />
The code was originally written in Ruby, with some parts later rewritten in Go, initially as a source code management solution to collaborate with his team on software development. It later evolved to an integrated solution covering the software development life cycle, and then to the whole DevOps life cycle. The current technology stack includes Go, Ruby on Rails and Vue.js.
<br /><br />
GitLab follows an open-core development model where the core functionality is released under an open-source (MIT) license while the additional functionality is under a proprietary license.
<br /><br />
GitLab users in Crimea, Cuba, Iran, North Korea, Sudan, and Syria may not be accessible after the migration to Google. Google has informed GitLab developers that there are legal restrictions that are imposed for those countries by Office of Foreign Assets Control of the United States.

<a name="references"></a>
## 2. Official references websites.
GitLab official website : https://about.gitlab.com <br />

**__GitLab related tools__** <br />
BITNAMI GITLAB CE STACK : https://bitnami.com/stack/gitlab <br />
VMWare : https://www.vmware.com <br />

**_GitLab documentation by GitLab_** <br />
502-Whoops, GitLab is taking too much time to respond by GitLab : https://gitlab.com/gitlab-org/gitlab-foss/issues/30095 <br />

<a name="initializing"></a>
## 3. Initializing GitLab.
Type on your browser address bar `https://bitnami.com/stacks` and press **[ Enter ]**, under the text box below `Search applications` label, type `GitLab` and press **[ Enter ]**, when the word `GitLab CE` shown on your active browser, **[ Mouse Left Click ]** on it. Wait for the new page to appear, then  **[ Mouse Left Click ]** the word **[ Virtual Machines ]**, the text box will turn into yellow colour when your mouse hover over that text. Then check your active web browser address bar, the address of the website is changed into `https://bitnami.com/stack/gitlab/virtual-machine`, press **[ Ctrl ]** + **[ F ]**, then type `Download .VMDK format`, check on your web browser, the same text with orange colour on it, then  **[ Mouse Left Click ]** that `Download .VMDK format` text on your web browser and wait until your web browser download that folder into your local machine.

On your local machine, **[ Mouse Right Click ]** the zip folder that you downloaded earlier, in this case `bitnami-gitlab-12.9.2-0-linux-debian-9-x86_64.zip`, then **[ Mouse Hover ]** into 7-Zip, the 7zip application can be downloaded from : https://www.7-zip.org, then **[ Mouse Left Click ]** into the text `Extract to "bitnami-gitlab-12.9.2-0-linux-debian-9-x86_64.zip"`, then open the newly created `bitnami-gitlab-12.9.2-0-linux-debian-9-x86_64` folder in your local machine by **[ Mouse Double Click ]** on that folder, then **[ Mouse Double Click ]** on `bitnami-gitlab-12.9.2-0-linux-debian-9-x86_64.vmx` file to run the Bitnami Virtual Machine file of GitLab using your hypervisor software such as VMWare Workstation Player, https://www.vmware.com/my/products/workstation-player/workstation-player-evaluation.html or Oracle Virtualbox, https://www.virtualbox.org. Read the Linux documentation, https://github.com/syakirharis25/Linux to make a choice of the desired hypervisor software to run Bitnami GitLab virtual machine.

When your selected hypervisor virtual machine fully initialized on your local machine, enter debian login : `bitnami` and press **[ Enter ]** and the Password: `bitnami`. Wait at least 2 minutes or equivalent to 120 seconds for GitLab fully initialized on your virtual machine.

Do the below commands to check whether GitLab is fully initialized or not on your virtual machine.
```
$ ls
$ cat bitnami_credentials
```

When the GitLab is fully initialized, take note of the default username and the password shown on the screen.

If the GitLab is not fully initialized yet or it takes too long to initialized, then shut down completely the virtual machine, then start again the Bitnami GitLab virtual machine, enter debian login : `bitnami` and press **[ Enter ]** and the Password: `bitnami`, and do this below commands.
```
$ sudo gitlab-ctl restart
$ sudo gitlab-ctl tail
```
Wait for some time for GitLab to fully initialized, until it says on the screen `Use Ctrl-C to stop`, then press **[ Ctrl ]** + **[ C ]** on your keyboard. Shut down your virtual machine, and start it again by **[ Mouse Double Click ]** on `bitnami-gitlab-12.9.2-0-linux-debian-9-x86_64.vmx` file to run the Bitnami Virtual Machine file.

When the GitLab is fully initialized, take note of the default username and the password shown on the screen, also the ip address shown on the screen. Type that ip address shown on your web browser address bar and hit **[ Enter ]** to see whether GitLab is fully initialized or not.

If your web browser show the error message `Whoops, GitLab is taking too much time to respond.`, then do the below command.
```
$ sudo gitlab-ctl reconfigure
```

Wait about 2 minutes to give GitLab to fully reconfigure the configuraytions. Then on your web browser, press **[ Ctrl ]** + **[ R ]** to refresh the page and see whether GitLab is fully inialized or not without the previous error message.

Then register your GitLab account, fill-in all the required information on the form shown on the web browser screen.

<a name="developers"></a>
## 4. GitLab developers.
Dmitriy Zaporozhets : https://github.com/dzaporozhets, https://twitter.com/dzaporozhets <br />
Valery Sizov : https://twitter.com/_ValerySizov_ <br />
 
<a name="github"></a>
## 5. GitHub notes.
Clone the current GitHub remote repository contents into local machine.
```
$ git clone https://github.com/syakirharis25/GitLab.git
$ cd GitLab/
$ git remote -v
$ git status
```

<a name="calculation"></a>
## 6. GitHub repository calculation.
```
draft
```
Refer to : https://github.com/syakirharis25/cloc
