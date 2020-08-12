Test MIRI Cubes:

Generated image cubes for Uranus, one cube for each of the 12 spectral settings.
 For each setting, you have:
 
* A *rad.fits.gz file containing spectral radiance (W/cm2/sr/µm) and a *TB.fits.gz file containing brightness temperatures, without any form of convolution with an MRS FWHM.
* A *rad_gprf.fits.gz and *TB_gprf.fits.gz file with the same units as before, but this time convolved with a wavelength-dependent Gaussian to simulate diffraction from a 6.5-m mirror.
* A *wave.fits.gz file that provides the calculation wavelengths for our forward model.  I realise that I don't actually know the MIRI wavelength grids, so these calculations are on a grid that's half the smallest resolution element for that particular channel, in the hope that we can interpolate to the true grid.

All of the calculations are performed on the 0.11 arcsec/pixel plate scale of the MIRI imager, simply for ease. 
