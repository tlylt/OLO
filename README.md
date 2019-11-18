# OLO
Only Learn Once

# ML
## Overview
- Images -> blobFromImages() -> Blob -> Trained Model -> Inference

## The dnn Process  
1. Load the pretrained model  
- net = cv2.dnn.readNetFrom( prototxt, caffeModel)
2. Process image into 4D Tensor  
- blob = cv2.dnn.blobFromImage(image,scalefactor,size,mean,swapRB,crop,ddepth)
3. Input image  
- net.setInput(blob)
4. Create inference  
- outp = net.forward()
