# Programs - Bash

## ...

```
{ echo "Message"; } 2> /dev/null

{
  echo "The quick brown fox"
  echo "jumps over the lazy dog."
} 2> /dev/null
```

Source

- Suppress execution trace for echo command?
  - https://superuser.com/questions/806599/suppress-execution-trace-for-echo-command 

## ...

> Running a command through /usr/bin/env has the benefit of looking for whatever the default version of the program is in your current environment.
>
> This way, you don't have to look for it in a specific place on the system, as those paths may be in different locations on different systems. As long as it's in your path, it will find it.
>
> One downside is that you will be unable to pass more than one argument (e.g. you will be unable to write /usr/bin/env awk -f) if you wish to support Linux, as POSIX is vague on how the line is to be interpreted, and Linux interprets everything after the first space to denote a single argument. You can use /usr/bin/env -S on some versions of env to get around this, but then the script will become even less portable and break on fairly recent systems (e.g. even Ubuntu 16.04 if not later).
>
> Another downside is that since you aren't calling an explicit executable, it's got the potential for mistakes, and on multiuser systems security problems (if someone managed to get their executable called bash in your path, for example).
>
> #!/usr/bin/env bash #lends you some flexibility on different systems
> 
> #!/usr/bin/bash     #gives you explicit control on a given system of what executable is called
> 
> In some situations, the first may be preferred (like running python scripts with multiple versions of python, without having to rework the executable line). But in situations where security is the focus, the latter would be preferred, as it limits code injection possibilities.

Source

- What is the difference between "#!/usr/bin/env bash" and "#!/usr/bin/bash"?
  - https://stackoverflow.com/questions/16365130/what-is-the-difference-between-usr-bin-env-bash-and-usr-bin-bash
