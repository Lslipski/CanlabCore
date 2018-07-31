---
title: "Output Example 1"
excerpt: "Example 1<br>

```
img_obj = load_image_set('emotionreg'); % Load a dataset
t = ttest(img_obj, .005, 'unc');  % Do a group t-test
t = threshold(t, .005, 'unc', 'k', 10); % Re-threshold with extent threshold of 10 contiguous voxels
r = region(t); % Turn t-map into a region object with one element per contig region
montage(r, 'colormap');
``` 
<br/><img src='{{ base_path}}||/images/example-1.png'>"
collection: examples
---

This is an example of how a small amount of code can produce power fMRI visualizations. 

Example 1
======
This simple code

```
img_obj = load_image_set('emotionreg'); % Load a dataset
t = ttest(img_obj, .005, 'unc');  % Do a group t-test
t = threshold(t, .005, 'unc', 'k', 10); % Re-threshold with extent threshold of 10 contiguous voxels
r = region(t); % Turn t-map into a region object with one element per contig region
montage(r, 'colormap');
```

Produces this output:
<br/><img src='/images/example-1.png'>
