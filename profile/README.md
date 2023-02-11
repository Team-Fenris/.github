# Team Fenris
Team Fenris consisted of five members; [Ørjan Jacobsen](https://github.com/orjanj) ([Cyber Security](https://www.noroff.no/en/studies/university-college/cyber-security)), [Dan Solberg](https://github.com/dansolb) ([Digital Forensics](https://www.noroff.no/en/studies/university-college/digital-forensics)), [Ragnhild Sageng](https://github.com/Lixona) ([Cyber Security](https://www.noroff.no/en/studies/university-college/cyber-security)), [Pål Larssen](https://github.com/palarssen) ([Cyber Security](https://www.noroff.no/en/studies/university-college/cyber-security)) and [Georg Wedel](https://github.com/DarkGogg) ([Cyber Security](https://www.noroff.no/en/studies/university-college/cyber-security)).


## Project description summary
The project delivery is virtual machines that runs several scripts to fake internet connection for any other device connecting to it. The traffic that the device connected sends and requests will be sniffed and analysed. The analysed content can be viewed on a web interface.

## Project demonstration
https://user-images.githubusercontent.com/47573432/218265539-77c6dcac-4305-4d2a-9b92-7cae37188c76.mp4

Video demonstration by [Ragnhild Sageng](https://github.com/Lixona) ([Cyber Security](https://www.noroff.no/en/studies/university-college/cyber-security)).

### Left window
In the left window, the [traffic controller](https://github.com/Team-Fenris/tfcctrl) is started.
The traffic controller sets up an HTTP server, HTTPS server and DNS server on localhost.
The retrieved requests are then saved to a JSON file, and posted to the API side which is located in the [FenrisCMS](https://github.com/Team-Fenris/fenrisCMS).

### Right window
In the right window the [FenrisCMS](https://github.com/Team-Fenris/fenrisCMS) is started.
API calls is tracked which shows POST requests from the traffic controller to various parts of the API (the `/dns`, `/http` and the `/https` side).
