# A PyTorch implementation of MobileNetV3

This is a PyTorch implementation of MobileNetV3 architecture as described in the paper [Searching for MobileNetV3](https://arxiv.org/pdf/1905.02244.pdf).

Some details may be different from the original paper, welcome to discuss and help me figure it out.

### MobileNetV3
|              | Madds     | Parameters | Top1-acc  |
| -----------  | --------- | ---------- | --------- |
| Large        | 219 M     | 5.4  M     | 75.2%     |
| Small        | 66  M     | 2.9  M     | 67.4%     |
| Ours Large   | 263 M     | 3.7  M     | 75.454%   |
| My Small     | 65  M     | 3.1  M     | 69.069%   |

  The mobilenetv3.py is fork from https://github.com/xiaolai-sqlai/mobilenetv3
  
  But there are some different implement details between the original paper setting and the personal one's. 
  
  Like the SeModule, and the last few layers of fc, the paper didn't use Batch Norm, but this implemented add BN in the code.

  So, I re-implemented the MobileNetV3 in detailed. See mobilenetv3_version2.py for more detailed information.
  
  You can compare the mobilenetv3_version2.py with mobilenetv3.py. 
  
  The output is the same. You can just run the py file without other third part lib or package.
