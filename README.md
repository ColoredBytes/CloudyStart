<p align="center">
  <img src="./assets/github-header-image.png" alt="Header">
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License: MIT">
  </a>
</p>

# :link: Table of Contents

- [:x: Problem](#x-problem)
- [:heavy\_check\_mark: Solution](#heavy_check_mark-solution)
- [:gear: Instructions](#gear-instructions)
- [:memo: Notes](#memo-notes)


## :x: Problem

I've used Proxmox for years and when I came back last year I found out about Cloud-init templates and was blown away by how easy it was. I had one issue though any time I wanted to change the specs of the VM I always needed to clone the Template and then modify the specs. A Little tedious for me So I need an idea. 

## :heavy_check_mark: Solution

**CloudyStart**, is my Solution. As I started getting more into scripting. I worked on this as a side project as I still work a full-time job as an IT Analyst. The cool thing about this script is it still uses cloud-init at its core but it lets you spec down the VM on all sides. Minus Advanced cloud-init configs. Still a WIP but this has done wonders in automating my workflow within Proxmox.

## :gear: Instructions

- **Clone the repo.**
```
git clone https://github.com/ColoredBytes/CloudyStart.git
```


- **Make the script executable.**
 ```
 chmod +x CloudyStart/CloudyStart.sh
 ```

- **Run the script.**
 ```
 ./CloudyStart/CloudyStart.sh
```

## :memo: Notes

I've added a secondary verison of this script using [`whiptail`](CloudyStart-whiptail.sh).

- This is a more interactive version if that's something you like.
    -  Same Changes are required as stated in the notes as well!


> [!NOTE]
> For this script, two variables need to be changed on your end.<br>
```
 VM_STO="" # Set to the storage used for VMs
 CIDR="23 # Should be changed to whatever the CIDR notation is used on your end. 
```
> [!WARNING]
> **Change these before running the script.**
