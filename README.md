This is a fork of HubbeKing's WeeChat dockerfile, twisted to my own uses.  Chances are you have less use for this than you have for his original, as this just tweaks a thing or two and that's it.  Also, I kinda don't use the usual port for the relay.  I'm not sure why.

  - docker compile -t [whatever]/weechat .
  - docker run -d --rm --name weechat [whatever]/weechat
  - Season with -v and -p params to taste
  - Serves one
  - docker exec -it $(docker ps -q -f 'name=weechat') tmux attach

Or maybe with compose?
  - docker-compose up -d
  - docker-compose exec weechat tmux attach
