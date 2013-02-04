jtn
===

Use your own dictionary when translating documents.

###why?
So you can maintain your own translation database. Easily extensible, easily searchable.

###how?
With grep(1).

###examples?
Sure.

    $ cat $HOME/.config/jtnrc
    /home/pzel/.local/share/JA_EN_dict.txt
  
    $ cat /home/pzel/.local/share/JA_EN_dict.txt | head -n3
    利用している      |	Utilizing
    利用を　検討中      |	Considering utilization
    利用していない（予定なし）      |	Not utilizing (No plan to utilize)
  
    $ jtn 利用
    利用している      |	Utilizing
    利用を　検討中      |	Considering utilization
    利用していない（予定なし）      |	Not utilizing (No plan to utilize)


###$HOME/.config/jtnrc?
I don't like dotfiles in my home directory.