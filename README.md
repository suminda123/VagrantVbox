#Vagrant, Virtual box and cygwin

#Let's get Chocolatey first
#open administrative PowerShell and then run 
iex ((new-object net.webclient).DownloadString('https://chocolatey.org/install.ps1'))

#Then install vagrant and virtualbox run following
cinst vagrant virtualbox

#Then install Cygwin
choco install cyg-get

#Then install sshclient
cyg-get openssh

#then install clear command
cyg-get ncurses

#now all good to go
#open cygwin from windows applications and type ssh to see ssh client been install.

#type vagrant -v to check vagrant been setup
vagrant -v

#fun stuff now
# setup ubuntu vbox
mkdir ubuntu
cd ubuntu

#then run
vagrant init hashicorp/precise32
#then
vagrant up

#from now, all help need is in following link

http://docs.vagrantup.com/v2/getting-started/index.html