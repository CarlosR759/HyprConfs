# Hyprland conf files

***Just my personal Hyprland ecosystem config files***

## Prerequisites 

The following programs should be installed first: 

  - hyprland
  - hyprpaper
  - hyprpicker 
  - hyprlock
  - xdg-desktop-portal-hyprland
  - hyprpolkitagent
  - hyprsunset 
  - eww

Of course you can change the config files or delete them if you just want to use Hyprland compositor without the Hypr suit of tools added in the configs files.  Also you can delete the eww bar and put whatever bar you want. More description of this down below in the FAQ. 


## Installation

<details>
  <summary>Arch</summary>

  ```
    sudo pacman -S hyprland hyprpaper hyprpicker hyprlock xdg-desktop-portal-hyprland hyprpolkitagent hyprsunset
  ```
</details>

<details markdown="1">
  <summary>Debian/ubuntu</summary>

   > - Read this: https://wiki.hypr.land/Getting-Started/Installation/ 
  
</details>

<details markdown="1">
  <summary>RedHat/Fedora</summary>

   > - Read this: https://wiki.hypr.land/Getting-Started/Installation/
   > - This: https://copr.fedorainfracloud.org/coprs/solopasha/hyprland
   > - And this: https://github.com/hyprwm/Hyprland/discussions/284 

</details> 

After installation just git clone this repo and put the files into ~/.config/hypr/ folder.

## FAQ

#### How can not use eww bars ? 

<details markdown="1">
  <content>
    Just go into hyprland.conf and delete the following lines: 

    ```sh
    exec-once = eww daemon
    exec-once = eww open clock
    ```

But remember that if you want to add another sys bar or widget, you need to follow the docs of the specific bar. The default config file is made in mind to work with my eww system bar.
  </content>
</details>



#### How can I just use the keybinds ? 

<details markdown="1">
  <content>
Just go into hyprland.conf and delete all the exec-once = * lines 

But if you delete the exec-once = systemctl --user start hyprpolkitagen, then probably is better to find another alternative for your system. I recomend to use the hyprpolkitagen if you are going to use Hyprland in any case.
  </content>
</details>


#### My distro is not in the installation part: 

<details markdown="1">
  <content>
Just go into this page: https://wiki.hypr.land/Getting-Started/Installation/  

You can notice that some distros are more friendly to install, mainly because Hyprland is very active in development and distros that are made with rolling release of by compiling packages are more friendly to Hyprland, others distros are not generally recomended. In that case I3 window manager can be a nice option if you have an AMD gpu .
  </content>
</details>



