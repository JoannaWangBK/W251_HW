# W251_HW9
1) How long does it take to complete the training run? (hint: this session is on distributed training, so it will take a while)
 
 It has been going on for more than 13h. Have to terminate due to low AWS credit. 

2) Do you think your model is fully trained? How can you tell?

  The TensorBoard graph was still updating as I terminate

3) Were you overfitting?

  In the beginning it was overfitting, after 60K it was better. 

4) Were your GPUs fully utilized?
  Almost. 98% 
  
5) Did you monitor network traffic (hint: apt install nmon ) ? Was network the bottleneck?

Had issue with this step

6) Take a look at the plot of the learning rate and then check the config file. Can you explain this setting?
 warmup_steps 8000 explains the sharp increase in the plot. 

7) How big was your training set (mb)? How many training lines did it contain?
```
-rw-r--r-- 1 root root  952952494 Mar 19 02:12 train.clean.en.shuffled.BPE.32K.tok
```
8) What are the files that a TF checkpoint is comprised of?

```
-rw-r--r-- 1 root root 730570768 Mar 19 03:23 model.ckpt-0.data-00000-of-00001
-rw-r--r-- 1 root root     27441 Mar 19 03:23 model.ckpt-0.index
-rw-r--r-- 1 root root  11980264 Mar 19 03:23 model.ckpt-0.meta
```
9) How big is your resulting model checkpoint (mb)?
```
-rw-r--r-- 1 root root        81 Mar 19 03:23 checkpoint
```
10) Remember the definition of a "step". How long did an average step take?
```
some samples:
time per step = 0:00:1.013
time per step = 0:00:1.063
time per step = 0:00:1.073
```
About 1 second

