# ssh

## root password and IP addresses

Root password and IP addresses can be found at the bottom of "Help" / "Copyrights and licenses".

## Updating authorised keys

As `/home/root` is encrypted, ensure authorised keys are stored in both the plain (underlay) `/home/root` as well as the `gocryptfs` layer.


## Linux and ssh over USB

```
sudo ip route add 10.11.99.1 dev usb0    # Or whatever device appears in "ip addr" output
ssh root@10.11.99.1
```
