# Advance-Forensics-Analysis-Tool



<p <img src="![image](https://github.com/user-attachments/assets/7f04cc1f-d9db-480d-ade4-107060788d25)
"/></a></p>

<b>Try it now: https://www.aperisolve.com</b>

# I . What is Advance-Forensics-Analysis-Tool?
Advance-Forensics-Analysis-Tool is a platform which performs layer analysis on image.<br/>
The platform also uses "*zsteg*", "*steghide*", "*outguess*", "*exiftool*", "*binwalk*", "*foremost*" and "*strings*" for deeper steganography analysis.




# IV . Features
Advance-Forensics-Analysis-Tool is based on Python3 with Flask and PIL module, the platform currently supports the following images format: `.png`, `.jpg`, `.gif`, `.bmp`, `.jpeg`, `.jfif`, `.jpe`, `.tiff`.

The platform allow you to:
- **Visualise each bit layer** of each channel for a given image (ie. LSB of Red channel).
- **Browse** and **Download each bit layer image**.
- **Visualise `zsteg` informations** such as text encoded on LSB
- **Download `zsteg` files** such as mp3 encoded on LSB
- **Download `steghide` files** using a defined password
- **Download `outguess` files** using a defined password
- **Visualise `exiftool` informations** such as geolocation or author
- **Visualise `binwalk` informations**
- **Download `binwalk` files** such as zip in png headers
- **Download `foremost` files** such as zip in png headers
- **Visualise `strings` output**

# V . Application

The Aperi'Solve platform is a *Flask* web service (/web) (python 3.7) with backend daemons (/backend) which perform analysis.

Both of the two part has its own docker container.

# VI . Run with Docker-Compose

You can pull all the images from the GitHub Container Registry. A simple docker compose file is included in the repos. Just use:  
```bash
docker compose -f docker-compose.yml up
```

Then check your browser at [http://localhost:5000/](http://localhost:5000).

---


