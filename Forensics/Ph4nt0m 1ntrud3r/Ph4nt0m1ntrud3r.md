# Ph4nt0m 1ntrud3r

## Tools
- Wireshark
- Cyberchef

# Challenge
Insert the .pcap file inside Wireshark, in order to see the captured traffic.
We can see that all the packets end with a string that can be identified as a Base64 encoded string.
Given that a common pattern of Base64 encoded strings is the fact that they terminate with "==", we should try to
put a filter to see if all of them terminate with that pattern.

If we click on the Base64 part, we can see that it is inside the "tcp.segment_data": so we put the filter `tcp.segment_data contains 3d:3d`, with `3d:3d` the hex value
of "==".

Then, we take all the filtered packets and translate all the contents of it to find the flag:
1. cGljb0NURg== : picoCTF
2. ezF0X3c0cw== : {1t_w4s
3. bnRfdGg0dA== : nt_th4t
4. XzM0c3lfdA== : _34sy_t
5. YmhfNHJfYQ== : bh_4r_a
6. ZjE2MDk4MA== : f160980
7. fQ== : }

Flag: `picoCTF{1t_w4snt_th4t_34sy_tbh_4r_af160980}`