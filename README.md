# Real-time Video Segmentation on iPhone

This repository provides analysis of different segmentation CoreML models on predicting water surface of a given video input. Video is recorded via Iphone camera in real-time and prediction has been done also in real-time. CoreML models are originally trained with PyTorch and later then converted to CoreML from .pth. You can find [here](https://github.com/erdemunal35/Water-Segmentation-Networks) more information about how these models are constructed, trained with PyTorch and converted to CoreML.

The test [video](https://www.youtube.com/watch?v=K1QICrgxTjA&t=131s&ab_channel=LoungeVFilms-RelaxingMusicandNatureSounds) used in the illustrations below is recorded via Iphone XR camera and the mask prediction is computed in real-time.

<table>
    <tr>
        <td colspan=2 align="center"><b>Real-time water surface segmentation using different encoder-decoder pairs on iPhone XR<b></td>
    </tr>
    <tr>
        <td>
            <img src="https://github.com/erdemunal35/Real-time-Video-Segmentation-on-Iphone/blob/master/linknet_mobilenetv2_gif.gif?raw=true" alt="Seg demo on iPhoneXR"></img>
        </td>
        <td>
            <img src="https://github.com/erdemunal35/Real-time-Video-Segmentation-on-Iphone/blob/master/linknet_resnet18_gif.gif?raw=true" alt="Seg demo on iPhoneXR"></img>
        </td>
    </tr>
    <tr>
    <td>
            <img src="https://github.com/erdemunal35/Real-time-Video-Segmentation-on-Iphone/blob/master/unet_mobilenetv2_gif.gif?raw=true" alt="Seg demo on iPhoneXR"></img>
        </td>
        <td>
            <img src="https://github.com/erdemunal35/Real-time-Video-Segmentation-on-Iphone/blob/master/unet_resnet18_gif.gif?raw=true" alt="Seg demo on iPhoneXR"></img>
        </td>
    </tr>
</table>

<table>
    <tr>
        <td colspan=2 align="center"><b>Real-time water surface segmentation using different encoder-decoder pairs on iPhone XR<b></td>
    </tr>
    <tr>
        <td>
            <img src="https://github.com/erdemunal35/Real-time-Video-Segmentation-on-Iphone/blob/master/linknet_mobilenetv2_gif.gif?raw=true" alt="Seg demo on iPhoneXR"></img>
        </td>
        <td>
            <img src="https://github.com/erdemunal35/Real-time-Video-Segmentation-on-Iphone/blob/master/linknet_resnet18_gif.gif?raw=true" alt="Seg demo on iPhoneXR"></img>
        </td>
    </tr>
    <tr>
    <td>
            <img src="https://github.com/erdemunal35/Real-time-Video-Segmentation-on-Iphone/blob/master/unet_mobilenetv2_gif.gif?raw=true" alt="Seg demo on iPhoneXR"></img>
        </td>
        <td>
            <img src="https://github.com/erdemunal35/Real-time-Video-Segmentation-on-Iphone/blob/master/unet_resnet18_gif.gif?raw=true" alt="Seg demo on iPhoneXR"></img>
        </td>
    </tr>
</table>

## Acknowledgement
The XCODE project in this repository is directly built on [ESPNetv2-COREML](https://github.com/sacmehta/ESPNetv2-COREML) repository with no major change at all. Many thanks to [sacmehta](https://github.com/sacmehta) for providing the Swift environment. It enabled me to run my trained CoreML models from the repository [Water-Segmentation-Networks](https://github.com/erdemunal35/Water-Segmentation-Networks) succesfully.
