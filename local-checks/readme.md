#local-checks

## cmk_cifsmounts

Script ermittelt anhand "/proc/mounts" cifs mounts und prüft mit ls ob auf die entsprechenden mountpoints zugegriffen werden kann.
Im Script wird das Kommando timeout verwendet um ein hängen z.B. bei nicht Erreichbarkeit zu verhindern.

P.S. Eine Version "stat -f" statt ls war leider bei Netzausfall nicht zu gebrauchen.
