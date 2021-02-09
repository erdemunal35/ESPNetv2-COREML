# Real-time Video Segmentation on iPhone

This repository provides analysis of different segmentation CoreML models on predicting water surface. CoreML models were originally trained with PyTorch and later converted to CoreML from .pth. You can find [the main repository](https://github.com/erdemunal35/WaterSegNets) for more information about how these models were constructed, trained with PyTorch and converted to CoreML. Currently, only linknet-mobilenetv2.mlmodel is available in the repository since other models exceed 25Mb threshold.

The test [video](https://www.youtube.com/watch?v=K1QICrgxTjA&t=131s&ab_channel=LoungeVFilms-RelaxingMusicandNatureSounds) used in the illustrations below is recorded via Iphone XR camera and the mask prediction is computed in real-time.

<table align="center">
    <tr>
        <td colspan=3 align="center"><b>Real-time water surface segmentation using different encoder-decoder pairs on iPhone XR<b></td>
    </tr>
    <tr>
        <td>
            <img src="https://github.com/erdemunal35/Real-time-Video-Segmentation-on-Iphone/blob/master/github_data/linknet_mobilenetv2_gif.gif?raw=true" alt="Seg demo on iPhoneXR"></img>
        </td>
        <td>
            <img src="https://github.com/erdemunal35/Real-time-Video-Segmentation-on-Iphone/blob/master/github_data/linknet_resnet18_gif.gif?raw=true" alt="Seg demo on iPhoneXR"></img>
        </td>
    </tr>
    <tr>
    <td>
            <img src="https://github.com/erdemunal35/Real-time-Video-Segmentation-on-Iphone/blob/master/github_data/unet_mobilenetv2_gif.gif?raw=true" alt="Seg demo on iPhoneXR"></img>
        </td>
        <td>
            <img src="https://github.com/erdemunal35/Real-time-Video-Segmentation-on-Iphone/blob/master/github_data/unet_resnet18_gif.gif?raw=true" alt="Seg demo on iPhoneXR"></img>
        </td>
    </tr>
</table>

<table align="center">
    <tr>
        <td colspan=2 align="center"><b>Layer distributions of CoreML models<b></td>
    </tr>
    <tr>
        <td>
            <img src="https://github.com/erdemunal35/Real-time-Video-Segmentation-on-Iphone/blob/master/github_data/linknet-mobilenetv2.png" alt="Layer distribution of linknet-mobilenetv2.mlmodel"></img><p align="center">linknet-mobilenetv2.mlmodel</p>
        </td>
        <td>
            <img src="https://github.com/erdemunal35/Real-time-Video-Segmentation-on-Iphone/blob/master/github_data/linknet-resnet18.png" alt="Layer distribution of linknet-resnet18.mlmodel"></img><p align="center">linknet-resnet18.mlmodel</p>
        </td>
    </tr>
    <tr>
    <td>
            <img src="https://github.com/erdemunal35/Real-time-Video-Segmentation-on-Iphone/blob/master/github_data/unet-mobilenetv2.png" alt="Layer distribution of unet-mobilenetv2.mlmodel"></img><p align="center">unet-mobilenetv2.mlmodel</p>
        </td>
        <td>
            <img src="https://github.com/erdemunal35/Real-time-Video-Segmentation-on-Iphone/blob/master/github_data/unet-resnet18.png" alt="Layer distribution of unet-resnet18.mlmodel"></img><p align="center">unet-resnet18.mlmodel</p>
        </td>
    </tr>
</table>

## Acknowledgement
The XCODE project in this repository is directly built on [ESPNetv2-COREML](https://github.com/sacmehta/ESPNetv2-COREML) repository with no major change. Many thanks to [sacmehta](https://github.com/sacmehta) for providing the Swift environment. It enabled me to run my trained CoreML models from the repository [WaterSegNets](https://github.com/erdemunal35/WaterSegNets) succesfully.
