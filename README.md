This is about how Seestar S50 can be used for real-world scientific tasks, such as plotting color-magnitude diagrams for star clusters from the fits file Seestar creates.

I have created the simple html file with javascript inside that allows generating diagrams for "Color Index G-R vs. Apparent Magnitude" and "Color Index B_G vs. Color Index G_R" for star fields in FITS files produced by the Seestar S50.

If your FITS file comes from a source other than the Seestar S50, please note that the program expects a 3-channel RGB FITS file with 16-bit data in each channel.

The file is available also at: https://apximhd.github.io/star-diagram/gr-diagram.html — file is completely free for use and modification; you can download it locally and alter it as you see fit.

No hidden server-side calculations—everything happens in a single file within your local browser.

You can download this file locally and open it in your browser, and it will work exactly the same way.

To generate the diagrams, you need to load your Seestar S50 FITS file (you may need to crop the selected group of stars or star cluster beforehand, which can be done using software like Siril).

Next, configure the star detection parameters: Threshold, FWHM, Relaxed Tolerance for Smaller Stars, Radius, and Default Magnitude Zero Point. The purpose of each parameter and tips for tuning them are provided in the field descriptions.

Then, click the Build Diagram button.

The illustration shows an example of diagrams generated for the Pleiades star cluster.

There is also a Python file that performs the same tasks but much more elegantly, as it uses specialized astronomical libraries that have no equivalents in JavaScript.
