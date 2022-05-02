# image-processing

## Contrast Stretching
p2, p98 = np.percentile(img, (2, 98))

img_rescale = exposure.rescale_intensity(img, in_range=(p2, p98))

## Histogram Equalization
img_eq = exposure.equalize_hist(img)

## Adaptive Equalization
img_adapteq = exposure.equalize_adapthist(img, clip_limit=0.03)
