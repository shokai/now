now command
===========
- https://github.com/shokai/now


Install
-------

    % git clone https://github.com/shokai/now.git


Usage
-----

```
% now home
% now
home
% now 'home?'
home ## exit status == 0
% now office
% now
office
% now 'home?'
home ## exit status == 1
```

with pipe and crontab

```
0 * * * * now 'home?' &&  say '家にいます'    > /dev/null 2>&1
0 * * * * now 'home?' || (say '家にいません') > /dev/null 2>&1
```
