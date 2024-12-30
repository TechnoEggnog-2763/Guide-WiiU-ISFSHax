---
prev: true
next: true
---

# DNSpresso

DNSpresso is an exploit that abuses a vulnerability in the DNS response parsing system to achieve remote code execution. A technical write-up can be found [here](https://garyodernichts.blogspot.com/2023/10/exploiting-dns-response-parsing-on-wii-u.html). Make sure your Wii U has internet access fot this step.

## Instructions

1. Take your SD Card out of your console, and plug it into your Wii U console.
2. Launch System Settings, then navigate to `Internet -> Connect to the Internet`.
3. Press the X button or tap the `Connection List` button, then navigate to your connection
4. Go to `Change Settings -> DNS` and select `Do not auto-obtain`.
5. Enter `85.215.57.182` as the primary DNS, then select `Confirm`.
6. Go back and start a connection test.

Now, you should see the minute main menu.

::: warning

Minute only outputs 1080p through HDMI, though you may see a picture on the gamepad during this step. If you know you do not have a TV that outputs at 1080p through HDMI, you should not continue to follow this guide.

:::
