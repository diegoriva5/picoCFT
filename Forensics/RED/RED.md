# RED

## Tools
- zsteg

### zsteg
Installation:
1. `sudo apt install ruby ruby-dev build-essential -y`
2. `sudo gem install zsteg`

Verify installation with `zsteg -h`: you should see the menu.

Usage: 
- `zsteg image.png`

## Challenge

An image is given to us. Analyzing it with `zsteg` we can find a text that looks like a Base64 encoded text: `cGljb0NURntyM2RfMXNfdGgzX3VsdDFtNHQzX2N1cjNfZjByXzU0ZG4zNTVffQ==cGljb0NURntyM2RfMXNfdGgzX3VsdDFtNHQzX2N1cjNfZjByXzU0ZG4zNTVffQ==cGljb0NURntyM2RfMXNfdGgzX3VsdDFtNHQzX2N1cjNfZjByXzU0ZG4zNTVffQ==cGljb0NURntyM2RfMXNfdGgzX3VsdDFtNHQzX2N1cjNfZjByXzU0ZG4zNTVffQ==`

The decoded version is: `picoCTF{r3d_1s_th3_ult1m4t3_cur3_f0r_54dn355_}` repeated 4 times.