# Linux-Commnd
All Linux command 

**Top 50 Linux Commands You Must Know as a Regular User**

ls - The most frequently used command in Linux to list directories.

pwd - Print working directory command in Linux.

cd - Linux command to navigate through directories

mkdir - Command used to create directories in Linux

mv - Move or rename files in Linux

cp - Similar usage as mv but for copying files in Linux

rm - Delete files or directories

touch - Create blank/empty files

ln - Create symbolic links (shortcuts) to other files

clear - Clear the terminal display

cat - Display file contents on the terminal

echo - Print any text that follows the command

less - Linux command to display paged outputs in the terminal

man - Access manual pages for all Linux commands

uname - Linux command to get basic information about the OS

whoami - Get the active username

tar - Command to extract and compress files in linux

grep - Search for a string within an output

head - Return the specified number of lines from the top

tail - Return the specified number of lines from the bottom

diff - Find the difference between two files

cmp - Allows you to check if two files are identical

comm - Combines the functionality of diff and cmp

sort - Linux command to sort the content of a file while outputting

export - Export environment variables in Linux

zip - Zip files in Linux

unzip - Unzip files in Linux

ssh - Secure Shell command in Linux

service - Linux command to start and stop services

ps - Display active processes

kill and killall - Kill active processes by process ID or name

df - Display disk filesystem information

mount - Mount file systems in Linux

chmod - Command to change file permissions

chown - Command for granting ownership of files or folders

ifconfig - Display network interfaces and IP addresses

traceroute - Trace all the network hops to reach the destination

wget - Direct download files from the internet

ufw - Firewall command

iptables - Base firewall for all other firewall utilities to interface with

apt, pacman, yum, rpm - Package managers depending on the distribution

sudo - Command to escalate privileges in Linux

cal - View a command-line calendar

alias - Create custom shortcuts for your regularly used commands

dd - Majorly used for creating bootable USB sticks

whereis - Locate the binary, source, and manual pages for a command

whatis - Find what a command is used for

top - View active processes live with their system usage

useradd and usermod - Add a new user or change existing user data

passwd - Create or update passwords for existing users



# WHAT IS CRONTAB = Alarm clock for your server. crontab is a time based job scheduler in Linux. 
It help you to run scripts or commands automatically at given time interval.

# Step 1. Install Cron 

Ubuntu / Debian:  sudo apt update -> [Updates package list (basically: "what software versions are available?") ]

sudo apt install cron -> [Installs the cron service (the thing that actually runs scheduled jobs)]

CentOS/RHEL / Amazon Linux: sudo yum install cronie -> [ Installs cron (just a different name: cronie) ]



# Step 2. Start & Enable Service

sudo systemctl start cron -> Starts cron right now

sudo systemctl enable cron -> Makes sure cron starts automatically after reboot

For CentOS / RHEL / Amazon Linux

sudo systemctl start crond -> start cron

sudo systemctl enable crond -> starts automatically after reboot



# Step 3. Check Status

sudo systemctl status cron -> Shows if cron is running, stopped, or silently judging you

# Step 4. Crontab Format (The Star Puzzle *)

*  Minute (0-59)    * Hour (0-23)    * Day of month (1-31)    * Month (1-12)   * Day of week (0-7)     


# Step 5. Example (with meaning)

0 2 * * * /home/app/backup.sh

0 minute (exactly at 00)

2 hour (2 AM)

* → every day

* → every month

* → every weekday










