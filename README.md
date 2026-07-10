# Dell USB Imaging Tool for Wyse 3040 Thin Client
Documentation about how to obtain the Dell USB Imaging Tool 

<p>As I was experimenting with the Dell Wyse 3040 Thin Client that I have, I got curious about trying out the ThinOS and ThinLinux, though there's one thing that's hindering me from trying out the two. Which is <b>Where can I found the Dell USB Imaging Tool needed for it?</b> Luckily after hours of finding I found this blog site (though outdated).</p>

<a href="https://blog.terenceluk.com/2017/01/where-to-download-wyse-usb-firmware.html">Where to download the latest Wyse USB Firmware Tool / Dell USB Firmware Tool</a>

Unfortunately the website is dead. But luckily we have our good old wayback machine https://web.archive.org/

<h1>Steps:</h1>
  <ol>
    <li>Go to https://web.archive.org/ and type https://downloads.dell.com/wyse/ in the search bar</li>
        <img width="1919" height="753" alt="image" src="https://github.com/user-attachments/assets/56bb4ea7-4df3-4251-aaa0-2e25fa0d1b9d" />
    <li>Navigate to the oldest one archived (in this case, 2018),</li>
        <img width="1919" height="979" alt="image" src="https://github.com/user-attachments/assets/700eec39-9fbc-4b55-ac25-6447e8e1aed5" />
    <li>The URL brings you to this archived file directory of the webpage</li>
        <img width="442" height="398" alt="image" src="https://github.com/user-attachments/assets/2395db70-4d37-453e-b498-1ea41f957581" />
           <p>The directory we’re interested in is the <b>USBFT</b></p>
    <li>In the USBFT directory, you will find the different firware version for the USB Tool </li>
        <img width="407" height="370" alt="Screenshot 2026-07-10 194153" src="https://github.com/user-attachments/assets/edb79e36-2c20-424e-b0d9-33a43a586c14" />
    <li>Each version directory you will find a exe file, pdf release note and user guide </li>
        <img width="641" height="267" alt="image" src="https://github.com/user-attachments/assets/404db96a-9e40-4afd-ac87-36f24ee2c7c8" />
    <li>With that done, search you for the merlin image file (of ThinOS/ThinLinux) in the drivers website I've provided below</li>
        <img width="1919" height="940" alt="image" src="https://github.com/user-attachments/assets/f87779af-88e2-4c42-bed6-d90a548e7d20" />
        <img width="725" height="270" alt="image" src="https://github.com/user-attachments/assets/cd6d10cc-3816-43b1-8b83-f98aab343034" />
        <img width="1481" height="70" alt="image" src="https://github.com/user-attachments/assets/2d3466b8-28ce-41a9-b42f-a965a8df7fb8" />
            <p>After download, unzip them either with the Windows File Explorer or Winrar (or even 7-zip)</p>
    <li>Run the USB Imaging Tool installer exe, select the destination path, and let it install</li>
        <img width="687" height="522" alt="Screenshot 2026-07-10 195919" src="https://github.com/user-attachments/assets/e257b884-fa8d-4e83-a72e-91634e42d680" />
        <img width="685" height="519" alt="image" src="https://github.com/user-attachments/assets/1dd75095-03ec-4494-8ac5-3b7176984c36" />
        <img width="690" height="517" alt="image" src="https://github.com/user-attachments/assets/a89b4842-f644-46f7-8e48-7189379fdb17" />
        <img width="686" height="519" alt="image" src="https://github.com/user-attachments/assets/c8d656fa-1516-4200-87a1-896ea85e9300" />
    <li>But before we continue, you must ensure that the USB flash drive you're using is formatted into <b>FAT32</b></li>
        <img width="139" height="54" alt="image" src="https://github.com/user-attachments/assets/c6100ffe-c091-4aaf-866b-34ecec350439" />
            <p>If not, then you could format it via File Explorer by right-clicking on the USB flash drive and selecting <b>format</b></p>
        <img width="352" height="229" alt="image" src="https://github.com/user-attachments/assets/a695e4b7-e285-4c39-926b-63175d2ac6de" />
        <br>
        <img width="240" height="437" alt="image" src="https://github.com/user-attachments/assets/900906e8-8de9-4ee5-93f7-88d414739545" />
    <li>Once done, open the USB Imaging tool and select the correct Drive Letter of your USB drive</li>
        <img width="80" height="104" alt="image" src="https://github.com/user-attachments/assets/91a6a083-b249-4fef-9b39-e0a6bcc7eac2" />
        <img width="1012" height="697" alt="image" src="https://github.com/user-attachments/assets/c1eb2c8d-1701-4300-aca1-46eb968c8523" />
    <li>Go to the Image Push navigation and select 64-bit</li>
        <img width="1016" height="697" alt="image" src="https://github.com/user-attachments/assets/dbfa5b67-c203-4008-871d-9cfdc74083cf" />
    <li>Click on the (+) Icon on the button and locate the .rsp image file within the extracted merlin image folder</li>
        <img width="230" height="69" alt="image" src="https://github.com/user-attachments/assets/163abf7d-abce-4939-a9c3-5a2e0c5dec70" />
        <br>
        <img width="650" height="200" alt="image" src="https://github.com/user-attachments/assets/48c13bde-b390-4f29-9179-6e264f48dab3" />
          <p>In this case it's the first one you'll see within the folder</p>  
    <li>The image should now appear in the table</li>
          <img width="676" height="429" alt="image" src="https://github.com/user-attachments/assets/640d3c22-f2d0-4560-9529-7c2058fca79e" />
    <li>Hit Configure Drive</li>
          <img width="176" height="54" alt="image" src="https://github.com/user-attachments/assets/45be5aa9-057d-4946-9266-a90321d7a5c6" />
          <br>
          <img width="637" height="124" alt="image" src="https://github.com/user-attachments/assets/78106798-8ba0-466d-a71d-c1463cf3fd10" />
    <li>The download is complete, you could now eject your USB drive</li>
          <img width="639" height="126" alt="image" src="https://github.com/user-attachments/assets/5bfcca1c-9356-47be-b695-07a42c6709f8" />
    <li>On your device, press the F12 key or P key to choose from the boot menu</li>
          <img width="674" height="550" alt="image" src="https://github.com/user-attachments/assets/2464637f-92f3-42e5-8e61-e9949ea9b915" />
          <img width="669" height="397" alt="image" src="https://github.com/user-attachments/assets/01f878a4-36cc-4614-be3e-1e4ac83953cf" />
    <li>After selecting your USB drive, you will be brought up on this sceen</li>
          <img width="728" height="403" alt="image" src="https://github.com/user-attachments/assets/9cd4cbdc-0fd5-4e05-966e-3d597fcf23dc" />
    <li>Select the image file and then press <b>ok</b></li>
    <li>After it has installed, reboot your device and you're all set!</li>
  </ol>


<a href="https://www.dell.com/support/product-details/en-us/product/wyse-3040-thin-client/drivers">Wyse 3040 Thin Client Drivers</a>

<br>
<h1>Youtube Video Reference used:</h1>

how to create Dell Wyse 3040 bootable USB and installation os | Jordan IT Services
https://youtu.be/lDb2zUvtP3Q

Do These CHEAP PCs Live Up To The Hype?
https://www.youtube.com/watch?v=9C7UGogyTWo

<br>

<h1>Note</h1>
<ul>
  <li>For Windows 10 or later, it is advisable to use version 3.2.0</li>
  <li>You might need to refresh or reopen the wayback machine website because it seems like it won't load unless you type a new one again (don't know if this only happens to me or what)</li>
  <li>Please refer to the User Guide for more further dive, especially during the post-boot process of the image file</li>
</ul>
