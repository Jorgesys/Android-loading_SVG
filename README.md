# Android-loading_SVG
Android : How to load a SVG file from resources (/raw) and internet.

This app show you how to load a SVG from resources 

```SVG svg = SVGParser.getSVGFromResource(getResources(), R.raw.android_robot);
Drawable drawable = svg.createPictureDrawable();
mImageView.setImageDrawable(drawable);
mImageView.setLayerType(View.LAYER_TYPE_SOFTWARE, null);```

or from internet using an Asynctask:

```new HttpImageRequestTask().execute();```
