<img width="484" height="201" alt="image" src="https://github.com/user-attachments/assets/ac1730eb-e4c0-47e3-95f1-8ee613ea2a4c" />

This Challenge is a bonus as to solve it we just follow the steps of the challenge in `DOM XSS` but replace the payload with the new one:

`<iframe width="100%" height="166" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/771984076&color=%23ff5500&auto_play=true&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true"></iframe>` 


The payload embeds a SoundCloud track inside an iframe with specific size and playback settings.


<img width="1599" height="842" alt="Screenshot 2025-07-30 121902" src="https://github.com/user-attachments/assets/1133f9b4-63a8-4654-a2c0-43a732ddc55d" />

