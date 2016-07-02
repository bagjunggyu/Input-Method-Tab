## Input-Method-Tab
##### Wishlist] Proposal for Input-Method tab to Keyboard plug
##### https://bugs.launchpad.net/switchboard-plug-keyboard/+bug/1397776
##### 
##### Proposal )
##### picture -  https://plus.google.com/101028813073033149665/posts/hFPy9kjVxm3
##### 
##### We Asians don't use keyboard layout when typing our characters,
##### We use Input Method instead.
##### 
##### English or English based keyboard users can choose their keyboard layout in layout
##### but We didn't have this kind of feature until now
##### so we need Input Method tab which we can choose and set our Input Method easily.
##### 
##### * unswitchable between language in Slingshot
##### https://bugs.launchpad.net/scratch/+bug/1397766
##### 
##### * can't write characters
##### https://bugs.launchpad.net/scratch/+bug/1198794
##### 
##### * crash pantheon-files when searching by ibus
##### 
##### 1)
##### set Input Method is GUI of "im-config" usage
##### it output the "im-config -n" Input Method by user selected
##### It shows current input method what user chose to use
##### 
##### usage of im-config is as below ex) 
##### nimf, ibus, fcitx, uim  
##### ex)
##### $ im-config -n nimf 
##### 2)
##### Install/Remove input method
##### it is needed for the new users who don't know well of input method what to use.
##### even we can support default input method though, sometimes users choose their input method by their behaviours.
##### in that cases, it will help users install/remove it easily
##### 
##### 3)
##### settings tool by set IM
##### Loki doesn't support Ayatana and all the input method doesn’t show current state to wingpanel like keyboard layout does.
##### but we need this tools to set up which keyboard to use to input characters.
##### 
##### Settings tool)
##### $ nimf-settings
##### $ ibus-setup
##### $ fcitx-config-gtk
##### $ uim-pref-gtk
##### 
##### ex) for Korean 
##### Hangul, Shift + Space for Hangul
##### Hangul_Hanja for Hanja
##### 
##### [ Input Method for Asian users ]
##### 
##### also it will be used in Install/Remove as packages
##### 
##### * Install
##### $ sudo apt install [below packages]
##### ex)
##### $ sudo apt install uim uim-byeoru
##### 
##### * remove
##### $ sudo apt autoremove [below packages]
##### ex)
##### $ sudo apt autoremove uim uim-byeoru
##### 
##### note]
##### DO NOT remove, purge, or autoremove "ibus" alone like this  “$ sudo apt remove ibus “
##### It must be removed like this “$ sudo apt autoremove ibus-hangul”
##### or, it will crash systems
##### it is allocated with some plugins in switchboard due to its name ibus
##### 
##### == Input Method for CJK
##### Available in scratch-text-editor is marked (0)
##### All of them are package name itself need to install themselves
##### 
##### < Korean >
##### (0) nimf
##### (0) uim uim-byeoru
##### (x) fcitx-hangul
##### (x) ibus-hangul
##### 
##### < Japanese >
##### nimf is preparing for Japanese based on Anthy and it will be added soon on July.
##### https://github.com/cogniti/nimf
##### 
##### (x) ibus-mozc
##### (x) fcitx-mozc
##### (can't test ,nor no need to do in 64-bit) uim uim-mozc:i386
##### (x) ibus-anthy
##### (x) fcitx-anthy
##### (0) uim uim-anthy
##### 
##### < Chinese >
##### (0) nimf
##### (0) uim uim-pinyin
##### (x) fcitx-pinyin
##### (x) fcitx-sunpinyin
##### (x) ibus-pinyin
##### (x) ibus-sunpinyin
##### 
##### Reference]
##### uim - https://packages.debian.org/sid/uim
##### 
##### Note]
##### uim is not working in Github.
##### scratch-text-editor is default text editor of elementary OS
##### 
##### ibus issue
##### https://code.google.com/p/ibus/issues/detail?id=1726
##### 
##### uim issue
##### https://github.com/uim/uim/issues/30
##### 
##### I recommend nimf as default input method for universial usage for CJK
##### and unfortunately, I don't know well of Vietnamese in fact. If we can find more infos ,
##### we need to add it to the Input Method tab.
