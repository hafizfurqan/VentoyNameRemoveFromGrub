# Remove Ventoy Name From Grub

Remove Annoying Ventoy Name and web url or change it to another without changing source file.

> [!IMPORTANT]
># Only works in text mode

## To
[Modded](https://raw.githubusercontent.com/hafizfurqan/VentoyNameRemoveFromGrub/refs/heads/main/img/Modded.png)

> [!CAUTION]
> Will need to update file with every Ventoy upgrade.

> [!IMPORTANT]
> This guide is focused on Windows based users.

>  [!TIP]
> Will work with other os but will need to manually mount 30MB partition of drive/device and skip to 4th step.

>  [!NOTE]
> At the time of writing, I tested it on Ventoy 1.1.05 at the time of writing is latest.

  

### Software needed

[`BootIce`](https://www.softpedia.com/get/System/Boot-Manager-Disk/Bootice.shtml) for mounting hidden partition.
`Microsoft Notepad or Your preferred editor.`

  

### Steps

1. Download BootIce and run as administrator.

2. Select drive from dropdown menu and select **Parts Manage**.

3. Select second partition with lable **VTOYEFI** and click **Assign Drive Letter** and assign desired letter.

4. Open with Notepad or your editor **VTOYEFI\grub\grub.cfg**.

5. Below picture shows on left is orignal and on left is removed parts.

![Difference of Ventoy config file](https://raw.githubusercontent.com/hafizfurqan/VentoyNameRemoveFromGrub/55af7c03f0269af620df76d5d7bd4778e5d8ed43/img/Vtoy.PNG)

6. Save file with needed changes and test your Ventoy.

#### Reboot/Eject and enjoy your "Ventoy" without it mentioning as Ventoy.


<details>

<summary>Bonus</summary>

#### To remove even the version and only show boot mode, simply remove **$VENTOY_VERSION**

</details>
