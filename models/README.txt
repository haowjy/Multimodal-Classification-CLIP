This is where the notebooks (for CLIP models) will store the models.
The structure would be:

```
models
├─── clipclassifier  # model name
│   ├─── 1 # model version
│   │   ├─── cliptextclassifier.pth # model weights
├─── clipimageclassifier
│   ├─── 1
│   │   ├─── clipimageclassifier.pth
...
```