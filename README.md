# OneDrive for Business Straight

OneDrive for Business Converting a file sharing link to a direct link only applies to a single file, and folder sharing cannot take effect.

## code run

- `pip install -r requirements.txt`
- `python main.py`

## binary file
from [release](https://github.com/JingqingLin/OneDrive-directlink/releases) Download binaries directly
<br><br>
- Some links that are not in the correct format may not be judged correctly.

## Instructions
Select the file in OneDrive, right-click - Share

<img src="https://cdn.jsdelivr.net/gh/JingqingLin/ImageHosting/img/20200130155810.png" width = "40%" height = "40%">

copy Link

<img src="https://cdn.jsdelivr.net/gh/JingqingLin/ImageHosting/img/20200115000743.png" width = "40%" height = "40%">

### Picture bed direct link
> The direct link to the picture bed is only applicable to files in image format.

Open the software, click `Direct Link to Image Bed`, and the link will be automatically copied to the clipboard.

<img src="https://cdn.jsdelivr.net/gh/JingqingLin/ImageHosting/img/20200130153230.png" width = "70%" height = "70%">

Paste link into browser and open

<img src="https://cdn.jsdelivr.net/gh/JingqingLin/ImageHosting/img/20200130153545.png" width = "70%" height = "70%">

### Download direct link
Open the software and click `Download direct link`

<img src="https://cdn.jsdelivr.net/gh/JingqingLin/ImageHosting/img/20200130153722.png" width = "70%" height = "70%">

Paste the link into the browser and open it, a download box will pop up.

<img src="https://cdn.jsdelivr.net/gh/JingqingLin/ImageHosting/img/20200115002131.png" width = "70%" height = "70%">

## Compile yourself
- `pip install pyinstaller`
- `pyinstaller -F -w -i OneDrive.ico main.py -p entryplaceholder.py`
- Modify the icon and program name in main.spec, as shown below
`[('.\\OneDrive.ico',icon_path,'DATA')],
          name='OneDrive for Business',`

<img src="https://cdn.jsdelivr.net/gh/jingqinglin/image-hosting/img/20220225140900.png">

- ` pyinstaller main.spec`，The .exe file will be regenerated
